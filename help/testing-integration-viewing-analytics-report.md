---
title: 檢視 Adobe Analytics 報告以測試整合
description: 了解如何檢視Adobe Analytics報表以測試整合。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 15%

---

# 檢視 Adobe Analytics 報告以測試整合{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中建立必要變數、將其連結至Dynamic Media Classic事件，以及完成必要的實作步驟後，您就可以測試設定。 您可以測試並確認 Adobe Analytics 本身正在擷取資料。如果設定在此有效，則不需再執行其他步驟。假設您依照上述步驟操作，並將Dynamic Media Classic事件資料連結至一或多個自訂流量變數，然後依照此工作流程在Adobe Analytics內測試您的資料。

**若要檢視Adobe Analytics報表以測試整合：**

1. 從您的帳戶啟動Dynamic Media Classic檢視器，尤其是廣播您要取得的量度，並與其互動以建立一些事件資料的檢視器。

   例如，如果您想要測量影像集中的熱門替代檢視，然後預覽影像集並按一下不同的縮圖影像。

1. 在Adobe Analytics內，前往「**[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > [Prop名稱]」，從功能表選項中選取您的流量prop名稱。

   例如，若要存取範例帳戶中的&#x200B;**[!UICONTROL LoadAsset]** prop，正確的功能表選項會是&#x200B;**[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > **[!UICONTROL LoadAsset]**。 如果您有10個以上的自訂Prop，您也會看到其他功能表選項。

1. 檢視 Adobe Analytics 產生的圖表此圖表通常只是單一量度的資料。 如果您也想知道此資料與哪些資產相關聯，請取得此事件的資產資料。 例如，了解哪部影片的觀看率僅為50%，或某組影像的受歡迎度通常很實用。

>[!NOTE]
>
>所有Dynamic Media Classic檢視器資料都會顯示在Adobe Analytics的「自訂流量」報表或「自訂轉換」報表中，並加以報告。

如需詳細資訊，請參閱[AnalyticsTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)。