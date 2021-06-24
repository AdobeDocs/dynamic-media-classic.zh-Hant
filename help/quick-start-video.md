---
title: '"快速入門: 視訊"'
description: AdobeDynamic Media Classic影片的簡介和快速入門，可協助您快速上手並執行。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic，檢視器，影片
role: Business Practitioner
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 43%

---

# 快速入門: 視訊{#quick-start-video}

AdobeDynamic Media Classic Video是端對端解決方案，可讓您輕鬆發佈高品質的最適化視訊，以在多個螢幕間串流，包括桌上型電腦、iOS、Android™、BlackBerry®和Windows®行動裝置。 最適化視訊集會將以不同位元速率和格式 (如 400 kbps、800 kbps 和 1000 kbps) 編碼之相同視訊的版本分組。桌上型電腦或行動裝置會偵測可用的頻寬。

例如，iOS 行動裝置會偵測 3G、4G 或 Wi-Fi 的頻寬。然後，它會自動從最適化視訊集的各種視訊位元速率中選取正確編碼的視訊。視訊會串流至桌上型電腦、行動裝置或平板電腦。

此外，如果桌上型電腦或行動裝置上的網路條件有所變更，則視訊品質會自動動態切換。此外，如果客戶在桌上型電腦上進入全螢幕模式，適用性視訊集會使用更佳的解析度來回應，改善客戶的觀看體驗。 使用最適化視訊集，可讓客戶在多個畫面和裝置上播放Dynamic Media Classic視訊，獲得最佳的播放效果。

在播放期間，視訊播放程式用來判斷要播放或選取之編碼視訊的邏輯乃是基於下列演算法:

1. 視訊播放器會根據最接近播放器本身中為「初始位元速率」所設定的值的位元速率，載入初始視訊片段。
1. 視訊播放器會根據頻寬速度的變更，使用下列條件進行切換：

   1. 播放器會選擇低於或等於估計頻寬的最高頻寬流。
   1. 播放器僅考慮可用頻寬的80%。 然而，如果它在轉換，則只有70%會更為保守，以避免高估，並且不得不立即重新轉換。

如需相關技術資訊，請參閱演算法的邏輯，網址為[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)。

若要管理單一視訊和最適化視訊集，Dynamic Media Classic支援下列功能：

* 從多種支援的視訊格式和音訊格式上載視訊，並將視訊編碼為 MP4 H.264 格式，以便在多種螢幕上播放。您可以使用預先定義的Dynamic Media Classic最適化視訊預設集、單一視訊編碼預設集，或自訂自己的編碼以控制視訊的品質和大小。

   產生最適化視訊集時，會包含MP4視訊。

   >[!NOTE]
   >
   >主版/來源視訊和任何其他來源格式視訊皆已新增至適用性視訊集&#x200B;*not*。

* Universal_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light檢視器中的視訊字幕，以及Universal_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light檢視器中的視訊章節導覽。

   請參閱[增加註解至視訊](adding-captions-video.md)。

   請參閱[增加章節標記至視訊](adding-chapter-markers-video.md)。

