---
title: 快速入門：整合Adobe Dynamic Media Classic和Adobe Analytics
description: 如何整合Adobe Dynamic Media Classic和Adobe Analytics的簡介和快速入門。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 21%

---

# 快速入門：整合Adobe Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款領先同業的產品，可讓行銷人員僅從一個地方就能針對整合自多個行銷通路的所有線上方案的資料進行評估、分析及最佳化。

將Adobe Analytics與Adobe Dynamic Media Classic整合後，您可以在網站上使用Adobe Dynamic Media Classic檢視器取得網站訪客行為的相關報表。 例如，當網站訪客在Adobe Dynamic Media Classic縮放檢視器中選取縮放目標時，Adobe Analytics會記錄此動作。 Adobe Analytics報表可收集Adobe Dynamic Media Classic檢視器中使用者活動的累計資訊。

透過 Adobe Analytics 報告，可以非常清楚地瞭解客戶在網站上的活動。您可以判斷哪些產品簡報會導致轉換，以及哪些不會吸引客戶興趣。

另請參閱Adobe Analytics中的[測量視訊](https://experienceleague.adobe.com/zh-hant/docs/media-analytics/using/media-overview)。

>[!NOTE]
>
>必須具備有效的Adobe Analytics帳戶，才能整合Analytics與Adobe Dynamic Media Classic並產生Analytics報表。

本快速入門旨在協助您快速上手並執行Adobe Analytics Instrumentation Kit。

## 1.透過Adobe Dynamic Media Classic登入Adobe Analytics並下載Adobe Analytics報表變數

>[!NOTE]
>
>確認您已新增為Adobe Analytics中「Web服務存取」群組的成員。 請在設定Adobe Analytics報表之前進行此驗證。 此外，在將Adobe Analytics報表變數與Adobe Dynamic Media Classic事件比對之前。 此群組中的成員可以存取指定報表套裝中的所有報表。 無論介面中設定的許可權為何，您皆可使用Experience Cloud的Web Services API完成此操作。 若要新增成員到群組，請在Adobe Analytics中移至&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**。

確認您是Web服務存取群組成員後，在Adobe Dynamic Media Classic中，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL Adobe Analytics]**。 在Adobe Analytics設定頁面上，選取&#x200B;**[!UICONTROL Adobe Analytics登入]**。

請參閱[登入Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在「Adobe Analytics登入」對話方塊中，輸入您的Experience Cloud組織ID （選擇性）和完整的認證，然後選取「**[!UICONTROL 登入]**」。 在「報告套件」下拉式選單中，選取您要使用的報告套件名稱。

## 2.將Adobe Analytics報表變數指派給Adobe Dynamic Media Classic檢視器事件和Adobe Dynamic Media Classic變數

在「Adobe Analytics 配置」頁面上，指定要用在 Adobe Analytics 報告中的資訊。針對您想瞭解的每個Adobe Dynamic Media Classic檢視器事件，選擇一個Adobe Analytics變數（從報表套裝中）和一個Adobe Dynamic Media Classic變數。

* 檢視器事件描述了要在報告中評估的使用者活動。
* Adobe Dynamic Media Classic變數說明您希望報表傳送之使用者事件的相關資料。

「Adobe Analytics 配置」也提供用於啟用、編輯、刪除檢視器事件的工具。

在Adobe Analytics設定頁面中選取&#x200B;**[!UICONTROL 儲存]**&#x200B;後，測量使用者活動的自訂追蹤程式碼會插入Adobe Dynamic Media Classic檢視器中。 透過該功能可以在 Adobe Analytics 報告中追蹤使用者活動。

請參閱[設定Adobe Analytics報表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## 3.發佈您的Adobe Dynamic Media Classic檢視器

發佈您的Adobe Dynamic Media Classic檢視器，以便將檢視器(包含追蹤Adobe Analytics報表中使用者活動的程式碼)載入Adobe Dynamic Media Classic伺服器。 發佈後，此資訊會包含在檢視器中。 使用它進行Adobe Analytics的分析。

請參閱[發佈組態資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 4.將Adobe Dynamic Media Classic檢視器放置在您的網站上

將含有Adobe Analytics追蹤程式碼的Adobe Dynamic Media Classic檢視器放在您的網站上。

## 5.檢視Adobe Analytics報表，以測試Adobe Analytics整合

若要檢視 Adobe Analytics 報告，請前往 Adobe Analytics 網站。「報告」頁面可讓您檢視資料及產生圖形和圖表，以便評估不同檢視器中的使用者活動。

檢視[檢視Adobe Analytics報表，以測試Adobe Analytics整合](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
