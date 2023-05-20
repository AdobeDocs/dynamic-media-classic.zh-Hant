---
title: 檢視 報告以測試 Adobe Analytics 整合
description: 通過查看Adobe Analytics報告，瞭解如何testAdobe Dynamic Media Classic的一體化。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 15%

---

# 檢視 報告以測試 Adobe Analytics 整合{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中建立必要的變數，將它們連結到Adobe Dynamic Media Classic事件，並完成必要的實施步驟後，您可以test設定。 您可以測試並確認 Adobe Analytics 本身正在擷取資料。如果設定在此有效，則不需再執行其他步驟。假設您遵循上述步驟並將Adobe Dynamic Media Classic事件資料連結到一個或多個自定義流量變數，則按照此工作流在Adobe Analytics內test資料。

**要test整合，請查看Adobe Analytics報告：**

1. 從您的帳戶啟動Adobe Dynamic Media Classic查看器，尤其是廣播您要獲取的度量並與其交互以建立某些事件資料的查看器。

   例如，如果要測量「影像集」中的常用替代視圖，則預覽「影像集」並按一下不同的縮略圖影像。

1. 在Adobe Analytics內，轉到 **[!UICONTROL 自定義通信]** > **[!UICONTROL 自定義流量1-10]** > [prop的名稱]，從菜單選項中選擇您的通信流量名稱。

   例如，訪問 **[!UICONTROL 載入資產]** prop在示例帳戶中，正確的菜單選項是 **[!UICONTROL 自定義通信]** > **[!UICONTROL 自定義流量1-10]** > **[!UICONTROL 載入資產]**。 如果您有10個以上的自定義道具，您還會看到其他菜單選項。

1. 檢視 Adobe Analytics 產生的圖表此圖表通常只是單個度量的資料。 如果您還想知道此資料與哪些資產關聯，請獲取此事件的資產資料。 例如，瞭解哪個視頻只被50%觀看，或某個集合中哪個影像比較流行，這通常非常有用。

>[!NOTE]
>
>所有Adobe Dynamic Media Classic查看器資料都顯示並報告在Adobe Analytics的自定義流量報告或自定義轉換報告中。

有關詳細資訊，請參見 [分析Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)。