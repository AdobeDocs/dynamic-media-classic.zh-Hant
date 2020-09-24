---
title: 在公開資產前加以測試
seo-title: 在公開資產前加以測試
description: 'null'
seo-description: 瞭解如何在資產公開之前先進行測試。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 03ca030531f8d9fa0a6944bd5050e2c865adf5f5
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 54%

---


# 在公開資產前加以測試 {#testing-assets-before-making-them-public}

安全測試可以協助您根據可設定的 IP 位址集和範圍，定義安全測試環境並建置健全的 B2B 解決方案。此功能可讓您將Dynamic Media Classic部署與內容管理與商務平台的架構搭配使用。

進行安全測試之後，您便能預覽內容未發佈的網站測試版本。

出於下列原因，您可能會希望建立測試環境而不將資產公開:

* 公開推出前的預覽網站 (測試網站)
* 供應必須限制存取的資產，如在 B2B 網路應用程式中顯示價格的 eCatalog。
* 使用產品資訊管理系統、客戶服務應用程式、訓練網站等部分防火牆後的資產。

>[!NOTE]
>
>安全測試不會影響對Dynamic Media Classic的存取。 Dynamic Media Classic安全性仍維持一致，並需要通常的認證才能存取Dynamic Media Classic和相關的web services。

## 安全測試的運作方式 {#how-secure-testing-works}

大多數企業都是在防火牆後方執行網際網路。可以通過特定路由，一般而言也可以透過限制範圍的公開 IP 位址存取網際網路。

從您的公司網路，您可以使用https://whatismyip.com等網站來判斷您的公開IP位址，或向您的公司IT組織要求這項資訊。

使用安全測試，Dynamic Media Classic為測試環境或內部應用程式建立專用的映像伺服器。 向此伺服器提出的任何要求都會檢查其原始 IP 位址。如果要求不在已核准 IP 位址清單中，則會傳回失敗回應。Dynamic Media Classic Company Administrator會為其公司的安全測試環境設定已核准的IP位址清單。

由於必須確認原始請求的位置，因此安全測試服務的流量不會透過內容散發網路（例如公用動態媒體影像伺服器流量）路由。 與公用動態媒體影像伺服器相比，要求安全測試服務的延遲可能略高。

可立即從安全測試服務使用未發佈的資產，而不需加以發佈。這讓您可以在將資產發佈至公開影像伺服器之前先執行預覽。

***注意&#x200B;**:Secure Testing Services運用已設定內部發佈內容的Catalog Server。 因此，如果您的公司已設定發佈至Secure Testing，請注意，Dynamic Media Classic中任何已上傳的資產都會立即在Secure Testing服務上使用。 此功能具強制性，不管資產上載時是否標記為發佈。*

安全測試服務目前支援下列資產類型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 影像.
* 暈映 (演算伺服器要求)。
* Render Server請求（支援，但客戶必須明確要求）。
* 集，包含影像集、eCatalog、演算集和媒體集。
* 標準Dynamic Media Classic多媒體檢視器。
* Dynamic Media Classic OnDemand JSP頁。
* 靜態內容，如 PDF 檔案和逐步伺服視訊。
* HTTP 視訊串流。
* 漸進式視訊串流。

目前不支援下列資產類型和功能:

* RTMP 視訊串流
* UGC 服務
* 網路印刷
* 動態媒體經典資訊或eCatalog搜尋

## 測試安全測試服務 {#testing-the-secure-testing-service}

您應測試安全測試服務以確保如預期運作。

注意：如果您未提及「設定>發佈設定>影像伺服器>測試影像服務」下方的任何IP，則您只新增IP，讓IP能夠呼叫資產，且不允許其他IP進行呼叫。 只要該節未提及IP，所有IP都可以呼叫資產，而且會顯示。

**準備帳戶**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 聯絡「技術支援」並要求啟用您帳戶的安全測試。
1. 在Dynamic Media Classic中，按一下「 **設定** >發 **布設定** >影 **像伺服器**」。
1. 在「影像伺服器發佈」頁面的「發佈內容」下拉式清單中，選取「**測試影像伺服**」。
1. 針對「用戶端位址篩選器」按一下「**增加**」。
1. 選取核取方塊以啟用 (開啟) 位址，然後在個別的文字欄位中輸入 IP 位址和網路遮罩。

   >[!NOTE]
   >
   >如果您新增單一IP位址和網路遮色片，該位址可進行資產呼叫。 不過，您新增的任何其他IP位址和網路遮色片均不允許進行資產呼叫。 因此，您可考慮停用（關閉）上述步驟中的核取方塊，以關閉指定IP位址和網路遮色片的功能。 如此可有效 *率地允許* 所有IP位址進行資產呼叫，而且所有IP位址都會出現。

1. 進行以下一項操作:
   * 重複前兩個步驟以增加更多 IP 位址。
   * 繼續下一步。
1. 在「影像伺服器發佈」頁面的左下角，按一下「**儲存**」。
1. 將所要的影像上傳至您的Dynamic Media Classic帳戶。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 請務必標記某些影像用於發佈，其他則取消標記，然後送出發佈工作。

   請參閱[發佈](publishing-files.md#publishing_files)。

1. 按一下「**設定** > **應用程式設定** > **一般設定**」以確定安全測試服務的名稱。
1. 在「應用程式一般設定」頁面的「伺服器」群組下方，尋找「**測試發佈內容伺服器名稱**」右側的名稱。

如果伺服器名稱遺失或伺服器的URL無法運作，請連絡Adobe Care。

**準備網站變體**

您需要兩個網站變體，分別連結至已發佈和未發佈的資產: 

* 公用版本——使用傳統Dynamic Media Classic URL語法連結資產。
* 測試版本——使用相同語法但使用Secure Testing網站名稱來連結資產。

**執行測試**

請執行下列測試:

1. 檢查資產在您的企業網路中是否可見。

   在先前定義的 IP 位址範圍所識別的企業網路中，網站測試版本應顯示所有影像，不論其是否標記為發佈。這讓您得以進行測試而不會意外地在預覽批准或產品推出前使影像曝光。

   確認您網站的公開版會像之前使用Dynamic Media Classic時那樣顯示已發佈的資產。

1. 從企業網路外部確認未發佈 (也就是未標記為發佈) 的資產皆受到保護，不受第三方存取。

   從外部 (例如家中電腦或 3G 連線) 存取網路，然後確認網站公開版本顯示了所有已發佈的資產，而並未顯示任何未發佈內容。

   確認測試版本並未顯示任何資產，因為您是透過未經核准的 IP 位置存取安全測試服務。

