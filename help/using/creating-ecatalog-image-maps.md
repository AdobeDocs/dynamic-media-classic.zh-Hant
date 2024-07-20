---
title: 建立eCatalog影像地圖
description: 瞭解如何在Adobe Dynamic Media Classic中建立eCatalog影像地圖。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 26%

---

# 建立eCatalog影像地圖{#creating-ecatalog-image-maps}

「影像地圖」是eCatalog頁面上的區域，您可以用滑鼠滑動，或選取它來觸發各種動作。 例如，當您將指標移到「影像地圖」上時，您會看到專案的變換文字描述。 當您選取「影像地圖」時，會起始另一個動作。 例如，您可以開啟網頁，讓檢視者進一步瞭解專案或購買專案，或者您可以啟動視訊來觀看使用中的專案。

## 繪製eCatalog影像地圖 {#drawing-ecatalog-image-maps}

如果是eCatalog，請在「eCatalog」畫面的「地圖頁面」標籤上繪製影像地圖。此畫面包含顯示 eCatalog 頁面的影像地圖區域，以及右方的影像地圖清單。當您建立「影像地圖」時，其名稱會在「影像地圖」清單中輸入。

1. 選取eCatalog的變換影像&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕。
1. 選取&#x200B;**[!UICONTROL 對應頁面]**。
1. 在「地圖頁面」畫面的左方，選取您要的頁面。
1. 在影像地圖區域中，繪製一個矩形或多邊形影像地圖:

   * **矩形對應**：選取「矩形影像對應」工具，並在頁面上拖曳以建立矩形。

   * **多邊形對映**：選取「多邊形影像對映」工具，然後視需要多次選取影像周邊。 當您選取時，Adobe Dynamic Media Classic會繪製影像地圖的邊界。

     繪製「影像地圖」後，Adobe Dynamic Media Classic會在「影像地圖」清單中為其指定一個名稱。 為了形成名稱，Adobe Dynamic Media Classic會在您正在使用的eCatalog頁面名稱后面附加一個循序號碼。

1. （選擇性）從「影像地圖」清單的[!UICONTROL 名稱]欄中，您可以為「影像地圖」輸入新名稱。 請勿在輸入的名稱中包含空格。
1. 您可以讓檢視者在選取「影像地圖」時開啟新的網頁。 在「影像地圖」清單面板的「URL」欄中，輸入網頁的URL。

   若要更輕鬆地輸入URL （Href範本），請選取&#x200B;**[!UICONTROL 編輯]**&#x200B;並輸入範本。

