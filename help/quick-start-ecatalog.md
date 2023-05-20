---
title: 「快速啟動：eCatalogs"
description: eCatalog簡介和快速入門幫助您利用Adobe Dynamic Media Classic的eCatalog技術快速啟動和運行。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 36%

---

# 快速啟動：電子目錄{#quick-start-ecatalogs}

eCatalog 為列印材料的數位網頁版本 — 例如目錄、傳單、文宣、產品手冊或廣告傳單。eCatalog 顯示於網站上的 eCatalog 檢視器中。此檢視器會模擬閱讀列印材料的體驗。

另請參閱以下培訓視頻：

* [快速入門1:電子目錄](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [快速入門2:電子目錄](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

根據您為eCatalog選擇的設定，查看器可讓您執行以下操作：

* 搜索目錄以查找關鍵字或關鍵字。 搜索結果在目錄左側的搜索面板中顯示為縮略圖清單。 每個可點擊的縮略圖都表示在其中找到突出顯示的搜索詞的目錄跨頁。

* 通過社交媒體共用目錄；下載目錄離線查看；啟用收藏夾以標籤要快速返回的項目或打印目錄。
* 使用目錄或頁面網格視圖瀏覽目錄；按一下頁面的中間邊緣，向前或向後頁面。
* 放大、縮小與平移即可檢查頁面上的項目。
* 將指針移到頁面區域（稱為「影像映射」）上，這樣您就可以看到一個彈出窗口，其中包含有關項的資訊。
* 選擇一個頁面區域，以便開啟一個新網頁，其中包含有關項目的詳細資訊。
* 撰寫註解並將其附加到 eCatalog 頁面。
* 如果要啟動相關網頁或上下文資訊面板，請點擊影像映射表徵圖。
* 使用手勢互動，包括雙指縮放與揮動翻頁。
* 依項目關鍵字搜尋。

![eCatalog對用戶顯示的樣式。 A)電子目錄開啟頁面。 B)eCatalog轉到第2頁。](/help/assets/ec_cat_viewer_popup.png)

要建立eCatalog，您通常使用在Adobe Acrobat或其他打印程式中建立的高解析度PDF檔案，但您也可以從影像檔案建立eCatalog。

建立 eCatalog 時，您可以依選擇的順序安排頁面或頁面跨頁。您也可以指定要採用單一頁面、雙頁式跨頁或多頁式跨頁。您可以為頁面區域建立影像映射，以便查看者可以選擇頁面上的某個區域，並在您的網站上開啟新頁面。 您可以使用 eCatalog 畫面中的「資訊面板」設定來管理顯示的滑鼠指向效果文字。您也可從超過 100 個不同的設定選項中選擇，以設定 eCatalog 檢視器。您可以為特定對象量身訂作檢視器的功能與外觀。

