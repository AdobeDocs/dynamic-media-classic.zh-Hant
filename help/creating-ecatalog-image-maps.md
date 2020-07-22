---
title: 建立 eCatalog 影像地圖
seo-title: 建立 eCatalog 影像地圖
description: 'null'
seo-description: 瞭解如何建立eCatalog影像地圖。
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 77%

---


# 建立 eCatalog 影像地圖{#creating-ecatalog-image-maps}

影像地圖是 eCatalog 頁面上的一個區域，您可以使用滑鼠滑過其上或按一下，以觸發各種動作。例如，當您移動指標至影像地圖上，您會看到某個項目的滑鼠指向效果文字描述。您按一下「影像地圖」時，會啟動其他動作。例如，您可以開啟一個網頁，以便檢視者瞭解更多關於某項目的資訊或購買項目，或者您可以啟動視訊查看使用中的項目。

## 繪製 eCatalog 影像地圖 {#drawing-ecatalog-image-maps}

如果是eCatalog，請在「eCatalog」畫面的「地圖頁面」標籤上繪製影像地圖。此畫面包含顯示 eCatalog 頁面的影像地圖區域，以及右方的影像地圖清單。建立影像地圖時，其名稱會輸入影像地圖清單中。

1. 按一下 eCatalog 的滑鼠指向「編輯」按鈕。
1. Click **Map Pages**.
1. 在「地圖頁面」畫面的左方，選取您要的頁面。
1. 在影像地圖區域中，繪製一個矩形或多邊形影像地圖:

   * **矩形地**&#x200B;圖選擇「矩形影像地圖」工具，並拖曳至頁面以建立矩形。

   * **多邊形地**&#x200B;圖選取「多邊形影像地圖」工具，並在影像周長周圍按一下必要的次數。 當您按一下時，Dynamic Media Classic會繪製影像地圖的邊界。
   在您繪製影像地圖後，Dynamic Media Classic會在影像地圖清單中為其指派名稱。 若要建立名稱，Dynamic Media Classic會在您正在工作的eCatalog頁面名稱中附加一個循序編號。

