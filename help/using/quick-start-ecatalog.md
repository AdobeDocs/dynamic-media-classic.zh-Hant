---
title: 「快速入門：eCatalogs」
description: eCatalogs簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速上手並執行eCatalog技術。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 36%

---

# 快速入門：eCatalogs{#quick-start-ecatalogs}

eCatalog 為列印材料的數位網頁版本 — 例如目錄、傳單、文宣、產品手冊或廣告傳單。eCatalog 顯示於網站上的 eCatalog 檢視器中。此檢視器會模擬閱讀列印材料的體驗。

另請觀看下列訓練影片：

* [快速入門1：eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [快速入門2：eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

根據您為eCatalog選擇的設定，檢視器可讓您執行下列動作：

* 在目錄中搜尋一或多個關鍵字。 搜尋結果會在目錄左側的搜尋面板中顯示為縮圖清單。 每個可點按的縮圖代表目錄跨頁，其中會找到反白顯示的搜尋字詞。

* 透過社群媒體分享目錄；下載目錄以離線檢視；啟用「我的最愛」以標籤您要快速返回的專案，或列印目錄。
* 使用目錄或頁面格線檢視來瀏覽目錄；按一下頁面中邊緣可向前或向後瀏覽頁面。
* 放大、縮小與平移即可檢查頁面上的項目。
* 將指標移到頁面區域（稱為影像地圖）上，以便看到包含專案相關資訊的快顯視窗。
* 選取頁面區域，開啟包含專案詳細資訊的新網頁。
* 撰寫註解並將其附加到 eCatalog 頁面。
* 如果您想要啟動相關網頁或內容資訊面板，請點選影像地圖圖示。
* 使用手勢互動，包括雙指縮放與揮動翻頁。
* 依項目關鍵字搜尋。

![向使用者顯示的eCatalog。 A) eCatalog開啟頁面。 B)eCatalog已翻到第2頁。](/help/using/assets/ec_cat_viewer_popup.png)

若要建立eCatalog，您通常會使用在Adobe Acrobat或其他列印程式中建立的高解析度PDF檔案，但您也可以從影像檔案建立eCatalog。

建立 eCatalog 時，您可以依選擇的順序安排頁面或頁面跨頁。您也可以指定要採用單一頁面、雙頁式跨頁或多頁式跨頁。您可以為頁面區域建立影像地圖，讓檢視者可以選取頁面上的某個區域，並在您的網站上開啟新頁面。 您可以使用 eCatalog 畫面中的「資訊面板」設定來管理顯示的滑鼠指向效果文字。您也可從超過 100 個不同的設定選項中選擇，以設定 eCatalog 檢視器。您可以為特定對象量身訂作檢視器的功能與外觀。

>[!NOTE]
>
>如果您是Dynamic Media - Scene7模式使用者，並且想要使用eCatalog，請編輯 `pdfbrochure` CRXDE Lite中的值。 若要這麼做，請在Adobe Experience Manager中前往 **[!UICONTROL 工具]** > **[!UICONTROL 一般]** > **[!UICONTROL CRXDE Lite]**. 在左側面板導覽樹狀結構中，導覽至 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>在右下方的窗格中， **[!UICONTROL 屬性]** 索引標籤中，選取 `jobParam` 列。 設定值 `pdfbrochure` 從 `false` 至 `true`. 如在 `pdfbrochure=true`
>
>在CRXDE Lite頁面的左上角，選取 **[!UICONTROL 全部儲存]**.
>
>您現在可以在Adobe Dynamic Media Classic中撰寫eCatalogs。

「eCatalog 快速入門」的設計可讓您迅速熟練 eCatalog。依照步驟 1 至 7 執行。每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.上傳PDF檔案

Adobe PDF 檔案通常是 eCatalog 的來源。因為 PDF 檔案須列印，所以通常包含 CMYK 影像。Adobe Dynamic Media Classic會偵測這些影像，並使用標準CMYK色彩設定檔進行轉換。 不過，您必須上傳並使用自訂色彩設定檔。

在全域導覽列上，選取 **[!UICONTROL 上傳]** 以開始上傳eCatalog的PDF檔案或影像。 您可以從桌面或透過 FTP 上載檔案；如果您上載多個檔案或檔案大小超過 100 MB，則建議使用 FTP。

在 PDF 選項之下，「上載」畫面提供以適當解析度與正確色域上載 PDF 檔案的選項。建議使用每英吋 150 像素的解析度。上載 PDF 檔案時，您可以選取「自動產生 eCatalog」選項來建立 eCatalog。

