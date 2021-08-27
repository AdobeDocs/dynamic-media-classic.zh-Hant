---
title: 啟用Adobe Analytics視訊報表
description: 了解如何在Adobe Analytics Classic中啟用AdobeDynamic Media視訊報表。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# 啟用Adobe Analytics視訊報表{#enabling-adobe-analytics-video-reports}

使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，您不再必須啟用四個視訊檢視器事件（播放、暫停、停止、里程碑）。 視訊心率可用於現成可用的AdobeDynamic Media Classic HTML5視訊和混合媒體檢視器。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 如需串流媒體和「心率測量」的簡介，請參閱[關於Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* Adobe Analytics視訊報表與AdobeDynamic Media Classic的整合支援解決方案變數，但不支援自訂變數。

   如需解決方案變數和自訂變數的詳細資訊，請參閱[音訊和視訊參數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)。

* 支援以1分鐘為增量的現成可用區段。 不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   如需串流媒體需求和設定的詳細資訊，請參閱[在Adobe Analytics中測量串流媒體](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 如需自訂和解決方案變數的相關資訊，請參閱啟用媒體報表](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。[

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，您必須繼續使用本章所述步驟，將Adobe Analytics變數指派給AdobeDynamic Media Classic檢視器事件和變數。
