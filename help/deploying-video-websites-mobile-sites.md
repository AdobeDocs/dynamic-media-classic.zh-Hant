---
title: 將視訊部署到網站和行動裝置網站
description: 瞭解如何將視頻部署到您來自Adobe Dynamic Media Classic的網站和移動站點。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 33%

---

# 將視訊部署到網站和行動裝置網站{#deploying-video-to-your-websites-and-mobile-sites}

網站、移動站點和案頭應用程式使用URL字串或嵌入代碼訪問Adobe Dynamic Media Classic伺服器內容（包括視頻）。 Adobe Dynamic Media Classic在發佈過程中激活這些URL字串。 要將視頻的URL字串或嵌入代碼放在網頁、移動頁面和案頭應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 或內嵌程式碼不會產生作用。

## 發佈視訊 {#publishing-video}

發佈視頻使Adobe Dynamic Media Classic伺服器能夠將視頻傳送到您的網站、移動站點或應用程式。

可以使用兩種不同的方法發佈視頻：

* **上傳時自動即時發佈視頻**  — 作為視頻上傳過程的一部分，Adobe Dynamic Media Classic可以在上傳和編碼視頻時自動發佈視頻。 此立即發佈功能意味著不需要另外再發佈視訊 (因為已經發佈了)。

* **在上載後手動發佈視訊**  — 如果您不想立即發佈視頻，則可以隨時手動發佈視頻。

發佈視頻後，Adobe Dynamic Media Classic會為您的HTML頁或應用程式碼激活URL字串。

**發佈視訊:**

1. 進行以下一項操作:

   * 要在上載時自動立即發佈視頻，請在「上載」頁面中選擇 **[!UICONTROL 上載後發佈]**。 程序已完成，您不需要再做任何步驟。
   * 要在上載後手動發佈視頻，請在「瀏覽面板」中選擇視頻，然後在「全局導航」欄上選擇 **發佈**。

## 將視頻URL連結到移動站點或網站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

發佈視訊後，您便可以取得其 URL，以在您的網站、行動網站或桌上型電腦應用程式中使用。當您想要在網頁頂端的彈出式視窗或浮出視窗中顯示視訊，請使用視訊 URL。

當客戶選擇鏈路時，將自動檢測其設備、頻寬和螢幕大小。 系統會在預先定義的桌上型電腦檢視器或智慧型手機和平板電腦的行動裝置本機視訊播放器中，顯示適當的視訊以供播放。

另請參閱 [將視頻查看器嵌入網頁](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)。

**將視訊 URL 連結至行動網站或網站:**

1. 在「資產瀏覽」面板中， **[!UICONTROL 顯示]** 下拉清單，選擇 **[!UICONTROL 視頻]** 或 **[!UICONTROL 自適應視頻集]**。
1. 在左側的「資產庫」面板中，瀏覽至包含您要連結之視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL」和「嵌入代碼」面板中的「HTTP流」下，選擇 **[!UICONTROL 複製URL]** 按鈕。 作為最佳做法，複製與 `Universal_HTML5_Video` 查看器。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。 作為最佳做法，複製與 `Universal_HTML5_Video` 查看器。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。 作為最佳做法，複製與 `Universal_HTML5_Video` 查看器。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。 作為最佳做法，複製與 `Universal_HTML5_Video` 查看器。

1. 將 HTML5 視訊 URL 連結貼到您的網站和行動網站上。

## 將視頻查看器嵌入網頁 {#embedding-the-video-viewer-on-a-web-page}

當您想播放網頁上內嵌的視訊時，請使用「內嵌程式碼」功能。將內嵌程式碼複製到剪貼簿上，以便貼到網頁中。不可在「內嵌程式碼」對話框中編輯程式碼。

