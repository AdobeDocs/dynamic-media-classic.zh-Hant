---
title: 新增章節標籤至視訊
description: 了解如何在Dynamic Media Classic中將章節標籤新增至視訊。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic，檢視器，影片
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 40%

---

# 新增章節標籤至視訊 {#adding-chapter-markers-to-video}

透過加入章節標記至單一視訊或最適化視訊集中，您可以讓您的長版視訊更易於觀看或導覽。當使用者播放視訊時，可以選取視訊時間軸上的章節標籤（也稱為視訊清除程式）。 如此可讓使用者輕鬆導覽至其興趣點，或立即跳至新內容、示範、教學課程等。

>[!NOTE]
>
>使用的視訊播放程式必須支援使用章節記號。

如果要配置`Universal_HTML5_Video`查看器(HTML5)的章節導航提示點和章節標題彈出文本，請參閱[添加或編輯視頻查看器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另請參閱[新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

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

在上述範例中，`Chapter 1`是提示識別碼，且為選用。 `00:00:000 --> 01:04:364`的提示時間以00:00:000格式指定章節的開始時間和結束時間。 最後的三個數字為毫秒，如需要可保留為 000。`The bicycle store behind it all`的章節標題是該章節內容的實際說明。 當指標置於影片時間軸的視覺提示點上方時，提示識別碼、開始提示時間和章節標題都會顯示在影片播放器的快顯視窗中。

因為您使用 HTML5 視訊檢視器，請確定您所建立的章節檔案符合 WebVTT (Web Video Text Tracks) 標準。章節副檔名為.VTT。 您可以深入瞭解有關 WebVTT 註解標準的資訊。

請參閱[WebVTT:Web視頻文本跟蹤格式](https://w3c.github.io/webvtt/)。

**增加章節標記至視訊:**

1. 使用Dynamic Media Classic以外的簡單文字編輯器，建立您的視訊章節檔案。

   >[!NOTE]
   >
   >為全域支援英文以外的語言的視訊章節，WebVTT標準要求您針對要支援的每種語言建立個別的.vtt檔案和呼叫。

1. 以UTF8編碼儲存VTT檔案，以避免章節標題文字的字元轉譯問題。

   一般而言，我們建議您用和視訊檔案相同的名稱來命名章節 VTT 檔案，然後在名稱後附加「`chapters`」。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。

1. 在Dynamic Media Classic中，上傳您的WebVTT章節檔案。

   請參閱[上傳檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的章節檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方，選取「預覽&#x200B;**** > **[!UICONTROL 檢視器清單]**」。
1. 在「檢視器清單」表格中，找到命名為「**Univeral_HTML5_Video**」的 HTML5 檢視器，然後執行下列任一操作:

   * 對於快顯視訊檢視器體驗，請選取名稱最右側的&#x200B;**[!UICONTROL 複製URL]**。

      使用下列語法附加視訊的複製URL，以便將其與複製的URL關聯至註解檔案：

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 針對內嵌的視訊檢視器體驗，選取名稱最右側的&#x200B;**[!UICONTROL 內嵌程式碼]**。

      在「內嵌代碼」對話方塊中，選取「**[!UICONTROL 複製到剪貼簿]**」。

      對於HTML5 `Universal_HTML5_Video`檢視器，請將複製的內嵌程式碼附加至下列項目：

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
