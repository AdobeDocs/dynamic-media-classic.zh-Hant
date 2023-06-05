---
title: 啟用Adobe Analytics視訊報表
description: 瞭解如何在Adobe Dynamic Media Classic中啟用Adobe Analytics視訊報告。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# 啟用Adobe Analytics視訊報表{#enabling-adobe-analytics-video-reports}

當您使用Adobe Analytics心率型視訊報表來設定Adobe Dynamic Media Classic中的Adobe Analytics時，不再需要啟用四個視訊檢視器事件（播放、暫停、停止、里程碑）。 影片心率適用於現成可用的Adobe Dynamic Media Classic HTML5影片和混合媒體檢視器。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。

* 如需串流媒體和「心率測量」的簡介，請參閱 [關於適用於流媒體的 Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Adobe Analytics影片報表與Adobe Dynamic Media Classic的整合可支援解決方案變數，但無法支援自訂變數。

   另請參閱 [音訊和視訊引數](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) 以取得解決方案變數和自訂變數的詳細資訊。

* 一分鐘遞增的現成可用區段受到支援。 不過，不支援自訂區段，例如客戶根據時間增量、% 里程碑、偏移里程碑定義的里程碑。

   如需串流媒體需求和設定的詳細資訊，請參閱 [在Adobe Analytics中測量串流媒體](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* 如需自訂和解決方案變數的詳細資訊，請參閱 [啟用媒體報表](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>如果您授權的Adobe Analytics解決方案不包含視訊心率，您必須繼續使用本章所述的步驟，將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數。
