---
title: 新增註解至視訊
description: 瞭解如何在Adobe Dynamic Media Classic中為影片新增註解。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 17%

---

# 新增註解至視訊 {#add-captions-to-video}

將視訊的觸角伸展至全球市場。 若要這麼做，您可以在單一視訊或最適化視訊集新增字幕。 您可增加字幕，如此一來便無須為音訊配音或請本地人重新以不同語言錄製音訊。以錄製的語言播放視訊。畫面會出現外國語言字幕，以便使用不同語言的人瞭解音訊部份的內容。

為有聽力障礙或重聽問題的使用者提供隱藏式字幕，註解功能可提供更佳的協助工具服務。

>[!NOTE]
>
>您使用的視訊播放程式必須支援顯示註解功能。

若要設定「註解效果」並編輯「註解選單」本身，包括下列任一檢視器的選單文字：

* `Universal_HTML5_Video` 檢視者
* `Universal_HTML5_MixedMedia_dark` 檢視者
* `Universal_HTML5_MixedMedia_light` 檢視者

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic可以將註解檔案轉換為JSON （JavaScript物件標籤法）格式。 此轉換表示您可以將JSON文字內嵌至網頁，做為影片隱藏但完整的文字記錄。 搜尋引擎接著可以編目和索引內容，讓影片更容易被找到，並為客戶提供更多有關影片內容的詳細資訊。

另請參閱 [提供靜態（非影像）內容](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) 中的以取得在URL中使用JSON函式的詳細資訊。

**若要在視訊中新增註解：**

1. 使用Adobe Dynamic Media Classic以外的協力廠商應用程式，根據您使用的檢視器型別建立視訊標題檔案。

   | 檢視器類型 | 註解檔案 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 視訊檢視器，請確定您所建立的註解檔案符合 WebVTT (Web Video Text Tracks) 標準。字幕副檔名為 `.VTT`. 您可以深入瞭解有關 WebVTT 註解標準的資訊。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/)：網頁視訊文字追蹤格式。 <br><br>有許多網站提供免費和收費的工具與服務，供您用來撰寫WebVTT插圖示題檔案。 <br><br>依照網站上的熒幕指示製作及儲存您的WebVTT檔案。 完成後，複製註解檔案內容並貼到純文字編輯器中，以VTT副檔名儲存。 <br><br><b>注意：</b> 為了在全球支援英文以外的其他語言的視訊標題，WebVTT標準要求您建立個別的 `.VTT` 您要支援的每種語言的檔案和呼叫。 <br><br>通常，您會想要將註解VTT檔案命名為與視訊檔案相同的名稱，並附加註解。 如此一來，即可協助您使用現有的網頁內容管理系統，自動化視訊URL的產生作業。 |

1. 在Adobe Dynamic Media Classic中，上傳您的WebVTT、DFXP或SMPTE XML標題檔案。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 在左側的「資產庫」面板中，導覽至包含視訊檔案的資產資料夾，以與您上傳的註解檔案建立關聯。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方選取「 」 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
1. 在「檢視器清單」表格中，找到名為的HTML5檢視器 **Univeral_HTML5_視訊**， **Universal_HTML5_MixedMedia_dark**，或 **Universal_HTML5_MixedMedia_light**，然後執行下列任一項作業：

   * 若要取得快顯視訊檢視器體驗，請選取 **[!UICONTROL 複製URL]** 名稱的最右側。

     使用以下語法附加複製的視訊URL，以便將其與複製的標題URL建立關聯：

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     請注意 `,1` 位於標題URL路徑結尾。 在路徑中的VTT副檔名後面緊接著著，您可以選擇將設定為，啟用或停用視訊播放器列上的隱藏式字幕按鈕 `1` 或 `0`，依序輸入。

   * 若要取得內嵌視訊檢視器體驗，請選取「 」 **[!UICONTROL 內嵌程式碼]** 名稱的最右側。

     在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

     針對HTML5 `Universal_HTML5_Video`， `Universal_HTML5_MixedMedia_dark`，或 `Universal_HTML5_MixedMedia_light` 檢視器，請在複製的內嵌程式碼後附加下列內容：

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     請注意 `,1` URL路徑結尾。 在URL路徑中的VTT副檔名後面緊接著，您可以選擇將設定為，啟用或停用視訊播放器列上的註解按鈕 `1` 或 `0`，依序輸入。
