---
title: 檢視Adobe Analytics報表以測試整合
description: 瞭解如何檢視Adobe Analytics報表，以測試Adobe Dynamic Media Classic中的整合。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# 檢視Adobe Analytics報表以測試整合{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中建立必要的變數、將其連結至Adobe Dynamic Media Classic事件，並完成必要的實作步驟後，您就可以測試設定。 您可以測試及驗證Adobe Analytics本身是否擷取資料。 如果設定在此有效，則不需再執行其他步驟。假設您依照上述步驟進行，並將Adobe Dynamic Media Classic事件資料連結至一或多個自訂流量變數，接著依照此工作流程在Adobe Analytics中測試您的資料。

**若要檢視Adobe Analytics報表以測試整合：**

1. 從您的帳戶啟動Adobe Dynamic Media Classic檢視器，尤其是要廣播您要取得之量度的帳戶，並與該帳戶互動以建立某些事件資料。

   例如，如果您想要測量「影像集」中常用的替代檢視，請預覽「影像集」並按一下不同的縮圖影像。

1. 在Adobe Analytics中，前往&#x200B;**[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > [prop名稱]，從選單選項中選取您的流量prop名稱。

   例如，若要存取範例帳戶中的&#x200B;**[!UICONTROL LoadAsset]** prop，正確的功能表選擇是&#x200B;**[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > **[!UICONTROL LoadAsset]**。 如果您有十個以上的自訂Prop，您也會看到其他選單選項。

1. 檢視 Adobe Analytics 產生的圖表此圖表通常只是單一量度的資料。 如果您也想知道此資料與哪個資產相關聯，請取得此事件的資產資料。 例如，通常知道觀看了哪個影片僅50%，或集合中的哪個影像受歡迎會很有用。

>[!NOTE]
>
>所有Adobe Dynamic Media Classic檢視器資料都會顯示於Adobe Analytics的「自訂流量」報表或「自訂轉換」報表中，並彙整成報表。

如需詳細資訊，請參閱[Analytics教學課程](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview)。