---
title: 將章節標籤新增至視訊
description: 瞭解如何在Adobe Dynamic Media Classic中新增章節標籤至影片。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 28%

---

# 將章節標籤新增至視訊 {#adding-chapter-markers-to-video}

您可以新增章節標籤至單一視訊或自我調整視訊集，讓長格式視訊更易於觀看和導覽。 當使用者播放視訊時，他們可以在視訊時間軸上選取章節標籤（也稱為視訊筆畫壓感）。 如此可讓他們輕鬆導覽至興趣點，或立即跳至新內容、示範、教學課程等。

>[!NOTE]
>
>使用的視訊播放程式必須支援使用章節記號。

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) 如果您想要為以下專案設定章節導覽提示點和章節標題快顯文字： `Universal_HTML5_Video` 檢視器(HTML5)。

另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

為視訊建立章節清單的方式與建立註解的方式非常類似。也就是說，您會建立 WebVTT 檔案。但請注意，該檔案必須與您可能在使用的任何 WebVTT 註解檔案不同；您不能將註解與章節合併在一個 WebVTT 檔案中。

您可以使用下列範例，做為用來建立含有章節導覽之 WebVTT 檔案的格式範例:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

在上述範例中， `Chapter 1` 是提示識別碼，且為選用。 的提示時間 `00:00:000 --> 01:04:364` 指定章節的開始時間和結束時間（以00為單位）:00:000格式。 最後的三個數字為毫秒，如需要可保留為 000。的章節標題 `The bicycle store behind it all` 是章節內容的實際說明。 當指標停留在視訊時間軸中的視覺提示點上時，提示識別碼、開始提示時間和章節標題都會顯示在視訊播放器的快顯視窗中。

因為您使用 HTML5 視訊檢視器，請確定您所建立的章節檔案符合 WebVTT (Web Video Text Tracks) 標準。章節副檔名為.VTT。 您可以深入瞭解有關 WebVTT 註解標準的資訊。

另請參閱 [WebVTT：網頁視訊文字追蹤格式](https://w3c.github.io/webvtt/).

**若要將章節標籤新增至視訊：**

1. 使用Adobe Dynamic Media Classic外部的簡單文字編輯器，建立您的視訊章節檔案。

   >[!NOTE]
   >
   >為了全球支援英文以外的其他語言的視訊章節，WebVTT標準要求您為要支援的每種語言建立個別的.vtt檔案和呼叫。

1. 請以UTF8編碼儲存VTT檔案，這樣就能避免在章節標題文字中出現字元轉譯問題。

   一般來說，您會想要將章節VTT檔案命名為與視訊檔案相同的名稱，並附加上 `chapters`. 如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。

1. 在Adobe Dynamic Media Classic中，上傳您的WebVTT章節檔案。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 在左側的「資產庫」面板中，導覽至包含要與您上傳的章節檔案建立關聯的視訊檔案的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方選取「 」 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
1. 在「檢視器清單」表格中，找到命名為「**Univeral_HTML5_Video**」的 HTML5 檢視器，然後執行下列任一操作:

   * 若要取得快顯視訊檢視器體驗，請選取 **[!UICONTROL 複製URL]** 名稱的最右側。

     使用以下語法附加複製的視訊URL，以便將其與複製的標題URL建立關聯：

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 若要取得內嵌視訊檢視器體驗，請選取「 」 **[!UICONTROL 內嵌程式碼]** 名稱的最右側。

     在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

     針對HTML5 `Universal_HTML5_Video` 檢視器，請在複製的內嵌程式碼後附加下列內容：

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
