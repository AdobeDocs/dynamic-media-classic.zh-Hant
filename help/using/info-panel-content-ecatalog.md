---
title: 管理eCatalogs中的資訊面板內容
description: 瞭解如何在Adobe Dynamic Media Classic中管理eCatalogs中的資訊面板內容。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 40%

---

# 管理eCatalogs中的資訊面板內容{#managing-info-panel-content-in-ecatalogs}

除了針對 eCatalog 中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用計時的快取及排程內容更新來管理資訊面板。

您可以使用Adobe Dynamic Media Classic中的下列功能來管理資訊面板設定和資料：

* 「資訊面板設定」面板可讓您指定用來顯示「資訊面板」文字的範本、預設的錯誤回應，以及快取資訊的小時數。 此外，您還可以指定是否要自動發佈 eCatalog。
* 「資訊面板」資料摘要面板可讓您指定CSV檔案，其中包含您要顯示在「資訊面板」滑鼠指向效果文字中的文字，以及更新資訊的排程時間。
* 「匯入中繼資料」(Import Metadata)對話方塊(從「對映頁面」(Map Pages)檢視中存取)可讓您匯入包含滑鼠指向效果文字資訊的Tab字元分隔的TXT檔案。 您可以針對滑鼠指向效果文字，使用此TXT選項或具有CSV檔案選項的「資料摘要」面板。
* 「對應頁面」檢視提供預覽針對特定「影像地圖」顯示之xml的選項。

## 設定eCatalogs的回應範本 {#set-up-a-response-template-for-ecatalogs}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取預設的回應範本，或建立您自己的回應範本。

>[!NOTE]
>
>您也可以在檢視器預設集中設定回應範本。若要改用檢視器預設集中的回應範本，請新增 `fmt=1` 到檢視器預設集中的Information Server URL結尾。
>
>另請參閱 [設定eCatalog檢視器預設集](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]** 面板。
1. 選取回應範本:

   * 從「回應範本」選單中選取一個預設集。用於範本設計的 XML 會顯示在「使用者範本」方框中。
   * 若要建立自己的回應範本，請選取 **[!UICONTROL 自訂]**. 在「使用者範本」方框中鍵入範本 XML 定義。您可以使用預設範本作為自訂範本的基礎。

1. （選擇性）在「預設回應」方塊中，輸入您要在Adobe Dynamic Media Classic擷取「影像地圖」資訊時發生錯誤，顯示的文字。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」方框中輸入快取資料前要等候的時數:

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要一整天頻繁更新，請設定較高的數字。 預設為十小時。

1. 選取 **[!UICONTROL 發佈]**.

## 匯入eCatalogs中資訊面板的來源內容 {#import-source-content-for-the-info-panel-in-ecatalogs}

對於 eCatalog 之資訊面板的來源文字，您可以使用逗號分隔值檔案 (CSV) 或 Tab 字元分隔檔案 (TXT)。Tab 字元分隔檔案必須使用 UTF16 (Unicode) 編碼。您可以使用不同的方法匯入不同的檔案型別。

格式化來源內容時，請記住下列準則:

* 確定 Tab 字元分隔與逗號分隔的資料所包含的欄數目，與滑鼠指向範本所需的欄數相等。
* 請確定資料的第一個專案或欄是滑鼠指向效果識別碼（與影像地圖URL中的rollover_key值相關聯）。
* 請確定識別碼之後的每個定位字元或逗號分隔專案都是您要取代到回應範本中的專案。 因此，第一欄會替換為$1$，第二欄會替換為$2$，以此類推。

### 從外部託管位置將CSV內容匯入eCatalogs {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板資料摘要]** 面板。
1. 在「外部代管的 CSV 檔案位置」方框中輸入 CSV 檔案的 URL。您可以在此欄位中貼上 URL，也可以直接鍵入。
1. （選用）使用「排程更新」功能表指定更新內容的時間，然後選取 **[!UICONTROL 新增]**. 您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」方框中。(若要移除時間，請選取該時間，然後選取 **[!UICONTROL 刪除]**.)
1. （選用）選取 **[!UICONTROL 立即執行更新]** 以便您立即更新內容。

### 匯入 Tab 字元分隔檔案或 CSV 檔案 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]** 面板。
1. 選取 **[!UICONTROL 上傳S7Info內容]**.
1. 選取 **[!UICONTROL 瀏覽]**，選取要使用的Tab字元分隔的TXT檔案、CSV或SSV檔案，然後選取 **[!UICONTROL 開啟]**.
1. 選取 **[!UICONTROL 上傳]**.

Adobe Dynamic Media Classic會傳送電子郵件訊息給您，讓您知道上傳是否成功。

## 預覽影像地圖的滑鼠指向效果關鍵文字 {#preview-rollover-key-text-for-an-image-map}

使用「地圖頁面」畫面，您可以輕鬆且快速地檢視 eCatalog 特定頁面之影像地圖的「資訊面板」文字。

1. 選取目錄的變換影像 **[!UICONTROL 編輯]** 按鈕。
1. 選取 **[!UICONTROL 對應頁面]**.
1. 在表格頂端的熒幕右側，選擇 **[!UICONTROL 資訊面板]** 從「顯示」功能表。

   滑鼠指項效果關鍵文字會顯示在每個包含「資訊面板」文字的影像地圖旁邊。
