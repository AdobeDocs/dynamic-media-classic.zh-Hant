---
title: 增加章節標記視訊
seo-title: 增加章節標記視訊
description: 'null'
seo-description: 瞭解如何新增章節標籤至視訊。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 87%

---


# 增加章節標記視訊{#adding-chapter-markers-to-video}

透過加入章節標記至單一視訊或最適化視訊集中，您可以讓您的長版視訊更易於觀看或導覽。使用者播放視訊時，他們可以按一下視訊時間軸上的章節記號 (也稱為視訊筆畫壓感)，輕鬆導覽到感興趣的點，或立即跳至新內容、示範、教學課程等等。

>[!NOTE]
>
>使用的視訊播放程式必須支援使用章節記號。

請參閱[增加或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)，以設定 `Universal_HTML5_Video` 檢視器 (HTML5) 的章節導覽提示點和章節標題彈出式文字。

另請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

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

在上述範例中，`Chapter 1`是提示識別碼，是選用的。 `00:00:000 --> 01:04:364` 的提示時間指定章節的開始時間和結束時間，格式為 00:00:000。最後的三個數字為毫秒，如需要可保留為 000。`The bicycle store behind it all`的章節標題是章節內容的實際說明。 當使用者將滑鼠指標移過視訊時間軸中的視覺提示點時，提示識別名稱、開始提示時間和章節標題全都會出現在視訊播放程式的彈出式視窗中。

因為您使用 HTML5 視訊檢視器，請確定您所建立的章節檔案符合 WebVTT (Web Video Text Tracks) 標準。章節檔案名稱的副檔名為 .vtt。您可以深入瞭解有關 WebVTT 註解標準的資訊。

請參閱[WebVTT:網頁視訊文字軌道格式](https://dev.w3.org/html5/webvtt/)。

**增加章節標記至視訊**

1. 使用Dynamic Media Classic外部的簡單文字編輯器，建立您的視訊章節檔案。

   >[!NOTE]
   >
   >若要對視訊章節提供非英文語言的全域支援，請注意，根據 WebVTT 標準，您必須針對要支援的每個語言，建立個別的 .vtt 檔案和呼叫。

1. 將 .vtt 檔案以 UTF8 編碼儲存可避免章節標題文字中的節目字元發生問題。

   一般而言，我們建議您用和視訊檔案相同的名稱來命名章節 VTT 檔案，然後在名稱後附加「`chapters`」。如此一來，系統便可使用既有的網頁內容管理系統自動產生視訊 URL。

1. 在Dynamic Media Classic中，上傳您的WebVTT章節檔案。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 在左側的「資產庫」面板中，導覽至要與已上載的章節檔案相關聯的視訊檔案所在的資產資料夾。
1. 在「資產瀏覽」面板中，選取單一資產，然後在資產的縮圖影像下方按一下「**[!UICONTROL 預覽]**」>「**[!UICONTROL 檢視器清單]**」。
1. 在「檢視器清單」表格中，找到命名為「**Univeral_HTML5_Video**」的 HTML5 檢視器，然後執行下列任一操作:

   * 如欲以彈出式視窗使用視訊檢視器，請按一下名稱最右側的「**[!UICONTROL 複製 URL]**」。

      以下列語法附加複製的視訊 URL，使其與複製的註解檔案 URL 產生關聯:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 如欲以內嵌視訊使用檢視器，請按一下名稱最右側的「**[!UICONTROL 內嵌程式碼]**」。

      在「內嵌程式碼」對話框中，按一下「**[!UICONTROL 複製至剪貼簿]**」。

      對於HTML5 `Universal_HTML5_Video`檢視器，請附加複製的內嵌程式碼，並附加下列項目：

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

