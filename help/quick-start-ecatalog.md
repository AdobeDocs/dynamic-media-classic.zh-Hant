---
title: 「快速入門：eCatalogs」
seo-title: 「快速入門：eCatalogs」
description: 'null'
seo-description: eCatalogs簡介和快速入門，可協助您快速上手使用eCatalog技術。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: 管理員
content-type: 參考
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: e1b74f30faab334453f941e9075910c8a8565462

---


# 快速入門：eCatalogs{#quick-start-ecatalogs}

eCatalog 為列印材料的數位網頁版本 — 例如目錄、傳單、文宣、產品手冊或廣告傳單。eCatalog 顯示於網站上的 eCatalog 檢視器中。此檢視器會模擬閱讀列印材料的體驗。視您為eCatalog選擇的設定而定，檢視器可讓您執行下列動作：

* 搜尋目錄以尋找關鍵字或關鍵字。 搜尋結果會在目錄左側的搜尋面板中顯示為縮圖清單。 每個可點按的縮圖代表一個目錄跨頁，其中已找到反白顯示的搜尋詞。

* 通過社交媒體分享目錄；下載目錄以離線檢視；啟用「我的最愛」，以快速標籤您要傳回的項目，或列印目錄。
* 使用目錄或頁面格線檢視導覽目錄；按一下頁面的中間邊緣，即可向前或向後顯示頁面。
* 放大、縮小與平移即可檢查頁面上的項目。
* 將指標移動到某個頁面區域 (稱為「影像地圖」) 即可檢視含有項目相關資訊的彈出式視窗。
* 按一下頁面區域即可開啟含有更多項目相關資訊的新網頁。
* 撰寫註解並將其附加到 eCatalog 頁面。
* 點選影像地圖圖示即可啟動相關網頁或有關上下文的資訊面板。
* 使用手勢互動，包括雙指縮放與揮動翻頁。
* 依項目關鍵字搜尋。

![eCatalog 顯示給使用者的外觀。A)eCatalog開啟頁面。 B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

為了建立 eCatalog，一般會使用 Adobe® Acrobat® 或其他列印程式中建立的高解析度 PDF 檔案，但也可以從影像檔建立 eCatalog。

建立 eCatalog 時，您可以依選擇的順序安排頁面或頁面跨頁。您也可以指定要採用單一頁面、雙頁式跨頁或多頁式跨頁。您可以為頁面區域建立影像地圖，以便檢視者可以進行不同操作，如按一下頁面上的某個區域，以及在網站上開啟新頁面。您可以使用 eCatalog 畫面中的「資訊面板」設定來管理顯示的滑鼠指向效果文字。您也可從超過 100 個不同的設定選項中選擇，以設定 eCatalog 檢視器。您可以為特定對象量身訂作檢視器的功能與外觀。

