---
title: 「快速啟動：整合Adobe Dynamic Media Classic和Adobe Analytics"
description: 介紹和快速入門，介紹如何整合Adobe Dynamic Media Classic和Adobe Analytics，幫助您快速啟動和運行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# 快速啟動：整合Adobe Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款領先同業的產品，可讓行銷人員僅從一個地方就能針對整合自多個行銷通路的所有線上方案的資料進行評估、分析及最佳化。

將Adobe Analytics與Adobe Dynamic Media Classic整合後，你可以在網站上看到網站訪問者使用Adobe Dynamic Media Classic瀏覽者的行為報告。 例如，當網站訪問者按一下Adobe Dynamic Media Classic縮放查看器中的縮放目標時，Adobe Analytics會記錄此操作。 Adobe Analytics的報告可以收集有關Adobe Dynamic Media Classic觀眾中用戶活動的累積資訊。

透過 Adobe Analytics 報告，可以非常清楚地瞭解客戶在網站上的活動。您可以確定哪些產品演示會導致轉換，哪些產品不會吸引客戶的興趣。

另請參閱 [測量視頻在Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>要將分析與Adobe Dynamic Media Classic整合併生成分析報告，需要有有效的Adobe Analytics帳戶。

本快速入門的設計理念是幫助您快速設定和使用 Adobe Analytics 檢測套件。

## 1。通過Adobe Dynamic Media Classic登錄Adobe Analytics並下載Adobe Analytics報告變數

>[!NOTE]
>
>在配置Adobe Analytics報告並將Adobe Analytics報告變數與Adobe Dynamic Media Classic事件匹配之前，請驗證您是否作為Adobe AnalyticsWeb服務訪問組的成員添加。 此組中的成員可以通過Experience Cloud的Web服務API訪問指定報告套件中的所有報告，而不管在介面中設定了何種權限。 要向組添加成員，請在Adobe Analytics，轉到 **[!UICONTROL 管理工具]** > **[!UICONTROL 用戶管理]** > **[!UICONTROL 編輯組]**。

驗證您是Web服務訪問組的成員後，請轉至Adobe Dynamic Media Classic **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL Adobe Analytics]**。 在「Adobe Analytics配置」頁面上，選擇 **[!UICONTROL Adobe Analytics登錄]**。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在「Adobe Analytics登錄」對話框中，鍵入Experience Cloud組織ID（可選）和完整的身份證明，然後選擇 **[!UICONTROL 登錄]**。 在「報告套件」下拉式選單中，選取您要使用的報告套件名稱。

## 2.將Adobe Analytics報告變數分配給Adobe Dynamic Media Classic查看器事件和Adobe Dynamic Media Classic變數

在「Adobe Analytics 配置」頁面上，指定要用在 Adobe Analytics 報告中的資訊。對於每個您想要有關的Adobe Dynamic Media Classic查看器事件，選擇一個Adobe Analytics變數（從您的報告套件中）和一個Adobe Dynamic Media Classic變數。

* 檢視器事件描述了要在報告中評估的使用者活動。
* Adobe Dynamic Media Classic變數描述您希望報告傳遞的用戶事件資料。

「Adobe Analytics 配置」也提供用於啟用、編輯、刪除檢視器事件的工具。

選擇後 **[!UICONTROL 保存]** 在「Adobe Analytics配置」頁中，用於測量用戶活動的自定義跟蹤代碼插入Adobe Dynamic Media Classic查看器。 透過該功能可以在 Adobe Analytics 報告中追蹤使用者活動。

請參閱 [配置Adobe Analytics報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## 3.發佈您的Adobe Dynamic Media Classic觀眾

發佈您的Adobe Dynamic Media Classic查看器，以便將查看器(帶有用於跟蹤Adobe Analytics報告中用戶活動的代碼)載入到Adobe Dynamic Media Classic伺服器上。 發佈之後，檢視器中即包含該資訊，可供 Adobe Analytics 用於分析。

請參閱 [發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 4.將Adobe Dynamic Media Classic觀眾置於您的網站中

把Adobe Dynamic Media Classic觀眾的Adobe Analytics追蹤密碼放到你的網站上。

## 5.TestAdobe Analytics一體化，觀看一份Adobe Analytics報告

若要檢視 Adobe Analytics 報告，請前往 Adobe Analytics 網站。「報告」頁面可讓您檢視資料及產生圖形和圖表，以便評估不同檢視器中的使用者活動。

請參閱 [TestAdobe Analytics一體化，觀看一份Adobe Analytics報告](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