>[!NOTE]
>
>如果您是Dynamic Media-Scene7模式用戶並想使用eCatalogs，請編輯 `pdfbrochure` 值CRXDE Lite。 要執行此操作，請在Adobe Experience Manager **[!UICONTROL 工具]** > **[!UICONTROL 常規]** > **[!UICONTROL CRXDE Lite]**。 在左側面板導航樹中，導航到 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`。
>
>在右下窗格中， **[!UICONTROL 屬性]** 頁籤 `jobParam` 欄。 設定 `pdfbrochure` 從 `false` 至 `true`。 與 `pdfbrochure=true`
>
>在CRXDE Lite頁的左上角，選擇 **[!UICONTROL 全部保存]**。
>
>您現在可以在Adobe Dynamic Media Classic製作eCatalogs。

「eCatalog 快速入門」的設計可讓您迅速熟練 eCatalog。依照步驟 1 至 7 執行。在每個步驟之後，都會出現一個主題標題的交叉引用，您可以在其中找到更多資訊。

## 1。上載PDF檔案

Adobe PDF 檔案通常是 eCatalog 的來源。因為 PDF 檔案須列印，所以通常包含 CMYK 影像。Adobe Dynamic Media Classic檢測這些影像，並使用標準CMYK顏色配置檔案進行轉換。 但是，必須上載和使用自定義顏色配置檔案。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 開始為您的eCatalog上載PDF檔案或影像。 您可以從桌面或透過 FTP 上載檔案；如果您上載多個檔案或檔案大小超過 100 MB，則建議使用 FTP。

在 PDF 選項之下，「上載」畫面提供以適當解析度與正確色域上載 PDF 檔案的選項。建議使用每英吋 150 像素的解析度。上載 PDF 檔案時，您可以選取「自動產生 eCatalog」選項來建立 eCatalog。

請參閱 [上載PDF檔案](uploading-pdf-files.md#uploading_the_pdf_files)。

## 2.建立電子目錄

通過在「瀏覽面板」中選擇PDF或影像檔案來建立eCatalog。 選擇 **[!UICONTROL 生成]**，然後選擇 **[!UICONTROL 電子目錄]**。

在eCatalog頁面上， **[!UICONTROL 訂單頁]** 頁籤，選擇佈局選項： **[!UICONTROL 1上]**。 **[!UICONTROL 2個]**&#x200B;或 **[!UICONTROL 自定義]**。 您可以拖曳頁面，或是在大型的eCatalog 的「移動至」選單上選擇頁面名稱，來重新排序頁面或跨頁。

若要新增頁面，請在資產庫中選取檔案夾，然後將 PDF 或影像檔案從檔案夾拖曳至「排序頁面」畫面。您可以提供自定義頁名或導入許多頁名，而不是預設頁碼。

選擇 **[!UICONTROL 保存]**，輸入eCatalog的名稱，選擇用於儲存eCatalog的Adobe Dynamic Media Classic資料夾，然後選擇 **[!UICONTROL 保存]**。 每次更改頁面順序或編輯eCatalog時，通過按一下 **[!UICONTROL 保存]**。

請參閱 [建立電子目錄](creating-ecatalog.md)。

## 3.建立影像映射

「影像映射」向eCatalog頁添加了另一個方面。 影像地圖是頁面的某個區域，提供更多有關項目的資訊。檢視者捲動指標至影像地圖上時，就會看到項目的描述。按一下影像地圖會啟動外部參照，它會開啟一個新網頁，您可以在其中瞭解更多有關項目的資訊。

若要建立影像地圖，請開啟「eCatalog」畫面。然後轉到 **[!UICONTROL 映射頁]** 頁籤，並使用矩形影像映射工具或多邊形影像映射工具對映射進行框架。 您可以使用平移工具  來拖曳地圖邊框，以調整影像地圖的位置與大小。

在對「影像映射」進行框架後，輸入選擇「影像映射」時要轉到的URL地址。 您也可以輸入將指標移動到影像地圖上時會顯示的滑鼠指向效果文字。

請參閱 [建立電子目錄映像映射](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)。

請參閱 [使用映像映射將富媒體嵌入到eCatalog中](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)。

您可以使用「eCatalog」畫面中的「資訊面板」設定，來設定和管理影像地圖文字。

請參閱 [管理電子目錄中的資訊面板內容](/help/info-panel-content-ecatalog.md)。

## 4.設定eCatalog Viewer預設

終端使用者會在 eCatalog 檢視器中檢視您的 eCatalog。如果您是管理員，便可以設定 eCatalog 檢視器。您可以變更其外框色彩，並選取新的「外觀」，讓 eCatalog 擁有品牌特色。Adobe Dynamic Media Classic提供了幾個「最佳實踐」 eCatalog Viewer預設。 您可以選擇其中一個預設集，來顯示 eCatalog。如果您是管理員，也可以建立自己的 eCatalog 檢視器預設集。

要建立eCatalog Viewer預設，請在「全局導航」欄上選擇 **[!UICONTROL 設定]**，然後選擇 **[!UICONTROL 查看器預設]**。 選擇 **[!UICONTROL 添加]**，然後選擇 **[!UICONTROL 電子目錄]** > **[!UICONTROL 查看器]**。

請參閱 [設定eCatalog Viewer預設](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)。

## 5.在eCatalog查看器中預覽eCatalog

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式與行為。

要瞭解eCatalog Viewer Presets如何顯示eCatalog，請在「瀏覽面板」中選擇eCatalog，然後選擇 **[!UICONTROL 預覽]**。 「預覽」畫面會在預設的檢視器中開啟。

請注意方向、色彩方案、變更頁面的控制項外觀，以及頁面翻頁時的外觀。

請參閱 [在eCatalog查看器中預覽eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)。

## 6。發佈電子目錄和關聯PDF

發佈eCatalog和關聯的PDF會將其放在Dynamic Media映像伺服器上，以便可將其發送到您的網站和應用程式。 作為發佈過程的一部分，Adobe Dynamic Media Classic會為eCatalog激活URL字串。 使用此URL將eCatalog從Dynamic Media映像伺服器調用到您的網站或應用程式。

在「瀏覽面板」中標籤要發佈的電子目錄和PDF後，選擇全局導航欄上的「發佈」按鈕以啟動發佈。 在「發佈」螢幕上，選擇 **[!UICONTROL 提交發佈]**。

請參閱 [發佈電子目錄和關聯PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

## 7。將eCatalog連結到網頁

Adobe Dynamic Media Classic在將電子目錄發佈到Dynamic Media影像伺服器時激活顯示電子目錄所需的URL標注字串。 通過在面板中選擇URL，可以從「預覽」螢幕和「瀏覽面板」（在「詳細資訊視圖」中）複製此URL字串。 複製 URL 字串後，它便可供網站及應用程式使用。

請與您的 IT 團隊合作，將 eCatalog 的連結放置於網頁中的適當位置。當用戶選擇該連結時，將顯示eCatalog Viewer，用戶可以瀏覽您的eCatalog。

請參閱 [將eCatalog連結到網頁](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)。
