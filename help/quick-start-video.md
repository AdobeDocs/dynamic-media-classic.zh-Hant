---
title: 「快速啟動：Adobe Dynamic Media Classic視頻」
description: Adobe Dynamic Media Classic視頻簡介和快速入門，幫助您快速啟動並運行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1808'
ht-degree: 25%

---

# 快速啟動：Adobe Dynamic Media Classic視頻{#quick-start-video}

Adobe Dynamic Media Classic視頻是端到端解決方案，它使發佈高質量自適應視頻在多個螢幕(包括案頭、iOS、Android™、BlackBerry®和Windows®移動設備)上流傳輸變得輕鬆。 最適化視訊集會將以不同位元速率和格式 (如 400 kbps、800 kbps 和 1000 kbps) 編碼之相同視訊的版本分組。桌上型電腦或行動裝置會偵測可用的頻寬。

例如，iOS 行動裝置會偵測 3G、4G 或 Wi-Fi 的頻寬。然後，它會自動從最適化視訊集的各種視訊位元速率中選取正確編碼的視訊。視訊會串流至桌上型電腦、行動裝置或平板電腦。

此外，如果桌上型電腦或行動裝置上的網路條件有所變更，則視訊品質會自動動態切換。此外，如果客戶在案頭上進入全屏模式，自適應視頻集會通過使用更好的解析度來響應，從而改善客戶的觀看體驗。 使用自適應視頻集為客戶在多個螢幕和設備上播放Adobe Dynamic Media Classic視頻提供了最佳的可回放。

在播放期間，視訊播放程式用來判斷要播放或選取之編碼視訊的邏輯乃是基於下列演算法:

1. 視頻播放器基於與在播放器本身中為「初始比特率」設定的值最接近的比特率來載入初始視頻片段。
1. 視頻播放器根據頻寬速度的更改使用以下標準進行切換：

   1. 播放器選擇低於或等於估計頻寬的最高頻寬流。
   1. 玩家只考慮80%的可用頻寬。 但是，如果換了，就比較保守，只有70%，免得高估，不得不立即換。

查看算法的邏輯 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 獲取有關它的技術資訊。

為了管理單個視頻和自適應視頻集，Adobe Dynamic Media Classic支援以下內容：

* 從眾多受支援的視頻格式和音頻格式上傳視頻，並將視頻編碼為MP4 H.264格式，以便在多個螢幕上播放。 可以使用預定義的Adobe Dynamic Media Classic自適應視頻預設、單個視頻編碼預設或自定義自己的編碼來控制視頻的質量和大小。

