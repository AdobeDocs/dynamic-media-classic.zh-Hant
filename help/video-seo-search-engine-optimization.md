---
title: 視訊 SEO (搜尋引擎最佳化)
description: 瞭解如何設定視訊SEO設定。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media經典
role: Administrator
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 40%

---

# 視訊 SEO (搜尋引擎最佳化){#video-seo-search-engine-optimization}

SEO 是改善來自搜尋引擎之網站流量的程序。雖然搜尋引擎擅於收集以文字為基礎之內容的相關資訊，但除非向其提供此資訊，否則也無法充分取得視訊相關資訊。

使用Dynamic Media經典視訊搜尋引擎優化(SEO)，您可以套用視訊中繼資料，提供搜尋引擎視訊的說明。 Dynamic Media經典可讓您建立視訊網站地圖和mRSS饋送。 這些標準XML檔案可用來將視訊資訊送出至搜尋引擎：

* **視訊網站地圖** -告知Google視訊內容在網站的確切位置和內容。因此，視訊可在Google上完全搜尋。 例如，視訊網站地圖可以指出視訊的執行時間和類別。如需視訊網站地圖的詳細資訊，請參閱[視訊網站地圖和視訊網站地圖替代項目](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

* **mRSS（媒體真正簡單的匯集）摘要** -內容發佈者用來將媒體檔案饋送到Yahoo!視訊搜尋。如需mRSS饋送的詳細資訊，請參閱[視訊網站地圖和視訊網站地圖替代項目](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

>[!NOTE]
>
>Google 同時支援視訊網站地圖和 mRSS 新聞頻道通訊協定，可用來送出資訊至搜尋引擎。

Dynamic Media經典可以根據儲存在每個視訊中的中繼資料，產生視訊網站地圖和mRSS饋送。 建立視訊網站地圖和 mRSS 新聞頻道後，請決定要包含哪些中繼資料欄位來自視訊檔案。這樣，您可以向搜尋引擎描述視訊，以便搜尋引擎能夠更精確地將流量引導至您網站上的視訊。

>[!NOTE]
>
>在建立視訊網站地圖或 mRSS 新聞頻道前，請先確定搜尋引擎需要 XML 檔案中的哪些欄位，以及如何建立這些欄位的結構。若要建立成功的視訊網站地圖或 mRSS 新聞頻道，它必須符合搜尋引擎的要求。

Dynamic Media經典會在您產生視訊網站地圖和mRSS饋送後建立相關報表。 這些報表可在「視訊搜尋引擎最佳化報表」頁面上使用。

>[!NOTE]
>
>對於視訊網站地圖和mRSS饋送，Dynamic Media經典僅會從標籤為發佈的視訊擷取中繼資料。 將視訊標記為發佈，即可將其中繼資料包含於視訊網站地圖和 mRSS 新聞頻道中。

## 選擇視頻SEO設定{#choosing-video-seo-settings}

在&#x200B;**[!UICONTROL 視訊搜尋引擎最佳化設定]**&#x200B;頁面上，按一下視訊網站地圖和mRSS饋送的視訊SEO設定。 若要開啟此頁面，請在全域導覽列上按一下「設定&#x200B;**** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊搜尋引擎最佳化(SEO)>>**[!UICONTROL &#x200B;設定&#x200B;]**」。]**

在&#x200B;**[!UICONTROL 一般設定]**&#x200B;區域中，選擇是要產生視訊網站地圖、mRSS饋送，還是兩者。 在&#x200B;**[!UICONTROL 「層代設定」]**&#x200B;區域中，將元資料欄位映射到輸入欄位。

選擇設定後，按一下「儲存」(**[!UICONTROL Save]**)(或&#x200B;**[!UICONTROL 「儲存並產生」(]**)以建立視訊網站地圖、mRSS饋送或兩者。

### 選擇一般設定 {#choosing-general-settings}

在&#x200B;**[!UICONTROL 產生模式]**&#x200B;下拉式清單中，選擇報表模式：

* **視訊網站地圖** -建立視訊網站地圖。

* **mRSS饋送** -建立媒體RSS(mRSS)饋送。

* **兩者** -建立這兩種XML檔案。

* **關閉** -若要停止產生視訊網站地圖和媒體RSS(mRSS)饋送，請選擇此選項。

在&#x200B;**[!UICONTROL 自動／手動模式]**&#x200B;下拉式清單中，選擇自動或手動產生：

* **自動模式** -Dynamic Media經典網站每天自動產生一個視訊網站地圖、媒體RSS(mRSS)饋送，或兩者。選擇「標籤為發佈」選項，以自動標籤為發佈Dynamic Media·Classic生成的XML檔案。

   * **標籤為** PublishMarks以發佈所產生的XML檔案。

* **手動模式** -在「視訊搜尋最佳化設定」畫面中按一下「產生」或「儲存並產生」時，Dynamic Media經典會產生視訊網站地圖、媒體RSS(mRSS)饋送或兩者。同時，也請選擇這些選項:

   * **無進一步設定** -不標籤為發佈所產生的XML檔案。

   * **標籤為發佈** -標籤為發佈生成的XML檔案。

   * **允許部分產生** -如果XML檔案未包含所有視訊的完整中繼資料資訊，搜尋引擎可以拒絕它。即使部分視訊沒有中繼資料，此選項也會產生 XML 檔案。警告會登錄在「報告」畫面上。如果您要匯出 XML 檔案並手動處理遺失的資訊，請選擇此選項。

### 選擇產生設定 {#choosing-generation-settings}

「層代設定」區域會列出視訊網站地圖或mRSS饋送的輸入欄位，或兩者皆列出，而中繼資料面板中則會列出中繼資料欄位的名稱。 使用「一般設定」區域，即可將輸入欄位對應至中繼資料欄位。如此一來，您就會告訴Dynamic MediaClassic如何取得視訊網站地圖和／或mRSS饋送的中繼資料。

1. 在「中繼資料檢視」選單上選擇中繼資料檢視。選擇檢視後，中繼資料欄位的名稱便會顯示在「中繼資料」面板中。請參閱[中繼資料檢視](application-setup.md#metadata_views)。
1. 將中繼資料欄位名稱從「中繼資料」面板拖曳至「登陸頁面」、「標題」、「描述」、「標籤」和「類別」輸入欄位。「登陸頁面」、「標題」和「描述」欄位為必填。

   >[!NOTE]
   >
   >您也可以手動將資料輸入至輸入欄位。

1. 進行以下一項操作:

   * 要保存設定而不生成XML檔案，請按一下「保存」。****
   * 若要儲存並產生檔案，請按一下「儲存並產生&#x200B;**[!UICONTROL 」。]**

      XML 檔案會產生並記錄在工作記錄檔中。視訊網站地圖 (video-sitemap) 和媒體 RSS (mRSS) 新聞頻道 (mrss-feed) 檔案會儲存在公司的根檔案夾中。

>[!NOTE]
>
>先發佈視訊網站地圖或mRSS饋送，再將它送出至搜尋引擎。 視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中。如有必要，請標籤這些XML檔案以進行發佈，然後按一下「**[!UICONTROL 發佈]**」。

## 將視訊網站地圖和 mRSS 新聞頻道檔案送出至搜尋引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

將上述其中一個 URL 複製到搜尋引擎的站長工具，即可將您的視訊網站地圖或媒體 RSS (mRSS) 新聞頻道檔案送出至搜尋引擎。

## 檢視視訊 SEO 報告  {#viewing-video-seo-reports}

在「視訊搜尋引擎最佳化報表」頁面上檢視視訊搜尋引擎最佳化報表。 若要開啟此頁面，請在全域導覽列上按一下「設定&#x200B;**** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊搜尋引擎最佳化(SEO)>**[!UICONTROL &#x200B;報表&#x200B;]**」。]**

如果產生報表時發生錯誤，則會列在「報表」頁面上。
