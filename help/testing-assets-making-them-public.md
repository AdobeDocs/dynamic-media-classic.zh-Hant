---
title: 在公開資產前加以測試
description: 了解如何在將資產公開之前先測試資產。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic，資產管理
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 37%

---

# 在公開資產前加以測試 {#testing-assets-before-making-them-public}

Secure Testing可協助您定義安全的測試環境，並根據一組可設定的IP位址和範圍，建立強大的B2B解決方案。 此功能可讓您搭配Dynamic Media Classic部署，搭配內容管理和業務系統的架構。

進行安全測試之後，您便能預覽內容未發佈的網站測試版本。

如果需要，請建立測試環境，而非公開提供資產，原因如下：

* 公開推出前的預覽網站 (測試網站)
* 供應必須限制存取的資產，如在 B2B 網路應用程式中顯示價格的 eCatalog。
* 使用產品資訊管理系統、客戶服務應用程式、訓練網站等部分防火牆後的資產。

>[!NOTE]
>
>安全測試不會影響對Dynamic Media Classic的存取。 Dynamic Media Classic安全性仍維持一致，且需要通常的憑證，才能存取Dynamic Media Classic和相關的Web服務。

## 安全測試的運作方式 {#how-secure-testing-works}

大多數企業都是在防火牆後方執行網際網路。可以通過特定路由，一般而言也可以透過限制範圍的公開 IP 位址存取網際網路。

從您的公司網路，您可以使用https://whatismyip.com等網站來確定您的公開IP地址，或向您的公司IT組織請求此資訊。

透過安全測試，Dynamic Media Classic為中繼環境或內部應用程式建立專用的影像伺服器。 向此伺服器提出的任何要求都會檢查其原始 IP 位址。如果要求不在已核准 IP 位址清單中，則會傳回失敗回應。Dynamic Media Classic公司管理員會為其公司的安全測試環境設定已核准的IP位址清單。

由於必須確認原始請求的位置，因此安全測試服務的流量不會經由內容分發網路(如公用Dynamic Media影像伺服器流量)路由。 與公開的Dynamic Media影像伺服器相比，向安全測試服務提出的延遲略高。

可立即從安全測試服務使用未發佈的資產，而不需加以發佈。如此一來，您就可以在資產發佈至其公開的影像伺服器之前，執行預覽。

>[!NOTE]
>
>安全測試服務使用配置了內部發佈上下文的目錄伺服器。 因此，如果貴公司已設定為發佈至Secure Testing，則Dynamic Media Classic中任何上傳的資產都會立即在Secure Testing服務上使用。 無論資產是否在上傳時標示為要發佈，此功能都為true。

安全測試服務目前支援下列資產類型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 影像.
* 暈映 (演算伺服器要求)。
* 呈現伺服器請求（支援，但必須由客戶明確請求）。
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
* Dynamic Media傳統資訊或eCatalog搜尋

## 測試安全測試服務 {#testing-the-secure-testing-service}

測試安全測試服務，以確保其正常運作。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 準備帳戶

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 請連絡Adobe客戶服務，要求他們在您的帳戶上啟用安全測試。
1. 在Dynamic Media Classic中，在全域導覽列上，按一下&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**。
1. 在「影像伺服器發佈」頁面的「**[!UICONTROL 發佈內容]**」下拉式清單中，選取「測試影像伺服」**[!UICONTROL 。]**
1. 針對「用戶端位址篩選器」按一下「**[!UICONTROL 增加]**」。
1. 選中複選框以啟用（開啟）地址，然後在相應的文本欄位中鍵入IP地址和網路掩碼。

   >[!NOTE]
   >
   >如果您新增單一IP位址和網路遮罩，該位址可能會進行資產呼叫。 不過，您新增的任何其他IP位址和網路遮罩都不允許進行資產呼叫。 因此，請考慮停用（關閉）上述步驟中的核取方塊，以關閉指定IP位址和網路遮罩的功能。 這麼做可以有效允許&#x200B;*所有* IP位址進行資產呼叫，而且都會顯示。

1. 進行以下一項操作:
   * 如果您必須新增更多IP位址，請重複前兩個步驟。
   * 繼續下一步。
1. 在「影像伺服器發佈」頁面的左下方，按一下「**[!UICONTROL 儲存]**」
1. 將所需的影像上傳至您的Dynamic Media Classic帳戶。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 請務必標記某些影像用於發佈，其他則取消標記，然後送出發佈工作。

   請參閱[發佈](publishing-files.md#publishing_files)。

1. 按一下「**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**」以確定安全測試服務的名稱。
1. 在「應用程式一般設定」頁面的「伺服器」群組下方，尋找「**[!UICONTROL 測試發佈內容伺服器名稱]**」右側的名稱。

如果伺服器名稱遺失或伺服器的URL無法運作，請聯絡Adobe服務。

### 準備網站變體

您需要兩個網站變體，分別連結至已發佈和未發佈的資產: 

* 公開版本 — 使用傳統Dynamic Media Classic URL語法連結資產。
* 測試版本 — 使用相同語法但使用安全測試網站名稱連結資產。

### 執行測試

請執行下列測試:

1. 檢查資產在您的企業網路中是否可見。

   從由先前定義的IP位址範圍所識別的公司網路中，網站的測試版本會顯示所有影像，無論是否標示為發佈。 因此，您可以在預覽核准或產品發佈之前，不會意外讓影像可供使用，進行測試。

   確認網站的公開版本顯示先前使用Dynamic Media Classic所體驗的已發佈資產。

1. 從企業網路外部確認未發佈 (也就是未標記為發佈) 的資產皆受到保護，不受第三方存取。

   從外部 (例如家中電腦或 3G 連線) 存取網路，然後確認網站公開版本顯示了所有已發佈的資產，而並未顯示任何未發佈內容。

   確認測試版本並未顯示任何資產，因為您是透過未經核准的 IP 位置存取安全測試服務。
