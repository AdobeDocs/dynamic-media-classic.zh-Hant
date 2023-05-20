---
title: 啟用Adobe Analytics視頻報告
description: 瞭解如何在Adobe Dynamic Media Classic啟用Adobe Analytics視頻報告。
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

# 啟用Adobe Analytics視頻報告{#enabling-adobe-analytics-video-reports}

使用基於Adobe Analytics心跳的視頻報告，在Adobe Dynamic Media Classic配置Adobe Analytics時，不必再啟用四個視頻查看器事件（播放、暫停、停止、里程碑）。 Video Heartbat可與開箱即用的Adobe Dynamic Media ClassicHTML5視頻和混合媒體觀看器配合使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 有關流媒體和「心跳測量」的簡介，請參見 [關於適用於串流媒體的 Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* Adobe Analytics視頻報告與Adobe Dynamic Media Classic的整合支援解決方案變數，但不支援自定義變數。

   請參閱 [音頻和視頻參數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) 的子菜單。

* 支援以1分鐘為增量的現成段。 不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   有關流媒體要求和設定的詳細資訊，請參閱 [衡量蒸媒在Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 有關自定義變數和解決方案變數的資訊，請參見 [媒體報告支援](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics許可解決方案不包括視頻心跳信號，則必須繼續使用本章中介紹的步驟將Adobe Analytics變數分配給Adobe Dynamic Media Classic查看器事件和變數。
