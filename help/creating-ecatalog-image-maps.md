---
title: 建立電子目錄映像映射
description: 瞭解如何在Adobe Dynamic Media Classic建立eCatalog映像映射。
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 40%

---

# 建立電子目錄映像映射{#creating-ecatalog-image-maps}

「影像映射」是「電子目錄」頁面上的一個區域，您可以用滑鼠滾動或選擇以觸發各種操作。 例如，當將指針移到影像映射上時，將看到項目的滾動文本說明。 選擇「影像映射」時，將啟動另一個操作。 例如，您可以開啟一個網頁，以便檢視者瞭解更多關於某項目的資訊或購買項目，或者您可以啟動視訊查看使用中的項目。

## 繪製電子目錄影像映射 {#drawing-ecatalog-image-maps}

如果是eCatalog，請在「eCatalog」畫面的「地圖頁面」標籤上繪製影像地圖。此畫面包含顯示 eCatalog 頁面的影像地圖區域，以及右方的影像地圖清單。建立影像地圖時，其名稱會輸入影像地圖清單中。

1. 選擇eCatalog的滾動更新 **[!UICONTROL 編輯]** 按鈕
1. 選擇 **[!UICONTROL 映射頁]**。
1. 在「地圖頁面」畫面的左方，選取您要的頁面。
1. 在影像地圖區域中，繪製一個矩形或多邊形影像地圖:

   * **矩形地圖**  — 選擇「矩形影像映射」工具，然後拖動到頁面上建立矩形。

   * **多邊形地圖**  — 選擇「多邊形影像映射」工具，然後在影像周長周圍根據需要選擇多次。 在您選擇時，Adobe Dynamic Media Classic繪製影像映射的邊框。

      繪製影像映射後，Adobe Dynamic Media Classic會在「影像映射」清單中為其指定名稱。 要形成名稱，Adobe Dynamic Media Classic會在您正在工作的eCatalog頁的名稱中附加一個順序號。

1. （可選）在「影像映射」清單中， [!UICONTROL 名稱] 列中，可以輸入影像映射的新名稱。 請勿在輸入的名稱中包含空格。
1. 當查看者選擇「影像映射」時，可以讓他們開啟新網頁。 在「影像地圖」清單面板中的「URL」欄中輸入網頁的 URL。

   要使輸入URL（Href模板）更容易，請選擇 **[!UICONTROL 編輯]** 並輸入模板。

