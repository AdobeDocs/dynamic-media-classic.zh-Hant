---
title: 啟用Adobe Analytics視訊報表
description: 了解如何在Adobe Dynamic Media Classic中啟用Adobe Analytics視訊報表。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# 啟用Adobe Analytics視訊報表{#enabling-adobe-analytics-video-reports}

使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，您不再必須啟用四個視訊檢視器事件（播放、暫停、停止、里程碑）。 視訊心率可用於現成可用的Adobe Dynamic Media ClassicHTML5視訊和混合媒體檢視器。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 如需串流媒體和「心率測量」的簡介，請參閱 [關於Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Adobe Analytics視訊報表與Adobe Dynamic Media Classic的整合支援解決方案變數，但不支援自訂變數。

   請參閱 [音訊和視訊參數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) 以取得解決方案變數和自訂變數的詳細資訊。

* 支援以1分鐘為增量的現成可用區段。 不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   如需串流媒體需求和設定的詳細資訊，請參閱 [在Adobe Analytics測量蒸媒](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* 如需自訂和解決方案變數的相關資訊，請參閱 [啟用媒體報表](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，您必須繼續使用本章所述步驟，將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數。
