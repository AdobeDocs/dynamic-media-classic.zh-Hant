---
title: 增加註解至視訊
seo-title: 增加註解至視訊
description: 'null'
seo-description: 瞭解如何新增字幕至視訊
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 70%

---


# 增加註解至視訊{#adding-captions-to-video}

您可以在單一視訊或最適化視訊集中加入註解，將您的視訊推向全球市場。您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

請參閱[增加或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)以設定「註解效果」，以及編輯「註解選單」本身，包括以下任一檢視器的選單文字:

* `Universal_HTML5_Video` viewer.
* `Universal_HTML5_MixedMedia_dark` viewer.
* `Universal_HTML5_MixedMedia_light` viewer.

另請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

Dynamic Media Classic可將標題檔案轉換為JSON（JavaScript物件註解）格式。 這項轉換意味著您可以在網頁中內嵌 JSON 文字，成為隱藏但完整的視訊文字。搜尋引擎便可以為內容建立編目或索引，讓視訊更易於尋找，為客戶提供更多有關視訊內容的詳細資訊。

See [Serving static (non-image) contents](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**增加註解至視訊**

1. 使用 Scene7 Publishing System 以外的第三方應用程式，根據您所使用的檢視器類型建立視訊註解檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。註解檔案的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://dev.w3.org/html5/webvtt/): 網頁視訊文字追蹤格式。 <br><br>您可以使用免費與付費的工具與服務，在 Scene7 Publishing System 以外撰寫註解檔案。例如，若要建立沒有樣式的簡單視訊標題檔案，您可以使用下列免費的線上標題製作和編輯工具： <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html)<br><br>為獲得最佳效果，請使用Internet Explorer 9或更新版本、Google Chrome或Safari中的工具。 <br><br>在此工具的 <b>Enter URL of video file</b> 欄位中，貼上視訊檔案的 URL，然後按一下 <b>Load</b>。<br><br>例如，如果您的視訊檔案使用Dynamic Media Classic URL，請在SPS中連按兩下個別視訊資產（非最適化視訊集或主視訊），以在詳細資料檢視中開啟它。 在「詳細檢視」的右側面板中，展開「URL 和內嵌程式碼」。接著，在「行動裝置」群組下的「行動裝置 (漸進式)」右側，按一下「複製 URL」。This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. 然後，Internet Explorer、Chrome或Safari就可以原生播放視訊。此時，請遵循網站畫面上的指示，撰寫並儲存您的 WebVTT 檔案。完成時，請將註解檔案內容複製並貼至純文字編輯器中，並以 .vtt 副檔名儲存。<br><br><b>注意：</b> 若要全域支援英文以外的語言的視訊標題，請注意，WebVTT標準要求您針對想要支援的每種語言建立個別的。vtt檔案和呼叫。 <br><br>一般而言，我們建議您用和視訊檔案相同的名稱來命名 VTT 註解檔案，然後在名稱後附加 captions。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。 |

1. 在 Scene7 Publishing System 中，上載您的 WebVTT、DFXP 或 SMPTE XML 註解檔案。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的註解檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一資產，然後在資產的縮圖影像下方按一下「**預覽**」>「**檢視器清單**」。
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * 如欲以彈出式視窗使用視訊檢視器，請按一下名稱最右側的「**複製 URL**」。

      以下列語法附加複製的視訊 URL，使其與複製的註解檔案 URL 產生關聯:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. 緊接在路徑中的 .vtt 副檔名之後，您可以選擇啟用或停用視訊播放程式列上的隱藏式註解按鈕 (方法分別是設為 `1` 或 `0`)。

   * 如欲以內嵌視訊使用檢視器，請按一下名稱最右側的「**內嵌程式碼**」。

      在「內嵌程式碼」對話框中，按一下「**複製至剪貼簿**」。

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. 緊接在 URL 路徑中的 .vtt 副檔名之後，您可以選擇啟用或停用視訊播放程式列上的註解按鈕 (方法分別是設為 `1` 或 `0`)。

