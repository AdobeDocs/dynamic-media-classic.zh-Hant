---
title: 將章節標籤添加到視頻
description: 瞭解如何將章節標籤添加到Adobe Dynamic Media Classic的視頻中。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 40%

---

# 將章節標籤添加到視頻 {#adding-chapter-markers-to-video}

透過加入章節標記至單一視訊或最適化視訊集中，您可以讓您的長版視訊更易於觀看或導覽。當用戶播放視頻時，他們可以選擇視頻時間軸上的章節標籤（也稱為視頻掃描器）。 這樣，他們就可以輕鬆瀏覽到自己的興趣點，或立即跳到新內容、演示、教程等。

>[!NOTE]
>
>使用的視訊播放程式必須支援使用章節記號。

請參閱 [添加或編輯視頻查看器預設](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) 如果要為 `Universal_HTML5_Video` 查看器(HTML5)。

另請參閱 [添加和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)。

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

在上例中， `Chapter 1` 是提示標識符，是可選的。 的提示時間 `00:00:000 --> 01:04:364` 指定本章的開始時間和結束時間，以00為單位:00:000格式。 最後的三個數字為毫秒，如需要可保留為 000。章標題 `The bicycle store behind it all` 是本章內容的實際描述。 當指針懸停在視頻時間軸中的視覺提示點上時，提示標識符、起始提示時間和章節標題都會出現在視頻播放器的彈出窗口中。

因為您使用 HTML5 視訊檢視器，請確定您所建立的章節檔案符合 WebVTT (Web Video Text Tracks) 標準。章檔案名副檔名為.VTT。 您可以深入瞭解有關 WebVTT 註解標準的資訊。

請參閱 [WebVTT:Web視頻字幕資訊格式](https://w3c.github.io/webvtt/)。

**增加章節標記至視訊:**

1. 使用Adobe Dynamic Media Classic外的簡單文本編輯器建立視頻章節檔案。

   >[!NOTE]
   >
   >要全局支援英語以外語言的視頻章節，WebVTT標準要求您為要支援的每種語言建立單獨的.vtt檔案和調用。

1. 以UTF8編碼保存VTT檔案，這樣您就可以避免章節標題文本中字元格式副本的問題。

   一般而言，我們建議您用和視訊檔案相同的名稱來命名章節 VTT 檔案，然後在名稱後附加「`chapters`」。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。

1. 在Adobe Dynamic Media Classic上傳WebVTT章節檔案。

   請參閱 [上載檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的章節檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選擇單個視頻資產，然後在資產的縮略圖下面選擇 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
1. 在「檢視器清單」表格中，找到命名為「**Univeral_HTML5_Video**」的 HTML5 檢視器，然後執行下列任一操作:

   * 要獲得彈出式視頻查看器體驗，請選擇 **[!UICONTROL 複製URL]** 最右邊。

      使用以下語法添加視頻的複製URL，以便可以將其與複製的URL關聯到字幕檔案：

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 對於嵌入式視頻查看器體驗，請選擇 **[!UICONTROL 嵌入代碼]** 最右邊。

      在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。

      HTML5 `Universal_HTML5_Video` 查看器，將複製的嵌入代碼添加到以下內容：

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
