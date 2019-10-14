---
title: 在公開資產前加以測試
seo-title: 在公開資產前加以測試
description: 'null'
seo-description: 瞭解如何在公開資產之前測試資產。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012 a70
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/pload_ and_ publish_ assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9 f87 ffc2 f67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 在公開資產前加以測試 {#testing-assets-before-making-them-public}

安全測試可以協助您根據可設定的 IP 位址集和範圍，定義安全測試環境並建置健全的 B2B 解決方案。此功能可讓您與您的Dynamic Media Classic部署搭配使用您的內容管理和商務平台架構。

進行安全測試之後，您便能預覽內容未發佈的網站測試版本。

出於下列原因，您可能會希望建立測試環境而不將資產公開:

* 公開推出前的預覽網站 (測試網站)
* 供應必須限制存取的資產，如在 B2B 網路應用程式中顯示價格的 eCatalog。
* 使用產品資訊管理系統、客戶服務應用程式、訓練網站等部分防火牆後的資產。

>[!NOTE]
>
>安全測試不影響 Scene7 Publishing System 的存取。SPS 安全性將會保持一致，且存取 SPS 和相關網路服務時會要求一般認證。

## 安全測試的運作方式 {#how-secure-testing-works}

大多數企業都是在防火牆後方執行網際網路。可以通過特定路由，一般而言也可以透過限制範圍的公開 IP 位址存取網際網路。

您可以從公司網路，使用https://whatismyip.com之類的網站找到您的公開IP位址，或從公司IT組織索取此項資訊。

透過安全測試，Dynamic Media Classic可為測試環境或內部應用程式建立專用的Image Server。向此伺服器提出的任何要求都會檢查其原始 IP 位址。如果要求不在已核准 IP 位址清單中，則會傳回失敗回應。Dynamic Media Classic Company管理員會為公司的安全測試環境設定已核准IP位址清單。

因為必須確認原始請求的位置，所以安全測試服務的流量不會透過內容散髮網路路由，例如公開動態媒體影像伺服器流量。與公開動態媒體影像伺服器相比，「保全測試」服務的要求可能會稍有延遲。

可立即從安全測試服務使用未發佈的資產，而不需加以發佈。這讓您可以在將資產發佈至公開影像伺服器之前先執行預覽。

***附註**：安全測試服務運用設定為內部發佈內容的目錄伺服器。因此請注意，若公司設定為發佈至安全測試，任何在 Scene7 Publishing System 中上載的資產，將立刻在安全測試服務中呈現可用的狀態。此功能具強制性，不管資產上載時是否標記為發佈。*

安全測試服務目前支援下列資產類型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 影像.
* 暈映 (演算伺服器要求)。
* 演算伺服器要求(支援，但必須由客戶明確要求)。
* 集，包含影像集、eCatalog、演算集和媒體集。
* Standard Dynamic Media Classic豐富媒體檢視器。
* Dynamic Media Classic OnDemand JSP頁面。
* 靜態內容，如 PDF 檔案和逐步伺服視訊。
* HTTP 視訊串流。
* 漸進式視訊串流。

目前不支援下列資產類型和功能:

* RTMP 視訊串流
* UGC 服務
* 網路印刷
* Dynamic Media Classic Info或eCatalog搜尋

## 測試安全測試服務 {#testing-the-secure-testing-service}

您應測試安全測試服務以確保如預期運作。

**準備帳戶**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 聯絡「技術支援」並要求啟用您帳戶的安全測試。
1. 在 Scene7 Publishing System 中按一下「**設定** &gt; **發佈設定** &gt; **影像伺服器**」。
1. 在「影像伺服器發佈」頁面的「發佈內容」下拉式清單中，選取「**測試影像伺服**」。
1. 針對「用戶端位址篩選器」按一下「**增加**」。
1. 選取核取方塊以啟用 (開啟) 位址，然後在個別的文字欄位中輸入 IP 位址和網路遮罩。
1. 重複前兩個步驟以增加更多 IP 位址。或者，繼續下一個步驟。
1. 在「影像伺服器發佈」頁面的左下角，按一下「**儲存**」。
1. 將所需的影像上載到您的 Scene7 Publishing System 帳戶。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 請務必標記某些影像用於發佈，其他則取消標記，然後送出發佈工作。

   請參閱[發佈](publishing-files.md#publishing_files)。

1. 按一下「**設定** &gt; **應用程式設定** &gt; **一般設定**」以確定安全測試服務的名稱。
1. 在「應用程式一般設定」頁面的「伺服器」群組下方，尋找「**測試發佈內容伺服器名稱**」右側的名稱。

如果伺服器名稱遺失或伺服器 URL 無效，請聯絡「技術支援」。

**準備網站變體**

您需要兩個網站變體，分別連結至已發佈和未發佈的資產: 

* 公開版本：使用您傳統的Dynamic Media Classic URL語法連結資產
* 測試版本: 使用相同的語法，但以安全測試網站名稱連結資產

**執行測試**

請執行下列測試:

1. 檢查資產在您的企業網路中是否可見。

   在先前定義的 IP 位址範圍所識別的企業網路中，網站測試版本應顯示所有影像，不論其是否標記為發佈。這讓您得以進行測試而不會意外地在預覽批准或產品推出前使影像曝光。

   確認您的網站版本顯示已發佈資產，如先前使用Dynamic Media Classic所提供的資產。

1. 從企業網路外部確認未發佈 (也就是未標記為發佈) 的資產皆受到保護，不受第三方存取。

   從外部 (例如家中電腦或 3G 連線) 存取網路，然後確認網站公開版本顯示了所有已發佈的資產，而並未顯示任何未發佈內容。

   確認測試版本並未顯示任何資產，因為您是透過未經核准的 IP 位置存取安全測試服務。
