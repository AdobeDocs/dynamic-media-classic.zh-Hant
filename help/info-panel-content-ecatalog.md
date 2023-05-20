---
title: 管理電子目錄中的資訊面板內容
description: 瞭解如何管理Adobe Dynamic Media ClassiceCatalogs中的「資訊面板」內容。
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# 管理電子目錄中的資訊面板內容{#managing-info-panel-content-in-ecatalogs}

除了針對 eCatalog 中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用定時快取與排程內容更新來管理資訊面板。

可以使用Adobe Dynamic Media Classic的以下功能管理InfoPanel設定和資料：

* 「資訊面板設定」面板可讓您指定範本，用來顯示資訊面板文字、預設的錯誤回應以及資訊快取的時數。此外，您還可以指定是否要自動發佈 eCatalog。
* 「資訊面板」資料源面板允許您指定包含要顯示在「資訊面板」滾動更新文本中的文本的CSV檔案，以及更新資訊的計畫時間。
* 「匯入中繼資料」對話框 (可從「地圖頁面」檢視中存取) 可讓您匯入包含滑鼠指向效果文字資訊之 Tab 字元分隔的 TXT 檔案。針對滑鼠指向效果文字，您可以使用此 TXT 選項或含有 CSV 檔案選項的「資料摘要」面板。
* 「地圖頁面」檢視提供一個選項，可用來預覽針對特定影像地圖所顯示的 xml。

## 為eCatalog設定響應模板 {#set-up-a-response-template-for-ecatalogs}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取一個預設回應範本，也可以自行建立一個。

>[!NOTE]
>
>您也可以在檢視器預設集中設定回應範本。要改用「查看器預設」中的「響應模板」，請添加 `fmt=1` 到「查看器預設」中「資訊伺服器URL」的末尾。
>
>請參閱 [設定eCatalog Viewer預設](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)。

1. 按兩下eCatalog，使其在「詳細資訊視圖」中開啟。
1. 選擇 **[!UICONTROL InfoPanel安裝]** 的子菜單。
1. 選取回應範本:

   * 從「回應範本」選單中選取一個預設集。用於範本設計的 XML 會顯示在「使用者範本」方框中。
   * 要建立您自己的響應模板，請選擇 **[!UICONTROL 自定義]**。 在「使用者範本」方框中鍵入範本 XML 定義。您可以使用預設範本作為自訂範本的基礎。

1. （可選）在「預設響應」框中，鍵入在Adobe Dynamic Media Classic檢索影像映射資訊時遇到錯誤時要顯示的文本。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」方框中輸入快取資料前要等候的時數:

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要整天經常更新，請設定較高的數字。預設為十小時。

1. 選擇 **[!UICONTROL 發佈]**。

## 導入eCatalogs中「資訊」面板的源內容 {#import-source-content-for-the-info-panel-in-ecatalogs}

對於 eCatalog 之資訊面板的來源文字，您可以使用逗號分隔值檔案 (CSV) 或 Tab 字元分隔檔案 (TXT)。Tab 字元分隔檔案必須使用 UTF16 (Unicode) 編碼。您可以使用不同的方法來匯入不同的檔案類型。

格式化來源內容時，請記住下列準則:

* 確定 Tab 字元分隔與逗號分隔的資料所包含的欄數目，與滑鼠指向範本所需的欄數相等。
* 確定第一個項目或資料欄為滑鼠指向效果識別名稱 (與影像地圖 URL 的 rollover_key 值相關聯)。
* 確保標識符後的每個制表符或逗號分隔項是要替換到響應模板中的項。因此，第一列被替換為$1$ ，第二列被替換為$2$，依此類推。

### 從外部托管位置將CSV內容導入eCatalogs {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 按兩下eCatalog，使其在「詳細資訊視圖」中開啟。
1. 選擇 **[!UICONTROL InfoPanel資料源]** 的子菜單。
1. 在「外部代管的 CSV 檔案位置」方框中輸入 CSV 檔案的 URL。您可以在此欄位中貼上 URL，也可以直接鍵入。
1. （可選）使用「計畫更新」菜單指定更新內容的時間，然後選擇 **[!UICONTROL 添加]**。 您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」方框中。(要刪除時間，請選擇它並選擇 **[!UICONTROL 刪除]**。)
1. （可選）選擇 **[!UICONTROL 立即運行更新]** 以立即更新內容。

### 匯入 Tab 字元分隔檔案或 CSV 檔案 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 按兩下eCatalog，以在「詳細資訊視圖」中開啟它。
1. 選擇 **[!UICONTROL InfoPanel安裝]** 的子菜單。
1. 選擇 **[!UICONTROL 上載S7Info內容]**。
1. 選擇 **[!UICONTROL 瀏覽]**，選擇要使用的制表符分隔的TXT檔案、CSV或SSV檔案，然後選擇 **[!UICONTROL 開啟]**。
1. 選擇 **[!UICONTROL 上載]**。

Adobe Dynamic Media Classic給你發一封電子郵件，告訴你上載是否成功。

## 預覽影像地圖的滑鼠指向效果關鍵文字 {#preview-rollover-key-text-for-an-image-map}

使用「地圖頁面」畫面，您可以輕鬆且快速地檢視 eCatalog 特定頁面之影像地圖的「資訊面板」文字。

1. 選擇目錄的滾動更新 **[!UICONTROL 編輯]** 按鈕
1. 選擇 **[!UICONTROL 映射頁]**。
1. 在螢幕右側的表格頂部，選擇 **[!UICONTROL 資訊面板]** 按鈕。

   滑鼠指項效果關鍵文字會顯示在每個包含「資訊面板」文字的影像地圖旁邊。
