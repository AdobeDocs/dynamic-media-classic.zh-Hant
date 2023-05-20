---
title: 視訊 SEO (搜尋引擎最佳化)
description: 瞭解如何在Adobe Dynamic Media Classic配置視頻SEO設定。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# 視訊 SEO (搜尋引擎最佳化){#video-seo-search-engine-optimization}

SEO 是改善來自搜尋引擎之網站流量的程序。雖然搜尋引擎擅於收集以文字為基礎之內容的相關資訊，但除非向其提供此資訊，否則也無法充分取得視訊相關資訊。

使用Adobe Dynamic Media Classic視頻SEO，您可以應用視頻元資料來為搜索引擎提供您的視頻說明。 Adobe Dynamic Media Classic讓您能夠建立視頻小節集和mRSS源。 這些標準XML檔案用於向搜索引擎提交視頻資訊：

* **視頻站點地圖**  — 告知Google網站上的視頻內容的確切位置和內容。 因此，視頻可以在Google上完全搜索。 例如，視訊網站地圖可以指出視訊的執行時間和類別。有關視頻Sitemaps的資訊，請參見 [視頻模板和視頻站點地圖替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

* **mRSS（媒體真正簡單的聯合）源**  — 內容發佈者用於將媒體檔案饋送到Yahoo! 視訊搜尋。有關mRSS源的資訊，請參見 [視頻模板和視頻站點地圖替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

>[!NOTE]
>
>Google 同時支援視訊網站地圖和 mRSS 新聞頻道通訊協定，可用來送出資訊至搜尋引擎。

Adobe Dynamic Media Classic可以根據每個視頻儲存的元資料生成視頻小節集和mRSS源。 建立視訊網站地圖和 mRSS 新聞頻道後，請決定要包含哪些中繼資料欄位來自視訊檔案。這樣，您可以向搜尋引擎描述視訊，以便搜尋引擎能夠更精確地將流量引導至您網站上的視訊。

>[!NOTE]
>
>在建立視訊網站地圖或 mRSS 新聞頻道前，請先確定搜尋引擎需要 XML 檔案中的哪些欄位，以及如何建立這些欄位的結構。若要建立成功的視訊網站地圖或 mRSS 新聞頻道，它必須符合搜尋引擎的要求。

Adobe Dynamic Media Classic在生成視頻小節集和mRSS源後建立相關報告。 這些報告可在視頻SEO報告頁面上找到。

>[!NOTE]
>
>對於視頻小節集和mRSS源，Adobe Dynamic Media Classic僅從標籤為要發佈的視頻中捕獲元資料。 將視訊標記為發佈，即可將其中繼資料包含於視訊網站地圖和 mRSS 新聞頻道中。

## 選擇視頻SEO設定 {#choosing-video-seo-settings}

為上的視頻小節和mRSS源選擇視頻SEO設定 **[!UICONTROL 視頻搜索引擎優化設定]** 的子菜單。 要開啟此頁，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視頻SEO]** > **[!UICONTROL 設定]**。

在 **[!UICONTROL 常規設定]** 區域，選擇是生成視頻小節集、mRSS源還是兩者。 在 **[!UICONTROL 層代設定]** 將元資料欄位映射到輸入欄位。

選擇設定後，選擇 **[!UICONTROL 保存]** 或 **[!UICONTROL 保存並生成]**)建立視頻站點地圖、mRSS源或兩者。

### 設定常規設定 {#choosing-general-settings}

在 **[!UICONTROL 生成模式]** 下拉清單，選擇報告模式：

* **視頻站點地圖**  — 建立視頻站點地圖。

* **mRSS源**  — 建立媒體RSS(mRSS)源。

* **兩者**  — 建立兩種類型的XML檔案。

* **關閉**  — 要停止生成視頻小節集和媒體RSS(mRSS)源，請選擇此選項。

在 **[!UICONTROL 自動/手動模式]** 下拉清單，選擇是自動生成還是手動生成：

* **自動模式** -Adobe Dynamic Media Classic每天自動生成一個視頻站點地圖、媒體RSS(mRSS)源，或兩者。 選擇 **[!UICONTROL 標籤為發佈]** 選項，以自動標籤為發佈Adobe Dynamic Media Classic生成的XML檔案。

   * **標籤為發佈** 用於發佈生成的XML檔案的標籤。

* **手動模式**  — 選擇時，Adobe Dynamic Media Classic將生成視頻站點地圖、媒體RSS(mRSS)源或兩者 **[!UICONTROL 生成]** 或 **[!UICONTROL 保存並生成]** 在視頻搜索優化設定螢幕中。 同時，也請選擇這些選項:

   * **無其他設定**  — 不標籤為發佈生成的XML檔案。

   * **標籤為發佈**  — 用於發佈生成的XML檔案的標籤。

   * **允許部分生成**  — 如果XML檔案不包含所有視頻的完整元資料資訊，則搜索引擎可以拒絕該檔案。 即使某些視頻的元資料不可用，此選項也會生成XML檔案。 警告會登錄在「報告」畫面上。如果您要匯出 XML 檔案並手動處理遺失的資訊，請選擇此選項。

### 選擇產生設定 {#choosing-generation-settings}

「層代設定」區域列出「視頻站點地圖」或mRSS源的輸入欄位，或兩者都列出，並在「元資料」面板中列出元資料欄位的名稱。 使用「一般設定」區域，即可將輸入欄位對應至中繼資料欄位。通過這樣做，您可以告訴Adobe Dynamic Media Classic從何處獲取視頻站點地圖和/或mRSS源的元資料。

1. 在「中繼資料檢視」選單上選擇中繼資料檢視。選擇檢視後，中繼資料欄位的名稱便會顯示在「中繼資料」面板中。請參閱[中繼資料檢視](application-setup.md#metadata_views)。
1. 將中繼資料欄位名稱從「中繼資料」面板拖曳至「登陸頁面」、「標題」、「描述」、「標籤」和「類別」輸入欄位。「登陸頁面」、「標題」和「描述」欄位為必填。

   >[!NOTE]
   >
   >您也可以手動將資料輸入至輸入欄位。

1. 進行以下一項操作:

   * 要保存設定而不生成XML檔案，請選擇 **[!UICONTROL 保存]**。
   * 要保存和生成檔案，請選擇 **[!UICONTROL 保存並生成]**。

      XML 檔案會產生並記錄在工作記錄檔中。視訊網站地圖 (video-sitemap) 和媒體 RSS (mRSS) 新聞頻道 (mrss-feed) 檔案會儲存在公司的根檔案夾中。

>[!NOTE]
>
>在將視頻站點地圖或mRSS源提交到搜索引擎之前，先發佈該源。 視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中。如果需要，將這些XML檔案標籤為要發佈，然後選擇 **[!UICONTROL 發佈]**。

## 將視頻站點地圖和mRSS-Feed檔案提交到搜索引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

將上述其中一個 URL 複製到搜尋引擎的站長工具，即可將您的視訊網站地圖或媒體 RSS (mRSS) 新聞頻道檔案送出至搜尋引擎。

## 查看視頻SEO報告 {#viewing-video-seo-reports}

在「視頻搜索引擎優化報告」頁上查看視頻SEO報告。 要開啟此頁，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視頻SEO]** > **[!UICONTROL 報告]**。

如果在生成報告時出錯，則會在「報告」頁中列出這些錯誤。
