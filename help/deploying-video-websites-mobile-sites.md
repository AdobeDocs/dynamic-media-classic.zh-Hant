---
title: 將視訊部署到網站和行動裝置網站
seo-title: 將視訊部署到網站和行動裝置網站
description: 'null'
seo-description: 瞭解如何將視訊部署至您的網站和行動網站。
uuid: 22bb4402-c0 ab-4df0-89b9-99707d111927
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/video
discoiquuid: 0d006314-c4 cc-4f6 c-a51 c-6075bb445 e39
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 將視訊部署到網站和行動裝置網站{#deploying-video-to-your-websites-and-mobile-sites}

網站、行動網站和桌面應用程式使用URL字串或內嵌程式碼，存取Dynamic Media Classic伺服器內容(包括視訊)。Dynamic Media Classic會在發佈程序期間啓動這些URL字串。若要將視訊的 URL 字串或內嵌程式碼放在網頁、行動網頁和桌上型電腦應用程式中，請從 Scene7 Publishing System 中複製該字串。

>[!NOTE]
>
>在發佈資產之前，URL 或內嵌程式碼不會產生作用。

## 發佈視訊 {#publishing-video}

發佈影片可讓動態媒體Classic Server將視訊傳送至您的網站、行動網站或應用程式。

您可使用兩種不同的方法來發佈視訊: 

* **在上載時立即自動發佈視訊**

   在視訊上傳程序中，Dynamic Media Classic可在上傳和編碼視訊時自動發佈視訊。此立即發佈功能意味著不需要另外再發佈視訊 (因為已經發佈了)。

* **在上載後手動發佈視訊**

   如果您不想立即發佈視訊，可以隨時手動發佈視訊。

在您發佈視訊之後，Scene7 Publishing System 會啟用 HTML 頁面或應用程式代碼的 URL 字串。

**發佈視訊**

1. 進行以下一項操作:

   * 若要在上載時立即自動發佈視訊，請按一下「上載」畫面中的「**上載後發佈**」。程序已完成，您不需要再做任何步驟。
   * 若要在上載後手動發佈視訊，請在「瀏覽」面板中選取視訊，然後按一下全域導覽列上的「**發佈**」。

## 將視訊 URL 連結至行動網站或網站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

發佈視訊後，您便可以取得其 URL，以在您的網站、行動網站或桌上型電腦應用程式中使用。當您想要在網頁頂端的彈出式視窗或浮出視窗中顯示視訊，請使用視訊 URL。

當客戶按下連結時，便會自動偵測其裝置、頻寬和螢幕大小。系統會在預先定義的桌上型電腦檢視器或智慧型手機和平板電腦的行動裝置本機視訊播放器中，顯示適當的視訊以供播放。

另請參閱[在網頁上內嵌視訊檢視器](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)。

**將視訊 URL 連結至行動網站或網站**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，按一下「**視訊**」或「**最適化視訊集**」。
1. 在左側的「資產庫」面板中，瀏覽至包含您要連結之視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 按一下「**格點檢視**」或「**清單檢視**」。在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側「URL 和內嵌程式碼」面板的「HTTP 串流」底下，按一下您要的檢視器右側的「**複製 URL**」。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方按一下「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * 按一下「**清單檢視**」。在「資產瀏覽」面板中，選取單一資產，然後按一下縮圖影像右側的「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * 按一下「**格點檢視**」、「**清單檢視**」或「**詳細檢視**」。在同一個工具列上，按一下「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. 將 HTML5 視訊 URL 連結貼到您的網站和行動網站上。

## 在網頁上內嵌視訊檢視器 {#embedding-the-video-viewer-on-a-web-page}

當您想播放網頁上內嵌的視訊時，請使用「內嵌程式碼」功能。將內嵌程式碼複製到剪貼簿上，以便貼到網頁中。不可在「內嵌程式碼」對話框中編輯程式碼。

另請參閱[將視訊 URL 連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

**在網頁上內嵌視訊檢視器**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，按一下「**視訊**」或「**最適化視訊集**」。
1. 在左側的「資產庫」面板中，瀏覽至包含您要複製其內嵌程式碼的視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 按一下「**格點檢視**」或「**清單檢視**」。在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側「URL 和內嵌程式碼」面板的「HTTP 串流」底下，按一下您要的檢視器右側的「**內嵌程式碼**」。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，選取單一資產，然後在視訊縮圖影像下方按一下「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * 按一下「**清單檢視**」。在「資產瀏覽」面板中，選取單一資產，然後按一下縮圖影像右側的「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * 按一下「**格點檢視**」、「**清單檢視**」或「**詳細檢視**」。在同一個工具列上，按一下「**預覽** &gt; **檢視器清單**」。

      在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. 在「內嵌程式碼」對話框中，按一下「**複製至剪貼簿**」。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 按一下「**關閉**」。
1. 在您的網頁中貼上內嵌程式碼。

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 以 `"S7 video thumbnail URL"` 影片的縮圖URL取代。此為使用者在播放視訊前所看見的視訊縮圖影像。

   請參閱[取得視訊縮圖 URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)。

* 以 `"S7 OGG video asset URL (no player)"` 視訊的漸進式URL取代OGG視訊。

   請參閱[將視訊 URL 連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

* 以 `"S7 MP4 mobile progressive video asset URL (no player)"` 影片的行動漸進式URL取代。

   請參閱[將視訊 URL 連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

## 部署使用第三方視訊播放器的視訊 {#deploying-video-using-a-third-party-video-player}

如果您使用協力廠商視訊播放器或自訂內建的視訊播放程式而非Dynamic Media Classic視訊檢視器，則可取得適用於HLS多重位元速率視訊串流或漸進式下載的直接視訊URL。

**部署使用第三方視訊播放器的視訊**

1. 在 Scene7 Publishing System 的「全域導覽」列上，按一下「**設定** &gt; **應用程式設定** &gt; **一般設定**」。
1. 依據您要使用的 URL 類型，執行下列其中一項工作: 
* 產生直接HLS串流視訊URL(多位元速率)

   在 **「應用程式一般設定** 」頁面的 **「伺服器** 」群組中，於 **「發佈伺服器名稱** 」文字欄位中，使用下列語法建構直接URL： `server/is/content/company/folder/filename.m3u8`
例如，假設已發佈的伺服器名稱 `https://s7d9.scene7.com/.` 在步驟使用語法，直接URL可能看起來像是：
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 產生直接HLS串流視訊URL(位元速率)

   On the **Application General Settings** page, in the **Servers** group, in the **HLS Streaming Server Name** text field, construct the direct URL using the following syntax:
   `server/company/folder/filename.ext.m3u8`例如，假設HLS串流伺服器名稱 `https://s7mbrstream.scene7.com/hls-vod/`為。使用步驟 2 的語法，直接 URL 可能如下所示:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 產生直接漸進式視訊 URL

   在「**應用程式一般設定**」頁面之「**伺服器**」群組的「**漸進式視訊伺服器名稱**」文字欄位上，使用下列語法建構直接 eVideo URL:`server/company/folder/filename`例如，假設漸進式視訊伺服器名稱 `https://s7d9.scene7.com/is/content/`為。使用步驟 2 的語法，直接 URL 可能如下所示:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用視訊縮圖 {#working-with-video-thumbnails}

Dynamic Media Classic會產生編碼視訊的縮圖，以及預先編碼的視訊。您可以像使用任何影像資產一樣使用視訊縮圖。此外，您也可以取得Dynamic Media Classic在SPS之外產生和部署這些URL的URL縮圖URL。例如，您可以在網站的搜尋結果、相關視訊清單和視訊播放清單中部署縮圖。

縮圖的產生以視訊中的首個異質影格 (非全黑影格或全白影格等等) 為基礎。

### 取得視訊縮圖 URL {#obtaining-video-thumbnail-urls}

Dynamic Media Classic會在上傳程序期間自動產生視訊縮圖。縮圖在清單檢視和格點檢視的瀏覽面板中顯示。

若要產生視訊縮圖的 URL，請執行發佈作業。

請參閱[發佈視訊](deploying-video-websites-mobile-sites.md#publishing_video)。

在發佈後，您可以在「URL 和內嵌程式碼」面板的「詳細檢視」中，取得視訊縮圖 URL。按一下視訊縮圖右側的「**複製 URL**」以複製其 URL

### 在視訊檢視器中修改海報影格 {#modifying-poster-frames-in-video-viewers}

「*海報影格*」是視訊開始播放之前在「視訊」檢視器中顯示的初始影格。Dynamic Media Classic使用視訊縮圖做為海報影格。

您可以將影像修飾元套用至海報影格。例如，您可以裁切海報影格或使其變得透明。若要修改海報影格，請開啟視訊檢視器配置畫面，並在「海報影像修飾元」區段輸入修飾元。

請參閱[增加或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

請參閱 [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en)。

還可以透過將修飾元附加到視訊縮圖 URL 來修改視訊縮圖。

>[!MORELIKETHIS]
>
>* [發佈檔案](publishing-files.md#publishing_files)

