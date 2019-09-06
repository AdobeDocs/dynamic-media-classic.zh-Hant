---
title: 視訊 SEO (搜尋引擎最佳化)
seo-title: 視訊 SEO (搜尋引擎最佳化)
description: 'null'
seo-description: 瞭解如何設定視訊SEO設定。
uuid: bac2c6a9-8466-4b8f-b835-6cb0 b4168513
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/類別/設定
discoiquuid: 34d868-775f-452b-b26 e-d139 f0 e280 ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# 視訊 SEO (搜尋引擎最佳化){#video-seo-search-engine-optimization}

SEO 是改善來自搜尋引擎之網站流量的程序。雖然搜尋引擎擅於收集以文字為基礎之內容的相關資訊，但除非向其提供此資訊，否則也無法充分取得視訊相關資訊。

使用Dynamic Media Classic Video SEO，您可以運用視訊中繼資料來提供搜尋引擎，並提供視訊說明。Dynamic Media Classic可建立視訊網站地圖和MMR饋送。下列為標準 XML 檔案，可用來將視訊資訊送出至搜尋引擎:

**視訊網站地圖** 會精確告知Google視訊內容在網站上的位置和位置。因此，您完全可以在 Google 上搜尋視訊。例如，視訊網站地圖可以指出視訊的執行時間和類別。如需有關視訊網站地圖的詳細資訊，請參閱https://www.google.com/support/webmasters/bin/answer.py?answer=80471。

**內容發佈者使用的MRS(Media True Simple Syndication)摘要** 內容出版業者將媒體檔案傳送至Yahoo！視訊搜尋。如需MMR饋送的詳細資訊，請參閱https://www.rssboard.org/media-rss。

>[!NOTE]
>
>Google 同時支援視訊網站地圖和 mRSS 新聞頻道通訊協定，可用來送出資訊至搜尋引擎。

Dynamic Media Classic可從每個視訊儲存的中繼資料產生視訊網站地圖和MMR饋送。建立視訊網站地圖和 mRSS 新聞頻道後，請決定要包含哪些中繼資料欄位來自視訊檔案。這樣，您可以向搜尋引擎描述視訊，以便搜尋引擎能夠更精確地將流量引導至您網站上的視訊。

>[!NOTE]
>
>在建立視訊網站地圖或 mRSS 新聞頻道前，請先確定搜尋引擎需要 XML 檔案中的哪些欄位，以及如何建立這些欄位的結構。若要建立成功的視訊網站地圖或 mRSS 新聞頻道，它必須符合搜尋引擎的要求。

動態媒體Classic會在您產生視訊網站地圖和MMR摘要後建立報表。您可以在「視訊 SEO 報告」畫面取得這些報告。

>[!NOTE]
>
>對於視訊網站地圖和MMR摘要，Dynamic Media Classic只會擷取標記為發佈的影片。將視訊標記為發佈，即可將其中繼資料包含於視訊網站地圖和 mRSS 新聞頻道中。

## Choosing video SEO settings {#choosing-video-seo-settings}

在「視訊搜尋引擎最佳化設定」畫面上，為視訊網站地圖和 mRSS 新聞頻道選擇「Video SEO」設定。若要開啟此畫面，請選擇「設定 &gt; 應用程式設定 &gt; 視訊 SEO &gt; 設定」。

在「一般設定」區域中選擇要產生視訊網站地圖、mRSS 新聞頻道或同時產生兩者。在「一般設定」區域中，將中繼資料欄位對應至輸入欄位。

選擇設定後，請按一下「產生」(或「儲存並產生」) 以建立視訊網站地圖、mRSS 新聞頻道或同時建立兩者。

### 選擇一般設定 {#choosing-general-settings}

在「產生模式」下拉式清單上選擇報告模式:

**視訊網站地圖** 建立視訊網站地圖。

**MRS饋送** 建立媒體RSS(MRS)摘要。

**兩者** 皆可建立兩種XML檔案。

**關閉** 選擇此選項以停止產生視訊網站地圖和媒體RSS(MRS)饋送。

在「自動/手動模式」下拉式清單中，選擇要自動或手動產生:

**自動模式** 動態媒體Classic會每天自動產生一個視訊網站地圖、媒體RSS(MRS)饋送或兩者。選擇「標記為發佈」選項，自動標示發佈Dynamic Media Classic產生之XML檔案的標記。

**當您在「視訊搜尋最佳化設定」畫面中按一下「產生或儲存並產生」時，手動模式** 動態媒體Classic會產生視訊網站地圖、媒體RSS(MRS)饋送或兩者。同時，也請選擇這些選項:

**「不進一步設定** 」不會標記發佈的XML檔案。

**標記發佈** 標記以發佈產生的XML檔案。

**如果部分產生** 的搜尋引擎未包含所有影片的完整中繼資料資訊，則允許「部分產生」搜尋引擎。即使部分視訊沒有中繼資料，此選項也會產生 XML 檔案。警告會登錄在「報告」畫面上。如果您要匯出 XML 檔案並手動處理遺失的資訊，請選擇此選項。

### 選擇產生設定 {#choosing-generation-settings}

「產生設定」區域會列出視訊網站地圖和/或 mRSS 新聞頻道的輸入欄位，並在「中繼資料」面板中列出中繼資料欄位名稱。使用「一般設定」區域，即可將輸入欄位對應至中繼資料欄位。這麼做，您會告訴Dynamic Media Classic，在其中取得視訊網站地圖和/或MMR饋送的中繼資料。

1. 在「中繼資料檢視」選單上選擇中繼資料檢視。選擇檢視後，中繼資料欄位的名稱便會顯示在「中繼資料」面板中。(如需有關中繼資料檢視的資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views)。)
1. 將中繼資料欄位名稱從「中繼資料」面板拖曳至「登陸頁面」、「標題」、「描述」、「標籤」和「類別」輸入欄位。「登陸頁面」、「標題」和「描述」欄位為必填。

   >[!NOTE]
   >
   >您也可以手動將資料輸入至輸入欄位。

1. 按一下「儲存」(儲存設定而不產生 XML 檔案)、「產生」(產生 XML 檔案) 或「儲存並產生」(儲存並產生檔案)。

   XML 檔案會產生並記錄在工作記錄檔中。視訊網站地圖 (video-sitemap) 和媒體 RSS (mRSS) 新聞頻道 (mrss-feed) 檔案會儲存在公司的根檔案夾中。

>[!NOTE]
>
>您必須先發佈視訊網站地圖或 mRSS 新聞頻道，才能將其送出至搜尋引擎。視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中。如有需要，請將這些 XML 檔案標記為發佈，並按一下「發佈」。

## 將視訊網站地圖和 mRSS 新聞頻道檔案送出至搜尋引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

視訊網站地圖和媒體 RSS (mRSS) 新聞頻道檔案儲存於公司的根檔案夾中:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

將上述其中一個 URL 複製到搜尋引擎的站長工具，即可將您的視訊網站地圖或媒體 RSS (mRSS) 新聞頻道檔案送出至搜尋引擎。

## 檢視視訊 SEO 報告 {#viewing-video-seo-reports}

在「視訊搜尋引擎最佳化報告」畫面上檢視視訊 SEO 報告。若要開啓此畫面，請按一下「設定&gt;應用程式設定&gt;視訊SEO&gt;報表」。

如果在報告產生時發生錯誤，則會在「報告」畫面上列出錯誤。
