---
title: '向視頻添加字幕 '
description: 了解如何在Dynamic Media Classic中為視訊新增字幕。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic，檢視器，影片
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 32%

---

# 向視頻添加字幕 {#adding-captions-to-video}

您可以在單一視訊或最適化視訊集中加入註解，將您的視訊推向全球市場。您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

要配置字幕效果並編輯字幕菜單本身，包括下列任意檢視器的菜單文本：

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` 檢視者
* `Universal_HTML5_MixedMedia_light` 檢視者

請參閱[新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另請參閱[新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

Dynamic Media Classic可將註解檔案轉換為JSON（JavaScript物件標籤法）格式。 這項轉換意味著您可以在網頁中內嵌 JSON 文字，成為隱藏但完整的視訊文字。然後，搜尋引擎可對內容進行編目並建立索引，讓您更容易找到影片，並為客戶提供影片內容的詳細資訊。

如需有關在URL中使用JSON函式的詳細資訊，請參閱&#x200B;*Adobe影像提供API說明*&#x200B;中的[提供靜態（非影像）內容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)。

**增加註解至視訊:**

1. 使用Dynamic Media Classic以外的協力廠商應用程式，根據您使用的檢視器類型建立您的視訊註解檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。註解檔案的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/):網路視訊文字追蹤格式。<br><br>您可使用免費和付費的工具和服務，在Dynamic Media Classic外製作註解檔案。例如，要建立不帶樣式的簡單視頻字幕檔案，可以使用以下免費線上字幕創作和編輯工具：<br><br>[WebVTT字幕製作器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>為獲得最佳結果，請使用Internet Explorer 9或更高版本、Google Chrome或Safari中的工具。 <br><br>在工具的「輸入視 <b>訊檔案的URL」欄</b> 位中，貼上視訊檔案的URL，然後選取「載 <b>入」</b>。<br><br>例如，如果您的視訊檔案使用Dynamic Media Classic URL，請連按兩下個別視訊資產（非適用性視訊集或主視訊），以在「詳細資料檢視」中開啟它。在「詳細檢視」的右側面板中，展開「URL 和內嵌程式碼」。然後在「行動裝置」群組下方的「行動裝置」（漸進式）右側，選取「<b>複製URL</b>」。 此程式會提供視訊檔案本身的URL，然後您可將其貼入視訊檔案<b>的「輸入URL」欄位</b>。 然後，Internet Explorer、Chrome或Safari就可以原生播放視訊。此時，請遵循網站畫面上的指示，撰寫並儲存您的 WebVTT 檔案。完成後，複製字幕檔案內容並貼到純文字編輯器中，然後以VTT副檔名儲存。 <br><br><b>注意： </b> 若要以英文以外的語言支援視訊標題，WebVTT標準需要您針對您要支援的每種語言建立個別的.vtt檔案和呼叫。<br><br>一般而言，我們建議您用和視訊檔案相同的名稱來命名 VTT 註解檔案，然後在名稱後附加 captions。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。 |

1. 在Dynamic Media Classic中，上傳您的WebVTT、DFXP或SMPTE XML註解檔案。

   請參閱[上傳檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的註解檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方，選取「預覽&#x200B;**** > **[!UICONTROL 檢視器清單]**」。
1. 在「查看器清單」表中，找到名為&#x200B;**Univeral_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;或&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;的HTML5查看器，然後執行以下操作之一：

   * 對於快顯視訊檢視器體驗，請選取名稱最右側的&#x200B;**[!UICONTROL 複製URL]**。

      使用下列語法附加視訊的複製URL，以便將其與複製的URL關聯至註解檔案：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      注意標題URL路徑末尾的`,1`。 緊接在路徑中的VTT副檔名後面，您可以選擇性地啟用或停用視訊播放器列上的隱藏式字幕按鈕，方法是分別將設定為`1`或`0`。

   * 針對內嵌的視訊檢視器體驗，選取名稱最右側的&#x200B;**[!UICONTROL 內嵌程式碼]**。

      在「內嵌代碼」對話方塊中，選取「**[!UICONTROL 複製到剪貼簿]**」。

      對於HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`或`Universal_HTML5_MixedMedia_light`檢視器，請將複製的內嵌程式碼附加至下列項目：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      記下URL路徑結尾的`,1`。 緊接在URL路徑中的VTT副檔名後面，您可以選擇性地啟用或停用視訊播放器列上的註解按鈕，方法是分別將設定為`1`或`0`。
