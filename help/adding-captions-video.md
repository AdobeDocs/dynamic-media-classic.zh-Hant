---
title: 增加註解至視訊
description: 瞭解如何新增字幕至視訊
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media經典，觀眾，影片
role: Business Practitioner
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 51%

---

# 增加註解至視訊{#adding-captions-to-video}

您可以在單一視訊或最適化視訊集中加入註解，將您的視訊推向全球市場。您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

若要設定標題效果並編輯標題功能表本身，包括下列任何檢視器的功能表文字：

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` 檢視器
* `Universal_HTML5_MixedMedia_light` 檢視器

請參閱[新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

Dynamic MediaClassic可將標題檔案轉換為JSON（JavaScript™物件註解）格式。 這項轉換意味著您可以在網頁中內嵌 JSON 文字，成為隱藏但完整的視訊文字。然後搜尋引擎可以搜尋並索引內容，讓影片更容易被發現，並提供客戶更多有關視訊內容的詳細資訊。

如需在URL中使用JSON函式的詳細資訊，請參閱&#x200B;*Adobe影像服務API說明*&#x200B;中的[伺服靜態（非影像）內容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)。

**增加註解至視訊**

1. 使用Dynamic Media經典影像以外的協力廠商應用程式，根據您使用的檢視器類型建立您的影片標題檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。註解檔案的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/):網頁視訊文字追蹤格式。<br><br>您可以免費和付費購買工具和服務，用於在Dynamic MediaClassic以外製作標題檔。例如，若要建立沒有樣式的簡單視訊標題檔案，您可以使用下列免費的線上標題製作和編輯工具：<br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>為獲得最佳效果，請使用Internet Explorer 9或更新版本、Google Chrome或Safari中的工具。 <br><br>在此工具的 <b>Enter URL of video file</b> 欄位中，貼上視訊檔案的 URL，然後按一下 <b>Load</b>。<br><br>例如，如果您的視訊檔案使用Dynamic Media經典URL，請連按兩下個別視訊資產（非最適化視訊集或主視訊），以在詳細資料檢視中開啟它。在「詳細檢視」的右側面板中，展開「URL 和內嵌程式碼」。接著，在「行動裝置」群組下的「行動裝置 (漸進式)」右側，按一下「複製 URL」。此程式會提供視訊檔案本身的URL，您可將它貼入視訊檔案的<b>輸入視訊檔案的URL</b>欄位。 然後，Internet Explorer、Chrome或Safari就可以原生播放視訊。此時，請遵循網站畫面上的指示，撰寫並儲存您的 WebVTT 檔案。完成時，請將註解檔案內容複製並貼至純文字編輯器中，並以 .vtt 副檔名儲存。<br><br><b>注意：</b> 若要全域支援英文以外的語言的視訊標題，WebVTT標準要求您針對想要支援的每種語言分別建立。vtt檔案和呼叫。<br><br>一般而言，我們建議您用和視訊檔案相同的名稱來命名 VTT 註解檔案，然後在名稱後附加 captions。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。 |

1. 在Dynamic MediaClassic中，上傳您的WebVTT、DFXP或SMPTE XML標題檔案。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的註解檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一資產，然後在資產的縮圖影像下方按一下「**[!UICONTROL 預覽]**」>「**[!UICONTROL 檢視器清單]**」。
1. 在「檢視器清單」表格中，尋找名為&#x200B;**Universal_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;或&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;的HTML5檢視器，然後執行下列其中一項：

   * 如欲以彈出式視窗使用視訊檢視器，請按一下名稱最右側的「**[!UICONTROL 複製 URL]**」。

      以下列語法附加複製的視訊 URL，使其與複製的註解檔案 URL 產生關聯:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      請注意標題URL路徑結尾的`,1`。 緊接在路徑中的。vtt副檔名後，您可以選擇性地啟用或停用視訊播放器列上的隱藏字幕按鈕，方法是分別設定為`1`或`0`。

   * 如欲以內嵌視訊使用檢視器，請按一下名稱最右側的「**[!UICONTROL 內嵌程式碼]**」。

      在「內嵌程式碼」對話框中，按一下「**[!UICONTROL 複製至剪貼簿]**」。

      對於HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`或`Universal_HTML5_MixedMedia_light`檢視器，請附加複製的內嵌程式碼，內容如下：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      請注意URL路徑結尾的`,1`。 緊接在URL路徑中的。vtt副檔名後，您可以選擇性地啟用或停用視訊播放器列上的標題按鈕，方法是分別設定為`1`或`0`。
