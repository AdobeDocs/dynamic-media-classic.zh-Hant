---
title: 管理eCatalog中的資訊面板內容
description: 了解如何在Dynamic Media Classic中管理eCatalog中的資訊面板內容。
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# 管理eCatalog中的資訊面板內容{#managing-info-panel-content-in-ecatalogs}

除了針對 eCatalog 中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用定時快取與排程內容更新來管理資訊面板。

您可以使用Dynamic Media Classic中的下列功能來管理您的InfoPanel設定和資料：

* 「資訊面板設定」面板可讓您指定範本，用來顯示資訊面板文字、預設的錯誤回應以及資訊快取的時數。此外，您還可以指定是否要自動發佈 eCatalog。
* 「資訊面板」資料源面板可讓您指定CSV檔案，其中包含您要顯示在「資訊面板」變換文字中的文字，並排程更新資訊的時間。
* 「匯入中繼資料」對話框 (可從「地圖頁面」檢視中存取) 可讓您匯入包含滑鼠指向效果文字資訊之 Tab 字元分隔的 TXT 檔案。針對滑鼠指向效果文字，您可以使用此 TXT 選項或含有 CSV 檔案選項的「資料摘要」面板。
* 「地圖頁面」檢視提供一個選項，可用來預覽針對特定影像地圖所顯示的 xml。

## 設定eCatalog的回應範本 {#set-up-a-response-template-for-ecatalogs}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取一個預設回應範本，也可以自行建立一個。

>[!NOTE]
>
>您也可以在檢視器預設集中設定回應範本。若要改用檢視器預設集中的「回應範本」，請將`fmt=1`新增至檢視器預設集中的資訊伺服器URL結尾。
>
>請參閱[設定eCatalog檢視器預設集](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)。

1. 按兩下您的eCatalog，以在「詳細資訊檢視」中開啟。
1. 選擇&#x200B;**[!UICONTROL InfoPanel Setup]**&#x200B;面板。
1. 選取回應範本:

   * 從「回應範本」選單中選取一個預設集。用於範本設計的 XML 會顯示在「使用者範本」方框中。
   * 要建立自己的響應模板，請選擇&#x200B;**[!UICONTROL Custom]**。 在「使用者範本」方框中鍵入範本 XML 定義。您可以使用預設範本作為自訂範本的基礎。

1. （可選）在「預設回應」方塊中，輸入如果AdobeDynamic Media Classic在擷取影像地圖的資訊時發生錯誤，您要顯示的文字。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」方框中輸入快取資料前要等候的時數:

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要整天經常更新，請設定較高的數字。預設為十小時。

1. 選擇&#x200B;**[!UICONTROL Publish]**。

## 導入eCatalog中「資訊面板」的源內容 {#import-source-content-for-the-info-panel-in-ecatalogs}

對於 eCatalog 之資訊面板的來源文字，您可以使用逗號分隔值檔案 (CSV) 或 Tab 字元分隔檔案 (TXT)。Tab 字元分隔檔案必須使用 UTF16 (Unicode) 編碼。您可以使用不同的方法來匯入不同的檔案類型。

格式化來源內容時，請記住下列準則:

* 確定 Tab 字元分隔與逗號分隔的資料所包含的欄數目，與滑鼠指向範本所需的欄數相等。
* 確定第一個項目或資料欄為滑鼠指向效果識別名稱 (與影像地圖 URL 的 rollover_key 值相關聯)。
* 請確定識別碼後面的每個定位點或逗號分隔項目，都是您要取代回應範本的項目。因此，第一欄會取代為$1$，第二欄會取代為$2$，以此類推。

### 從外部托管位置將CSV內容匯入eCatalog {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 按兩下eCatalog，以在「詳細資訊檢視」中開啟。
1. 選擇&#x200B;**[!UICONTROL InfoPanel Datafeed]**&#x200B;面板。
1. 在「外部代管的 CSV 檔案位置」方框中輸入 CSV 檔案的 URL。您可以在此欄位中貼上 URL，也可以直接鍵入。
1. （可選）指定使用「計畫更新」菜單更新內容的時間，並選擇&#x200B;**[!UICONTROL Add]**。 您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」方框中。（若要移除時間，請選取該時間，然後選取&#x200B;**[!UICONTROL Delete]**。）
1. （可選）選擇&#x200B;**[!UICONTROL 立即運行更新]**&#x200B;以立即更新內容。

### 匯入 Tab 字元分隔檔案或 CSV 檔案 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 連按兩下eCatalog，以在「詳細資訊檢視」中開啟它。
1. 選擇&#x200B;**[!UICONTROL InfoPanel Setup]**&#x200B;面板。
1. 選擇「**[!UICONTROL 上傳S7Info內容]**」。
1. 選擇&#x200B;**[!UICONTROL 瀏覽]**，選擇要使用的以制表符分隔的TXT檔案、CSV或SSV檔案，然後選擇&#x200B;**[!UICONTROL 開啟]**。
1. 選擇&#x200B;**[!UICONTROL Upload]**。

AdobeDynamic Media Classic會傳送電子郵件給您，通知上傳是否成功。

## 預覽影像地圖的滑鼠指向效果關鍵文字 {#preview-rollover-key-text-for-an-image-map}

使用「地圖頁面」畫面，您可以輕鬆且快速地檢視 eCatalog 特定頁面之影像地圖的「資訊面板」文字。

1. 選擇目錄的滾動&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕。
1. 選擇&#x200B;**[!UICONTROL 映射頁]**。
1. 在螢幕右側的表頂部，從「顯示」菜單中選擇「**[!UICONTROL 資訊面板]**」。

   出現在每個包含「資訊面板」文字的影像對應旁邊的變換金鑰文字。
