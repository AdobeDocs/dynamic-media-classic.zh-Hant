---
title: 將視訊部署到網站和行動裝置網站
description: 瞭解如何從Adobe Dynamic Media Classic將視訊部署至您的網站和行動網站。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 23%

---

# 將視訊部署到網站和行動裝置網站{#deploying-video-to-your-websites-and-mobile-sites}

網站、行動網站和案頭應用程式可使用URL字串或內嵌程式碼來存取Adobe Dynamic Media Classic伺服器內容，包括視訊。 Adobe Dynamic Media Classic會在發佈程式期間啟用這些URL字串。 若要將視訊的URL字串或內嵌程式碼放置在網頁、行動頁面和案頭應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>發佈資產後，URL或內嵌程式碼才會啟用。

## 發佈視訊 {#publishing-video}

發佈影片可讓Adobe Dynamic Media Classic伺服器將影片傳送至您的網站、行動網站或應用程式。

您有兩種不同的發佈視訊方法：

* **上傳時自動立即發佈影片**：在視訊上傳程式中，Adobe Dynamic Media Classic可在上傳及編碼視訊時自動發佈視訊。 這種即時發佈功能表示事後不需要個別發佈視訊。

* **上傳後手動發佈視訊**：如果您不想立即發佈視訊，可以隨時手動發佈視訊。

在您發佈影片後，Adobe Dynamic Media Classic會啟用HTML頁面或應用程式程式碼的URL字串。

**若要發佈視訊：**

1. 進行以下一項操作:

   * 若要在上傳時自動立即發佈視訊，請在「上傳」頁面中選取「 」 **[!UICONTROL 上傳後發佈]**. 程序已完成，您不需要再做任何步驟。
   * 若要在上傳後手動發佈影片，請在「瀏覽」面板中選取影片，然後在「全域導覽」列上選取「 」 **發佈**.

## 將視訊URL連結至行動網站或網站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

發佈視訊時，您可以取得其相關URL，以用於您的網站、行動網站或案頭應用程式。 當您想要在網頁頂端的快顯視窗或強制回應視窗中顯示視訊時，請使用視訊URL。

當客戶選取連結時，會自動偵測其裝置、頻寬和熒幕大小。 系統會在預先定義的桌上型電腦檢視器或智慧型手機和平板電腦的行動裝置本機視訊播放器中，顯示適當的視訊以供播放。

另請參閱 [將視訊檢視器內嵌在網頁上](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**若要將視訊URL連結至行動網站或網站：**

1. 在「資產瀏覽」面板的 **[!UICONTROL 顯示]** 下拉式清單，選取 **[!UICONTROL 視訊]**，或 **[!UICONTROL 最適化視訊集]**.
1. 在左側的「資產庫」面板中，瀏覽至包含您要連結之視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]** 或 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL和內嵌程式碼」面板中，在「HTTP串流」下方，選取「 」 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

1. 將 HTML5 視訊 URL 連結貼到您的網站和行動網站上。

## 將視訊檢視器內嵌在網頁上 {#embedding-the-video-viewer-on-a-web-page}

當您想要播放內嵌在網頁上的影片時，請使用內嵌程式碼功能。 您可以將內嵌程式碼複製到剪貼簿，以便貼到網頁中。 不可在「內嵌程式碼」對話框中編輯程式碼。

另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**若要將視訊檢視器內嵌在網頁上：**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 視訊]**，或 **[!UICONTROL 最適化視訊集]**.
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的視訊或最適化視訊集。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]** 或 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL和內嵌程式碼」面板中，在「HTTP串流」下方，選取「 」 **[!UICONTROL 內嵌程式碼]** 位於您想要的檢視器右側。 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在視訊縮圖影像下方選取 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取 **[!UICONTROL 關閉]**.
1. 將內嵌程式碼貼入您的網頁。

### 實作內嵌程式碼，以搭配MP4視訊資產使用HTML5視訊 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

