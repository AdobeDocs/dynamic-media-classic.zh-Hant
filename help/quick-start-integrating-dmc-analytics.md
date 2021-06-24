---
title: 「快速入門：整合Dynamic Media Classic和Adobe Analytics」
description: 整合Dynamic Media Classic和Adobe Analytics的簡介和快速入門，可協助您快速上手並執行。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 41%

---

# 快速入門：整合Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款領先同業的產品，可讓行銷人員僅從一個地方就能針對整合自多個行銷通路的所有線上方案的資料進行評估、分析及最佳化。

將Adobe Analytics與Dynamic Media Classic整合後，您就可以在網站上使用Dynamic Media Classic檢視器取得網站訪客行為的相關報表。 例如，當網站訪客在Dynamic Media Classic縮放檢視器中按一下縮放目標時，Adobe Analytics會記錄此動作。 Adobe Analytics報表可在Dynamic Media Classic檢視器中收集使用者活動的累積資訊。

透過 Adobe Analytics 報告，可以非常清楚地瞭解客戶在網站上的活動。您可以決定哪些產品簡報能帶來轉換，哪些不能吸引客戶的興趣。

另請參閱[在 Adobe Analytics 中測量視訊](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>必須具備有效的Adobe Analytics帳戶，才能整合Analytics與Dynamic Media Classic並產生Analytics報表。

本快速入門的設計理念是幫助您快速設定和使用 Adobe Analytics 檢測套件。

## 1.透過Dynamic Media Classic登入Adobe Analytics並下載Adobe Analytics報表變數

>[!NOTE]
>
>在設定Adobe Analytics報表並將Adobe Analytics報表變數與Dynamic Media Classic事件相符之前，請確認您已新增為Adobe Analytics中「網站服務存取」群組的成員。 不論在介面中設定的權限為何，此群組的成員皆可經由 Marketing Cloud 的「網路服務 API」存取指定報告套件中的所有報告。若要在群組中增加成員，請在 Adobe Analytics 中按一下「**[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**」。

在確認您是Web服務訪問組的成員後，在Dynamic Media Classic中，按一下&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**。 在「Adobe Analytics 配置」頁面中，按一下「**[!UICONTROL Adobe Analytics 登入]**」。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在「Adobe Analytics登入」對話方塊中，輸入您的Marketing Cloud組織ID（選用）和您的完整憑證，然後按一下「**[!UICONTROL 登入]**」。 在「報告套件」下拉式選單中，選取您要使用的報告套件名稱。

## 2.將Adobe Analytics報表變數指派給Dynamic Media Classic檢視器事件和Dynamic Media Classic變數

在「Adobe Analytics 配置」頁面上，指定要用在 Adobe Analytics 報告中的資訊。針對您想要了解的每個Dynamic Media Classic檢視器事件，選擇Adobe Analytics變數（來自您的報表套裝）和Dynamic Media Classic變數。

* 檢視器事件描述了要在報告中評估的使用者活動。
* Dynamic Media Classic變數會說明您希望報表傳送的使用者事件相關資料。

「Adobe Analytics 配置」也提供用於啟用、編輯、刪除檢視器事件的工具。

在「Adobe Analytics設定」頁面中按一下「**[!UICONTROL 儲存]**」後，會在Dynamic Media Classic檢視器中插入測量使用者活動的自訂追蹤代碼。 透過該功能可以在 Adobe Analytics 報告中追蹤使用者活動。

請參閱[設定 Adobe Analytics 報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## 3.發佈您的Dynamic Media Classic檢視器

發佈您的Dynamic Media Classic檢視器，以便在Dynamic Media Classic伺服器上載入檢視器(包含用於追蹤Adobe Analytics報表中使用者活動的程式碼)。 發佈之後，檢視器中即包含該資訊，可供 Adobe Analytics 用於分析。

請參閱[發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 4.將Dynamic Media Classic檢視器放入您的網站

將Dynamic Media Classic檢視器與Adobe Analytics追蹤程式碼一起放置在您的網站上。

## 5.檢視Adobe Analytics報表以測試Adobe Analytics整合

若要檢視 Adobe Analytics 報告，請前往 Adobe Analytics 網站。「報告」頁面可讓您檢視資料及產生圖形和圖表，以便評估不同檢視器中的使用者活動。

請參閱[檢視 Adobe Analytics 報告以測試 Adobe Analytics 整合](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