>[!NOTE]
>
>如果您是AEM Dynamic Media - Scene7模式使用者，並想要使用eCatalogs，則需要在CRXDE Lite中 `pdfbrochure` 編輯值。 若要這麼做，請在AEM中按一下「 **[UICONTROL工具&gt;一般&gt; CRXDE Lite]**」。 在左側面板導覽樹狀結構中，導覽至 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`。
在右下方窗格的「屬性 **」頁籤** ，選擇 `jobParam` 行。 將值從 `pdfbrochure` 到 `false` 設定 `true`。 如同 `pdfbrochure=true`在CRXDE Lite頁面的左上角，按一下「全 **部儲存」**。
您現在可以在SPS中製作eCatalog。

**快速入門**

「eCatalog 快速入門」的設計可讓您迅速熟練 eCatalog。依照步驟 1 至 7 執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

**1. 上載 PDF 檔案**

Adobe PDF 檔案通常是 eCatalog 的來源。因為 PDF 檔案須列印，所以通常包含 CMYK 影像。Scene7 Publishing System 會偵測這些影像，並使用標準 CMYK 色彩設定檔來加以轉換。不過，您可能需要上載並使用自訂的色彩設定檔。

按一下全域導覽列上的「上傳」，開始上傳eCatalog的PDF檔案或影像。 您可以從桌面或透過 FTP 上載檔案；如果您上載多個檔案或檔案大小超過 100 MB，則建議使用 FTP。

在 PDF 選項之下，「上載」畫面提供以適當解析度與正確色域上載 PDF 檔案的選項。建議使用每英吋 150 像素的解析度。上載 PDF 檔案時，您可以選取「自動產生 eCatalog」選項來建立 eCatalog。

請參閱[上載 PDF 檔案](uploading-pdf-files.md#uploading_the_pdf_files)。

**2. 建立 eCatalog**

在瀏覽面板中選取 PDF 或影像檔案，然後按一下「建置」按鈕並選擇 eCatalog 來建立 eCatalog。「eCatalog」畫面開啟。

在「排序頁面」標籤上選取「版面」按鈕 —「1 欄式」、「2 欄式」或「自訂」— 即可選擇是否採用單一頁面、雙頁式跨頁或自訂跨頁。您可以拖曳頁面，或是在大型的eCatalog 的「移動至」選單上選擇頁面名稱，來重新排序頁面或跨頁。

若要新增頁面，請在資產庫中選取檔案夾，然後將 PDF 或影像檔案從檔案夾拖曳至「排序頁面」畫面。除了預設頁碼外，您可以提供自訂頁面名稱或匯入大量的頁面名稱。

按一下「儲存」按鈕，接著輸入 eCatalog 名稱，再選擇用來存放該 eCatalog 的 SPS 檔案夾，然後選取「儲存」按鈕。每次變更頁面順序或編輯 eCatalog 時，請按一下「儲存」按扭來儲存變更。

請參閱[建立 eCatalog](creating-ecatalog.md)。

**3. 建立影像地圖**

影像地圖會將其他尺寸增加到 eCatalog 頁面。影像地圖是頁面的某個區域，提供更多有關項目的資訊。檢視者捲動指標至影像地圖上時，就會看到項目的描述。按一下影像地圖會啟動外部參照，它會開啟一個新網頁，您可以在其中瞭解更多有關項目的資訊。

若要建立影像地圖，請開啟「eCatalog」畫面。然後前往「eCatalog」畫面的「地圖頁面」標籤，並使用矩形影像地圖工具  或多邊形影像地圖工具  來繪製地圖。您可以使用平移工具  來拖曳地圖邊框，以調整影像地圖的位置與大小。

繪製影像地圖之後，輸入按一下影像地圖時要前往的 URL 位址。您也可以輸入將指標移動到影像地圖上時會顯示的滑鼠指向效果文字。

請參閱[建立 eCatalog 影像地圖](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)。

請參閱[使用影像地圖在 eCatalog 中內嵌豐富媒體](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)。

您可以使用「eCatalog」畫面中的「資訊面板」設定，來設定和管理影像地圖文字。

請參閱[管理資訊面板內容](info-panel-content.md#managing-info-panel-content)。

**4. 設定 eCatalog 檢視器預設集**

終端使用者會在 eCatalog 檢視器中檢視您的 eCatalog。如果您是管理員，便可以設定 eCatalog 檢視器。您可以變更其外框色彩，並選取新的「外觀」，讓 eCatalog 擁有品牌特色。Dynamic Media Classic隨附數種「最佳實務」eCatalog檢視器預設集。 您可以選擇其中一個預設集，來顯示 eCatalog。如果您是管理員，也可以建立自己的 eCatalog 檢視器預設集。

若要建立 eCatalog 檢視器預設集，請按一下全域導覽列上的「設定」按鈕，並選擇「檢視器預設集」。Then click Add, choose a platform, and choose **[UICONTROL eCatalog &gt; Viewer]**.

請參閱[設定 eCatalog 檢視器預設集](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)。

**5. 在 eCatalog 檢視器中預覽 eCatalog**

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式與行為。

若要瞭解 eCatalog 檢視器預設集如何顯示 eCatalog，請選取瀏覽面板中的「eCatalog」，然後按一下「預覽」。「預覽」畫面會在預設的檢視器中開啟。

請注意方向、色彩方案、變更頁面的控制項外觀，以及頁面翻頁時的外觀。

請參閱[在 eCatalog 檢視器中預覽 eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)。

**6. 發佈eCatalog和相關的PDF**

發佈您的eCatalog和相關PDF會將它放在動態媒體影像伺服器上，以便傳送至您的網站和應用程式。 在發佈程序中，Scene7 Publishing System 會針對 eCatalog 啟用 URL 字串。使用此URL，從動態媒體影像伺服器呼叫eCatalog至您的網站或應用程式。

在「瀏覽面板」中將eCatalog和PDF標示為要發佈後，選取「全域導覽列」上的「發佈」按鈕以開始發佈。 在「發佈」畫面上按一下「開始發佈」。

請參 [閱發佈eCatalogs和關聯的PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

**7. 連結 eCatalog 至網頁**

當您將eCatalog發佈至動態媒體影像伺服器時，Dynamic Media Classic會啟動顯示eCatalog所需的URL圖說字串。 您可以選取瀏覽面板中的 URL，從「預覽」畫面與瀏覽面板 (在詳細檢視中) 複製這個 URL 字串。複製 URL 字串後，它便可供網站及應用程式使用。

請與您的 IT 團隊合作，將 eCatalog 的連結放置於網頁中的適當位置。使用者按一下連結時，eCatalog 檢視器便會顯示，使用者也可以瀏覽 eCatalog。

請參閱[連結 eCatalog 至網頁](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)。
