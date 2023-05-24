---
title: 新增註解至視訊
description: 瞭解如何在Adobe Dynamic Media Classic中為影片新增字幕。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# 新增註解至視訊 {#adding-captions-to-video}

您可以在單一視訊或最適化視訊集中加入註解，將您的視訊推向全球市場。您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

若要設定「註解效果」並編輯「註解選單」本身，包括下列任一檢視器的選單文字：

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic可以將註解檔案轉換為JSON （JavaScript物件標籤法）格式。 這項轉換意味著您可以在網頁中內嵌 JSON 文字，成為隱藏但完整的視訊文字。搜尋引擎接著可以編目和索引內容，讓視訊更容易被發現，並為客戶提供更多有關視訊內容的詳細資訊。

另請參閱 [提供靜態（非影像）內容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) 在 *Adobe影像伺服API說明* 以取得在URL中使用JSON函式的詳細資訊。

**增加註解至視訊:**

1. 使用Adobe Dynamic Media Classic外部的第三方應用程式，根據您使用的檢視器型別建立您的視訊註解檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。註解檔案的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/)：網頁視訊文字追蹤格式。 <br><br>您可以在Adobe Dynamic Media Classic外部使用免費和付費的工具和服務來製作註解檔案。 例如，若要建立不含樣式的簡單視訊註解檔案，您可以使用下列免費線上註解製作與編輯工具： <br><br>[WebVTT註解製作器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>為達到最佳效果，請在Internet Explorer 9或更新版本、Google Chrome或Safari中使用工具。 <br><br>在工具中，在 <b>輸入視訊檔案的URL</b> 欄位，貼上視訊檔案的URL，然後選取 <b>載入</b>. <br><br>例如，如果您正在使用Adobe Dynamic Media Classic URL作為視訊檔案，請按兩下個別視訊資產（非最適化視訊集或主要視訊）以在「詳細資料檢視」中開啟它。 在「詳細檢視」的右側面板中，展開「URL 和內嵌程式碼」。然後在「行動」群組下方的「行動」 （漸進式）右側，選取 <b>複製URL</b>. 此程式會提供視訊檔案本身的URL，您隨後可將其貼到 <b>輸入視訊檔案的URL</b> 欄位。 Internet Explorer、Chrome 或 Safari 接著即可以原生方式播放視訊。此時，請遵循網站畫面上的指示，撰寫並儲存您的 WebVTT 檔案。完成後，複製註解檔案內容並將其貼到純文字編輯器中，並以VTT副檔名儲存。 <br><br><b>注意：</b> 為了全球支援英文以外的其他語言的視訊註解，WebVTT標準要求您建立個別的.vtt檔案，並針對您想要支援的每種語言呼叫。 <br><br>一般而言，我們建議您用和視訊檔案相同的名稱來命名 VTT 註解檔案，然後在名稱後附加 captions。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。 |

1. 在Adobe Dynamic Media Classic中，上傳您的WebVTT、DFXP或SMPTE XML註解檔案。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 在左側的「資產庫」面板中，導覽至要與已上載的註解檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方選取「 」 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
1. 在「檢視器清單」表格中，找到名為的HTML5檢視器 **Univeral_HTML5_影片**， **Universal_HTML5_MixedMedia_dark**，或 **Universal_HTML5_MixedMedia_light**，然後執行下列任一項作業：

   * 若要取得快顯視訊檢視器體驗，請選取「 」 **[!UICONTROL 複製URL]** 名稱的最右側。

      將複製的影片URL附加至下列語法，這樣您就可以將它與複製的URL與註解檔案建立關聯：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      請注意 `,1` 在註解URL路徑結尾。 路徑中的VTT副檔名後面緊接著可以設定為，選擇性地啟用或停用視訊播放器列上的隱藏式字幕按鈕 `1` 或 `0`（分別）。

   * 若要內嵌視訊檢視器體驗，請選取「 」 **[!UICONTROL 內嵌程式碼]** 名稱的最右側。

      在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

      針對HTML5 `Universal_HTML5_Video`， `Universal_HTML5_MixedMedia_dark`，或 `Universal_HTML5_MixedMedia_light` 檢視器，請在複製的內嵌程式碼後附加下列內容：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      請注意 `,1` 在URL路徑結尾。 在URL路徑中的VTT副檔名後面，您可以視需要選擇將設定為，啟用或停用視訊播放器列上的註解按鈕 `1` 或 `0`（分別）。