請參閱 [激活或停用自適應視頻預設](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

另請參閱 [視頻預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 培訓視頻。

當生成自適應視頻集時，它包括MP4視頻。

>[!NOTE]
>
>主/源視頻和任何其他源格式視頻 *不* 添加到自適應視頻集。

* Univeral_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_deark中的視頻字幕和視頻章節導航燈光觀眾。

   請參閱 [將字幕添加到視頻](adding-captions-video.md)。

   請參閱 [將章節標籤添加到視頻](adding-chapter-markers-video.md)。

* 以完整中繼資料支援來組織、瀏覽和搜尋視訊，以有效管理視訊資產。
* 將自適應視頻集傳送到Web和台式機以及移動設備，包括iPhone、iPad、Android™、BlackBerry®和Windows®電話。

   各種iOS平台支援自適應視頻流。

   請參閱 [Adobe查看器參考指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)。

   Adobe Dynamic Media Classic支援MP4 H.264視頻的移動視頻播放。 您可以在以下網站找到支援此視頻格式的BlackBerry®設備：

   請參閱 [BlackBerry®上支援的視頻格式](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)。

   您可以在以下位置找到支援此視頻格式的Windows®設備：

   請參閱 [Windows® Phone上支援的視頻格式](https://docs.microsoft.com/en-us/)。

* 使用Adobe Dynamic Media Classic查看器預設回放視頻，包括：

   * 單一視訊檢視器。
   * 合併視訊和影像內容的混合媒體檢視器。

* 設定視訊播放器來滿足您的品牌推廣需要。
* 透過一個簡單的 URL 或內嵌程式碼將視訊整合到您的網站、行動網站或行動應用程式。

請參閱以下培訓視頻：
* [MP4視頻概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4視頻預覽](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4視頻上載](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [流式處理概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**快速啟動**

下面的逐步工作流描述旨在幫助您快速啟動並運行Adobe Dynamic Media Classic的自適應視頻集。 在每個步驟之後，都會出現一個主題標題的交叉引用，您可以在其中找到更多資訊。

## 1。上傳和編碼視頻

使用下列其中一個案例，上載並產生最適化視訊集: 

* **上傳預編碼視頻**  — 如果您的視頻已在Adobe Dynamic Media Classic外編碼，請在全局導航欄上選擇 **[!UICONTROL 上載]** 瀏覽MP4視頻檔案並直接上傳到Adobe Dynamic Media Classic。 然後，轉到 **[!UICONTROL 生成]** > **[!UICONTROL 自適應視頻集]**。 瀏覽至視訊檔案。將想要的視頻檔案拖放到「自適應視頻集」表中，然後保存該集。
* **上載主源視頻**  — 如果您的視頻未編碼，請在全局導航欄上選擇 **[!UICONTROL 上載]** 上載主視頻源檔案（非MP4）。 Adobe Dynamic Media Classic為您編碼為MP4檔案。 在 **[!UICONTROL 上載作業選項]** 對話框，位於 **[!UICONTROL EVideo選項]**&#x200B;選中 **[!UICONTROL 自適應視頻]**。

   此優先選項可讓您建立會自動套用正確編碼預設集至視訊的最適化視訊集 (無論是 16:9 還是 4:3)，以符合您所上載之視訊的尺寸。在您提交上載作業時，系統會自動為您建立自適應視頻集，其中包括三個以正確長寬比編碼的視頻設定。

   或者，在同一 **[!UICONTROL 作業選項]** 對話框，位於 **[!UICONTROL EVideo選項]**&#x200B;展開 **[!UICONTROL 單個編碼預設]**。選擇要從中進行的單個視頻編碼預設 **案頭**。 **移動(iPhone、iPad、Android™)**, **平板電腦(iPad、Android™)** 以便建立MP4檔案。

* 或者，您可以使用 **[!UICONTROL 重新處理]** 的子菜單。 新編碼的視訊會增加到現有的最適化視訊集。

請參閱 [上傳和編碼視頻](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**選擇性**

Adobe Dynamic Media Classic提供了許多預定義的視頻編碼預設。 這些預定義預設反映了目前使用的最常見的視頻編碼設定，並已優化為在目標頁面上回放。

不過，如需進一步的自訂，管理員可以建立「視訊預設集」來自訂視訊的大小和終端使用者的播放體驗。管理員可以從下面的「視頻預設」頁面添加和管理「視頻預設」 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視頻預設]** > **[!UICONTROL 單個編碼預設]**。 「視訊預設集」頁面可提供增加、編輯、刪除及啟用視訊預設集所需的選項。

請參閱 [使用視頻編碼預設](uploading-encoding-videos.md#working_with_video_encoding_presets)。

## 2.在視頻查看器中預覽視頻

要查看視頻在案頭、網站或移動設備上如何為最終用戶播放，請在「瀏覽面板」中選擇視頻，然後選擇 **[!UICONTROL 預覽]**。

請參閱 [在視頻查看器中預覽視頻](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

可以在「預覽」頁面上播放視頻。 您也可以選擇不同的視頻查看器來瞭解視頻在不同播放器中的顯示方式。 最佳做法是使用 HTML5 視訊播放器，以便在桌上型電腦、平板電腦和行動裝置的多種螢幕上播放。

**選擇性**

查看器預設自定義 — Adobe Dynamic Media Classic提供預定義的查看器預設以提供視頻。 這些預設集決定了檢視器的外觀及其播放控制項的工作方式。若要自訂視訊檢視器，管理員可以在「檢視器預設集」頁面中增加及管理檢視器預設集。要開啟此頁面，請在Adobe Dynamic Media Classic右上角，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。 「檢視器預設集」頁面可提供增加、編輯、刪除及啟用檢視器預設集所需的命令。

請參閱 [使用視頻查看器預設](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

另請參閱 [視頻預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 培訓視頻。

## 3.將視頻部署到您的網站和移動站點

若要將視訊整合至網站，您可執行下列其中一項作業: 

* 在其自己的彈出窗口或模式窗口中顯示視頻，在這種情況下，使用 **[!UICONTROL 複製URL]** 的子菜單。

   若要取得視訊的 URL，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中加以選取。選擇 **[!UICONTROL 預覽]**，然後選擇 **[!UICONTROL 複製URL]** 權利 `Universal_HTML5_Viewer`。

   選擇時 **[!UICONTROL 複製URL]**, URL將複製到剪貼簿。 將此程式碼放置在網站、行動裝置網站或應用程式的 HTML 中。

   >[!NOTE]
   >
   >URL 只會在您發佈視訊或最適化視訊集之後啟用。

* 顯示網頁上嵌入的視頻，在這種情況下使用 **[!UICONTROL 嵌入代碼]** 的子菜單。

   若要取得視訊的內嵌程式碼，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中選取該視訊。轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。 在表的「操作」(Actions)列下，選擇 **[!UICONTROL 嵌入代碼]** 權利 `Universal_HTML5_Video`。 不允許編輯程式碼。

   選擇 **[!UICONTROL 關閉]** 將嵌入代碼貼上到網頁中。

   >[!NOTE]
   >
   >內嵌程式碼只會在您發佈視訊或最適化視訊集之後啟用。

請參閱 [將視頻部署到您的網站和移動站點](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [視訊編碼最佳實踐](uploading-encoding-videos.md#best_practices_for_video_encoding)