另請參閱 [將視頻URL連結到移動站點或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

**在網頁上內嵌視訊檢視器:**

1. 在「資產瀏覽」面板的「顯示」下拉清單中，選擇 **[!UICONTROL 視頻]** 或 **[!UICONTROL 自適應視頻集]**。
1. 在左側的「資產庫」面板中，瀏覽至包含您要複製其內嵌程式碼的視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL」和「嵌入代碼」面板中的「HTTP流」下，選擇 **[!UICONTROL 嵌入代碼]** 按鈕。 作為最佳做法，選擇 **[!UICONTROL 嵌入代碼]** 與 `Universal_HTML5_Video` 查看器。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在視頻縮略圖影像下方選擇 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。 作為最佳做法，選擇 **[!UICONTROL 嵌入代碼]** 與 `Universal_HTML5_Video` 查看器。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。 作為最佳做法，選擇 **[!UICONTROL 嵌入代碼]** 與 `Universal_HTML5_Video` 查看器。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。 作為最佳做法，選擇 **[!UICONTROL 嵌入代碼]** 與 `Universal_HTML5_Video` 查看器。

1. 在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選擇 **[!UICONTROL 關閉]**。
1. 在您的網頁中貼上內嵌程式碼。

### 用MP4視頻資產實現HTML5視頻的嵌入代碼 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

如果不使用Adobe Dynamic Media ClassicHTML5視頻播放器，而是希望使用本機HTML5 `<video>` 帶有MP4視頻資產的標籤，可以使用以下嵌入代碼示例：

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 替換 `"S7 video thumbnail URL"` 視頻的縮略圖URL，即用戶在播放視頻前看到的縮略圖。

   請參閱 [獲取視頻縮略圖URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)。

* 替換 `"S7 OGG video asset URL (no player)"` 顯示OGG視頻的漸進URL。

   請參閱 [將視頻URL連結到移動站點或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

* 替換 `"S7 MP4 mobile progressive video asset URL (no player)"` 顯示視頻的移動漸進URL。

   請參閱 [將視頻URL連結到移動站點或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

## 使用第三方視頻播放器部署視頻 {#deploying-video-using-a-third-party-video-player}

如果您使用第三方視頻播放器或定製的視頻播放器而不是Dynamic Media Classic視頻查看器，則將獲取適用於HLS多比特率視頻流或漸進式下載的直接視頻URL。

**部署使用第三方視訊播放器的視訊:**

1. 在Adobe Dynamic Media Classic，在全球導航欄上， **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]**。
1. 依據您要使用的 URL 類型，執行下列其中一項工作: 

* 生成直接HLS流視頻URL（多比特率）

   在 **[!UICONTROL 應用程式常規設定]** 的 **[!UICONTROL 伺服器]** 組，在 **[!UICONTROL 已發佈伺服器名稱]** 文本欄位，構造直接URL。 使用以下語法： `server/is/content/company/folder/filename.m3u8`

   例如，假設已發佈的伺服器名稱為 `https://s7d9.scene7.com/.` 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 生成直接HLS流視頻URL（單比特率）

   在 **[!UICONTROL 應用程式常規設定]** 的 **[!UICONTROL 伺服器]** 組，在 **[!UICONTROL HLS流伺服器名稱]** 文本欄位，使用以下語法構造直接URL:

   `server/company/folder/filename.ext.m3u8`

   例如，假設HLS流伺服器名稱為 `https://s7mbrstream.scene7.com/hls-vod/`。 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 產生直接漸進式視訊 URL

   在「**[!UICONTROL 應用程式一般設定]**」頁面之「**[!UICONTROL 伺服器]**」群組的「**[!UICONTROL 漸進式視訊伺服器名稱]**」文字欄位上，使用下列語法建構直接 eVideo URL:

   `server/company/folder/filename`

   例如，假設漸進視頻伺服器名稱為 `https://s7d9.scene7.com/is/content/`。 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用視頻縮略圖 {#working-with-video-thumbnails}

Adobe Dynamic Media Classic為編碼視頻生成縮略圖，並預編碼視頻。 您可以像使用任何影像資產一樣使用視訊縮圖。此外，您還可以獲取Adobe Dynamic Media Classic生成的視頻縮略圖的URL。 然後，您可以在Adobe Dynamic Media Classic以外部署這些URL。 例如，您可以在網站的搜尋結果、相關視訊清單和視訊播放清單中部署縮圖。

縮圖的產生以視訊中的首個異質影格 (非全黑影格或全白影格等等) 為基礎。

### 獲取視頻縮略圖URL {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic在上載過程中自動生成視頻縮略圖。 縮略圖顯示在「清單視圖」和「網格視圖」的「瀏覽」面板中。

若要產生視訊縮圖的 URL，請執行發佈作業。

請參閱 [發佈視頻](deploying-video-websites-mobile-sites.md#publishing_video)。

在發佈後，您可以在「URL 和內嵌程式碼」面板的「詳細檢視」中，取得視訊縮圖 URL。選擇 **[!UICONTROL 複製URL]** 表徵圖。

### 修改視頻查看器中的海報幀 {#modifying-poster-frames-in-video-viewers}

「*海報影格*」是視訊開始播放之前在「視訊」檢視器中顯示的初始影格。Adobe Dynamic Media Classic將視頻縮略圖用作海報框架。

您可以將影像修飾元套用至海報影格。例如，您可以裁切海報影格或使其變得透明。若要修改海報影格，請開啟視訊檢視器配置畫面，並在「海報影像修飾元」區段輸入修飾元。

請參閱 [添加或編輯視頻查看器預設](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

請參閱 [影像服務指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api)。

還可以透過將修飾元附加到視訊縮圖 URL 來修改視訊縮圖。

>[!MORELIKETHIS]
>
>* [發佈檔案](publishing-files.md#publishing_files)