---
title: 建立eCatalog影像映射
description: 了解如何在AdobeDynamic Media Classic中建立eCatalog影像地圖。
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 40%

---

# 建立eCatalog影像映射{#creating-ecatalog-image-maps}

「影像地圖」是eCatalog頁面上的一個區域，可以用滑鼠滾動，或選取以觸發各種動作。 例如，當您將指標移至影像地圖上時，您會看到項目的變換文字說明。 選取「影像地圖」時，會起始另一個動作。 例如，您可以開啟一個網頁，以便檢視者瞭解更多關於某項目的資訊或購買項目，或者您可以啟動視訊查看使用中的項目。

## 繪製eCatalog影像映射 {#drawing-ecatalog-image-maps}

如果是eCatalog，請在「eCatalog」畫面的「地圖頁面」標籤上繪製影像地圖。此畫面包含顯示 eCatalog 頁面的影像地圖區域，以及右方的影像地圖清單。建立影像地圖時，其名稱會輸入影像地圖清單中。

1. 選擇eCatalog的滾動&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕。
1. 選擇&#x200B;**[!UICONTROL 映射頁]**。
1. 在「地圖頁面」畫面的左方，選取您要的頁面。
1. 在影像地圖區域中，繪製一個矩形或多邊形影像地圖:

   * **矩形地圖**  — 選取「矩形影像地圖」工具，並拖曳頁面以建立矩形。

   * **多邊形圖**  — 選取「多邊形影像圖」工具，然後在影像周長附近選取必要的次數。當您選取時，AdobeDynamic Media Classic會繪製影像地圖的邊框。

      繪製影像地圖後，AdobeDynamic Media Classic會在「影像地圖」清單中為其指派名稱。 若要形成名稱，AdobeDynamic Media Classic會在您正在工作的eCatalog頁面名稱中附加一個循序編號。

1. （可選）從「影像地圖」清單中，在[!UICONTROL 名稱]欄中，您可以為「影像地圖」輸入新名稱。 請勿在輸入的名稱中包含空格。
1. 當檢視器選取「影像地圖」時，您可以讓其開啟新網頁。 在「影像地圖」清單面板中的「URL」欄中輸入網頁的 URL。

   要使輸入URL（Href模板）更容易，請選擇&#x200B;**[!UICONTROL Edit]**&#x200B;並輸入模板。