請參閱[使用範本輸入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. （選擇性）在「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 滑鼠指向效果文字]**，然後輸入當使用者在「影像地圖」上移動指標時，您希望使用者在熒幕上看到的文字。
1. （選擇性）在「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 其他動作]**，然後輸入屬性，以在使用者在影像地圖上移動指標時觸發模糊或焦點動作。

   請參閱[定義影像地圖的其他動作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 選取&#x200B;**[!UICONTROL 儲存]**。
1. （選擇性）選取&#x200B;**[!UICONTROL 預覽]**&#x200B;以檢視使用預設eCatalog檢視器預設集的eCatalog。

若要刪除影像地圖，請在「影像地圖」清單中選取其名稱，然後選取&#x200B;**[!UICONTROL 刪除]**。 您可以暫時停用頁面上的「影像地圖」，而不刪除「影像地圖」。 在「影像地圖」清單面板中選取「影像地圖開啟」選項。

## 在eCatalog中內嵌多媒體 {#embedding-rich-media-in-an-ecatalog}

您可以使用eCatalog的Rich Media選項，將MP4格式的視訊或迴轉集新增至eCatalog的影像地圖。 當使用者在eCatalog中選取「影像地圖」區域時，會顯示相關的「迴轉集」或視訊。 如果您希望可讓客戶查看使用中的項目，或從不同角度和視角查看項目，此功能特別實用。

客戶將指標移過影像地圖時，您也可以選擇顯示工具提示文字，讓客戶知道要選取的內容。

**若要在eCatalog中內嵌多媒體：**

1. 繪製 eCatalog 影像地圖

   檢視[繪製eCatalog影像地圖](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 多媒體]**。
1. 在左側的「新增Assets」面板中，導覽至包含您要內嵌之迴轉集或視訊（MP4格式）資產的資料夾。
1. 將資產拖曳至「影像地圖」。
1. （選擇性）在「影像地圖」清單面板的&#x200B;**[!UICONTROL 工具提示]**&#x200B;欄標題下，輸入檢視者在影像地圖上移動指標時，想在熒幕看到的文字。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

## 編輯 eCatalog 影像地圖 {#editing-ecatalog-image-maps}

在 eCatalog 畫面的「地圖頁面」標籤上開始作業，使用以下技巧來編輯 eCatalog 影像地圖:

* **調整位置**：選取「平移」工具，並將指標移到地圖邊框附近，但不要移到邊框上。 當指標顯示四向箭頭時，請將整個「影像地圖」拖曳到新位置。

  請參閱[調整影像地圖的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **變更形狀和大小**：若要調整矩形影像地圖的大小，請選取「平移」工具。 接著，將指標移動至邊框或角上，當您看到雙向箭頭圖示時，請加以拖曳。若要調整多邊形影像地圖的大小，請拖曳方形的選取範圍控制點。若要建立選取範圍控點，請選取「影像地圖」的框線並拖曳。

  請參閱[調整影像地圖的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **刪除影像地圖**：選取「平移」工具，選取「影像地圖」以選取它，然後選取&#x200B;**[!UICONTROL 刪除]**。

  若要從eCatalog移除所有影像地圖，請選取&#x200B;**[!UICONTROL 訂購頁面]**&#x200B;標籤，然後選取&#x200B;**[!UICONTROL 清除地圖]**。

* **處理重疊的影像地圖**：拖曳以變更影像地圖清單上的影像地圖順序。

  請參閱[處理重疊的影像地圖](creating-image-maps.md#handling_overlapping_image_maps)。

* **將影像地圖複製到其他頁面**：選取&#x200B;**[!UICONTROL 將地圖複製到]** （確定您位於[地圖頁面]索引標籤）。 在「選取影像」畫面上，選取您要複製影像地圖的頁面，然後選取&#x200B;**[!UICONTROL 選取]**。

  請參閱[將影像地圖複製到其他影像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>當您將「影像地圖」複製到eCatalog中的不同頁面時，可以將eCatalog中的所有影像地圖複製到不同的eCatalog。 檢視其他eCatalog ](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)中的[複製影像地圖。

## 檢閱及匯入影像地圖資料 {#reviewing-and-importing-image-map-data}

「地圖摘要」畫面提供有關 eCatalog 的中繼資料。在「地圖摘要」畫面上開始作業時，您也可以為 eCatalog 批次匯入影像地圖資料。使用這個方式匯入影像地圖資料，可讓您更輕鬆輸入影像地圖 URL 與滑鼠指向效果文字。

若要檢視[地圖摘要]畫面，請在eCatalog畫面的[地圖頁面]索引標籤上選取&#x200B;**[!UICONTROL 摘要]**。

### 檢視影像地圖資料摘要 {#review-image-map-data-summary}

1. 在[地圖頁面]畫面上，選取&#x200B;**[!UICONTROL 摘要]**。

   「地圖摘要」畫面會顯示eCatalog中有多少影像地圖、URL、滑鼠指向效果文字說明和其他動作。

1. 如果有滑鼠指向效果索引鍵錯誤，請選取&#x200B;**[!UICONTROL 滑鼠指向效果索引鍵錯誤]**&#x200B;欄中的錯誤，以檢視試算表中必須變更哪些專案才能更正錯誤。 您可以從這個訊息選取並複製文字，然後將其貼上試算表。
1. 選取「**[!UICONTROL 預覽]**」，以便在eCatalog檢視器中檢查頁面。 選取X以關閉[摘要]畫面並返回[地圖頁面]畫面，或選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回[瀏覽]。

### 匯入影像地圖資料 {#import-image-map-data}

您可以為整個 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入「影像地圖」資料可讓您在建立每個「影像地圖」時，在「影像地圖」清單中輸入資料的麻煩。

>[!NOTE]
>
>匯入影像地圖資料前，您必須先建立好影像地圖。

在「地圖摘要」畫面上開始作業，然後遵循下列步驟，為建立的影像地圖匯入影像地圖資料:

1. 選取&#x200B;**[!UICONTROL 匯入對應資料]**。
1. 在「匯入中繼資料」對話方塊中，選取&#x200B;**[!UICONTROL 瀏覽]**，然後選取以Tab分隔的或XML DTD檔案。
1. 在「工作名稱」欄位中，鍵入檔案的名稱 (請注意保留其副檔名)。
1. 選取&#x200B;**[!UICONTROL 上傳]**。

## 在其他eCatalog中複製影像地圖 {#copying-image-maps-between-ecatalogs}

您可以將一個 eCatalog 中的所有影像地圖複製到其它 eCatalog。以這種方式複製影像地圖，對於在相同 eCatalog 的外文翻譯之間複製影像地圖來說，是非常便利的方法。為了成功複製，Adobe Dynamic Media Classic建議您在具有相同頁數和相同影像的eCatalog之間複製。

>[!NOTE]
>
>如果您複製影像地圖的目標 eCatalog 中已包含影像地圖，則這些影像地圖會在複製時刪除。

若要將一個eCatalog中的所有影像地圖複製到另一個eCatalog，請執行下列動作：

1. 選取包含您要複製之影像地圖的eCatalog，然後選取eCatalog的滑鼠指向效果&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕。
1. 在「訂購頁面」索引標籤上，選取&#x200B;**[!UICONTROL 複製地圖]**。
1. 在「選取資產」對話方塊中，選取您要複製影像地圖的eCatalog，然後選取&#x200B;**[!UICONTROL 選取]**。

如果您複製影像地圖的目標eCatalog有不同的頁數或不同大小的影像，Adobe Dynamic Media Classic會顯示警告訊息。 選取&#x200B;**[!UICONTROL 繼續]**&#x200B;以複製影像地圖，無論是否有警告。
