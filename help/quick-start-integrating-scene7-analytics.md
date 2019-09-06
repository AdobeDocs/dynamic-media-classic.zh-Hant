---
title: 「快速入門：整合Dynamic Media Classic和Adobe Analytics」
seo-title: 「快速入門：整合Dynamic Media Classic和Adobe Analytics」
description: 'null'
seo-description: 整合Dynamic Media Classic和Adobe Analytic的簡介與快速入門，協助您快速上手使用。
uuid: 3f9e2c91-15d4-4b53-82220-9b1ca57c0b1d
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/adobe_ analytics_ tooling_ kit
discoiquuid: abec9a85-013c-4030-b129-bc27 a89 cb464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 快速入門：整合Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics 是一款領先同業的產品，可讓行銷人員僅從一個地方就能針對整合自多個行銷通路的所有線上方案的資料進行評估、分析及最佳化。

將Adobe Analytics與Scene Publishing System整合之後，您可以取得有關網站上使用動態媒體Classic檢視器的網站訪客行為報告。例如，當網站訪客在動態媒體Classic縮放檢視器中點按縮放目標時，Adobe Analytics會記錄此動作。Adobe Analytics報表可收集動態媒體Classic檢視器中使用者活動的累積資訊。

透過 Adobe Analytics 報告，可以非常清楚地瞭解客戶在網站上的活動。由此判定哪些產品簡報方式可以改變客戶的想法，哪些方式無法讓客戶感興趣。

另請參閱[在 Adobe Analytics 中測量視訊](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/)。

>[!NOTE]
>
>若要將 Analytics 與 Scene7 Publishing System 整合並產生 Analytics 報告，必須使用有效的 Adobe Analytics 帳戶。

**快速入門**

本快速入門的設計理念是幫助您快速設定和使用 Adobe Analytics 檢測套件。

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>在您可以設定Adobe Analytics報表並比對Adobe Analytics報表變數至Dynamic Media Classic事件之前，請確認您已新增為Adobe Analytics中「網站服務存取」群組的成員。不論在介面中設定的權限為何，此群組的成員皆可經由 Marketing Cloud 的「網路服務 API」存取指定報告套件中的所有報告。若要在群組中增加成員，請在 Adobe Analytics 中按一下「**管理工具** &gt; **使用者管理** &gt; **編輯群組**」。

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. 在「Adobe Analytics 配置」頁面中，按一下「**Adobe Analytics 登入**」。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在「Adobe Analytics登入」對話方塊中，輸入您的Marketing Cloud組織ID(選用)和完整的認證，然後按一下 **「登入**」。在「報告套件」下拉式選單中，選取您要使用的報告套件名稱。

**2. 將Adobe Analytics報表變數指派給Dynamic Media Classic檢視器事件和Dynamic Media Classic變數**

在「Adobe Analytics 配置」頁面上，指定要用在 Adobe Analytics 報告中的資訊。對於您想要的每個動態媒體Classic檢視器事件，請選擇Adobe Analytics變數(從您的報表套裝)和動態媒體Classic變數。

* 檢視器事件描述了要在報告中評估的使用者活動。
* 動態媒體Classic變數會說明您要傳送報表的使用者事件資料。

「Adobe Analytics 配置」也提供用於啟用、編輯、刪除檢視器事件的工具。

在您按一下「Adobe Analytics設定」畫面中的「儲存」後，可在動態媒體Classic檢視器中插入測量使用者活動的自訂追蹤代碼。透過該功能可以在 Adobe Analytics 報告中追蹤使用者活動。

請參閱[設定 Adobe Analytics 報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

**3. 發佈您的動態媒體Classic檢視器**

發佈您的動態媒體Classic檢視器，讓檢視器(在Adobe Analytics報表中追蹤使用者活動的程式碼)會載入Dynamic Media Classic伺服器上。發佈之後，檢視器中即包含該資訊，可供 Adobe Analytics 用於分析。

請參閱[發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

**4. 將動態媒體Classic檢視器置於您的網站**

在您的網站上使用Adobe Analytics追蹤代碼放置Dynamic Media Classic檢視器。

**5. 檢視 Adobe Analytics 報告以測試 Adobe Analytics 整合**

若要檢視 Adobe Analytics 報告，請前往 Adobe Analytics 網站。「報告」頁面可讓您檢視資料及產生圖形和圖表，以便評估不同檢視器中的使用者活動。

請參閱[檢視 Adobe Analytics 報告以測試 Adobe Analytics 整合](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
