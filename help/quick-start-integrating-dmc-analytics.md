---
title: 「快速入門：整合Dynamic Media經典與Adobe Analytics」
description: 將Dynamic Media經典與Adobe Analytics整合的簡介和快速入門，協助您快速上手使用。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media經典
role: Data Engineer,Administrator,Business Practitioner
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 41%

---

# 快速入門：整合Dynamic Media經典與Adobe Analytics{#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款領先同業的產品，可讓行銷人員僅從一個地方就能針對整合自多個行銷通路的所有線上方案的資料進行評估、分析及最佳化。

將Adobe Analytics與Dynamic Media經典整合後，您可以在網站上取得有關使用Dynamic Media經典檢視器的網站訪客行為的報告。 例如，當網站訪客在Dynamic Media經典縮放檢視器中按一下縮放目標時，Adobe Analytics會記錄此動作。 Adobe Analytics報告可以收集Dynamic Media經典檢視器中使用者活動的累積資訊。

透過 Adobe Analytics 報告，可以非常清楚地瞭解客戶在網站上的活動。您可以決定哪些產品簡報可帶來轉化，哪些不吸引客戶。

另請參閱[在 Adobe Analytics 中測量視訊](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>必須有有效的Adobe Analytics帳戶，才能將Analytics與Dynamic Media經典整合，並產生Analytics報表。

本快速入門的設計理念是幫助您快速設定和使用 Adobe Analytics 檢測套件。

## 1.透過Dynamic Media經典網站登入Adobe Analytics並下載Adobe Analytics報告變數

>[!NOTE]
>
>在您設定Adobe Analytics報表並將Adobe Analytics報表變數與Dynamic Media經典事件相符之前，請先確認您已新增為Adobe Analytics網站服務存取群組的成員。 不論在介面中設定的權限為何，此群組的成員皆可經由 Marketing Cloud 的「網路服務 API」存取指定報告套件中的所有報告。若要在群組中增加成員，請在 Adobe Analytics 中按一下「**[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**」。

在確認您是Web服務訪問組的成員後，在Dynamic MediaClassic中按一下&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**。 在「Adobe Analytics 配置」頁面中，按一下「**[!UICONTROL Adobe Analytics 登入]**」。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在「Adobe Analytics登錄」對話框中，鍵入您的Marketing Cloud組織ID（可選）和完整憑據，然後按一下&#x200B;**[!UICONTROL 登錄]**。 在「報告套件」下拉式選單中，選取您要使用的報告套件名稱。

## 2.將Adobe Analytics報表變數指派給Dynamic Media經典檢視器事件和Dynamic Media經典變數

在「Adobe Analytics 配置」頁面上，指定要用在 Adobe Analytics 報告中的資訊。針對您想要取得相關資訊的每個Dynamic Media經典檢視器事件，選擇Adobe Analytics變數（來自您的報表套裝）和Dynamic Media經典變數。

* 檢視器事件描述了要在報告中評估的使用者活動。
* Dynamic Media經典變數會描述您要報表傳遞之使用者事件的相關資料。

「Adobe Analytics 配置」也提供用於啟用、編輯、刪除檢視器事件的工具。

在您按一下「Adobe Analytics設定」頁面中的&#x200B;**[!UICONTROL Save]**&#x200B;後，會在「Dynamic Media傳統型」檢視器中插入用於測量使用者活動的自訂追蹤代碼。 透過該功能可以在 Adobe Analytics 報告中追蹤使用者活動。

請參閱[設定 Adobe Analytics 報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## 3.發佈您的Dynamic Media經典觀眾

發佈您的Dynamic Media經典檢視器，讓檢視器(在Adobe Analytics報表中使用追蹤使用者活動的程式碼)載入Dynamic Media經典伺服器。 發佈之後，檢視器中即包含該資訊，可供 Adobe Analytics 用於分析。

請參閱[發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 4.將Dynamic Media經典影像檢視器放入您的網站

將具有Adobe Analytics追蹤程式碼的Dynamic Media經典檢視器放在您的網站上。

## 5.檢視Adobe Analytics報告以測試Adobe Analytics整合

若要檢視 Adobe Analytics 報告，請前往 Adobe Analytics 網站。「報告」頁面可讓您檢視資料及產生圖形和圖表，以便評估不同檢視器中的使用者活動。

請參閱[檢視 Adobe Analytics 報告以測試 Adobe Analytics 整合](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