您可能不想使用Adobe Dynamic Media ClassicHTML5視訊播放程式。 如果您想使用原生HTML5 `<video>` 標籤時，您可以使用以下內嵌程式碼範例：

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 取代 `"S7 video thumbnail URL"` 使用視訊的縮圖URL，也就是使用者在播放視訊之前看到的視訊縮圖影像。

  另請參閱 [取得視訊縮圖URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* 取代 `"S7 OGG video asset URL (no player)"` 搭配視訊的漸進式URL以顯示OGG視訊。

  另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* 取代 `"S7 MP4 mobile progressive video asset URL (no player)"` 搭配視訊的行動漸進式URL。

  另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## 使用協力廠商視訊播放器部署視訊 {#deploying-video-using-a-third-party-video-player}

如果您使用協力廠商視訊播放器或自訂的視訊播放器，而非Dynamic Media Classic視訊檢視器，您將會取得適用於HLS多位元速率視訊串流或漸進式下載的直接視訊URL。

**若要使用協力廠商視訊播放器部署視訊：**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.
1. 依據您要使用的 URL 類型，執行下列其中一項工作: 

* 產生直接HLS串流視訊URL （多位元速率）的方式

  在 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL 已發佈的伺服器名稱]** 文字欄位，建構直接URL。 使用下列語法： `server/is/content/company/folder/filename.m3u8`

  例如，假設已發佈的伺服器名稱為 `https://s7d9.scene7.com/.` 使用步驟2中的語法，直接URL可能會如下所示：
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 產生直接HLS串流視訊URL （單位元速率）的方式

  在 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL HLS資料流伺服器名稱]** 文字欄位，使用下列語法建構直接URL：

  `server/company/folder/filename.ext.m3u8`

  例如，假設HLS串流伺服器名稱為 `https://s7mbrstream.scene7.com/hls-vod/`. 使用步驟2中的語法，直接URL可能會如下所示：
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 產生直接漸進式視訊 URL

  在「**[!UICONTROL 應用程式一般設定]**」頁面之「**[!UICONTROL 伺服器]**」群組的「**[!UICONTROL 漸進式視訊伺服器名稱]**」文字欄位上，使用下列語法建構直接 eVideo URL:

  `server/company/folder/filename`

  例如，假設漸進式視訊伺服器名稱為 `https://s7d9.scene7.com/is/content/`. 使用步驟2中的語法，直接URL可能會如下所示：
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用視訊縮圖 {#working-with-video-thumbnails}

Adobe Dynamic Media Classic會產生已編碼視訊的縮圖，以及預先編碼的視訊。 您可以像使用任何影像資產一樣使用視訊縮圖。此外，您也可以取得Adobe Dynamic Media Classic產生之視訊縮圖的URL。 然後，您就可以在Adobe Dynamic Media Classic外部部署這些URL。 例如，您可以在網站的搜尋結果、相關視訊清單和視訊播放清單中部署縮圖。

縮圖的產生以視訊中的首個異質影格 (非全黑影格或全白影格等等) 為基礎。

### 取得視訊縮圖URL {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic會在上傳程式期間自動產生視訊縮圖。 縮圖會出現在「清單檢視」和「格點檢視」的「瀏覽」面板中。

若要產生視訊縮圖的 URL，請執行發佈作業。

另請參閱 [發佈視訊](deploying-video-websites-mobile-sites.md#publishing_video).

在發佈後，您可以在「URL 和內嵌程式碼」面板的「詳細檢視」中，取得視訊縮圖 URL。選取 **[!UICONTROL 複製URL]** 位於視訊縮圖的右側，方便您複製其相關聯的URL。

### 修改視訊檢視器中的海報影格 {#modifying-poster-frames-in-video-viewers}

「*海報影格*」是視訊開始播放之前在「視訊」檢視器中顯示的初始影格。Adobe Dynamic Media Classic使用視訊縮圖作為海報框架。

您可以將影像修飾元套用至海報影格。例如，您可以裁切海報影格或使其變得透明。若要修改海報影格，請開啟視訊檢視器配置畫面，並在「海報影像修飾元」區段輸入修飾元。

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另請參閱 [影像伺服指南](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api).

還可以透過將修飾元附加到視訊縮圖 URL 來修改視訊縮圖。

>[!MORELIKETHIS]
>
>* [發佈檔案](publishing-files.md#publishing_files)