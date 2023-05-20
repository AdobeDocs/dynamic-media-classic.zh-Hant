---
title: 使用HTML5視頻查看器的最佳實踐
description: 瞭解使用HTML5視頻查看器的最佳做法。
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

# 使用HTML5視頻查看器的最佳做法{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media ClassicHTML5視頻查看器預設是強大的視頻播放器。 在播放器的設計端，您可以使用標準Web開發工具建立視頻播放器的全部功能。 例如，您可以使用 HTML5 和 CSS 來設計按鈕、控制項與自訂海報影像背景，並藉助自訂的外觀來吸引客戶。

在檢視器的播放方面，它會自動偵測瀏覽器的視訊功能，然後，它使用HLS(HTTP Live Streaming)（也稱為自適應視頻流）來提供視頻服務。 或者，如果不存在該傳遞方法，則改用HTML5累進。

通過組合成一個玩家，可以獲得以下能力：

* 使用HTML5和CSS設計的回放元件
* 嵌入式播放
* 基於瀏覽器功能的自適應和逐級流的使用

您可以將您的富媒體內容擴展到案頭和移動用戶。 您還可以確保簡化的視頻體驗。

另請參閱 [關於HTML5查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) 的下界。

另請參閱 [查看器預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 培訓視頻。

## 使用Adobe Dynamic Media Classic視頻查看器在台式電腦和移動設備上播放視頻 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

對於案頭和移動自適應視頻流，用於比特率切換的視頻基於自適應視頻集中的所有MP4視頻。

使用HLS或漸進視頻進行視頻回放。 HLS(HTTP Live Streaming)是Apple自適應視頻流的標準，可根據網路頻寬容量自動調整回放。 它還讓客戶可以「查找」視頻中的任何點，而無需等待視頻的其餘部分下載。 另請參閱 [HTTP即時流](https://developer.apple.com/streaming/)。 通過將視頻下載並本地儲存到用戶的案頭螢幕或移動設備來傳送漸進視頻。

下表介紹了使用Adobe Dynamic Media Classic視頻查看器在台式電腦和移動設備上播放視頻的設備、瀏覽器和播放方法。

| 裝置 | 瀏覽器 | 視頻播放模式 |
|--- |--- |--- |
| 桌上型電腦 | Internet Explorer 9和10 | 逐步下載。 |
| 桌上型電腦 | Internet Explorer 11+ | HLS視頻流。 |
| 桌上型電腦 | 火狐23-44 | 逐步下載。 |
| 桌上型電腦 | Firefox 45 或更高版本 | HLS視頻流。 |
| 桌上型電腦 | 鉻 | HLS視頻流。 |
| 桌上型電腦 | 薩法里(Mac) | HLS視頻流。 |
| 行動 | Chrome（Android™ 6或更早版本） | 逐步下載。 |
| 行動 | Chrome（Android™ 7或更高版本） | HLS視頻流。 |
| 行動 | Android™（預設瀏覽器） | 逐步下載。 |
| 行動 | 薩法里(iOS) | HLS視頻流。 |
| 行動 | 克羅姆語(iOS) | HLS視頻流。 |
| 行動 | BlackBerry® | HLS視頻流。 |
