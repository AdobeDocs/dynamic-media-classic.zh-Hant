---
title: 建立影像地圖
description: 瞭解如何在Adobe Dynamic Media Classic中建立影像地圖。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 31%

---

# 建立影像地圖 {#creating-image-maps}

「影像地圖」是影像、eCatalog頁面上的區域，或SpinSet中顯示包含文字的滑鼠指向效果面板的影像。 當使用者選取影像地圖時，就會觸發某種動作。 例如，啟動網頁以便使用者進一步瞭解產品。 當使用者將指標移到「影像地圖」上時，其周圍會顯示一個外框。

除了在Adobe Dynamic Media Classic中建立影像地圖功能以外，當您在Adobe Acrobat或Adobe InDesign中設計目錄時，也可以建立影像地圖。

當您建立「影像地圖」時，可以執行下列任一項作業：

* 輸入滑鼠指向效果文字。
* 輸入JavaScript和啟動網頁的URL。
* 為影像地圖建立 URL 範本。
* 將影像地圖複製到其它影像、eCatalog 頁面或迴轉集中。
* 將影像地圖匯出至 CSV 或 XML。
* 從以Tab分隔的檔案或XML檔案匯入影像中繼資料。
* 定義由全球資訊網協會決定的其他動作。
* 預覽影像地圖。

## 繪製和調整影像地圖 {#drawing-and-adjusting-an-image-map}

1. 進行以下一項操作:

   * 如果您正在處理格線檢視或清單檢視中的影像，請在「編輯」下拉式清單中選取&#x200B;**[!UICONTROL 影像地圖]**。 或者，在[詳細資料檢視]中開啟，然後選取影像上方的&#x200B;**[!UICONTROL 影像地圖]**。
   * 如果您正在使用格線檢視或清單檢視中的迴轉集，請選取&#x200B;**[!UICONTROL 編輯]**。 或者，在[詳細資料檢視]中開啟，然後選取[編輯]。**** 選取影像資產，然後選取&#x200B;**[!UICONTROL 影像地圖]**。
   * 如果您正在使用eCatalog，請在[網格檢視]、[清單檢視]、[詳細資料檢視]中選取&#x200B;**[!UICONTROL 編輯]**。 選取&#x200B;**[!UICONTROL 對應頁面]**&#x200B;索引標籤。

   ![影像地圖插圖](assets/ma_image_map.png)

1. 繪製矩形或多邊形影像地圖:

   * **矩形對應**：選取「矩形影像對應」工具，並在頁面上拖曳以建立矩形。 若要將點新增至矩形對映（因此將其變更為多邊形對映），請按下Ctrl，然後將插入工具放置在所需位置並選取。

   * **多邊形對映**：選取「多邊形影像對映」工具，並選取要包圍的影像區域周邊上的點。 使用多邊形密度滑桿，讓多邊形的點密度產生差異。如果選取其它地圖，則會記憶原始密度。如果在多邊形中新增、刪除或移動任何點，原始密度就會遺失。 滑桿會重設為其最大值。

1. 如有需要，可在「影像地圖」清單中輸入影像地圖的名稱。繪製影像地圖後，Adobe Dynamic Media Classic會為其指定一個名稱。

   若要建立名稱，Adobe Dynamic Media Classic會在您使用的影像或eCatalog頁面名稱后面附加一個循序號碼。 您也可以自行輸入名稱。

