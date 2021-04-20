---
title: 啟用 Adobe Analytics 視訊報告
description: 瞭解如何啟用Adobe Analytics視訊報告。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 16%

---


# 啟用 Adobe Analytics 視訊報告{#enabling-adobe-analytics-video-reports}

使用以Adobe Analytics心率為基礎的視訊報表，在Dynamic Media經典中設定Adobe Analytics時，您不再必須啟用四個視訊檢視器事件（播放、暫停、停止、里程碑）。 視訊心率可與現成可用的Dynamic MediaClassic HTML5視訊和MixedMedia檢視器搭配使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 如需串流媒體和「心率測量」的簡介，請參閱[關於串流媒體的Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* 將Adobe Analytics視訊報表與Dynamic Media經典整合，可支援解決方案變數，但不支援自訂變數。

   如需解決方案變數和自訂變數的詳細資訊，請參閱[音訊和視訊參數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)。

* 支援以1分鐘為增量的現成區段。 不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   如需串流媒體需求與設定的詳細資訊，請參閱[測量Adobe Analytics的串流媒體](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 如需自訂和解決方案變數的詳細資訊，請參閱[啟用媒體報表](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，您必須繼續使用本章所述的步驟，將Adobe Analytics變數指派給Dynamic Media經典檢視器事件和變數。

