---
title: 將視訊部署到網站和行動裝置網站
description: 了解如何從Adobe Dynamic Media Classic將視訊部署至您的網站和行動網站。
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

網站、行動網站和案頭應用程式可使用URL字串或內嵌程式碼來存取Adobe Dynamic Media Classic伺服器內容（包括視訊）。 Adobe Dynamic Media Classic會在發佈程式期間啟用這些URL字串。 若要將視訊的URL字串或內嵌程式碼放入網頁、行動頁面和案頭應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 或內嵌程式碼不會產生作用。

## 發佈視訊 {#publishing-video}

發佈視訊可讓Adobe Dynamic Media Classic伺服器傳送視訊至您的網站、行動網站或應用程式。

您可以使用兩種不同的方法來發佈視訊：

* **上傳時自動立即發佈影片**  — 在視訊上傳程式中，Adobe Dynamic Media Classic可在視訊上傳和編碼時自動發佈視訊。 此立即發佈功能意味著不需要另外再發佈視訊 (因為已經發佈了)。

* **在上載後手動發佈視訊**  — 如果您不想立即發佈影片，可隨時手動發佈影片。

發佈影片後，Adobe Dynamic Media Classic會為您的HTML頁面或應用程式程式碼啟用URL字串。

**發佈視訊:**

1. 進行以下一項操作:

   * 若要在上傳時自動立即發佈影片，請在「上傳」頁面中選取 **[!UICONTROL 上傳後發佈]**. 程序已完成，您不需要再做任何步驟。
   * 若要在上傳後手動發佈影片，請在「瀏覽」面板中選取影片，然後在全域導覽列上選取 **發佈**.

## 將視訊URL連結至行動網站或網站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

發佈視訊後，您便可以取得其 URL，以在您的網站、行動網站或桌上型電腦應用程式中使用。當您想要在網頁頂端的彈出式視窗或浮出視窗中顯示視訊，請使用視訊 URL。

當客戶選取連結時，會自動偵測其裝置、頻寬和螢幕大小。 系統會在預先定義的桌上型電腦檢視器或智慧型手機和平板電腦的行動裝置本機視訊播放器中，顯示適當的視訊以供播放。

另請參閱 [將視訊檢視器內嵌在網頁上](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**將視訊 URL 連結至行動網站或網站:**

1. 在「資產瀏覽」面板中， **[!UICONTROL 顯示]** 下拉清單，選擇 **[!UICONTROL 影片]** 或 **[!UICONTROL 最適化視訊集]**.
1. 在左側的「資產庫」面板中，瀏覽至包含您要連結之視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL」和「內嵌程式碼」面板中，選取「HTTP串流」下方 **[!UICONTROL 複製URL]** 右邊。 最佳作法是複製與 `Universal_HTML5_Video` 檢視器。
   * 選擇 **[!UICONTROL 網格視圖]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**. 最佳作法是複製與 `Universal_HTML5_Video` 檢視器。

   * 選擇 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**. 最佳作法是複製與 `Universal_HTML5_Video` 檢視器。

   * 選擇 **[!UICONTROL 網格視圖]**, **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**. 最佳作法是複製與 `Universal_HTML5_Video` 檢視器。

1. 將 HTML5 視訊 URL 連結貼到您的網站和行動網站上。

## 將視訊檢視器內嵌在網頁上 {#embedding-the-video-viewer-on-a-web-page}

當您想播放網頁上內嵌的視訊時，請使用「內嵌程式碼」功能。您可將內嵌代碼複製到剪貼簿，以便貼到網頁中。「內嵌代碼」對話方塊中不允許編 輯代碼 。

另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**在網頁上內嵌視訊檢視器:**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 影片]** 或 **[!UICONTROL 最適化視訊集]**.
1. 在左側的「資產庫」面板中，瀏覽至包含您要複製其內嵌程式碼的視訊或最適化視訊集的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，按兩下單一資產的視訊縮圖，即可在「詳細檢視」中開啟它。在右側的「URL」和「內嵌程式碼」面板中，選取「HTTP串流」下方 **[!UICONTROL 內嵌程式碼]** 右邊。 最佳實務是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。
   * 選擇 **[!UICONTROL 網格視圖]**. 在「資產瀏覽」面板中，選取單一資產，然後在視訊縮圖影像下方選取 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**. 最佳實務是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選擇 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**. 最佳實務是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選擇 **[!UICONTROL 網格視圖]**, **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**. 最佳實務是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

