---
title: 建立影像地圖
seo-title: 建立影像地圖
description: 'null'
seo-description: 瞭解如何建立影像地圖。
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/master_ files
discoiquuid: eddf983-38cb-4f00-b3 be-85c20 bdd6 f69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 建立影像地圖{#creating-image-maps}

影像地圖是影像、eCatalog 頁面，或迴轉集之影像中的某個區域，可顯示內含滑鼠指向效果文字的面板。使用者按一下「影像地圖」時，就會觸發某種動作。例如，啟動網頁讓使用者進一步瞭解產品。為了吸引使用者注意到影像地圖，當使用者將指標移到影像地圖上時，其周圍會出現外框。

除了能夠在Dynamic Media Classic中建立影像地圖外，您也可以在Adobe Acrobat或Adobe InDesign中設計目錄時建立影像地圖。

建立影像地圖時，您可以執行下列任一動作:

* 輸入滑鼠指向效果文字。
* 輸入用來啟動網頁的 JavaScript 與 URL。
* 為影像地圖建立 URL 範本。
* 將影像地圖複製到其它影像、eCatalog 頁面或迴轉集中。
* 將影像地圖匯出至 CSV 或 XML。
* 從 Tab 字元分隔檔案或 XML 檔案匯入影像中繼資料。
* 定義其它由全球資訊網協會決定的動作。
* 預覽影像地圖。

## 繪製和調整影像地圖 {#drawing-and-adjusting-an-image-map}

1. 進行以下一項操作:

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. Click the **Map Pages** tab.
   ![](assets/ma_image_map.png)

1. 繪製矩形或多邊形影像地圖:

   **矩形地圖** 選取矩形影像地圖工具並拖曳頁面以建立矩形。若要為矩形地圖增加一個點 (將它變成多邊形地圖)，請按 Ctrl 鍵，然後將插入工具放在想要的位置，再按一下滑鼠。

   **多邊形地圖** 選取多邊形影像地圖工具，並在想要關閉的影像區域周圍按一下點。使用多邊形密度滑桿，讓多邊形的點密度產生差異。如果選取其它地圖，則會記憶原始密度。如果在多邊形中增加、刪除或移動任一點，則會遺失原始密度，並將滑桿重設回最大值。

1. 如有需要，可在「影像地圖」清單中輸入影像地圖的名稱。在您繪制影像地圖後，Dynamic Media Classic會指派它名稱。

   若要建立名稱，Dynamic Media Classic會附加循序數字至您正在使用的影像或eCatalog頁面名稱。您也可以自行輸入名稱。

1. 如果要讓使用者在按一下影像地圖時開啟新網頁，請在「影像地圖」清單中輸入 URL。

   請參閱[以輸入 JavaScript 與 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 若要在使用者將指標移動到影像地圖上方時顯示滑鼠指向效果文字，請在「影像地圖」清單中輸入文字。在「影像地圖」清單中，選取「顯示」選單，然後選擇「滑鼠指向效果文字」。接著輸入要讓使用者在螢幕上看到的文字。您可以在文字處理器中撰寫該文字，並將其複製到「滑鼠指向效果文字」欄位。
1. 如果要在使用者將滑鼠移動到影像地圖上方時發生其它動作效果，請定義動作。在「顯示」下拉式清單中，按一下「其它動作」。輸入動作的屬性(按一下「顯示 &gt; 兩者」以為影像地圖建立滑鼠指向效果文字與動作。)

   請參閱[為影像地圖定義其它動作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. (選擇性) 執行下列任一項作業:

   * 按一下「預覽」以預覽影像地圖。
   * 若要刪除影像地圖或多邊形頂點，請在影像中選取一個形狀，然後按一下「刪除」。或者，如果是 eCatalog，則在「排序頁面」標籤上按一下「清除地圖」以從所有頁面移除影像地圖。
   * 若要暫時移除影像中的影像地圖、迴轉集中的影像或 eCatalog 頁面而不予以刪除，請取消選取「影像地圖」清單中適當的「開啟」選項。

1. 按一下「儲存」。

### 調整影像地圖的位置、形狀及大小 {#adjusting-the-position-shape-and-size-of-image-maps}

若要變更影像地圖的位置、形狀及大小，請選取「影像地圖」按鈕 。然後，選取「平移」工具並遵循下列指示：

**變更位置：** 將指標移至接近但不限於影像地圖邊框的位置。當您看到四向箭頭圖示時，請將地圖拖曳到新位置。

**變更影像地圖形狀和大小** 的大小和形狀，視您使用矩形或多邊形影像地圖而定：

***秘訣**：您可以拖曳畫面底部的「大小」滑桿來變更檢視，並更好地查看影像地圖。*

**矩形影像地圖** 將指標移到影像地圖的一側或角落。當您看到雙向箭頭圖示時，請開始拖曳。拖曳時按住 Shift 鍵即可變更大小，但會維持外觀比例 (形狀)。

**多邊形影像地圖** 拖曳正方形選取範圍控制點。若要建立選取範圍控制點，請按一下影像地圖的邊框，然後開始拖曳。

### 處理重疊影像地圖 {#handling-overlapping-image-maps}

如果影像或 eCatalog 頁面包含多個影像地圖，而地圖有重疊，則您可以決定地圖重疊的方式。若要這樣做，請變更「影像地圖」清單上的地圖順序。在清單上，將地圖名稱拖曳至較高處或較低處。影像地圖名稱在清單上的高度，可決定該影像地圖否覆蓋其它影像地圖。

### 匯入影像地圖資料 {#importing-image-map-data}

您可以為影像、迴轉集或 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入影像地圖資料可為您免除麻煩，就不需要在建立每個影像地圖時，都要在影像地圖清單中輸入資料。

**匯入影像地圖資料**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 按一下「匯入中繼資料」。
1. 在「上載中繼資料」對話框中，按一下「影像」或「影像地圖」，以從想要的資產屬性類型上載中繼資料。
1. 在「產生檔案」下拉式清單中，選取您想要建立的檔案類型。
1. (選擇性) 按一下「產生」即可依據您要建立的檔案類型預覽最終的資料。按一下「關閉」即可返回「上載中繼資料」對話框。
1. 瀏覽至您要上載的檔案。在「檔案名稱」文字欄位中，為產生檔案指定名稱。
1. (選擇性) 在「工作名稱」欄位中，為中繼資料上載工作指定名稱。
1. 按一下「上載」。

### 複製影像地圖 {#copying-image-maps}

您可以將影像地圖從某個影像或 eCatalog 頁面複製到另一個影像或 eCatalog 頁面。使用「複製影像地圖」可以更快開始建立影像地圖。您也可複製影像地圖，以在共用相同版面或對應結構的影像或頁面中，重新建立這些影像地圖。

例如，如果要在相同的 eCatalog 之各國語言版本之間複製所有影像地圖，直接在 eCatalog 中複製影像地圖就很方便。為獲得最佳效果，在頁數與及影像皆相同的 eCatalog 之間進行複製時，效果最為成功。如果您複製的目標 eCatalog 中已包含影像地圖，則這些影像地圖會在複製時刪除。

**複製影像地圖**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 按一下「複製地圖至」。
1. 如果您打算從影像或是 eCatalog 複製影像地圖，則請依據個別情況執行以下一項操作:

   * (影像) 在「選取影像」畫面中，選取您要複製影像地圖的目的影像。
   * (eCatalog) 在「選取資產」畫面中，選取您要複製影像地圖的目的影像或 eCatalog 頁面。

1. 按一下「選取」。

## 使用範本來輸入 JavaScript 與 URL {#using-a-template-to-enter-javascript-and-urls}

您可以定義 URL 範本 (亦稱為 Href 範本)，利用更方便有效的方式輸入影像地圖 URL。如果大多數的影像地圖 URL 共用一個通用的固定格式，則可定義 URL 範本。將固定的 URL 部分輸入 URL 範本之後，每次建立影像地圖時，就不需要輸入這個部分的 URL。URL 範本也可以包含 JavaScript 命令、路徑名稱及參數。By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>請注意，當您增加 Javascript 程式碼至影像地圖的 HREF 屬性時，程式碼是在用戶端電腦上執行。因此，請確定 Javascript 程式碼是安全的。

### 關於 URL 範本 {#about-url-templates}

URL 範本的運作方式，是以範本中的雙貨幣符號 (「$$」) 取代「影像地圖」清單中的「URL」欄內容:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

您可以將影像地圖中所有不會變更的值放入 URL 範本。只將會變更的值增加到「影像地圖」清單的「URL」欄中。例如: 

* URL範本：j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL值： `product.htm`
* 產生的實際URL： `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. 不過，您可以使用任何JavaScript程式碼取代此JavaScript處理常式或使用下列其中一個Dynamic Media Classic處理常式：

* `loadProductCW`

   顯示在目前視窗之「URL」欄中指定的 URL 目標。這個處理程式主要用於已整合成網站某一頁面的 eCatalog。

* `loadProductPW`

   顯示在父級視窗 (開啟目前視窗的頁面) 之「URL」欄中指定的 URL 目標。目前視窗會維持開啟，但父級視窗會變更以顯示 URL 目標。

   ***附註**：處理常式`loadProductPW`不支援DHTML和HTML檢視器。*

### 建立 URL 範本 {#creating-a-url-template}

建立 URL 範本︰

1. 在「地圖編輯器」畫面 (影像或迴轉集) 或 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤上，選取「URL 範本」選項旁的「編輯」。「編輯地圖範本」對話框開啟。
1. Enter the JavaScript code and the complete URL (with the variable portion replaced by dollar signs [$$]). 用滑鼠右鍵按一下，然後選擇「貼上」，即可貼上程式碼。
1. 選取「儲存」按鈕。

### 處理 URL 範本 {#handling-url-templates}

「地圖編輯器」頁面 (影像與迴轉集) 與 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤都提供下列命令，以處理 URL 範本:

**URL範本選項** ：選擇「URL範本」選項，將您的URL範本套用至影像或eCatalog頁面上的所有影像地圖。

**如果您不希望個別影像地圖使用URL範本，則範本選項** 會取消選取URL影像地圖清單中的「範本」選項。

## 為影像地圖定義其它動作 {#defining-other-actions-for-image-maps}

選取「顯示」選單，然後選擇「其他動作」，即可觸發滑鼠指向效果文字以外的動作，進而啟動網頁。當使用者將指標移動到影像地圖上方，您就可以啟動動作。這些動作是全球資訊網協會 HTML 規格針對用戶端影像地圖所定義的屬性， 包括︰

**accesskey** 會在使用者按下鍵盤上指定的按鍵時觸發動作。

**焦點** 會在影像地圖收到焦點(由游標、標籤或按下存取金鑰)時觸發事件。例如，您可以在影像地圖成為焦點時啟動網頁，並在影像地圖不再成為焦點時關閉該網頁。

**onblr** 會在影像地圖遺失焦點(由游標或標籤)遺失時觸發事件。

**定義影像地圖的其它動作**

1. 在「地圖編輯器」畫面 (影像與迴轉集) 或 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤上，選取「顯示」選單，然後選擇「其它動作」。
1. 使用全球資訊網協會 HTML 規格所指定的語法，在「影像地圖」清單的「其他動作」欄中增加支援的屬性。
1. 按一下&#x200B;**「儲存」**。

如果要讓影像地圖同時具備滑鼠指向效果文字與動作，請選取「顯示」選單，然後選擇「兩者」。

## 使用 Adobe Acrobat 或 Adobe InDesign 建立影像地圖 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

您可以在使用 Adobe Acrobat 或 Adobe InDesign 設計 eCatalog 時建立影像地圖。

使用 Acrobat 或 InDesign 時，在您要顯示影像地圖的位置建立超連結參照，然後針對影像地圖指定 URL 位置。上傳PDF檔案至Dynamic Media Classic時選取「摘取連結」選項，會自動轉換「影像地圖」的連結。

如需詳細資訊，請參閱 InDesign 說明或 Acrobat 說明。

### 在 Adobe InDesign 中建立影像地圖 {#to-create-image-maps-in-adobe-indesign}

1. 在 InDesign 中，按一下「視窗 &gt; 互動式 &gt; 超連結」，即可開啟「超連結」面板。
1. 選取要成為影像地圖的文字、框架或圖形。
1. 在「超連結」面板中，按一下面板選單中的「新增超連結」。
1. 在「新增超連結」對話框中，從「連結至」選單選擇「URL」。
1. 在「URL」方框中輸入或貼上產品，然後按一下「確定」 (Dynamic Media Classic使用Image Map URL範本完成URL)。

   >[!NOTE]
   >
   >您不需要在 InDesign 中設定外觀選項。您可以在Dynamic Media Classic中指定外觀。

1. 針對您要建立的所有影像地圖，重複步驟 2 到 5。
1. 將檔案匯出成 PDF。
1. 將PDF上傳至Dynamic Media Classic，然後從PDF選項中選取摘取連結。

### 在 Adobe Acrobat 中建立影像地圖 {#to-create-image-maps-in-adobe-acrobat}

1. 在 Acrobat 中，選擇「工具 &gt; 進階編輯 &gt; 連結工具」。
1. 拖曳即可建立影像地圖。「建立連結」方框開啟。
1. 選取「自訂連結」，然後按「下一步」。

   ***附註**：您不需要在Acrobat中設定外觀選項。您可以在Dynamic Media Classic中指定外觀。*

1. 在「連結屬性」方框中，按一下「動作」。
1. 從「選取動作」選單中選取「開啟網頁連結」，然後按一下「增加」。
1. 在「編輯 URL」方框中輸入影像地圖的產品 ID，然後按一下「確定」 (Dynamic Media Classic會使用影像地圖URL範本完成URL。)
1. 針對您要建立的所有影像地圖，重複步驟 1 到 7。
1. 儲存檔案。
1. 將PDF上傳至Dynamic Media Classic，然後從PDF選項中選取摘取連結。
