---
title: 建立影像地圖
description: 瞭解如何在Adobe Dynamic Media Classic中建立影像地圖。
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 46%

---

# 建立影像地圖 {#creating-image-maps}

影像地圖是影像、eCatalog 頁面，或迴轉集之影像中的某個區域，可顯示內含滑鼠指向效果文字的面板。當使用者選取影像地圖時，就會觸發某種動作。 例如，啟動網頁讓使用者進一步瞭解產品。當使用者將指標移到「影像地圖」上時，其周圍會出現一個外框。

除了在Adobe Dynamic Media Classic中建立影像地圖功能外，您也可以在Adobe Acrobat或Adobe InDesign中設計目錄時建立影像地圖。

當您建立「影像地圖」時，可以執行下列任一項作業：

* 輸入滑鼠指向效果文字。
* 輸入用來啟動網頁的 JavaScript 與 URL。
* 為影像地圖建立 URL 範本。
* 將影像地圖複製到其它影像、eCatalog 頁面或迴轉集中。
* 將影像地圖匯出至 CSV 或 XML。
* 從定位字元分隔檔案或XML檔案匯入影像中繼資料。
* 定義其它由全球資訊網協會決定的動作。
* 預覽影像地圖。

## 繪製和調整影像地圖 {#drawing-and-adjusting-an-image-map}

1. 進行以下一項操作:

   * 如果您在「格點檢視」或「清單檢視」中處理影像，請在「編輯」下拉式清單中選取 **[!UICONTROL 影像地圖]**. 或者，在「詳細資料檢視」中開啟它，然後選取 **[!UICONTROL 影像地圖]** 影像上方。
   * 如果您在「格點檢視」或「清單檢視」中使用迴轉集，請選取 **[!UICONTROL 編輯]**. 或者，在「詳細資料檢視」中開啟它，然後選取 **[!UICONTROL 編輯]**. 選取影像資產，然後選取 **[!UICONTROL 影像地圖]**.
   * 如果您正在使用eCatalog，請在「格點檢視」、「清單檢視」、「詳細資料檢視」中選取 **[!UICONTROL 編輯]**. 選取 **[!UICONTROL 對應頁面]** 標籤。

   ![影像地圖影像](assets/ma_image_map.png)

1. 繪製矩形或多邊形影像地圖:

   * **矩形地圖**  — 選取「矩形影像地圖」工具並在頁面上拖曳以建立矩形。 若要將點新增至矩形對映（因此將其變更為多邊形對映），請按下Ctrl，然後將插入工具置於所需位置並選取。

   * **多邊形地圖**  — 選取「多邊形影像地圖」工具，並選取要包圍的影像區域周邊上的點。 使用多邊形密度滑桿，讓多邊形的點密度產生差異。如果選取其它地圖，則會記憶原始密度。如果在多邊形中增加、刪除或移動任一點，則會遺失原始密度，並將滑桿重設回最大值。

1. 如有需要，可在「影像地圖」清單中輸入影像地圖的名稱。繪製影像地圖後，Adobe Dynamic Media Classic會為其指定一個名稱。

   若要建立名稱，Adobe Dynamic Media Classic會在您使用的影像或eCatalog頁面名稱后面附加一個序號。 您也可以自行輸入名稱。

1. 如果您希望使用者在選取「影像地圖」時開啟新網頁，請在「影像地圖」清單中輸入URL。

   請參閱[以輸入 JavaScript 與 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 若要在使用者將指標移動到影像地圖上方時顯示滑鼠指向效果文字，請在「影像地圖」清單中輸入文字。在「影像地圖」清單中，選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 變換文字]**. 然後輸入您希望使用者在熒幕上看到的文字。 您可以在文字處理器中撰寫該文字，並將其複製到「滑鼠指向效果文字」欄位。