1. (選擇性) 在「影像地圖」清單面板中的「名稱」欄下，輸入「影像地圖」的新名稱。請勿在輸入的名稱中包含空格。
1. 您可以讓檢視者在按一下「影像地圖」時開啟新網頁。在「影像地圖」清單面板中的「URL」欄中輸入網頁的 URL。

   按一下「編輯」並輸入範本，使輸入 URL (Href 範本) 的過程更容易。

   請參閱[使用範本來輸入 JavaScript 與 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. (Optional) In the Show drop-down list, click **Rollover Text**, and then enter the text that you want users to see onscreen when they move their pointers over the Image Map.
1. (Optional) In the Show drop-down list, click **Other Actions**, and enter an attribute to trigger a blur or focus action when users move their pointers over an Image Map.

   請參閱[為影像地圖定義其它動作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 按一下&#x200B;**「儲存」**。
1. (Optional) Click **Preview** to view the eCatalog with the default eCatalog Viewer preset.

若要刪除「影像地圖」，請在「影像地圖」清單中選取其名稱，並按一下「刪除」。若要從頁面暫時停用「影像地圖」而不刪除「影像地圖」，請在「影像地圖」清單面板中，取消選取該「影像地圖」的「開啟」選項。

## 在 eCatalog 中內嵌豐富媒體 {#embedding-rich-media-in-an-ecatalog}

您可以使用「eCatalog 豐富媒體」選項，將 MP4 格式的視訊或迴轉集增加到您已在 eCatalog 增加的「影像地圖」。使用者按一下 eCatalog 中的「影像地圖」區域時，會彈出相關聯的視訊或迴轉集。如果您希望可讓客戶查看使用中的項目，或從不同角度和視角查看項目，此功能特別實用。

您也可以選擇性顯示工具提示文字，以便客戶將指標移過「影像地圖」時知道自己即將點選的選項內容。

**在 eCatalog 中內嵌豐富媒體**

1. 繪製 eCatalog 影像地圖

   請參閱[繪製 eCatalog 影像地圖](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在「顯示」下拉式清單中選取「豐富媒體」。
1. 在左側的「增加資產」面板中，導覽至含有您要內嵌之迴轉集或視訊 (MP4 格式) 資產的資料夾。
1. 將資產拖曳至「影像地圖」。
1. (選擇性) 在「影像地圖」清單面板中的「工具提示」欄標題下，輸入您希望檢視者將游標移過「影像地圖」時，在螢幕上可看到的文字。
1. 按一下「儲存」。

## 編輯 eCatalog 影像地圖 {#editing-ecatalog-image-maps}

在 eCatalog 畫面的「地圖頁面」標籤上開始作業，使用以下技巧來編輯 eCatalog 影像地圖:

* **調整位置**&#x200B;選取「平移」工具，並將指標移至地圖邊界附近，但不移至地圖邊界上方。 指標顯示為四向箭頭時，請拖曳整個影像地圖至新位置。

   請參閱[調整影像地圖的位置、形狀及大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **變更形狀和大小若要**&#x200B;調整矩形影像地圖的大小，請選取「平移」工具。 接著，將指標移動至邊框或角上，當您看到雙向箭頭圖示時，請加以拖曳。若要調整多邊形影像地圖的大小，請拖曳方形的選取範圍控制點。若要建立選取範圍控制點，請按一下影像地圖的邊框，然後拖曳。

   請參閱[調整影像地圖的位置、形狀及大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **刪除影像地**&#x200B;圖選取平移工具，按一下影像地圖以選取它，然後按一下 
**刪除**.

   To remove all Image Maps from an eCatalog, click the **Order Pages** tab, and then click **Clear Maps**.

* **處理重疊的影像**&#x200B;地圖拖曳以變更「影像地圖」清單上的「影像地圖」順序。

   請參閱[處理重疊影像地圖](creating-image-maps.md#handling_overlapping_image_maps)。

* **將影像對應複製到其**&#x200B;他頁面選取「將對應複製到」按鈕（請確定您位於「對應頁面」標籤上）。 在「選取影像」畫面上，選取要複製影像地圖的頁面，然後按一下「選取」按鈕。

   請參閱[將影像地圖複製到其它影像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>如同在 eCatalog 中複製影像地圖到不同頁面，您可以在 eCatalog 中將所有影像地圖複製到不同的 eCatalog。請參閱[在 eCatalog 之間複製影像地圖](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)。

## 檢視及匯入影像地圖資料 {#reviewing-and-importing-image-map-data}

「地圖摘要」畫面提供有關 eCatalog 的中繼資料。在「地圖摘要」畫面上開始作業時，您也可以為 eCatalog 批次匯入影像地圖資料。使用這個方式匯入影像地圖資料，可讓您更輕鬆輸入影像地圖 URL 與滑鼠指向效果文字。

若要查看「地圖摘要」畫面，請在 eCatalog 畫面的「地圖頁面」標籤上按一下「摘要」。

### 檢視影像地圖資料摘要 {#review-image-map-data-summary}

1. 在「地圖頁面」畫面上按一下「摘要」。

   「地圖摘要」畫面會顯示 eCatalog 中的影像地圖數目、URL、滑鼠指向效果文字敘述以及其它動作。

1. 如果發生滑鼠指向按鍵錯誤，請按一下「Rollover_Key 錯誤」欄中的錯誤，即可在試算表中查看需要變更的內容，以更正錯誤。您可以從這個訊息選取並複製文字，然後將其貼上試算表。
1. 按一下「預覽」即可在 eCatalog 檢視器中檢視頁面，按一下「X」即可關閉「摘要」畫面，並返回至「地圖頁面」畫面，或按一下「關閉」以返回至「瀏覽」。

### 匯入影像地圖資料 {#import-image-map-data}

您可以為整個 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入影像地圖資料可為您免除麻煩，就不需要在建立每個影像地圖時，都要在影像地圖清單中輸入資料。

>[!NOTE]
>
>匯入影像地圖資料前，您必須先建立好影像地圖。

在「地圖摘要」畫面上開始作業，然後遵循下列步驟，為建立的影像地圖匯入影像地圖資料:

1. 按一下「匯入地圖資料」。
1. 在「匯入中繼資料」對話框中按一下「瀏覽」，然後選取 Tab 字元分隔或 XML DTD 檔案。
1. 在「工作名稱」欄位中，鍵入檔案的名稱 (請注意保留其副檔名)。
1. 按一下「上載」。

## 在 eCatalog 之間複製影像地圖 {#copying-image-maps-between-ecatalogs}

您可以將一個 eCatalog 中的所有影像地圖複製到其它 eCatalog。以這種方式複製影像地圖，對於在相同 eCatalog 的外文翻譯之間複製影像地圖來說，是非常便利的方法。為了成功複製，Dynamic Media Classic建議在具有相同頁數和相同影像的eCatalog之間複製。

>[!NOTE]
>
>如果您複製影像地圖的目標 eCatalog 中已包含影像地圖，則這些影像地圖會在複製時刪除。

遵循下列步驟，即可將一個 eCatalog 中的所有影像地圖複製到其它 eCatalog:

1. 選取您要複製其影像地圖的 eCatalog，然後按一下 eCatalog 的滑鼠指向「編輯」按鈕。
1. 在「排序頁面」標籤上，按一下「複製地圖」。
1. 在「選取資產」對話框中，選取您要複製其影像地圖的 eCatalog，然後按一下「選取」。

如果目標eCatalog（您複製影像對應的eCatalog）具有不同大小的頁數或影像，Dynamic Media Classic會顯示警告訊息。 您可以不理會警告，按一下「繼續」以複製影像地圖。
