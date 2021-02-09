---
title: 啟用 Adobe Analytics 視訊報告
description: 瞭解如何啟用Adobe Analytics視訊報表。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 20%

---


# 啟用 Adobe Analytics 視訊報告{#enabling-adobe-analytics-video-reports}

使用Adobe Analytics以心率為基礎的視訊報告，在Dynamic Media Classic中設定Adobe Analytics時，您不再需要啟用4個視訊檢視器事件（播放、暫停、停止、里程碑）。 「視訊心率」可與現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器搭配使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 如需串流媒體和「心率測量」的簡介，請參閱[關於Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* Adobe Analytics視訊報表與Dynamic Media Classic的整合支援解決方案變數，但不支援自訂變數。

   如需解決方案變數和自訂變數的詳細資訊，請參閱[音訊和視訊參數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)。

* 支援現成的一分鐘增量區段。不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   如需串流媒體需求與設定的詳細資訊，請參閱[在Adobe Analytics中測量串流媒體](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 如需自訂和解決方案變數的詳細資訊，請參閱[啟用媒體報表](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，則您需要繼續使用本章所述的步驟，將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數。

