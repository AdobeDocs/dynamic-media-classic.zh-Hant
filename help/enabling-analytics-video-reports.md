---
title: 啟用 Adobe Analytics 視訊報告
seo-title: 啟用 Adobe Analytics 視訊報告
description: 'null'
seo-description: 瞭解如何啟用Adobe Analytics視訊報表。
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 25%

---


# 啟用 Adobe Analytics 視訊報告{#enabling-adobe-analytics-video-reports}

使用Adobe Analytics以心率為基礎的視訊報告，在Dynamic Media Classic中設定Adobe Analytics時，您不再需要啟用4個視訊檢視器事件（播放、暫停、停止、里程碑）。 「視訊心率」可與現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器搭配使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* Adobe Analytics視訊報表與Dynamic Media Classic的整合支援解決方案變數，但不支援自訂變數。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 支援現成的一分鐘增量區段。不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>如果您的Adobe Analytics授權解決方案不包含視訊心率，則您需要繼續使用本章所述的步驟，將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數。

