---
title: '"最佳做法: 使用 HTML5 視訊檢視器"'
seo-title: '"最佳做法: 使用 HTML5 視訊檢視器"'
description: 'null'
seo-description: 瞭解使用HTML5視訊檢視器的最佳範例。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 30%

---


# 最佳做法: 使用 HTML5 視訊檢視器{#best-practice-using-the-html-video-viewer}

Dynamic Media Classic HTML5 Video檢視器預設集是強穩的視訊播放器。 在播放器的設計端，您可以使用標準網頁開發工具來建立視訊播放器的所有功能。 例如，您可以使用 HTML5 和 CSS 來設計按鈕、控制項與自訂海報影像背景，並藉助自訂的外觀來吸引客戶。

在檢視器的播放方面，它會自動偵測瀏覽器的視訊功能，然後，它使用HLS（自適應視訊串流）來提供視訊。 或者，如果該傳送方法不存在，則會改用HTML5漸進式。

此單一播放程式集諸多功能於一身，能夠使用 HTML5 與 CSS 來設計播放組件，能夠實現內嵌播放，還能夠根據瀏覽器的功能來使用最適化串流與漸進式串流，可協助您將多媒體內容同時提供給桌上型電腦使用者和行動裝置使用者，並確保順暢的視訊體驗。

另請參 [閱Adobe檢視器參考指南](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) 中的關於HTML5檢視器。

## 使用Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

針對桌上型電腦和行動裝置的可調式視訊串流，用於位元速率切換的視訊是以最適化視訊集中的所有MP4視訊為基礎。

使用HLS或漸進式視訊進行視訊播放。 HLS（HTTP即時串流）是Apple自適應視訊串流的標準，可根據網路頻寬容量自動調整播放。 它也可讓客戶「尋找」視訊中的任何點，而不需等待視訊的其餘部分下載。 另請參 [閱HTTP即時串流](https://developer.apple.com/streaming/)。 漸進式視訊是透過下載視訊並將它儲存在使用者的案頭螢幕或行動裝置上，來傳送。

下表說明使用Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊的裝置、瀏覽器和播放方法。

| 裝置 | 瀏覽器 | 視訊播放模式 |
|--- |--- |--- |
| 德斯科普 | Internet Explorer 9和10 | 漸進式下載。 |
| 桌上型電腦 | Internet Explorer 11+ | HLS視訊串流。 |
| 桌上型電腦 | Firefox 23-44 | 漸進式下載。 |
| 桌上型電腦 | Firefox 45 或更高版本 | HLS視訊串流。 |
| 桌上型電腦 | Chrome | HLS視訊串流。 |
| 桌上型電腦 | Safari(Mac) | HLS視訊串流。 |
| 行動 | Chrome（Android 6或更舊版本） | 漸進式下載。 |
| 行動 | Chrome（Android 7或更新版本） | HLS視訊串流。 |
| 行動 | Android（預設瀏覽器） | 漸進式下載。 |
| 行動 | Safari(iOS) | HLS視訊串流。 |
| 行動 | Chrome(iOS) | HLS視訊串流。 |
| 行動 | Blackberry | HLS視訊串流。 |