另請參閱 [上傳PDF檔案](uploading-pdf-files.md#uploading_the_pdf_files).

## 2.建立eCatalog

在「瀏覽」面板中選取PDF或影像檔案，以建立您的eCatalog。 選取 **[!UICONTROL 建置]**，然後選擇 **[!UICONTROL eCatalogs]**.

在eCatalog頁面的 **[!UICONTROL 排序頁面]** 索引標籤中，選取「版面」選項： **[!UICONTROL 1欄式]**， **[!UICONTROL 2欄式]**，或 **[!UICONTROL 自訂]**. 您可以拖曳頁面，或是在大型的eCatalog 的「移動至」選單上選擇頁面名稱，來重新排序頁面或跨頁。

若要新增頁面，請在資產庫中選取檔案夾，然後將 PDF 或影像檔案從檔案夾拖曳至「排序頁面」畫面。您可以提供自訂頁面名稱或匯入許多頁面名稱，而不是預設頁碼。

選取 **[!UICONTROL 儲存]**，輸入eCatalog的名稱，選擇用來儲存的Adobe Dynamic Media Classic資料夾，然後選取 **[!UICONTROL 儲存]**. 每次變更頁面順序或編輯eCatalog時，請按一下以儲存變更 **[!UICONTROL 儲存]**.

另請參閱 [建立eCatalog](creating-ecatalog.md).

## 3.建立影像地圖

「影像地圖」為eCatalog頁面新增了另一個面向。 影像地圖是頁面的某個區域，提供更多有關項目的資訊。檢視者捲動指標至影像地圖上時，就會看到項目的描述。按一下影像地圖會啟動外部參照，它會開啟一個新網頁，您可以在其中瞭解更多有關項目的資訊。

若要建立影像地圖，請開啟「eCatalog」畫面。然後前往 **[!UICONTROL 對應頁面]** 標籤，並使用「矩形影像地圖」工具或「多邊形影像地圖」工具將地圖框架化。 您可以使用平移工具  來拖曳地圖邊框，以調整影像地圖的位置與大小。

在設定「影像地圖」的框架後，輸入當您選取「影像地圖」時要前往的URL位址。 您也可以輸入將指標移動到影像地圖上時會顯示的滑鼠指向效果文字。

另請參閱 [建立eCatalog影像地圖](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

另請參閱 [使用影像地圖在eCatalog中內嵌多媒體](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

您可以使用「eCatalog」畫面中的「資訊面板」設定，來設定和管理影像地圖文字。

另請參閱 [管理eCatalogs中的資訊面板內容](/help/using/info-panel-content-ecatalog.md).

## 4.設定eCatalog檢視器預設集

終端使用者會在 eCatalog 檢視器中檢視您的 eCatalog。如果您是管理員，便可以設定 eCatalog 檢視器。您可以變更其外框色彩，並選取新的「外觀」，讓 eCatalog 擁有品牌特色。Adobe Dynamic Media Classic隨附數個「最佳實務」 eCatalog檢視器預設集。 您可以選擇其中一個預設集，來顯示 eCatalog。如果您是管理員，也可以建立自己的 eCatalog 檢視器預設集。

若要建立eCatalog檢視器預設集，請在全域導覽列上選取 **[!UICONTROL 設定]**，然後選擇 **[!UICONTROL 檢視器預設集]**. 選取 **[!UICONTROL 新增]**，選擇平台，然後選取 **[!UICONTROL eCatalog]** > **[!UICONTROL 檢視器]**.

另請參閱 [設定eCatalog檢視器預設集](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5.在eCatalog檢視器中預覽eCatalog

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式與行為。

若要瞭解eCatalog檢視器預設集如何顯示您的eCatalog，請在「瀏覽」面板中選取您的eCatalog，然後選取 **[!UICONTROL 預覽]**. 「預覽」畫面會在預設的檢視器中開啟。

請注意方向、色彩方案、變更頁面的控制項外觀，以及頁面翻頁時的外觀。

另請參閱 [在eCatalog檢視器中預覽eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6.發佈eCatalog和相關PDF

發佈eCatalog和相關PDF時，會將它置於Dynamic Media影像伺服器上，以便傳送至您的網站和應用程式。 在發佈程式中，Adobe Dynamic Media Classic會啟動eCatalog的URL字串。 使用此URL從Dynamic Media影像伺服器呼叫eCatalog至您的網站或應用程式。

在「瀏覽」面板中將eCatalog和PDF標籤為發佈後，選取「全域導覽」列上的「發佈」按鈕以啟動發佈。 在「發佈」畫面上，選取「 」 **[!UICONTROL 提交發佈]**.

另請參閱 [發佈eCatalog和相關PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7.將eCatalog連結至網頁

當您將eCatalog發佈至Adobe Dynamic Media Classic影像伺服器時，Dynamic Media會啟用顯示所需的URL圖說文字字串。 您可以選取面板中的URL，從「預覽」畫面和「瀏覽」面板（在「詳細資料檢視」中）複製此URL字串。 複製 URL 字串後，它便可供網站及應用程式使用。

請與您的 IT 團隊合作，將 eCatalog 的連結放置於網頁中的適當位置。當使用者選取連結時，eCatalog檢視器會出現，使用者可以瀏覽您的eCatalog。

另請參閱 [將eCatalog連結至網頁](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
