---
title: '"快速入門: 視訊"'
seo-title: '"快速入門: 視訊"'
description: 'null'
seo-description: 簡介和快速入門影片，協助您快速上手使用。
uuid: bf0ecf87-a1 f2-4e83-8041-df5192 dd26 a1
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/video
discoiquuid: 6cf541b-e9 df-48eb-9a16-ca3 e1 f07238 e
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# 快速入門: 視訊{#quick-start-video}

Adobe Dynamic Media Classic Video是端對端解決方案，可讓您輕鬆發佈高品質的最適化視訊，以便跨多種螢幕串流，包括桌上型電腦、iOS、Android、Blackberry和Windows行動裝置。最適化視訊集會將以不同位元速率和格式 (如 400 kbps、800 kbps 和 1000 kbps) 編碼之相同視訊的版本分組。桌上型電腦或行動裝置會偵測可用的頻寬。

例如，iOS 行動裝置會偵測 3G、4G 或 Wi-Fi 的頻寬。然後，它會自動從最適化視訊集的各種視訊位元速率中選取正確編碼的視訊。視訊會串流至桌上型電腦、行動裝置或平板電腦。

此外，如果桌上型電腦或行動裝置上的網路條件有所變更，則視訊品質會自動動態切換。還有，如果客戶進入桌上型電腦的全螢幕模式，則最適化視訊集會以更好的解析度來回應，因而提升客戶的觀賞體驗。使用最適化視訊集可為您提供最佳的播放方式，適用於在多種螢幕和裝置上播放動態媒體Classic視訊的客戶。

在播放期間，視訊播放程式用來判斷要播放或選取之編碼視訊的邏輯乃是基於下列演算法:

1. 視訊播放器會根據位元速率(與播放器本身的「初始位元速率」設定的值)載入初始視訊片段。
1. 視訊播放器切換根據頻寬速度改變，使用下列標準：

   1. 播放器會找出低於或等於估計頻寬的頻寬串流。
   1. 播放器只會考量80%可用頻寬。但是，如果它正在切換，則只會以70%的對話轉換，以避免估計過高並立即切換回圈。

如需相關技術資訊，請參閱 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 的演算法邏輯。

若要管理單一視訊和最適化視訊集，Dynamic Media Classic支援下列各項：

* 從多種支援的視訊格式和音訊格式上載視訊，並將視訊編碼為 MP4 H.264 格式，以便在多種螢幕上播放。您可以使用預先定義的Dynamic Media Classic可調式視訊預設集、單一視訊編碼預設集，或自訂您自己的編碼，以控制視訊的品質和大小。

   當產生最適化視訊集時，它會包含MP影片。

   `**Note:**` 主版/來源視訊和任何其他來源格式視訊 *都不* 會新增至最適化視訊集。

* 在Universal_ HTML5_ Video、Universal_ HTML5_ MixedMedia_ light檢視器和Universal_ HTML5_ VideedMedia_ light檢視器和視訊章節導覽中的視訊註解(Universal_ HTML5_ VideedMedia_ light和Universal_ HTML5_ MixedMedia_ light檢視器)中的視訊註解。

   請參閱[增加註解至視訊](adding-captions-video.md)。

   請參閱[增加章節標記至視訊](adding-chapter-markers-video.md)。

* 以完整中繼資料支援來組織、瀏覽和搜尋視訊，以有效管理視訊資產。
* 將最適化視訊集傳送到網路、桌上型電腦以及行動裝置，包括 iPhone、iPad、Android™、Blackberry 和 Windows Phone。

   在各種 iOS 平台上支援最適化視訊串流。

   請參閱 [Adobe檢視器參考指南](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)中的最新支援。

   Dynamic Media Classic支援MP H.264視訊的行動視訊播放。您可以在下列網站中找到支援此視訊格式的 Blackberry 裝置: 

   請參閱 [Blackberry上支援的視訊格式](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)。

   您可以在下列連結找到支援此視訊格式的 Windows 裝置:

   請參閱 [「Windows Phone支援的視訊格式](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx)」。

* 使用Dynamic Media Classic Viewer預設集來播放視訊，包括：

   * 單一視訊檢視器。
   * 合併視訊和影像內容的混合媒體檢視器。

* 設定視訊播放器來滿足您的品牌推廣需要。
* 透過一個簡單的 URL 或內嵌程式碼將視訊整合到您的網站、行動網站或行動應用程式。

**快速入門**

以下逐步工作流程說明旨在協助您使用Dynamic Media Classic中的可調式視訊集快速啓動和執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

**1. 上載與編碼視訊**

使用下列其中一個案例，上載並產生最適化視訊集: 

