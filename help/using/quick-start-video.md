---
title: 「快速入門：Adobe Dynamic Media Classic中的影片」
description: Adobe Dynamic Media Classic簡介和快速入門影片，可幫助您快速上手並執行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 25%

---

# 快速入門：Adobe Dynamic Media Classic中的影片{#quick-start-video}

Adobe Dynamic Media Classic Video是端對端解決方案，可讓您輕鬆發佈高品質的最適化視訊，以便跨多個畫面串流，包括桌上型電腦、iOS、Android™、BlackBerry®和Windows®行動裝置。 最適化視訊集會將以不同位元速率和格式 (如 400 kbps、800 kbps 和 1000 kbps) 編碼之相同視訊的版本分組。桌上型電腦或行動裝置會偵測可用的頻寬。

例如，iOS 行動裝置會偵測 3G、4G 或 Wi-Fi 的頻寬。然後，它會自動從最適化視訊集的各種視訊位元速率中選取正確編碼的視訊。視訊會串流至桌上型電腦、行動裝置或平板電腦。

此外，如果桌上型電腦或行動裝置上的網路條件有所變更，則視訊品質會自動動態切換。此外，如果客戶在桌上型電腦上進入全熒幕模式，Adaptive Video Set會使用更好的解析度來回應，進而改善客戶的觀看體驗。 使用「自我調整視訊集」可提供最佳播放效果。 它最適合在多個熒幕和裝置上播放Adobe Dynamic Media Classic視訊的客戶。

在播放期間，視訊播放程式用來判斷要播放或選取之編碼視訊的邏輯乃是基於下列演算法:

1. 視訊播放器會根據位元速率載入初始視訊片段，而該位元速率最接近為播放器本身中的「初始位元速率」所設定的值。
1. 視訊播放器會根據使用下列條件的頻寬速度變更進行切換：

   1. 播放器會挑選低於或等於預估頻寬的最高頻寬資料流。
   1. 播放器只考慮80%的可用頻寬。 不過，如果調高了，則比較保守的是只有70%，以避免高估並立即調回。

若要檢視演演算法的邏輯，請前往 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 以取得相關的技術資訊。

為管理單一視訊和自我調整視訊集，Adobe Dynamic Media Classic支援下列專案：

* 正在以許多支援的視訊格式上傳視訊。 此外，也會將音訊格式和視訊編碼為MP4 H.264格式，以便跨多個熒幕播放。 您可以使用預先定義的Adobe Dynamic Media Classic最適化視訊預設集、單一視訊編碼預設集，或自訂自己的編碼來控制視訊的品質和大小。

