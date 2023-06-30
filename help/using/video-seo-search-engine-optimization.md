---
title: 視訊 SEO (搜尋引擎最佳化)
description: 瞭解如何在Adobe Dynamic Media Classic中設定視訊SEO設定。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# 視訊 SEO (搜尋引擎最佳化){#video-seo-search-engine-optimization}

SEO 是改善來自搜尋引擎之網站流量的程序。雖然搜尋引擎擅於收集以文字為基礎之內容的相關資訊，但除非向其提供此資訊，否則也無法充分取得視訊相關資訊。

使用Adobe Dynamic Media Classic視訊SEO，您可以套用視訊中繼資料，以向搜尋引擎提供您視訊的說明。 Adobe Dynamic Media Classic可讓您建立視訊網站地圖和mRSS摘要。 這些標準XML檔案用於將視訊資訊提交至搜尋引擎：

* **視訊網站地圖**  — 通知Google視訊內容在網站上的確切位置與內容。 因此，您完全可以在Google上搜尋影片。 例如，視訊網站地圖可以指出視訊的執行時間和類別。如需視訊網站地圖的相關資訊，請參閱 [視訊網站地圖和視訊網站地圖的替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS (Media Really Simple Syndication)摘要**  — 內容發佈者用來將媒體檔案饋送至Yahoo！ 視訊搜尋。如需mRSS摘要的相關資訊，請參閱 [視訊網站地圖和視訊網站地圖的替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google 同時支援視訊網站地圖和 mRSS 新聞頻道通訊協定，可用來送出資訊至搜尋引擎。

Adobe Dynamic Media Classic可從儲存於每個視訊的中繼資料產生視訊網站地圖和mRSS摘要。 建立視訊網站地圖和 mRSS 新聞頻道後，請決定要包含哪些中繼資料欄位來自視訊檔案。這樣，您可以向搜尋引擎描述視訊，以便搜尋引擎能夠更精確地將流量引導至您網站上的視訊。

>[!NOTE]
>
>在建立視訊網站地圖或 mRSS 新聞頻道前，請先確定搜尋引擎需要 XML 檔案中的哪些欄位，以及如何建立這些欄位的結構。若要建立成功的視訊網站地圖或 mRSS 新聞頻道，它必須符合搜尋引擎的要求。

Adobe Dynamic Media Classic會在您產生視訊網站地圖和mRSS摘要後，建立相關報表。 這些報告可在視訊SEO報告頁面上取得。

>[!NOTE]
>
>對於視訊網站地圖和mRSS摘要，Adobe Dynamic Media Classic只會從標示為發佈的視訊中擷取中繼資料。 將視訊標記為發佈，即可將其中繼資料包含於視訊網站地圖和 mRSS 新聞頻道中。

## 選擇視訊SEO設定 {#choosing-video-seo-settings}

在上選取視訊網站地圖和mRSS摘要的視訊SEO設定 **[!UICONTROL 視訊搜尋引擎最佳化設定]** 頁面。 若要開啟此頁面，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊SEO]** > **[!UICONTROL 設定]**.

在 **[!UICONTROL 一般設定]** 區域，選擇是否要產生視訊網站地圖、mRSS摘要，或兩者都產生。 在 **[!UICONTROL 產生設定]** 區域，將中繼資料欄位對應至輸入欄位。

選擇設定後，選取 **[!UICONTROL 儲存]** (或 **[!UICONTROL 儲存並產生]**)，以建立「視訊網站地圖」和/或「mRSS摘要」。

### 設定一般設定 {#choosing-general-settings}

於 **[!UICONTROL 產生模式]** 從下拉式清單中選擇報表模式：

* **視訊網站地圖**  — 建立視訊網站地圖。

* **mRSS摘要**  — 建立媒體RSS (mRSS)摘要。

* **兩者**  — 建立兩種型別的XML檔案。

* **關閉**  — 若要停止產生視訊網站地圖和媒體RSS (mRSS)摘要，請選擇此選項。

於 **[!UICONTROL 自動/手動模式]** 下拉式清單，選擇是否要自動或手動產生：

* **自動模式** - Adobe Dynamic Media Classic每天都會自動產生一個視訊網站地圖、媒體RSS (mRSS)摘要，或兩者皆產生。 選取 **[!UICONTROL 標籤為發佈]** 自動標示為發佈Adobe Dynamic Media Classic產生的XML檔案的選項。

   * **標籤為發佈** 標籤為發佈產生的XML檔案。

* **手動模式** - Adobe Dynamic Media Classic會在您選取時產生視訊網站地圖、媒體RSS (mRSS)摘要，或兩者皆產生 **[!UICONTROL 產生]** 或 **[!UICONTROL 儲存並產生]** 在「視訊搜尋最佳化設定」畫面中。 同時，也請選擇這些選項:

   * **沒有其他設定**  — 不會標籤為發佈產生的XML檔案。

   * **標籤為發佈**  — 標籤為發佈產生的XML檔案。

   * **允許部分產生**  — 如果XML檔案未包含所有影片的完整中繼資料資訊，搜尋引擎可以拒絕該檔案。 即使某些影片沒有中繼資料，此選項也會產生XML檔案。 警告會登錄在「報告」畫面上。如果您要匯出 XML 檔案並手動處理遺失的資訊，請選擇此選項。

### 選擇產生設定 {#choosing-generation-settings}

「產生設定」區域會列出「視訊網站地圖」或mRSS摘要（或兩者）的輸入欄位，在「中繼資料」面板中則列出中繼資料欄位的名稱。 使用「一般設定」區域，即可將輸入欄位對應至中繼資料欄位。如此一來，您就能告訴Adobe Dynamic Media Classic從何處取得視訊網站地圖和/或mRSS摘要的中繼資料。

1. 在「中繼資料檢視」選單上選擇中繼資料檢視。選擇檢視後，中繼資料欄位的名稱便會顯示在「中繼資料」面板中。請參閱[中繼資料檢視](application-setup.md#metadata_views)。
1. 將中繼資料欄位名稱從「中繼資料」面板拖曳至「登陸頁面」、「標題」、「描述」、「標籤」和「類別」輸入欄位。「登陸頁面」、「標題」和「描述」欄位為必填。

   >[!NOTE]
   >
   >您也可以手動將資料輸入至輸入欄位。

1. 進行以下一項操作:

   * 若要儲存設定而不產生XML檔案，請選取 **[!UICONTROL 儲存]**.
   * 若要儲存並產生檔案，請選取 **[!UICONTROL 儲存並產生]**.

     XML 檔案會產生並記錄在工作記錄檔中。視訊網站地圖 (video-sitemap) 和媒體 RSS (mRSS) 新聞頻道 (mrss-feed) 檔案會儲存在公司的根檔案夾中。

>[!NOTE]
>
>先發佈視訊網站地圖或mRSS摘要，您才能將其提交至搜尋引擎。 視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中。視需要標籤這些XML檔案以供發佈，然後選取 **[!UICONTROL 發佈]**.

## 將視訊網站地圖和mRSS摘要檔案提交至搜尋引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

將上述其中一個 URL 複製到搜尋引擎的站長工具，即可將您的視訊網站地圖或媒體 RSS (mRSS) 新聞頻道檔案送出至搜尋引擎。

## 檢視視訊SEO報表 {#viewing-video-seo-reports}

在視訊搜尋引擎最佳化報告頁面上檢視視訊SEO報告。 若要開啟此頁面，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊SEO]** > **[!UICONTROL 報表]**.

如果產生報表時發生錯誤，就會列在報表頁面上。
