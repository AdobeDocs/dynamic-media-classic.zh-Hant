---
title: 啟用Adobe Analytics視訊報表
description: 瞭解如何在Adobe Dynamic Media Classic中啟用Adobe Analytics視訊報告。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# 啟用Adobe Analytics視訊報表{#enabling-adobe-analytics-video-reports}

使用Adobe Analytics心率型視訊報告時，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不再需要啟用四個視訊檢視器事件（播放、暫停、停止、里程碑）。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和混合媒體檢視器。 視訊播放器會產生追蹤資料，以便在Adobe Analytics視訊報表中檢視。

* 如需串流媒體和「心率測量」的簡介，請參閱[關於Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/zh-hant/docs/media-analytics/using/media-overview)。

* Adobe Analytics視訊報表與Adobe Dynamic Media Classic的整合可支援解決方案變數，但不支援自訂變數。

  如需解決方案變數和自訂變數的詳細資訊，請參閱[音訊和視訊引數](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters)。

* 支援一分鐘遞增的現成區段。 但是，不支援自訂區段報告，例如根據時間增量、百分比里程碑或位移里程碑的客戶定義里程碑。

  如需串流媒體需求和設定的詳細資訊，請參閱[在Adobe Analytics中測量串流媒體](https://experienceleague.adobe.com/zh-hant/docs/media-analytics/using/media-overview)。

* 如需自訂和解決方案變數的相關資訊，請參閱[啟用Media報表](https://experienceleague.adobe.com/zh-hant/docs/media-analytics/using/media-reports/media-reports-enable#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，請繼續使用本章所述的步驟，將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數。
