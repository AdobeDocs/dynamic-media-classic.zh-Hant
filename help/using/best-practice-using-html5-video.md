---
title: 使用HTML5視訊檢視器的最佳實務
description: 瞭解使用HTML5視訊檢視器的最佳做法。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5fdabd28c4d0defdf9f145b581c89640cc1f6118
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 2%

---

# 使用HTML5視訊檢視器的最佳做法{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5視訊檢視器預設集是高效能視訊播放器。 對於播放器設計，您可以使用標準Web開發工具來建立視訊播放器的整個功能。 若要自訂外觀，您可以使用HTML5和CSS設計按鈕、控制項以及自訂海報影像。

對於檢視器播放，會自動偵測瀏覽器的視訊功能。 接著，影片會使用HLS （HTTP即時資料流） （也稱為最適化視訊資料流）提供視訊。 或者，如果該傳送方法不存在，則改用HTML5 progressive。

將下列功能合併為單一播放器：

* 使用HTML5和CSS設計的播放元件。
* 內嵌式播放。
* 根據瀏覽器的功能使用最適化和漸進式串流。

您可以提高桌上型電腦和行動使用者對豐富媒體內容的可用性。 您也可以確保簡化的視訊體驗。

另請參閱HTML檢視器參考指南中的[關於Adobe5檢視器](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)。

另請觀看[檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)訓練影片。

## 使用Adobe Dynamic Media Classic視訊檢視器在桌上型電腦和行動裝置上播放視訊 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

就桌上型電腦和行動最適化視訊串流而言，用於位元速率切換的視訊均以最適化視訊集中的所有MP4視訊為基礎。

使用HLS或漸進式視訊進行視訊播放。 HLS （HTTP即時串流）是適用於最適化視訊串流的Apple標準，可依據網路頻寬容量自動調整播放。 它也可讓使用者導覽至視訊中的任何位置，而不需要等候下載視訊的其餘部分。 另請參閱[HTTP即時資料流](https://developer.apple.com/streaming/)。 系統會將漸進式視訊下載並儲存在使用者的案頭熒幕或行動裝置上，藉此提供漸進式視訊。

下表說明使用Adobe Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊的裝置、瀏覽器和方法。

| 裝置 | 瀏覽器 | 視訊播放模式 |
|--- |--- |--- |
| 桌上型電腦 | Internet Explorer 9和10 | 漸進式下載。 |
| 桌上型電腦 | Internet Explorer 11+ | HLS視訊串流。 |
| 桌上型電腦 | Firefox 23-44 | 漸進式下載。 |
| 桌上型電腦 | Firefox 45或更新版本 | HLS視訊串流。 |
| 桌上型電腦 | Chrome | HLS視訊串流。 |
| 桌上型電腦 | Safari (Mac) | HLS視訊串流。 |
| 行動 | Chrome （Android™ 6或更舊版本） | 漸進式下載。 |
| 行動 | Chrome （Android™ 7或更新版本） | HLS視訊串流。 |
| 行動 | ™ （預設瀏覽器） | 漸進式下載。 |
| 行動 | Safari (iOS) | HLS視訊串流。 |
| 行動 | Chrome (iOS) | HLS視訊串流。 |
| 行動 | BlackBerry® | HLS視訊串流。 |
