---
title: 在公開資產之前先測試資產
description: 瞭解如何先在Adobe Dynamic Media Classic中測試資產，然後再將資產公開。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# 在公開資產之前先測試資產 {#testing-assets-before-making-them-public}

安全測試可協助您定義安全的測試環境，並根據一組可設定的IP位址和範圍來建立強大的B2B解決方案。 此功能可讓您將Adobe Dynamic Media Classic部署與內容管理和業務系統的架構搭配起來。

進行安全測試之後，您便能預覽內容未發佈的網站測試版本。

如有需要，請建立測試環境，而非讓資產公開可用，理由如下：

* 公開推出前的預覽網站 (測試網站)
* 提供需要限制存取的資產，例如在B2B Web應用程式中顯示價格的eCatalog。
* 在防火牆後面使用資產，做為產品資訊管理系統、客戶服務應用程式、訓練網站等的一部分。

>[!NOTE]
>
>安全測試不會影響對Adobe Dynamic Media Classic的存取。 Adobe Dynamic Media Classic安全性會保持一致，且需要一般憑證才能存取Adobe Dynamic Media Classic及相關網站服務。

## 安全測試的運作方式 {#how-secure-testing-works}

大多數企業都是在防火牆後方執行網際網路。可以通過特定路由，一般而言也可以透過限制範圍的公開 IP 位址存取網際網路。

透過公司網路，您可以使用以下網站找出您的公用IP位址： [https://www.whatismyip.com](https://www.whatismyip.com/) 或向您的公司IT組織索取此資訊。

透過安全測試，Adobe Dynamic Media Classic可為中繼環境或內部應用程式建立專用的影像伺服器。 向此伺服器提出的任何要求都會檢查其原始 IP 位址。如果傳入的請求不在核准的IP位址清單中，則會傳回失敗回應。 Adobe Dynamic Media Classic公司管理員會為公司的安全測試環境設定已核准的IP位址清單。

由於原始請求的位置必須確認，因此Secure Testing Service的流量不會透過內容發佈網路(例如公用Dynamic Media影像伺服器流量)進行路由。 向安全測試服務提出的請求與公開Dynamic Media影像伺服器的請求相比，延遲時間稍微長一些。

可立即從安全測試服務使用未發佈的資產，而不需加以發佈。透過這種方式，您可以在資產發佈到公開顯示的影像伺服器之前執行預覽。

>[!NOTE]
>
>Secure Testing Services會使用已設定內部發佈內容的目錄伺服器。 因此，如果貴公司設定為發佈至Secure Testing，則可在Secure Testing服務上立即取得Adobe Dynamic Media Classic中上傳的任何資產。 不論資產是否標示為上傳時發佈，此功能皆為true。

Secure Testing服務目前支援下列資產型別和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 影像。
* 暈映 (演算伺服器要求)。
* 轉譯器伺服器請求（支援，但客戶必須明確要求）。
* 集，包含影像集、eCatalog、演算集和媒體集。
* 標準Adobe Dynamic Media Classic多媒體檢視器。
* Adobe Dynamic Media Classic OnDemand JSP頁面。
* 靜態內容，如 PDF 檔案和逐步伺服視訊。
* HTTP 視訊串流。
* 漸進式視訊串流。

目前不支援下列資產類型和功能:

* Adobe Dynamic Media Classic資訊或eCatalog搜尋
* RTMP 視訊串流
* 網路印刷
* UGC （使用者產生的內容）服務

>[!IMPORTANT]
>
>Adobe Dynamic Media Classic已於2021年9月30日停止支援新的或現有的UGC向量影像資產。

## 測試Secure Testing service {#testing-the-secure-testing-service}

測試Secure Testing服務，確保該服務可如預期般運作。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 準備帳戶

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. 請聯絡Adobe客戶服務，要求他們啟用您帳戶的安全測試。
1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]**.
1. 在「影像伺服器發佈」頁面的 **[!UICONTROL `Publish Context`]** 下拉式清單，選取 **[!UICONTROL 測試影像服務]**.
1. 對於使用者端位址篩選器，請選取 **[!UICONTROL 新增]**.
1. 選取核取方塊以啟用（開啟）地址，然後在各自的文字欄位中輸入IP位址和網路遮罩。

   >[!NOTE]
   >
   >如果您新增單一IP位址和網路遮罩，該位址可能會進行資產呼叫。 不過，您新增的任何其他IP位址和網路遮罩都不能進行資產呼叫。 因此，請考慮停用（關閉）上述步驟中的核取方塊，以關閉指定IP位址和網路遮罩的功能。 這麼做實際上允許 *全部* 進行資產呼叫的IP位址，這些位址都會顯示。

1. 進行以下一項操作:
   * 如果您必須新增更多IP位址，請重複前兩個步驟。
   * 繼續下一個步驟。
1. 在「影像伺服器發佈」頁面的左下方，選取「 」 **[!UICONTROL 儲存]**
1. 將所需的影像上傳至您的Adobe Dynamic Media Classic帳戶。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 請確定某些影像已標示為發佈，而其他影像已取消標籤，然後提交發佈工作。

   另請參閱 [發佈檔案](publishing-files.md#publishing_files).

1. 請前往「 」，判斷Secure Testing服務的名稱 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.
1. 在「應用程式一般設定」頁面的「伺服器」群組下方，尋找「**[!UICONTROL 測試發佈內容伺服器名稱]**」右側的名稱。

如果伺服器名稱遺失或伺服器的URL無法運作，請聯絡Adobe服務。

### 準備網站變體

您需要兩個網站變體，分別連結至已發佈和未發佈的資產: 

* 公開版本：使用舊版Adobe Dynamic Media Classic URL語法連結資產。
* 測試版本：使用相同語法但使用安全測試網站名稱的連結資產。

### 執行測試

請執行下列測試:

1. 檢查資產在您的企業網路中是否可見。

   從先前定義的IP位址範圍所識別的公司網路中，網站的測試版本會顯示所有影像，無論是否標示為發佈。 因此，在預覽核准或產品上市之前，您可以進行測試而不會意外讓影像可供使用。

   確認您的網站公開版本會顯示已發佈的資產，例如先前使用Adobe Dynamic Media Classic的體驗。

1. 在公司網路外部，確認未發佈的資產（亦即未標示為發佈）受到保護，不會受到第三方存取。

   從外部存取您的網路（例如從您的家用電腦或透過3G連線），然後確認網站的公開版本顯示所有已發佈的資產，但不顯示任何未發佈的內容。

   確認測試版本並未顯示任何資產，因為您是透過未經核准的 IP 位置存取安全測試服務。
