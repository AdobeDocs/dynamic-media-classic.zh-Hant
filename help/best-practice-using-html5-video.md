---
title: 使用HTML5視訊檢視器的最佳作法
description: 了解使用HTML5視訊檢視器的最佳實務。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 12%

---

# 使用HTML5視訊檢視器的最佳作法{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5視訊檢視器預設集是強大的視訊播放器。 在播放器的設計端，您可以使用標準網頁開發工具來建立視訊播放器的完整功能。 例如，您可以使用 HTML5 和 CSS 來設計按鈕、控制項與自訂海報影像背景，並藉助自訂的外觀來吸引客戶。

在檢視器的播放方面，它會自動偵測瀏覽器的視訊功能，接著，它會使用HLS（HTTP即時串流）（也稱為最適化視訊串流）提供視訊。 或者，如果該傳送方法不存在，則改用HTML5漸進式。

合併為單一播放器時，可提供下列功能：

* 使用HTML5和CSS設計的播放元件
* 內嵌播放
* 根據瀏覽器功能使用最適化和漸進式串流

您可以將多媒體內容的觸及範圍擴展至案頭和行動使用者。 您也可以確保簡化的影片體驗。

另請參閱 [關於HTML5檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) (位於「Adobe檢視器參考指南」中)。

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

## 使用Adobe Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

針對案頭和行動最適化視訊串流，用於位元速率切換的視訊是以最適化視訊集中的所有MP4視訊為基礎。

使用HLS或漸進式視訊時會發生視訊播放。 HLS（HTTP即時串流）是適用性視訊串流的Apple標準，可根據網路頻寬容量自動調整播放。 它也可讓客戶「搜尋」視訊中的任何點，而不需等待視訊的其餘部分下載。 另請參閱 [HTTP Live Streaming](https://developer.apple.com/streaming/). 通過將視頻下載並本地儲存到用戶的案頭螢幕或移動設備來提供漸進式視頻。

下表說明使用Adobe Dynamic Media Classic視訊檢視器在桌上型電腦和行動裝置上播放視訊的裝置、瀏覽器和播放方法。

| 裝置 | 瀏覽器 | 視訊播放模式 |
|--- |--- |--- |
| 桌上型電腦 | Internet Explorer 9和10 | 漸進式下載。 |
| 桌上型電腦 | Internet Explorer 11+ | HLS視訊串流。 |
| 桌上型電腦 | Firefox 23-44 | 漸進式下載。 |
| 桌上型電腦 | Firefox 45 或更高版本 | HLS視訊串流。 |
| 桌上型電腦 | 鉻黃 | HLS視訊串流。 |
| 桌上型電腦 | Safari(Mac) | HLS視訊串流。 |
| 行動 | Chrome(Android™ 6或更舊版本) | 漸進式下載。 |
| 行動 | Chrome(Android™ 7或更新版本) | HLS視訊串流。 |
| 行動 | Android™（預設瀏覽器） | 漸進式下載。 |
| 行動 | Safari(iOS) | HLS視訊串流。 |
| 行動 | Chrome(iOS) | HLS視訊串流。 |
| 行動 | BlackBerry® | HLS視訊串流。 |