1. 在「內嵌程式碼」對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取 **[!UICONTROL 關閉]**.
1. 在您的網頁中貼上內嵌程式碼。

### 實作內嵌程式碼以搭配MP4視訊資產使用HTML5視訊 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

如果您未使用Adobe Dynamic Media ClassicHTML5視訊播放器，但想使用原生HTML5 `<video>` 標籤和MP4視訊資產，您可以使用下列內嵌程式碼範例：

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 取代 `"S7 video thumbnail URL"` 以及影片的縮圖URL，該URL是使用者在播放影片前所看到的影片縮圖影像。

   請參閱 [取得視訊縮圖URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* 取代 `"S7 OGG video asset URL (no player)"` 和OGG影片的漸進式URL。

   請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* 取代 `"S7 MP4 mobile progressive video asset URL (no player)"` 使用視訊的行動漸進式URL。

   請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## 使用協力廠商視訊播放器部署視訊 {#deploying-video-using-a-third-party-video-player}

如果您使用協力廠商視訊播放器或自訂內建視訊播放器，而非Dynamic Media Classic視訊檢視器，則可取得適用於HLS多位元速率視訊串流或漸進式下載的直接視訊URL。

**部署使用第三方視訊播放器的視訊:**

1. 在Adobe Dynamic Media Classic的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.
1. 依據您要使用的 URL 類型，執行下列其中一項工作: 

* 若要產生直接HLS串流視訊URL（多位元速率）

   在 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL 已發佈的伺服器名稱]** 文字欄位，建構直接URL。 使用下列語法： `server/is/content/company/folder/filename.m3u8`

   例如，假設已發佈的伺服器名稱為 `https://s7d9.scene7.com/.` 使用步驟2中的語法，直接URL看起來可能如下所示：
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 若要產生直接HLS串流視訊URL（單位元速率）

   在 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL HLS串流伺服器名稱]** 文字欄位，使用下列語法來建構直接URL:

   `server/company/folder/filename.ext.m3u8`

   例如，假設HLS串流伺服器名稱為 `https://s7mbrstream.scene7.com/hls-vod/`. 使用步驟2中的語法，直接URL看起來可能如下所示：
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 產生直接漸進式視訊 URL

   在「**[!UICONTROL 應用程式一般設定]**」頁面之「**[!UICONTROL 伺服器]**」群組的「**[!UICONTROL 漸進式視訊伺服器名稱]**」文字欄位上，使用下列語法建構直接 eVideo URL:

   `server/company/folder/filename`

   例如，假設漸進式視訊伺服器名稱為 `https://s7d9.scene7.com/is/content/`. 使用步驟2中的語法，直接URL看起來可能如下所示：
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用視訊縮圖 {#working-with-video-thumbnails}

Adobe Dynamic Media Classic會為編碼的視訊產生縮圖，並預先編碼視訊。 您可以像使用任何影像資產一樣使用視訊縮圖。此外，您還可以取得Adobe Dynamic Media Classic產生之視訊縮圖的URL。 接著，您可以在Adobe Dynamic Media Classic外部部署這些URL。 例如，您可以在網站的搜尋結果、相關視訊清單和視訊播放清單中部署縮圖。

縮圖的產生以視訊中的首個異質影格 (非全黑影格或全白影格等等) 為基礎。

### 取得視訊縮圖URL {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic會在上傳程式期間自動產生視訊縮圖。 縮圖會出現在「清單視圖」和「網格視圖」的「瀏覽」面板中。

若要產生視訊縮圖的 URL，請執行發佈作業。

請參閱 [發佈影片](deploying-video-websites-mobile-sites.md#publishing_video).

在發佈後，您可以在「URL 和內嵌程式碼」面板的「詳細檢視」中，取得視訊縮圖 URL。選擇 **[!UICONTROL 複製URL]** 影片縮圖的右側，以便複製其URL。

### 在視訊檢視器中修改海報影格 {#modifying-poster-frames-in-video-viewers}

「*海報影格*」是視訊開始播放之前在「視訊」檢視器中顯示的初始影格。Adobe Dynamic Media Classic使用視訊縮圖作為海報框架。

您可以將影像修飾元套用至海報影格。例如，您可以裁切海報影格或使其變得透明。若要修改海報影格，請開啟視訊檢視器配置畫面，並在「海報影像修飾元」區段輸入修飾元。

請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

請參閱 [影像提供指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

還可以透過將修飾元附加到視訊縮圖 URL 來修改視訊縮圖。

>[!MORELIKETHIS]
>
>* [發佈檔案](publishing-files.md#publishing_files)