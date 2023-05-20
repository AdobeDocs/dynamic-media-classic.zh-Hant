---
title: 將字幕添加到視頻
description: 瞭解如何在Adobe Dynamic Media Classic向視頻中添加字幕。
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

# 將字幕添加到視頻 {#adding-captions-to-video}

您可以在單一視訊或最適化視訊集中加入註解，將您的視訊推向全球市場。您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

要配置字幕效果並編輯字幕菜單本身，包括下列任何查看者的菜單文本：

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

請參閱 [添加或編輯視頻查看器預設](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另請參閱 [添加和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)。

Adobe Dynamic Media Classic可以將字幕檔案轉換為JSON（JavaScript對象表示法）格式。 這項轉換意味著您可以在網頁中內嵌 JSON 文字，成為隱藏但完整的視訊文字。然後，搜索引擎可以對內容進行爬網和索引，使視頻更容易被發現，並為客戶提供有關視頻內容的更多詳細資訊。

請參閱 [提供靜態（非影像）內容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) 的 *Adobe映像服務API幫助* 的子菜單。

**增加註解至視訊:**

1. 使用Adobe Dynamic Media Classic以外的第三方應用程式，根據您使用的查看器類型建立視頻字幕檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。註解檔案的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/):Web視頻字幕資訊格式。 <br><br>您可以使用免費和付費的工具和服務，在Adobe Dynamic Media Classic以外製作字幕檔案。 例如，要建立沒有樣式的簡單視頻標題檔案，可以使用以下免費聯機標題創作和編輯工具： <br><br>[WebVTT字幕製作](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>為獲得最佳結果，請在Internet Explorer 9或更高版本、GoogleChrome或Safari中使用該工具。 <br><br>在工具中，在 <b>輸入視頻檔案的URL</b> 欄位，貼上視頻檔案的URL，然後選擇 <b>載入</b>。 <br><br>例如，如果您使用視頻檔案的Adobe Dynamic Media ClassicURL，請按兩下單個視頻資產（不是自適應視頻集或主視頻）以在詳細資訊視圖中開啟它。 在「詳細檢視」的右側面板中，展開「URL 和內嵌程式碼」。然後，在移動組右側（累進）下，選擇 <b>複製URL</b>。 此過程將為您提供視頻檔案本身的URL，然後您可以將其貼上到 <b>輸入視頻檔案的URL</b> 的子菜單。 Internet Explorer、Chrome 或 Safari 接著即可以原生方式播放視訊。此時，請遵循網站畫面上的指示，撰寫並儲存您的 WebVTT 檔案。完成後，複製標題檔案內容並將其貼上到純文字檔案編輯器中，並使用VTT檔案副檔名將其保存。 <br><br><b>注：</b> 為了全局支援英語以外語言的視頻字幕，WebVTT標準要求您為要支援的每種語言建立單獨的.vtt檔案和呼叫。 <br><br>一般而言，我們建議您用和視訊檔案相同的名稱來命名 VTT 註解檔案，然後在名稱後附加 captions。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。 |

1. 在Adobe Dynamic Media Classic，上載WebVTT、DFXP或SMPTE XML標題檔案。

   請參閱 [上載檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的註解檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選擇單個視頻資產，然後在資產的縮略圖下面選擇 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
1. 在「查看器清單」(Viewer List)表格中，查找名為的HTML5查看器 **通用HTML5_視頻**。 **Universal_HTML5_MixedMedia_dark**&#x200B;或 **通用HTML5_MixedMedia_light**，然後執行以下操作之一：

   * 要獲得彈出式視頻查看器體驗，請選擇 **[!UICONTROL 複製URL]** 最右邊。

      使用以下語法添加視頻的複製URL，以便可以將其與複製的URL關聯到字幕檔案：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      注意 `,1` 標題URL路徑的末尾。 緊隨路徑中的VTT檔案副檔名後，可以通過設定為來啟用或禁用視頻播放器欄上的隱藏字幕按鈕 `1` 或 `0`的下界。

   * 對於嵌入式視頻查看器體驗，請選擇 **[!UICONTROL 嵌入代碼]** 最右邊。

      在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。

      HTML5 `Universal_HTML5_Video`。 `Universal_HTML5_MixedMedia_dark`或 `Universal_HTML5_MixedMedia_light` 查看器，在複製的嵌入代碼後添加以下內容：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      注意 `,1` 地址欄。 緊隨URL路徑中的VTT檔案名副檔名後，可以通過設定為來選擇啟用或禁用視頻播放器欄上的標題按鈕 `1` 或 `0`的下界。