1. 如果您希望使用者在選取「影像地圖」時開啟新的網頁，請在「影像地圖」清單中輸入URL。

   請參閱[以輸入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 若要在使用者將指標移動到影像地圖上方時顯示滑鼠指向效果文字，請在「影像地圖」清單中輸入文字。在「影像地圖」清單中，選取&#x200B;**[!UICONTROL 顯示]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 滑鼠指向效果文字]**。 然後輸入您希望使用者在熒幕上看到的文字。 您可以在文字處理器中撰寫該文字，並將其複製到「滑鼠指向效果文字」欄位。

1. 如果要在使用者將滑鼠移動到影像地圖上方時發生其它動作效果，請定義動作。在&#x200B;**[!UICONTROL 顯示]**&#x200B;下拉式清單中，選取&#x200B;**[!UICONTROL 其他動作]**。 輸入動作的屬性（移至&#x200B;**[!UICONTROL 顯示]** > **[!UICONTROL 兩者]**&#x200B;以建立影像地圖的變換文字與動作。）

   請參閱[定義影像地圖的其他動作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. (選擇性) 執行下列任一項作業:

   * 若要預覽影像地圖，請選取&#x200B;**[!UICONTROL 預覽]**。
   * 若要刪除影像地圖或多邊形頂點，請選取影像上的形狀，然後選取&#x200B;**[!UICONTROL 刪除]**。 或者，若是eCatalog，請在[排序頁面]索引標籤上選取[清除對映] **[!UICONTROL ，以從所有頁面移除影像對映。]**
   * 若要移除：
      * 影像中的影像地圖
      * 迴轉集中的影像
      * 或eCatalog頁面

     暫時取消選取「影像地圖」清單中適當的「開啟」選項，而不刪除它。

1. 選取&#x200B;**[!UICONTROL 儲存]**。

### 調整影像地圖的位置、形狀和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

若要變更「影像地圖」的位置、形狀和大小，請選取「影像地圖」按鈕。 接著，選取&#x200B;**[!UICONTROL 平移]**&#x200B;工具，並依照下列指示進行：

* **變更位置**：將指標移近影像地圖的框線，但不要移過框線。 當您看到四向箭頭圖示時，請將地圖拖曳到新位置。

* **變更大小和形狀**：您如何變更影像地圖的形狀和大小，取決於您是使用矩形或多邊形影像地圖：

>[!TIP]
>
>您可以拖曳畫面下方的「大小」滑桿來變更視圖，以更清楚查看影像地圖。

* **矩形影像地圖**：將指標移到影像地圖的邊或角上。 當您看到雙向箭頭圖示時，請開始拖曳。按住Shift鍵拖曳以變更大小，但維持外觀比例（形狀）。

* **多邊形影像地圖**：拖曳方形選取範圍控點。 若要建立選取範圍控點，請選取「影像地圖」的框線並開始拖曳。

### 處理重疊的影像地圖 {#handling-overlapping-image-maps}

如果您的影像或eCatalog頁面包含多個影像地圖且地圖重疊，您可以決定地圖重疊的方式。 若要這樣做，請變更「影像地圖」清單上的地圖順序。在清單上，將地圖名稱拖曳至較高處或較低處。影像地圖名稱在清單上的高度，可決定該影像地圖否覆蓋其它影像地圖。

### 匯入影像地圖資料 {#importing-image-map-data}

您可以為影像、迴轉集或 eCatalog 匯入資料至「地圖摘要」畫面，而不用在各個頁面上輸入影像地圖資料。匯入影像地圖資料時，可以採用 Tab 字元分隔檔案或 XML DTD 的格式。檔案中的欄位必須依照「地圖摘要」畫面所顯示的順序:「名稱」、「TOC 標籤」、「地圖」、「URL」、「滑鼠指向效果文字」、「其它動作」與「搜尋字串」。匯入「影像地圖」資料可讓您在建立每個「影像地圖」時，在「影像地圖」清單中輸入資料的麻煩。

**若要匯入影像地圖資料：**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 選取&#x200B;**[!UICONTROL 匯入中繼資料]**。
1. 在「上傳中繼資料」對話方塊中，選取「影像」或「影像地圖」，從所需的資產屬性型別上傳中繼資料。
1. 在`Generate File`下拉式清單中，選取您要建立的檔案型別。
1. （選擇性）選取&#x200B;**[!UICONTROL 產生]**&#x200B;以根據您要建立的檔案型別預覽產生的資料。 選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回「上載中繼資料」對話方塊。
1. 瀏覽至您要上載的檔案。在「檔案名稱」文字欄位中，為產生檔案指定名稱。
1. (選擇性) 在「工作名稱」欄位中，為中繼資料上載工作指定名稱。
1. 選取&#x200B;**[!UICONTROL 上傳]**。

### 複製影像地圖 {#copying-image-maps}

您可以將影像地圖從某個影像或 eCatalog 頁面複製到另一個影像或 eCatalog 頁面。使用&#x200B;**[!UICONTROL 複製影像地圖]**&#x200B;以開始建立它們。 您也可以複製「影像地圖」，以在共用版面或地圖結構的影像或頁面中重新建立它們。

例如，在eCatalog中複製影像地圖是在相同eCatalog的外文版本之間複製所有影像地圖的便利方式。 為達到最佳效果，如果您在相同頁數的eCatalog與相同影像之間複製，復製作業將最成功。 如果您要複製的eCatalog已經包含「影像地圖」，則製作複製時會刪除這些「影像地圖」。

**複製影像地圖：**

1. 前往「影像地圖」編輯器頁面 (針對影像或迴轉集中的影像) 或是 eCatalog 編輯畫面的「地圖頁面」標籤。
1. 選取&#x200B;**[!UICONTROL 將地圖複製到]**。
1. 如果您打算從影像或是 eCatalog 複製影像地圖，則請依據個別情況執行以下一項操作:

   * (影像) 在「選取影像」畫面中，選取您要複製影像地圖的目的影像。
   * (eCatalog) 在「選取資產」畫面中，選取您要複製影像地圖的目的影像或 eCatalog 頁面。

1. 選擇&#x200B;**[!UICONTROL 選取]**。

## 使用範本輸入JavaScript和URL {#using-a-template-to-enter-javascript-and-urls}

您可以定義 URL 範本 (亦稱為 Href 範本)，利用更方便有效的方式輸入影像地圖 URL。如果大多數的影像地圖 URL 共用一個通用的固定格式，則可定義 URL 範本。將固定的 URL 部分輸入 URL 範本之後，每次建立影像地圖時，就不需要輸入這個部分的 URL。您的URL範本也可以包含JavaScript命令、路徑名稱和引數。 根據預設，URL範本包含名為`loadProduct`的專屬Adobe Dynamic Media Classic JavaScript處理常式，可在新視窗中開啟影像。

>[!NOTE]
>
>將JavaScript程式碼新增至影像地圖的HREF屬性時，該程式碼會在使用者端電腦上執行。 因此，請確定JavaScript程式碼是安全的。

### 關於 URL 範本 {#about-url-templates}

URL範本的運作方式是取代「影像地圖」清單中URL欄的內容。 在範本中使用雙美元符號(「$$」)加以取代：

```as3
Javascript:loadProduct('$$');void(0);
```

您可以在URL範本中的影像地圖之間放置所有不會變更的值。 只將會變更的值增加到「影像地圖」清單的「URL」欄中。例如: 

* URL範本： `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* URL值： `product.htm`
* 實際產生的URL： `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

根據預設，URL範本包含名為`loadProduct`的專屬Adobe Dynamic Media Classic JavaScript處理常式，可開啟包含URL目的地的新視窗。 不過，您可以使用任何JavaScript程式碼來取代此JavaScript處理常式，或使用下列其中一個Adobe Dynamic Media Classic處理常式：

* `loadProductCW`：顯示目前視窗的URL資料行中所指定的URL目標。 這個處理程式主要用於已整合成網站某一頁面的 eCatalog。

* `loadProductPW`：顯示父視窗（開啟目前視窗的頁面）的URL欄中所指定的URL目標。 目前視窗會維持開啟，但父級視窗會變更以顯示 URL 目標。

  >[!NOTE]
  >
  >處理常式`loadProductPW`不支援DHTML和HTML5檢視器。

### 建立URL範本 {#creating-a-url-template}

1. 在「地圖編輯器」畫面（影像或迴轉集）或eCatalog畫面的「地圖頁面」索引標籤(eCatalogs)上，選取URL範本選項旁的「編輯」。 「編輯地圖範本」對話框開啟。
1. 輸入JavaScript程式碼和完整URL （以貨幣符號[$$]取代變數部分）。 您可以按一下滑鼠右鍵並選擇&#x200B;**[!UICONTROL 貼上]**&#x200B;來貼上程式碼。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

### 處理URL範本 {#handling-url-templates}

「地圖編輯器」頁面 (影像與迴轉集) 與 eCatalog 畫面 (eCatalog) 的「地圖頁面」標籤都提供下列命令，以處理 URL 範本:

* **URL範本選項**：選取URL範本選項，以將您的URL範本套用至影像或eCatalog頁面上的所有影像地圖。

* **範本選項**：如果您不希望個別影像地圖使用URL範本，請取消選取「URL影像地圖」清單中的「範本」選項。

## 定義影像地圖的其他動作 {#defining-other-actions-for-image-maps}

您可以選取「**[!UICONTROL 顯示]**」功能表，然後選擇「**[!UICONTROL 其他動作]**」來觸發滑鼠指向效果文字和網頁啟動以外的動作。 當使用者將指標移動到影像地圖上方，您就可以啟動動作。這些動作是全球資訊網協會 HTML 規格針對用戶端影像地圖所定義的屬性， 包括︰

* **`accesskey`**：當使用者按下鍵盤上的指定鍵時會觸發動作。

* **`onfocus`**：影像地圖收到焦點時觸發事件 — 透過游標、Tab鍵或按存取鍵。 例如，您可以在影像地圖收到焦點時啟動網頁，並在影像地圖失去焦點時關閉網頁。

* **`onblur`**：影像地圖失去焦點時觸發事件（游標或Tab鍵）。

**若要定義影像地圖的其他動作：**

1. 在「地圖編輯器」畫面（影像和迴轉集）或eCatalog畫面(eCatalog)的「地圖頁面」索引標籤上，選取「**[!UICONTROL 顯示]**」功能表，然後選取「**[!UICONTROL 其他動作]**」。
1. 使用全球資訊網協會 HTML 規格所指定的語法，在「影像地圖」清單的「其他動作」欄中增加支援的屬性。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

如果您想要影像地圖有滑鼠指向效果文字和動作，請選取&#x200B;**[!UICONTROL 顯示]**&#x200B;功能表並選取&#x200B;**[!UICONTROL 兩者]**。

## 在Adobe Acrobat或Adobe InDesign中建立影像地圖 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

您可以在使用 Adobe Acrobat 或 Adobe InDesign 設計 eCatalog 時建立影像地圖。

在Adobe Acrobat或Adobe InDesign中，建立您要在其中顯示影像地圖的超連結參考，並指定影像地圖的URL位置。 選取「擷取連結」選項，將PDF檔案上傳至Adobe Dynamic Media Classic時，會自動將連結轉換為影像地圖。

如需詳細資訊，請參閱Adobe InDesign說明或Adobe Acrobat說明。

### 在 Adobe InDesign 中建立影像地圖 {#to-create-image-maps-in-adobe-indesign}

1. 在Adobe InDesign中，移至&#x200B;**[!UICONTROL Windows®]** > **[!UICONTROL 互動式]** > **[!UICONTROL 超連結]**。
1. 在「超連結」面板中，選取您要製作成「影像地圖」的文字、框架或圖形。
1. 從面板選單中選取&#x200B;**[!UICONTROL 新增超連結]**。
1. 在[新增超連結]對話方塊中，從&#x200B;**[!UICONTROL [連結至]**]功能表選擇&#x200B;**[!UICONTROL URL]**。
1. 在URL方塊中，輸入或貼上產品ID。
1. 選取&#x200B;**[!UICONTROL 確定]**。 (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)

   >[!NOTE]
   >
   >您不需要在Adobe InDesign中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 針對您要建立的所有影像地圖，重複步驟 2 到 6。
1. 將檔案匯出成 PDF。
1. 將PDF上傳至Adobe Dynamic Media Classic。
1. 在&#x200B;**[!UICONTROL PDF選項]**&#x200B;中，選取&#x200B;**[!UICONTROL 擷取連結]**。

### 在 Adobe Acrobat 中建立影像地圖 {#to-create-image-maps-in-adobe-acrobat}

1. 在Adobe Acrobat中，移至&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 進階編輯]** > **[!UICONTROL 連結工具]**。
1. 拖曳以建立影像地圖。
1. 在[建立連結]方塊中，選取[**[!UICONTROL 自訂連結]**]，然後選取[**[!UICONTROL 下一步]**]。

>[!NOTE]
>
>您不需要在Adobe Acrobat中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 在[連結屬性]方塊中，選取&#x200B;**[!UICONTROL 動作]**。
1. 從[選取動作]功能表選取[開啟網頁連結]****，然後選取[新增]****。
1. 在[編輯URL]方塊中輸入[影像地圖]的產品ID，然後選取[確定]。**** (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)
1. 針對您要建立的所有影像地圖，重複步驟 1 到 7。
1. 儲存檔案。
1. 將PDF上傳至Adobe Dynamic Media Classic，然後選取「從PDF選項擷取連結」 。