1. 如果要在使用者將滑鼠移動到影像地圖上方時發生其它動作效果，請定義動作。在 **[!UICONTROL 顯示]** 下拉式清單，選取 **[!UICONTROL 其他動作]**. 輸入動作的屬性(前往 **[!UICONTROL 顯示]** > **[!UICONTROL 兩者]** 為「影像地圖」建立滑鼠指向效果文字和動作)。

   另請參閱 [定義影像地圖的其他動作](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (選擇性) 執行下列任一項作業:

   * 若要預覽影像地圖，請選取 **[!UICONTROL 預覽]**.
   * 若要刪除「影像地圖」或多邊形頂點，請選取影像上的形狀，然後選取 **[!UICONTROL 刪除]**. 或者，針對eCatalog，在「訂單頁面」標籤上選取 **[!UICONTROL 清除地圖]** 以從所有頁面中移除影像地圖。
   * 若要暫時移除影像中的影像地圖、迴轉集中的影像或 eCatalog 頁面而不予以刪除，請取消選取「影像地圖」清單中適當的「開啟」選項。

1. 選取 **[!UICONTROL 儲存]**.

### 調整影像地圖的位置、形狀和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

若要變更影像地圖的位置、形狀及大小，請選取「影像地圖」按鈕 。然後，選取 **[!UICONTROL 平移]** 工具並遵循下列指示：

* **變更位置**  — 將指標移到「影像地圖」邊框附近，但不移到「影像地圖」邊框上方。 當您看到四向箭頭圖示時，請將地圖拖曳到新位置。

* **變更大小與形狀**  — 如何變更「影像地圖」的形狀和大小，取決於您是使用矩形或多邊形的「影像地圖」：

>[!TIP]
>
>您可以拖曳畫面下方的「大小」滑桿來變更視圖，以更清楚查看影像地圖。

* **矩形影像地圖**  — 將指標移到「影像地圖」的側邊或角落上方。 當您看到雙向箭頭圖示時，請開始拖曳。拖曳時按住 Shift 鍵即可變更大小，但會維持外觀比例 (形狀)。

* **多邊形影像地圖**  — 拖曳方形選取範圍控點。 若要建立選取範圍控點，請選取「影像地圖」的框線並開始拖曳。

### 處理重疊的影像地圖 {#handling-overlapping-image-maps}

如果影像或 eCatalog 頁面包含多個影像地圖，而地圖有重疊，則您可以決定地圖重疊的方式。若要這樣做，請變更「影像地圖」清單上的地圖順序。在清單上，將地圖名稱拖曳至較高處或較低處。影像地圖名稱在清單上的高度，可決定該影像地圖否覆蓋其它影像地圖。

### 匯入影像地圖資料 {#importing-image-map-data}

您可以為影像、迴轉集或 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入影像地圖資料可為您免除麻煩，就不需要在建立每個影像地圖時，都要在影像地圖清單中輸入資料。

**匯入影像地圖資料:**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 選取 **[!UICONTROL 匯入中繼資料]**.
1. 在「上傳中繼資料」對話方塊中，選取「影像」或「影像地圖」，從所需的資產屬性型別上傳中繼資料。
1. 在「產生檔案」下拉式清單中，選取您想要建立的檔案類型。
1. （選用）選取 **[!UICONTROL 產生]** 以根據您要建立的檔案型別預覽產生的資料。 選取 **[!UICONTROL 關閉]** 返回「上傳中繼資料」對話方塊。
1. 瀏覽至您要上載的檔案。在「檔案名稱」文字欄位中，為產生檔案指定名稱。
1. (選擇性) 在「工作名稱」欄位中，為中繼資料上載工作指定名稱。
1. 選取 **[!UICONTROL 上傳]**.

### 複製影像地圖 {#copying-image-maps}

您可以將影像地圖從某個影像或 eCatalog 頁面複製到另一個影像或 eCatalog 頁面。使用 **[!UICONTROL 複製影像地圖]** 以搶先一步建立它們。 您也可以複製「影像地圖」，以在共用版面或對應結構的影像或頁面中重新建立它們。

例如，如果要在相同的 eCatalog 之各國語言版本之間複製所有影像地圖，直接在 eCatalog 中複製影像地圖就很方便。為獲得最佳效果，在頁數與及影像皆相同的 eCatalog 之間進行複製時，效果最為成功。如果您複製的eCatalog已經包含「影像地圖」，則製作複製時會刪除這些「影像地圖」。

**複製影像地圖:**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 選取 **[!UICONTROL 將地圖複製到]**.
1. 如果您打算從影像或是 eCatalog 複製影像地圖，則請依據個別情況執行以下一項操作:

   * (影像) 在「選取影像」畫面中，選取您要複製影像地圖的目的影像。
   * (eCatalog) 在「選取資產」畫面中，選取您要複製影像地圖的目的影像或 eCatalog 頁面。

1. 選擇 **[!UICONTROL 選取]**.

## 使用範本輸入JavaScript和URL {#using-a-template-to-enter-javascript-and-urls}

您可以定義 URL 範本 (亦稱為 Href 範本)，利用更方便有效的方式輸入影像地圖 URL。如果大多數的影像地圖 URL 共用一個通用的固定格式，則可定義 URL 範本。將固定的 URL 部分輸入 URL 範本之後，每次建立影像地圖時，就不需要輸入這個部分的 URL。URL 範本也可以包含 JavaScript 命令、路徑名稱及參數。根據預設，URL範本包含專有的Adobe Dynamic Media Classic JavaScript處理常式，稱為 `loadProduct` 會在新視窗中開啟影像。

>[!NOTE]
>
>將JavaScript程式碼新增至影像地圖的HREF屬性時，該程式碼會在使用者端的電腦上執行。 因此，請確定JavaScript程式碼是安全的。

### 關於 URL 範本 {#about-url-templates}

URL 範本的運作方式，是以範本中的雙貨幣符號 (「$$」) 取代「影像地圖」清單中的「URL」欄內容:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

您可以在URL範本的影像地圖之間放置所有不會變更的值。 只將會變更的值增加到「影像地圖」清單的「URL」欄中。例如: 

* URL範本 —  `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL值 —  `product.htm`
* 實際產生的URL - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

依預設，URL範本包含專有的Adobe Dynamic Media Classic JavaScript處理常式，稱為 `loadProduct` 會開啟含有URL目的地的新視窗。 不過，您可以使用任何JavaScript程式碼來取代此JavaScript處理常式，或使用下列Adobe Dynamic Media Classic處理常式之一：

* `loadProductCW`  — 顯示在目前視窗的URL欄中指定的URL目標。 這個處理程式主要用於已整合成網站某一頁面的 eCatalog。

* `loadProductPW`  — 在父視窗（開啟目前視窗的頁面）的URL欄中顯示指定的URL目標。 目前視窗會維持開啟，但父級視窗會變更以顯示 URL 目標。

   >[!NOTE]
   >
   >處理程式 `loadProductPW` 不支援 DHTML 和 HTML5 檢視器。

### 建立URL範本 {#creating-a-url-template}

1. 在「地圖編輯器」畫面 (影像或迴轉集) 或 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤上，選取「URL 範本」選項旁的「編輯」。「編輯地圖範本」對話框開啟。
1. 輸入JavaScript程式碼和完整URL （以美元符號取代變數部分） [$$])。 您可以按一下滑鼠右鍵並選擇 **[!UICONTROL 貼上]**.
1. 選取 **[!UICONTROL 儲存]**.

### 處理URL範本 {#handling-url-templates}

「地圖編輯器」頁面 (影像與迴轉集) 與 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤都提供下列命令，以處理 URL 範本:

* **URL範本選項**  — 選取「URL範本」選項，將您的URL範本套用至影像或eCatalog頁面上的所有影像地圖。

* **範本選項**  — 如果您不希望個別影像對映使用URL範本，請取消選取「URL影像對映」清單中的「範本」選項。

## 定義影像地圖的其他動作 {#defining-other-actions-for-image-maps}

您可以選取 **[!UICONTROL 顯示]** 功能表並選擇 **[!UICONTROL 其他動作]** 以觸發滑鼠指向效果文字和網頁啟動以外的動作。 當使用者將指標移動到影像地圖上方，您就可以啟動動作。這些動作是全球資訊網協會 HTML 規格針對用戶端影像地圖所定義的屬性， 包括︰

* **`accesskey`**  — 當使用者按下鍵盤上的指定按鍵時觸發動作。

* **`onfocus`**  — 當影像地圖收到焦點時觸發事件 — 透過游標、Tab鍵或按存取鍵。 例如，您可以在影像地圖成為焦點時啟動網頁，並在影像地圖不再成為焦點時關閉該網頁。

* **`onblur`**  — 當影像地圖失去焦點時觸發事件（游標或Tab鍵瀏覽皆然）。

**定義影像地圖的其它動作:**

1. 在「地圖編輯器」畫面（影像和迴轉集）或eCatalog畫面(eCatalog)的「地圖頁面」標籤上，選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 其他動作]**.
1. 使用全球資訊網協會 HTML 規格所指定的語法，在「影像地圖」清單的「其他動作」欄中增加支援的屬性。
1. 選取 **[!UICONTROL 儲存]**.

選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 兩者]** 如果您希望「影像地圖」有滑鼠指向效果文字和動作。

## 在Adobe Acrobat或Adobe InDesign中建立影像地圖 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

您可以在使用 Adobe Acrobat 或 Adobe InDesign 設計 eCatalog 時建立影像地圖。

在Adobe Acrobat或Adobe InDesign中，建立您想要「影像地圖」出現的超連結參考，並指定影像地圖的URL位置。 選取「擷取連結」選項，將PDF檔案上傳至Adobe Dynamic Media Classic時，會自動將連結轉換為影像地圖。

如需詳細資訊，請參閱Adobe InDesign說明或Adobe Acrobat說明。

### 在 Adobe InDesign 中建立影像地圖 {#to-create-image-maps-in-adobe-indesign}

1. 在Adobe InDesign中，前往 **[!UICONTROL Windows®]** > **[!UICONTROL 互動式]** > **[!UICONTROL 超連結]**.
1. 在「超連結」面板中，選取您要製作成「影像地圖」的文字、框架或圖形。
1. 選取 **[!UICONTROL 新增超連結]** 從面板選單中。
1. 在新增超連結對話方塊中，從 **[!UICONTROL 連結至]** 功能表，選擇 **[!UICONTROL URL]**.
1. 在URL方塊中鍵入或貼上產品ID。
1. 選取 **[!UICONTROL 確定]**. (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)

   >[!NOTE]
   >
   >您不需要在Adobe InDesign中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 針對您要建立的所有影像地圖，重複步驟 2 到 6。
1. 將檔案匯出成 PDF。
1. 將PDF上傳至Adobe Dynamic Media Classic。
1. 在 **[!UICONTROL PDF選項]**，選取 **[!UICONTROL 擷取連結]**.

### 在 Adobe Acrobat 中建立影像地圖 {#to-create-image-maps-in-adobe-acrobat}

1. 在Adobe Acrobat中，前往 **[!UICONTROL 工具]** > **[!UICONTROL 進階編輯]** > **[!UICONTROL 連結工具]**.
1. 拖曳即可建立影像地圖。
1. 在建立連結方塊中，選取 **[!UICONTROL 自訂連結]**，並選取 **[!UICONTROL 下一個]**.

>[!NOTE]
>
>您不需要在Adobe Acrobat中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 在「連結屬性」方塊中，選取 **[!UICONTROL 動作]**.
1. 選取 **[!UICONTROL 開啟網頁連結]** 從「選取動作」功能表，然後選取 **[!UICONTROL 新增]**.
1. 在「編輯URL」方塊中輸入「影像地圖」的產品ID，然後選取 **[!UICONTROL 確定]**. (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)
1. 針對您要建立的所有影像地圖，重複步驟 1 到 7。
1. 儲存檔案。
1. 將PDF上傳至Adobe Dynamic Media Classic，然後從「PDF選項」中選取「擷取連結」 。
