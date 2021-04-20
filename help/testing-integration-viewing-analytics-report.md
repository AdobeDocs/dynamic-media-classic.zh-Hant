---
title: 檢視 Adobe Analytics 報告以測試整合
description: 瞭解如何檢視Adobe Analytics報告來測試整合。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 39%

---


# 檢視 Adobe Analytics 報告以測試整合{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics建立必要的變數後，請將它們連結至Dynamic Media經典事件並完成必要的實作步驟，然後您應測試設定。 您可以測試並確認 Adobe Analytics 本身正在擷取資料。如果設定在此有效，則不需再執行其他步驟。假設您遵循上述步驟，並將您的Dynamic Media經典事件資料連結至一或多個自訂流量變數，則請遵循此工作流程，在Adobe Analytics內測試您的資料。

**檢視 Adobe Analytics 報告以測試整合**

1. 從您的帳戶啟動Dynamic Media經典檢視器，尤其是廣播您要擷取的量度，並與它互動以建立某些事件資料的檢視器。

   例如，如果要測量影像集內最常用的替代檢視，請預設影像集，並按一下不同的縮圖影像。

1. 在Adobe Analytics內，前往「自訂流量>自訂流量1-10 > [prop名稱」，從功能表選項中選取您的流量prop名稱。]

   例如，若要存取範例帳戶中的 LoadAsset 屬性，則適當的選單選項為「自訂流量 > 自訂流量 1-10 > LoadAsset」。如果您有超過十個自訂屬性，可能還會看到其他選單選項。

1. 檢視 Adobe Analytics 產生的圖表請注意，這通常只是單一度量的資料。如果您也想知道此資料與哪些資產相關聯（例如，哪些視訊只被觀看50%，或某組影像最受歡迎），請務必也擷取此事件的資產資料。

>[!NOTE]
>
>所有Dynamic Media經典檢視器資料都會顯示並報告在Adobe Analytics的自訂流量報表或自訂轉換報表中。

如需詳細資訊，請參閱[www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)。
