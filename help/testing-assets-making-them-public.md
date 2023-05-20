---
title: Test資產，然後再公開
description: 在將資產公之於眾之前，學習如何testAdobe Dynamic Media Classic的資產。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 31%

---

# Test資產，然後再公開 {#testing-assets-before-making-them-public}

安全測試可幫助您定義安全test環境，並基於一組可配置的IP地址和範圍構建強健的B2B解決方案。 此功能允許您將您的Adobe Dynamic Media Classic部署與內容管理和業務系統的體系結構相匹配。

進行安全測試之後，您便能預覽內容未發佈的網站測試版本。

如果需要，請建立轉移環境，而不是使資產公開可用，原因如下：

* 公開推出前的預覽網站 (測試網站)
* 供應必須限制存取的資產，如在 B2B 網路應用程式中顯示價格的 eCatalog。
* 使用產品資訊管理系統、客戶服務應用程式、訓練網站等部分防火牆後的資產。

>[!NOTE]
>
>安全測試不影響訪問Adobe Dynamic Media Classic。 Adobe Dynamic Media Classic安全保持一致，需要通常的證書才能訪問Adobe Dynamic Media Classic和相關網路服務。

## 安全測試的運作方式 {#how-secure-testing-works}

大多數企業都是在防火牆後方執行網際網路。可以通過特定路由，一般而言也可以透過限制範圍的公開 IP 位址存取網際網路。

從公司網路中，您可以使用網站(如 [https://www.whatismyip.com](https://www.whatismyip.com/) 或從您的公司IT部門請求此資訊。

通過安全測試，Adobe Dynamic Media Classic為臨時環境或內部應用程式建立了專用的映像伺服器。 向此伺服器提出的任何要求都會檢查其原始 IP 位址。如果要求不在已核准 IP 位址清單中，則會傳回失敗回應。Adobe Dynamic Media Classic公司管理員為其公司的安全測試環境配置批准的IP地址清單。

因為必須確認原始請求的位置，所以安全測試服務的流量不會通過內容分發網路(如公共Dynamic Media映像伺服器流量)路由。 與公有的Dynamic Media映像伺服器相比，請求安全測試服務的延遲稍高一些。

可立即從安全測試服務使用未發佈的資產，而不需加以發佈。這樣，您就可以在資產發佈到面向公共的影像伺服器之前運行預覽。

>[!NOTE]
>
>安全測試服務使用配置了內部發佈上下文的目錄伺服器。 因此，如果您的公司配置為發佈到安全測試，則在Adobe Dynamic Media Classic上傳的任何資產都可立即在安全測試服務上使用。 無論資產是否標籤為在上載時發佈，此功能均為true。

安全測試服務當前支援以下資產類型和功能：

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
* 標準Adobe Dynamic Media Classic富媒體觀眾。
* Adobe Dynamic Media ClassicOnDemand JSP頁。
* 靜態內容，如 PDF 檔案和逐步伺服視訊。
* HTTP 視訊串流。
* 漸進式視訊串流。

目前不支援下列資產類型和功能:

* Adobe Dynamic Media Classic資訊或電子目錄搜索
* RTMP 視訊串流
* 網路印刷
* UGC（用戶生成的內容）服務

>[!IMPORTANT]
>
>2021年9月30日結束了對Adobe Dynamic Media Classic新的或現有的UGC向量影像資產的支援。

## Test安全測試服務 {#testing-the-secure-testing-service}

Test安全測試服務，確保它按預期工作。

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

1. 聯繫Adobe客戶關懷，並請求他們在您的帳戶上啟用安全測試。
1. 在Adobe Dynamic Media Classic，在全球導航欄上， **[!UICONTROL 設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 映像伺服器]**。
1. 在「影像伺服器發佈」頁上， **[!UICONTROL 發佈上下文]** 下拉清單，選擇 **[!UICONTROL Test影像服務]**。
1. 對於「客戶端地址篩選器」，選擇 **[!UICONTROL 添加]**。
1. 選中該複選框以啟用（開啟）地址，然後在相應的文本欄位中鍵入IP地址和網路掩碼。

   >[!NOTE]
   >
   >如果添加一個IP地址和網路掩碼，該地址可進行資產調用。 但是，您添加的任何其他IP地址和網路掩碼均不允許進行資產調用。 因此，請考慮禁用（關閉）上述步驟中的複選框，以關閉指定IP地址和網路掩碼的功能。 這樣做有效地允許 *全部* IP地址進行資產調用，所有地址都顯示出來。

1. 進行以下一項操作:
   * 如果必須添加更多IP地址，請重複前兩步。
   * 繼續下一步。
1. 在「影像伺服器發佈」頁的左下角，選擇 **[!UICONTROL 保存]**
1. 將所需映像上載到您的Adobe Dynamic Media Classic帳戶。

   請參閱 [上載檔案](uploading-files.md#uploading_files)。

1. 請務必標記某些影像用於發佈，其他則取消標記，然後送出發佈工作。

   請參閱 [發佈檔案](publishing-files.md#publishing_files)。

1. 通過轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]**。
1. 在「應用程式一般設定」頁面的「伺服器」群組下方，尋找「**[!UICONTROL 測試發佈內容伺服器名稱]**」右側的名稱。

聯繫Adobe如果伺服器名稱缺失或伺服器的URL無效，請小心。

### 準備網站變體

您需要兩個網站變體，分別連結至已發佈和未發佈的資產: 

* 公共版本 — 使用傳統的Adobe Dynamic Media ClassicURL語法連結資產。
* 臨時版本 — 使用相同語法但使用安全測試站點名稱連結資產。

### 執行測試

請執行下列測試:

1. 檢查資產在您的企業網路中是否可見。

   從由先前定義的IP地址範圍標識的公司網路中，網站的暫存版本顯示所有影像，無論是否標籤為發佈。 因此，您可以在預覽批准或產品發佈前不意外地使影像可用，而進行test。

   確認您的網站的公共版本顯示已發佈的資產，如以前在Adobe Dynamic Media Classic所經歷的那樣。

1. 從企業網路外部確認未發佈 (也就是未標記為發佈) 的資產皆受到保護，不受第三方存取。

   從外部 (例如家中電腦或 3G 連線) 存取網路，然後確認網站公開版本顯示了所有已發佈的資產，而並未顯示任何未發佈內容。

   確認測試版本並未顯示任何資產，因為您是透過未經核准的 IP 位置存取安全測試服務。