請參閱 [使用模板輸入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. （可選）在「顯示」下拉清單中，選擇 **[!UICONTROL 滾動文本]**，然後輸入希望用戶在影像映射上移動其指針時在螢幕上看到的文本。
1. （可選）在「顯示」下拉清單中，選擇 **[!UICONTROL 其他操作]**，並輸入一個屬性以在用戶將指針移到影像映射上時觸發模糊或聚焦操作。

   請參閱 [定義影像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 選擇 **[!UICONTROL 保存]**。
1. （可選）選擇 **[!UICONTROL 預覽]** 使用預設的eCatalog查看器預設查看eCatalog。

要刪除影像映射，請在「影像映射」清單中選擇其名稱，然後選擇 **[!UICONTROL 刪除]**。 若要從頁面暫時停用「影像地圖」而不刪除「影像地圖」，請在「影像地圖」清單面板中，取消選取該「影像地圖」的「開啟」選項。

## 將富媒體嵌入到eCatalog中 {#embedding-rich-media-in-an-ecatalog}

您可以使用「eCatalog 豐富媒體」選項，將 MP4 格式的視訊或迴轉集增加到您已在 eCatalog 增加的「影像地圖」。當用戶在eCatalog中選擇「影像映射」區域時，將顯示關聯的旋轉集或視頻。 如果您希望可讓客戶查看使用中的項目，或從不同角度和視角查看項目，此功能特別實用。

當客戶將其指針移到您的映像圖上時，您還可以選擇顯示工具提示文本，以便他們知道自己正在選擇什麼。

**在 eCatalog 中內嵌豐富媒體:**

1. 繪製 eCatalog 影像地圖

   請參閱 [繪製電子目錄影像映射](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在「顯示」(Show)下拉清單中，選擇 **[!UICONTROL 富媒體]**。
1. 在左側的「增加資產」面板中，導覽至含有您要內嵌之迴轉集或視訊 (MP4 格式) 資產的資料夾。
1. 將資產拖曳至「影像地圖」。
1. （可選）在「影像映射」清單面板中， **[!UICONTROL 工具提示]** 列標題，輸入希望查看者在將指針移到影像映射上時在螢幕上看到的文本。
1. 選擇 **[!UICONTROL 保存]**。

## 編輯 eCatalog 影像地圖 {#editing-ecatalog-image-maps}

在 eCatalog 畫面的「地圖頁面」標籤上開始作業，使用以下技巧來編輯 eCatalog 影像地圖:

* **調整位置**  — 選擇「平移」工具，將指針移到地圖邊框附近，但不移到地圖邊框上。 指標顯示為四向箭頭時，請拖曳整個影像地圖至新位置。

   請參閱 [調整影像映射的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **更改形狀和大小**  — 要調整矩形影像映射的大小，請選擇平移工具。 接著，將指標移動至邊框或角上，當您看到雙向箭頭圖示時，請加以拖曳。若要調整多邊形影像地圖的大小，請拖曳方形的選取範圍控制點。要建立選擇句柄，請選擇「影像映射」的邊框並拖動。

   請參閱 [調整影像映射的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **刪除影像映射**  — 選擇平移工具，選擇影像映射以選擇它，然後選擇 **[!UICONTROL 刪除]**。

   要從eCatalog中刪除所有映像映射，請選擇 **[!UICONTROL 訂單頁]** ，然後選擇 **[!UICONTROL 清除地圖]**。

* **處理重疊影像映射**  — 拖動以更改「影像映射」清單上的「影像映射」順序。

   請參閱 [處理重疊影像映射](creating-image-maps.md#handling_overlapping_image_maps)。

* **將影像映射複製到其他頁**  — 選擇 **[!UICONTROL 將映射複製到]** （確保您位於「映射頁」頁籤上）。 在「選擇影像」螢幕上，選擇要複製影像映射的頁或頁，然後選擇 **[!UICONTROL 選擇]**。

   請參閱 [將映像映射複製到其他映像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>除了將「影像映射」複製到eCatalog中的不同頁面外，您還可以將eCatalog中的所有「影像映射」複製到其他eCatalog。 請參閱 [在電子目錄之間複製映像映射](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)。

## 查看和導入映像圖資料 {#reviewing-and-importing-image-map-data}

「地圖摘要」畫面提供有關 eCatalog 的中繼資料。在「地圖摘要」畫面上開始作業時，您也可以為 eCatalog 批次匯入影像地圖資料。使用這個方式匯入影像地圖資料，可讓您更輕鬆輸入影像地圖 URL 與滑鼠指向效果文字。

要查看「映射摘要」螢幕，請在「電子目錄」螢幕的「映射頁」頁籤上，選擇 **[!UICONTROL 摘要]**。

### 檢視影像地圖資料摘要 {#review-image-map-data-summary}

1. 在「映射頁」螢幕上，選擇 **[!UICONTROL 摘要]**。

   「地圖摘要」畫面會顯示 eCatalog 中的影像地圖數目、URL、滑鼠指向效果文字敘述以及其它動作。

1. 如果存在滾動更新鍵錯誤，請選擇 **[!UICONTROL 滾動更新密鑰錯誤]** 列，查看電子錶格中必須更改哪些內容才能更正錯誤。 您可以從這個訊息選取並複製文字，然後將其貼上試算表。
1. 選擇 **[!UICONTROL 預覽]** 這樣，您就可以在eCatalog Viewer中查看頁面；選擇X以關閉「摘要」螢幕並返回「映射頁」螢幕，或選擇 **[!UICONTROL 關閉]** 的子菜單。

### 匯入影像地圖資料 {#import-image-map-data}

您可以為整個 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入影像地圖資料可為您免除麻煩，就不需要在建立每個影像地圖時，都要在影像地圖清單中輸入資料。

>[!NOTE]
>
>匯入影像地圖資料前，您必須先建立好影像地圖。

在「地圖摘要」畫面上開始作業，然後遵循下列步驟，為建立的影像地圖匯入影像地圖資料:

1. 選擇 **[!UICONTROL 導入映射資料]**。
1. 在「導入元資料」對話框中，選擇 **[!UICONTROL 瀏覽]**，然後選擇制表符分隔或XML DTD檔案。
1. 在「工作名稱」欄位中，鍵入檔案的名稱 (請注意保留其副檔名)。
1. 選擇 **[!UICONTROL 上載]**。

## 在電子目錄之間複製映像映射 {#copying-image-maps-between-ecatalogs}

您可以將一個 eCatalog 中的所有影像地圖複製到其它 eCatalog。以這種方式複製影像地圖，對於在相同 eCatalog 的外文翻譯之間複製影像地圖來說，是非常便利的方法。為使複製成功，Adobe Dynamic Media Classic建議在具有相同頁數和相同影像的eCatalog之間複製。

>[!NOTE]
>
>如果您複製影像地圖的目標 eCatalog 中已包含影像地圖，則這些影像地圖會在複製時刪除。

要將一個eCatalog中的所有映像映射複製到另一個eCatalog，請執行以下操作：

1. 選擇包含要複製的影像映射的eCatalog ，然後選擇eCatalog的滾動更新 **[!UICONTROL 編輯]** 按鈕
1. 在「訂單頁」頁籤上，選擇 **[!UICONTROL 複製映射]**。
1. 在「選擇資產」對話框中，選擇要複製映像映射的目錄，然後選擇 **[!UICONTROL 選擇]**。

如果目標eCatalog（您將映像映射複製到的eCatalog）具有不同大小的頁或影像數，Adobe Dynamic Media Classic將顯示警告消息。 選擇 **[!UICONTROL 繼續]** 複製映像圖，但不會出現警告。