另請參閱 [啟用或停用自我調整視訊預設集](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

另請參閱 [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片。

產生最適化視訊集時，其中會包含MP4視訊。

>[!NOTE]
>
>主要/來源視訊和任何其他來源格式視訊是 *非* 新增至最適化視訊集。

* Univeral_Media5_Video、Universal_Media5_MixedMedia_dark和Universal_Media5_Viewers和Universal_Media_light檢視器中的視訊字幕，以及Universal_HTMLHTML HTML HTML 5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light檢視器中的視訊章節導覽。

  另請參閱 [新增註解至視訊](adding-captions-video.md).

  另請參閱 [將章節標籤新增至視訊](adding-chapter-markers-video.md).

* 以完整中繼資料支援來組織、瀏覽和搜尋視訊，以有效管理視訊資產。
* 將最適化視訊集傳送至網頁以及桌上型電腦和行動裝置，包括iPhone、iPad、Android™、BlackBerry®和Windows® phone。

  各種iOS平台均支援最適化視訊串流。

  請參閱以下連結的最新支援： [Adobe檢視器參考指南](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。 <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  您可以在下列位置找到支援此視訊格式的Windows®裝置：

  [Windows® Phone支援的視訊格式](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* 使用Adobe Dynamic Media Classic檢視器預設集播放視訊，包括下列專案：

   * 單一視訊檢視器。
   * 合併視訊和影像內容的混合媒體檢視器。

* 設定視訊播放器來滿足您的品牌推廣需要。
* 使用簡單的URL或內嵌程式碼將視訊整合至您的網站、行動網站或行動應用程式。

請參閱下列訓練影片：
* [MP4視訊概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4視訊預覽](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4視訊上傳](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [串流概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**快速入門**

下列逐步工作流程說明可協助您快速上手並執行Adobe Dynamic Media Classic中的Adaptive Video Sets。 每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.上傳並編碼視訊

使用下列其中一個案例，上載並產生最適化視訊集: 

* **上傳預先編碼的視訊**：如果您的視訊已從Adobe Dynamic Media Classic外部編碼，請在全域導覽列上，選取 **[!UICONTROL 上傳]**. 直接瀏覽並上傳MP4視訊檔案至Adobe Dynamic Media Classic。 接著，前往 **[!UICONTROL 建置]** > **[!UICONTROL 最適化視訊集]**. 瀏覽至視訊檔案。將您想要的視訊檔案拖放至「自我調整視訊集」表格中，然後儲存該集合。
* **上傳主要來源影片**：如果您的視訊未編碼，請在全域導覽列上，選取 **[!UICONTROL 上傳]** 上傳主要視訊來源檔案（非MP4）。 Adobe Dynamic Media Classic會為您將其編碼為MP4檔案。 在 **[!UICONTROL 上載工作選項]** 對話方塊，在 **[!UICONTROL EVideo選項]**，選取 **[!UICONTROL 自我調整視訊]**.

  使用此偏好選項，您可以建立最適化視訊集。 正確的編碼預設集會自動套用至視訊（無論是16:9或4:3），以符合您上傳的視訊尺寸。 當您提交上載工作時，系統會自動為您建立最適化視訊集，其中包含三個以正確外觀比例編碼的視訊設定。

  或者，在同一個 **[!UICONTROL 工作選項]** 對話方塊，在 **[!UICONTROL EVideo選項]**，展開 **[!UICONTROL 單一編碼預設集]**. 選取您想要的個別視訊編碼預設集。 您可以選取 **案頭**， **行動(iPhone、iPad、Android™)**、和 **平板電腦(iPad、Android™)** 建立MP4檔案。

* 或者，您可以使用重新處理主要視訊 **[!UICONTROL 重新處理]** 功能。 新編碼的視訊會增加到現有的最適化視訊集。

另請參閱 [上傳並編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos).

**選擇性**

Adobe Dynamic Media Classic提供許多預先定義的視訊編碼預設集。 這些預先定義的預設集反映了目前最常用的視訊編碼設定，且已針對目標頁面上的播放進行最佳化。

不過，如需進一步的自訂，管理員可以建立「視訊預設集」來自訂視訊的大小和終端使用者的播放體驗。管理員可以從「 」下方的「視訊預設集」頁面新增及管理視訊預設集 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 單一編碼預設集]**. 「視訊預設集」頁面可提供增加、編輯、刪除及啟用視訊預設集所需的選項。

另請參閱 [使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2.在視訊檢視器中預覽視訊

若要檢視視訊在案頭、網站或行動裝置上播放給使用者的情形，請在「瀏覽」面板中選取視訊。 然後選取 **[!UICONTROL 預覽]**.

另請參閱 [在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

您可以在「預覽」頁面上播放視訊。 您也可以選擇不同的視訊檢視器，瞭解您的視訊在不同播放器中的顯示方式。 最佳做法是使用 HTML5 視訊播放器，以便在桌上型電腦、平板電腦和行動裝置的多種螢幕上播放。

**選擇性**

檢視器預設集自訂： Adobe Dynamic Media Classic提供預先定義的檢視器預設集，以供傳送視訊。 這些預設集決定了檢視器的外觀及其播放控制項的工作方式。若要自訂視訊檢視器，管理員可以在「檢視器預設集」頁面中增加及管理檢視器預設集。若要開啟此頁面，請前往Adobe Dynamic Media Classic右上角的 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**. 「檢視器預設集」頁面可提供增加、編輯、刪除及啟用檢視器預設集所需的命令。

另請參閱 [使用視訊檢視器預設集](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

另請參閱 [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片。

## 3.將視訊部署至您的網站和行動網站

若要將視訊整合至網站，您可執行下列其中一項作業: 

* 在其本身的快顯視窗或強制回應視窗中顯示視訊，在此情況下，請使用 **[!UICONTROL 複製URL]** 功能。

  若要取得視訊的 URL，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中加以選取。選取 **[!UICONTROL 預覽]**，然後選取 **[!UICONTROL 複製URL]** 右側 `Universal_HTML5_Viewer`.

  當您選取 **[!UICONTROL 複製URL]**，則URL會複製到剪貼簿。 將此程式碼放置在網站、行動裝置網站或應用程式的 HTML 中。

  >[!NOTE]
  >
  >URL 只會在您發佈視訊或最適化視訊集之後啟用。

* 顯示內嵌在網頁上的影片，在此情況下，請使用 **[!UICONTROL 內嵌程式碼]** 功能。

  若要取得視訊的內嵌程式碼，請在「格線檢視」或「清單檢視」中，選取「瀏覽」面板中的視訊。 前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**. 在表格的「動作」欄下，選取 **[!UICONTROL 內嵌程式碼]** 右側 `Universal_HTML5_Video`. 不允許編輯程式碼。

  選取 **[!UICONTROL 關閉]** 並將內嵌程式碼貼到一個或多個網頁中。

  >[!NOTE]
  >
  >內嵌程式碼僅會在您發佈視訊或自我調整視訊集後啟動。

另請參閱 [將視訊部署至您的網站和行動網站](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [視訊編碼最佳實踐](uploading-encoding-videos.md#best_practices_for_video_encoding)