請參閱[使用範本輸入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. （可選）在「顯示」下拉清單中，選擇&#x200B;**[!UICONTROL 滾動文本]**，然後輸入您希望用戶在影像映射上移動指針時在螢幕上看到的文本。
1. （可選）在「顯示」下拉清單中，選擇「**[!UICONTROL 其他操作]**」，並輸入屬性，以在用戶將指針移到影像映射上時觸發模糊或焦點操作。

   請參閱[定義影像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 選擇&#x200B;**[!UICONTROL 保存]**。
1. （可選）選擇&#x200B;**[!UICONTROL 預覽]**&#x200B;以使用預設的eCatalog查看器預設集查看eCatalog。

若要刪除影像地圖，請在「影像地圖」清單中選取其名稱，然後選取&#x200B;**[!UICONTROL Delete]**。 若要從頁面暫時停用「影像地圖」而不刪除「影像地圖」，請在「影像地圖」清單面板中，取消選取該「影像地圖」的「開啟」選項。

## 將多媒體內嵌在eCatalog中 {#embedding-rich-media-in-an-ecatalog}

您可以使用「eCatalog 豐富媒體」選項，將 MP4 格式的視訊或迴轉集增加到您已在 eCatalog 增加的「影像地圖」。當使用者選取eCatalog中的「影像對應」區域時，會顯示相關的回轉集或視訊。 如果您希望可讓客戶查看使用中的項目，或從不同角度和視角查看項目，此功能特別實用。

當客戶將指標移至影像地圖上時，您也可以選擇顯示工具提示文字，讓他們知道自己正在選取什麼。

**在 eCatalog 中內嵌豐富媒體:**

1. 繪製 eCatalog 影像地圖

   請參閱[繪製eCatalog影像映射](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在「顯示」下拉清單中，選擇&#x200B;**[!UICONTROL 富媒體]**。
1. 在左側的「增加資產」面板中，導覽至含有您要內嵌之迴轉集或視訊 (MP4 格式) 資產的資料夾。
1. 將資產拖曳至「影像地圖」。
1. （可選）在「影像地圖」清單面板的&#x200B;**[!UICONTROL 「工具提示」]**&#x200B;欄標題下，輸入當檢視者將指標移至「影像地圖」上時，要讓檢視者在螢幕上看到的文字。
1. 選擇&#x200B;**[!UICONTROL 保存]**。

## 編輯 eCatalog 影像地圖 {#editing-ecatalog-image-maps}

在 eCatalog 畫面的「地圖頁面」標籤上開始作業，使用以下技巧來編輯 eCatalog 影像地圖:

* **調整位置**  — 選取「平移」工具，並將指標移至地圖邊框附近，但不移至邊框上方。指標顯示為四向箭頭時，請拖曳整個影像地圖至新位置。

   請參閱[調整影像映射的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **變更形狀和大小**  — 若要調整矩形「影像地圖」的大小，請選取「平移」工具。接著，將指標移動至邊框或角上，當您看到雙向箭頭圖示時，請加以拖曳。若要調整多邊形影像地圖的大小，請拖曳方形的選取範圍控制點。要建立選取控制滑塊，請選取「影像映射」的邊框並拖動。

   請參閱[調整影像映射的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **刪除影像**  — 選取平移工具，選取影像地圖以選取，然後選取 **[!UICONTROL 刪除]**。

   要從eCatalog中刪除所有影像映射，請選擇&#x200B;**[!UICONTROL 訂購頁]**&#x200B;頁簽，然後選擇&#x200B;**[!UICONTROL 清除映射]**。

* **處理重疊的影像地圖**  — 拖曳以變更「影像地圖」清單上的「影像地圖」順序。

   請參閱[處理重疊的影像映射](creating-image-maps.md#handling_overlapping_image_maps)。

* **將影像映射複製到其他頁**  — 選 **[!UICONTROL 取「將映射複製到]** 」（請確定您位於「映射頁面」索引標籤）。在「選擇影像」螢幕上，選擇要複製影像映射的頁或頁，然後選擇&#x200B;**[!UICONTROL 選擇]**。

   請參閱[將影像映射複製到其他影像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>除了將影像映射複製到eCatalog中的不同頁面之外，您還可以將eCatalog中的所有影像映射複製到不同的eCatalog。 請參閱[在eCatalog之間複製影像映射](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)。

## 檢閱和匯入影像圖資料 {#reviewing-and-importing-image-map-data}

「地圖摘要」畫面提供有關 eCatalog 的中繼資料。在「地圖摘要」畫面上開始作業時，您也可以為 eCatalog 批次匯入影像地圖資料。使用這個方式匯入影像地圖資料，可讓您更輕鬆輸入影像地圖 URL 與滑鼠指向效果文字。

要查看「映射摘要」螢幕，請在eCatalog螢幕的「映射頁」頁簽上，選擇&#x200B;**[!UICONTROL Summary]**。

### 檢視影像地圖資料摘要 {#review-image-map-data-summary}

1. 在「映射頁面」螢幕上，選擇&#x200B;**[!UICONTROL 摘要]**。

   「地圖摘要」畫面會顯示 eCatalog 中的影像地圖數目、URL、滑鼠指向效果文字敘述以及其它動作。

1. 如果有變換金鑰錯誤，請在&#x200B;**[!UICONTROL 變換金鑰錯誤]**&#x200B;欄中選取錯誤，查看試算表中必須變更哪些項目才能更正錯誤。 您可以從這個訊息選取並複製文字，然後將其貼上試算表。
1. 選擇「**[!UICONTROL 預覽]**」，以便在eCatalog查看器中檢查頁面；選擇X以關閉「摘要」螢幕並返回「映射頁」螢幕，或選擇&#x200B;**[!UICONTROL Close]**&#x200B;以返回「瀏覽」。

### 匯入影像地圖資料 {#import-image-map-data}

您可以為整個 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入影像地圖資料可為您免除麻煩，就不需要在建立每個影像地圖時，都要在影像地圖清單中輸入資料。

>[!NOTE]
>
>匯入影像地圖資料前，您必須先建立好影像地圖。

在「地圖摘要」畫面上開始作業，然後遵循下列步驟，為建立的影像地圖匯入影像地圖資料:

1. 選擇&#x200B;**[!UICONTROL 導入映射資料]**。
1. 在「導入元資料」對話框中，選擇&#x200B;**[!UICONTROL Browse]**，然後選擇以制表符分隔或XML DTD檔案。
1. 在「工作名稱」欄位中，鍵入檔案的名稱 (請注意保留其副檔名)。
1. 選擇&#x200B;**[!UICONTROL Upload]**。

## 在eCatalog之間複製影像映射 {#copying-image-maps-between-ecatalogs}

您可以將一個 eCatalog 中的所有影像地圖複製到其它 eCatalog。以這種方式複製影像地圖，對於在相同 eCatalog 的外文翻譯之間複製影像地圖來說，是非常便利的方法。為了複製成功，AdobeAdobeDynamic Media Classic建議在具有相同頁數和相同影像的eCatalog之間複製。

>[!NOTE]
>
>如果您複製影像地圖的目標 eCatalog 中已包含影像地圖，則這些影像地圖會在複製時刪除。

要將一個eCatalog中的所有映像映射複製到另一個eCatalog，請執行以下操作：

1. 選擇包含要複製的影像映射的eCatalog，然後選擇eCatalog的滾動&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕。
1. 在「訂單頁」頁簽上，選擇&#x200B;**[!UICONTROL 複製映射]**。
1. 在「選擇資產」對話框中，選擇要複製影像映射的eCatalog，然後選擇&#x200B;**[!UICONTROL Select]**。

AdobeDynamic Media Classic如果目標eCatalog（您複製影像地圖的eCatalog）具有不同大小的不同頁數或影像，則會顯示警告訊息。 選擇&#x200B;**[!UICONTROL 繼續]**&#x200B;以複製影像映射（儘管出現警告）。