* 以完整中繼資料支援來組織、瀏覽和搜尋視訊，以有效管理視訊資產。
* 將最適化視訊集傳送至網路、桌上型電腦和行動裝置，包括iPhone、iPad、Android™、BlackBerry®和Windows®手機。

   各種iOS平台均支援最適化視訊串流。

   請參閱[Adobe檢視器參考指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)中的最新支援。

   Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。 您可以在以下網站上找到支援此視頻格式的BlackBerry®設備：

   請參閱[BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)上支援的視訊格式。

   您可以在以下位置找到支援此視頻格式的Windows®設備：

   請參閱[Windows® Phone](https://docs.microsoft.com/en-us/)上支援的視訊格式。

* 使用Dynamic Media Classic檢視器預設集播放視訊，包括下列內容：

   * 單一視訊檢視器。
   * 合併視訊和影像內容的混合媒體檢視器。

* 設定視訊播放器來滿足您的品牌推廣需要。
* 透過一個簡單的 URL 或內嵌程式碼將視訊整合到您的網站、行動網站或行動應用程式。

**快速入門**

下列逐步工作流程說明旨在協助您在Dynamic Media Classic中使用最適化視訊集快速上手並執行。 每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

## 1.上傳和編碼視訊

使用下列其中一個案例，上載並產生最適化視訊集: 

* **上傳預先編碼的影片**  — 如果您的影片已在Dynamic Media Classic外部編碼，請在全域導覽列上，按一下 **** 「上傳」以瀏覽MP4影片檔案，並直接上傳至Dynamic Media Classic。然後，按一下「**[!UICONTROL 建置]** > **[!UICONTROL 最適化視訊集]**」。瀏覽至視訊檔案。拖放您要的視訊檔案至「最適化視訊集」表格，然後儲存視訊集。
* **上傳主視訊**  — 如果您的視訊未編碼，請在全域導覽列上按一 **** 下「上傳」 ，上傳主視訊來源檔案（非MP4），並讓Dynamic Media Classic為您的MP4檔案編碼。在&#x200B;**[!UICONTROL 上載作業選項]**&#x200B;對話框的&#x200B;**[!UICONTROL EVideo選項]**&#x200B;下，選擇&#x200B;**[!UICONTROL 自適應視頻]**。

   此優先選項可讓您建立會自動套用正確編碼預設集至視訊的最適化視訊集 (無論是 16:9 還是 4:3)，以符合您所上載之視訊的尺寸。當您送出上載工作時，系統會自動為您建立一個最適化視訊集，內含三個具有正確外觀比例的視訊編碼。

   或者，在相同的&#x200B;**[!UICONTROL 作業選項]**&#x200B;對話框的&#x200B;**[!UICONTROL EVideo選項]**&#x200B;下，展開&#x200B;**[!UICONTROL 單一編碼預設集]**。從&#x200B;**Desktop**、**Mobile(iPhone、iPad、Android™)**&#x200B;和&#x200B;**平板電腦(iPad、Android™)**&#x200B;中，選擇您想要的個別視訊編碼預設集，以便建立MP4檔案。

* 或者，您可以使用&#x200B;**[!UICONTROL Reprocess]**&#x200B;功能重新處理主視訊。 新編碼的視訊會增加到現有的最適化視訊集。

請參閱[上載與編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**選擇性**

Dynamic Media Classic提供許多預先定義的視訊編碼預設集。 這些預先定義的預設會反映目前最常用的視訊編碼設定，並針對在目標頁面上播放而最佳化。

不過，如需進一步的自訂，管理員可以建立「視訊預設集」來自訂視訊的大小和終端使用者的播放體驗。管理員可以從&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**&#x200B;下的「視頻預設集」頁面添加和管理視頻預設集。 「視訊預設集」頁面可提供增加、編輯、刪除及啟用視訊預設集所需的選項。

請參閱[使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets)。

## 2.在視訊檢視器中預覽視訊

若要查看終端使用者在桌上型電腦、您的網站或是行動裝置上看到的視訊播放方式，請在瀏覽面板中選取該視訊，然後按一下「**[!UICONTROL 預覽]**」。

請參閱[在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

您可以在預覽頁面上播放視訊。 您也可以選擇不同的影片檢視器，以了解您的影片在不同播放器中的顯示方式。 最佳做法是使用 HTML5 視訊播放器，以便在桌上型電腦、平板電腦和行動裝置的多種螢幕上播放。

**選擇性**

檢視器預設集自訂 — Dynamic Media Classic提供預先定義的檢視器預設集，以傳送視訊。 這些預設集決定了檢視器的外觀及其播放控制項的工作方式。若要自訂視訊檢視器，管理員可以在「檢視器預設集」頁面中增加及管理檢視器預設集。若要開啟此頁面，請在Dynamic Media Classic的右上角按一下「**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**」。 「檢視器預設集」頁面可提供增加、編輯、刪除及啟用檢視器預設集所需的命令。

請參閱[使用視訊檢視器預設集](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

## 3.將影片部署至您的網站和行動網站

若要將視訊整合至網站，您可執行下列其中一項作業: 

* 在自己的快顯視窗或強制回應視窗中顯示視訊，在此情況下，請使用&#x200B;**[!UICONTROL 複製URL]**&#x200B;功能。

   若要取得視訊的 URL，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中加以選取。按一下「**[!UICONTROL 預覽]**」，然後按一下`Universal_HTML5_Viewer`右側的「複製URL ]**」。**[!UICONTROL 

   按一下「**[!UICONTROL 複製URL]**」時，URL會複製到剪貼簿。 將此程式碼放置在網站、行動裝置網站或應用程式的 HTML 中。

   >[!NOTE]
   >
   >URL 只會在您發佈視訊或最適化視訊集之後啟用。

* 顯示內嵌在網頁上的視訊，在此情況下，請使用&#x200B;**[!UICONTROL 內嵌程式碼]**&#x200B;功能。

   若要取得視訊的內嵌程式碼，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中選取該視訊。按一下「**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**」。 在表格的「動作」欄下，按一下`Universal_HTML5_Video`右側的&#x200B;**[!UICONTROL 內嵌程式碼]**。 不允許編輯程式碼。

   按一下「**[!UICONTROL 關閉]**」，然後將內嵌程式碼貼到您的網頁中。

   >[!NOTE]
   >
   >內嵌程式碼只會在您發佈視訊或最適化視訊集之後啟用。

請參閱[將視訊部署到網站和行動網站](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [視訊編碼最佳實踐](uploading-encoding-videos.md#best_practices_for_video_encoding)