* **上傳預先編碼的影片** -如果您的影片已在Dynamic Media Classic外部編碼，請按一下 **全域導覽列上的「上傳」** ，以瀏覽並上傳MP視訊檔案至Scene Publishing System。然後，按一下「**建置** &gt; **最適化視訊集**」。瀏覽至視訊檔案。拖放您要的視訊檔案至「最適化視訊集」表格，然後儲存視訊集。
* **上傳主碼來源影片** -如果您的影片未編碼，請按一下 **全域導覽列上的「上傳」** ，上傳主視訊來源檔案(非MP4)，並讓Scene Publishing System將它們編碼為MP檔案。在「上載工作選項」對話框的「EVideo 選項」底下，選取「**最適化視訊**」。

   此優先選項可讓您建立會自動套用正確編碼預設集至視訊的最適化視訊集 (無論是 16:9 還是 4:3)，以符合您所上載之視訊的尺寸。當您送出上載工作時，系統會自動為您建立一個最適化視訊集，內含三個具有正確外觀比例的視訊編碼。

   或者，在相同「工作選項」對話框的「EVideo 選項」底下，展開「**單一編碼預設集**」，然後從「**桌上型電腦**」、「**行動裝置 (iPhone、iPad、Android)**」與「**平板電腦 (iPad、Android)**」中選取您要使用的個別視訊轉碼預設集，以便建立 MP4 檔案。

* 或者，您可以使用「重新處理」功能重新處理主視訊。新編碼的視訊會增加到現有的最適化視訊集。

請參閱[上載與編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**選擇性**

Dynamic Media Classic提供許多預先定義的視訊編碼預設集。這些預先定義的預設集反映了現今最常用的通用視訊編碼設定，並已針對目標螢幕的播放進行了最佳化。

不過，如需進一步的自訂，管理員可以建立「視訊預設集」來自訂視訊的大小和終端使用者的播放體驗。管理員可以在「視訊預設集」頁面中增加及管理視訊預設集，此頁面可從「設定 &gt; 應用程式設定 &gt; 視訊預設集 &gt; 單一編碼預設集」存取。「視訊預設集」頁面可提供增加、編輯、刪除及啟用視訊預設集所需的選項。

請參閱[使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets)。

**2. 在視訊檢視器中預覽視訊**

若要查看終端使用者在桌上型電腦、您的網站或是行動裝置上看到的視訊播放方式，請在瀏覽面板中選取該視訊，然後按一下「**預覽**」。

請參閱[在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

您可以在「預覽」畫面上播放視訊。還可以選擇不同的「視訊檢視器」，以瞭解在不同的播放器中視訊的播放效果。最佳做法是使用 HTML5 視訊播放器，以便在桌上型電腦、平板電腦和行動裝置的多種螢幕上播放。

**選擇性**

檢視器預設集自訂-動態媒體Classic提供預先定義的檢視器預設集以提供視訊。這些預設集決定了檢視器的外觀及其播放控制項的工作方式。若要自訂視訊檢視器，管理員可以在「檢視器預設集」頁面中增加及管理檢視器預設集。若要開啟此頁，在 Scene7 Publishing System 右上角中按一下「設定 &gt; 檢視器預設集」。「檢視器預設集」頁面可提供增加、編輯、刪除及啟用檢視器預設集所需的命令。

請參閱[使用視訊檢視器預設集](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

**3. 將視訊部署到網站和行動裝置網站**

若要將視訊整合至網站，您可執行下列其中一項作業: 

* 在本身的彈出式視窗或強制回應視窗中顯示視訊，這種情況下您應使用「複製 URL」功能。

   若要取得視訊的 URL，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中加以選取。Click Preview, and then click Copy URL to the right of `Universal_HTML5_Viewer`.

   按一下「複製 URL」時，該 URL 便會複製到剪貼簿。將此程式碼放置在網站、行動裝置網站或應用程式的 HTML 中。

   ***附註**：URL只會在您發佈視訊或最適化視訊集後啓動。*

* 顯示網頁內嵌的視訊，這種情況下您應使用「內嵌程式碼」功能。

   若要取得視訊的內嵌程式碼，請在「格點檢視」或「清單檢視」中，在「瀏覽」面板中選取該視訊。按一下「預覽 &gt; 檢視器清單」。在表格的「動作」欄下，按一下 `Universal_HTML5_Video` 右邊的「內嵌程式碼」。不允許編輯程式碼。

   按一下「關閉」，然後將內嵌程式碼貼在網頁中。

   ***附註**：內嵌代碼只會在您發佈視訊或最適化視訊集後啓動。*

請參閱[將視訊部署到網站和行動網站](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [視訊編碼最佳實踐](uploading-encoding-videos.md#best_practices_for_video_encoding)
