---
title: '"最佳做法: 使用 HTML5 視訊檢視器"'
seo-title: '"最佳做法: 使用 HTML5 視訊檢視器"'
description: 'null'
seo-description: 瞭解使用HTML視訊檢視器的最佳實務。
uuid: 3c8924dc-7ba-4c25-b77 b-005b57 b71 b64
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 最佳做法: 使用 HTML5 視訊檢視器{#best-practice-using-the-html-video-viewer}

Dynamic Media Classic HTML視訊檢視器預設集是強穩的視訊播放器。在播放器的設計端，您可以使用標準的網頁開發工具來建立所有視訊播放器的功能。例如，您可以使用 HTML5 和 CSS 來設計按鈕、控制項與自訂海報影像背景，並藉助自訂的外觀來吸引客戶。

在檢視器的播放方面，它會自動偵測瀏覽器的視訊功能，然後使用HLS(可調式視訊串流)來服務視訊。或者，如果傳遞方法不存在，則會改用HTML漸進式功能。

此單一播放程式集諸多功能於一身，能夠使用 HTML5 與 CSS 來設計播放組件，能夠實現內嵌播放，還能夠根據瀏覽器的功能來使用最適化串流與漸進式串流，可協助您將多媒體內容同時提供給桌上型電腦使用者和行動裝置使用者，並確保順暢的視訊體驗。

請參閱Adobe檢視器參考指南中的 [關於HTML檢視器](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) 。

## 使用動態媒體Classic Video Viewer在桌上型電腦和行動裝置上播放視訊 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

對於桌面和行動可調式視訊串流，位元速率切換所使用的視訊是根據最適化視訊集中的所有MP視訊。

使用HLS或漸進式視訊來播放視訊。HLS(HTTP即時串流)是Apple標準，可自動調整視訊串流，以根據網路頻寬容量自動調整播放。它還可讓客戶「搜尋」視訊中的任何點，而不需等待其餘視訊下載(另請參閱 [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/))。漸進式視訊可透過下載並將視訊儲存在使用者的桌面螢幕或行動裝置上來傳送。

下表說明使用Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊的裝置、瀏覽器和播放方法。

| 裝置 | 瀏覽器 | 視訊播放模式 |
|--- |--- |--- |
| Deskop | Internet Explorer和10 | 漸進式下載。 |
| 桌上型電腦 | Internet Explorer11+ | HLS視訊串流。 |
| 桌上型電腦 | Firefox23-44 | 漸進式下載。 |
| 桌上型電腦 | Firefox 45 或更高版本 | HLS視訊串流。 |
| 桌上型電腦 | Chrome | HLS視訊串流。 |
| 桌上型電腦 | Safari(Mac) | HLS視訊串流。 |
| 行動 | Chrome(Android或更舊版本) | 漸進式下載。 |
| 行動 | Chrome(Android或更新版本) | HLS視訊串流。 |
| 行動 | Android(預設瀏覽器) | 漸進式下載。 |
| 行動 | Safari(iOS) | HLS視訊串流。 |
| 行動 | Chrome(iOS) | HLS視訊串流。 |
| 行動 | Blackberry | HLS視訊串流。 |
