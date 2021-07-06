---
title: 發佈檔案
description: 「了解如何將資產發佈至Dynamic Media影像伺服器。 您可以一次性發佈資產，或安排Dynamic Media Classic定期發佈資產。 發佈資產後，這些資產即可用來傳送。您可以從Dynamic Media Classic複製URL呼叫，並將其新增至您的網站或應用程式。」
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic，資產管理
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1712'
ht-degree: 59%

---

# 發佈檔案{#publishing-files}

您將資產發佈至Dynamic Media影像伺服器。 您可以一次性發佈資產，或安排Dynamic Media Classic定期發佈資產。 發佈資產後，這些資產即可用來傳送。您可以從Dynamic Media Classic複製URL呼叫，並將其新增至您的網站或應用程式。

Dynamic Media Classic現在支援透過HTTP/2傳送所有影像和視訊。 也就是說，影像或視訊的已發佈URL或內嵌程式碼可與接受託管資產的任何應用程式整合。 然後會透過HTTP/2通訊協定來傳送已發佈的資產。 此傳遞方法可改善瀏覽器和伺服器通訊的方式，讓所有Dynamic Media Classic資產的回應和載入時間都更佳。 請參閱[HTTP2內容傳送常見問題集](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic)。

## 上載後發佈 {#publish-after-uploading}

資產狀態一定是「已發佈」或「未發佈」。依預設，您上傳至Dynamic Media Classic的任何資產都會自動標示為要發佈。

如需詳細資訊，請參閱[即時發佈通知PDF](/help/assets/rendering-instant-publish-notification.pdf)。

使用以下方法將資產標記為發佈:

* **上傳後發佈**  — 在「上傳」頁面底部附近，選取「上傳後發佈」。預設狀態是已選取。

* **上傳後發佈**  — 在「工作選項」對話方塊中，選取「上傳後發佈」。預設狀態是已選取。

如果父項資產標記為發佈，則某些「子項」資產會自動標記為發佈。該表格列出自動標記為發佈的子項資產。

| 父項 (群組) 項目 | 子項 (成員) 項目 |
|--- |--- |
| 影像集 | 集內的影像。 |
| 色票集 | 集內的色票。 |
| 迴轉集 | 集內的影像。 |
| 範本 | 範本檔案、頁面和影像. |

發佈衍生影像的父項影像時，衍生影像也會自動標示為發佈。衍生影像包括您使用影像編輯選項調整的影像。您可以在「建立和衍生物」下的詳細檢視中查看這些衍生影像。

## 建立發佈工作 {#creating-a-publish-job}

建立發佈工作以發佈您已上傳至Dynamic Media Classic伺服器的資產，但選擇尚未自動發佈資產。 您可以執行一次性發佈作業，或排程作業定期重複執行。 Dynamic Media Classic提供進階發佈選項，可發佈至特定伺服器，以及重新發佈已發佈資產的選項。

**建立發佈工作:**

1. 在「全域導覽」列上按一下「**[!UICONTROL 發佈]**」。
1. 在「發佈」對話框中，選擇一次性或週期性發佈工作。

   請參閱[建立一次性發佈工作](publishing-files.md#creating_a_one_time_publish_job)和[建立週期性發佈工作](publishing-files.md#creating_a_recurring_publish_job)。

1. 輸入工作名稱。
1. 或者，顯示「進階」選項並選擇這些選項。

   請參閱[進階發佈選項](publishing-files.md#advanced_publish_options)。

1. 按一下「**[!UICONTROL 送出發佈]**」。

Dynamic Media Classic會追蹤「工作」頁面上的發佈工作。 您可以在該頁面上檢閱發佈工作。

>[!NOTE]
>
>由於內容傳遞網路 (CDN) 上的網路快取機制，您重新發佈的資產 (以前曾經發佈) 並不會立即顯示在網站上。請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 建立一次性發佈工作 {#creating-a-one-time-publish-job}

在「發佈」頁面上選取「一次性」選項，建立一次性發佈工作。

如果您希望發佈作業稍後發生，請在「發佈」頁面中，選擇「**[!UICONTROL 一次性]**」，然後按一下「**[!UICONTROL 稍後計畫]**」下拉式清單。 使用日曆和時間滑桿來選擇運行發佈作業的日期和時間。

### 建立週期性發佈工作 {#creating-a-recurring-publish-job}

在「發佈」頁面上選取&#x200B;**[!UICONTROL Recurring]**，以建立循環發佈作業。

然後選擇「重複」選項&#x200B;**[!UICONTROL Daily]**、**[!UICONTROL Weekly]**、**[!UICONTROL Monthly]**&#x200B;或&#x200B;**[!UICONTROL Custom]**，然後指定要重複發佈作業的時間。 Dynamic Media Classic提供日曆工具，可排程週期性發佈工作。 您可以按一下&#x200B;**[!UICONTROL Custom]**&#x200B;選項，並在「規則」文本欄位中輸入規則，以說明自定義作業間隔。

請參閱[建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)。

>[!NOTE]
>
>在「工作」頁面上會列出週期性發佈 (和上載) 工作。前往「工作」頁面的「已排程」標籤，可以編輯或刪除排程的工作。

### 進階發佈選項 {#advanced-publish-options}

您可以在「發佈」頁面上顯示「進階」選項，並選擇這些選項來處理發佈工作: 

* **發佈至**  — 若要僅將資產發佈至特定伺服器，請選擇伺服器類型。

* **發佈**  — 依預設，Dynamic Media Classic只會發佈之前未發佈的新資產（上次發佈後新增的選項）。不過，您可以按一下「**[!UICONTROL 完整發佈]**」，也可以發佈自上次發佈以來已更新或變更的資產。 如果要發佈eCatalog且希望讀者能夠按關鍵字搜索，請選擇&#x200B;**[!UICONTROL 包含搜索資料的完整]**。

* **運行方式**  — 從清單中選擇用戶名。可以在「工作」頁面上依使用者名稱排序工作。可以透過選擇名稱將發佈工作與使用者建立關聯。

**HTTP通知**  — 輸入URL以觸發後續的發佈作業。

請參閱[使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)。)

## 取消發佈工作 {#canceling-a-publish-job}

您可以取消進行中的發佈工作。此外，管理員還可以透過公司的「工作」頁面取消進行中的發佈工作。

要取消發佈作業，請轉至「作業」頁，然後按一下&#x200B;**[!UICONTROL 取消]**。 在「工作」頁面的「已排程」標籤上，您可以取消選取或選取工作的「作用中」欄內之核取方框，以暫停或繼續工作。

>[!NOTE]
>
>取消發佈工作之後，其狀態變更為「正在停止」，直至達到一個安全的停止點。如果工作正從資料庫取得資料，則停止發佈工作可能會花費一些時間。

## 手動發佈資產 {#manually-publishing-assets}

您可以手動發佈個別資產，而不是建立發佈工作。發佈集 (例如影像集或最適化視訊集) 時，將會發佈該集內的集 (或稱為「父項」) 和所有成員 (或稱為「子項」)。

取消發佈的資產在使用者介面中會以灰色的圓形圖示表示，並透過該圖示（取消發佈狀態），位於資產名稱左側。 發佈資產之後，圖示會變成綠色，並且在中心會有白色的勾選記號 (發佈的狀態)。

**手動發佈資產:**

1. 進行以下一項操作:

   * 在格點檢視、清單檢視或詳細資訊檢視中，用標準檔案選取方法來選取一或多個未發佈的資產。

      在全域導覽列上，按一下「**[!UICONTROL 檔案]** >**[!UICONTROL 發佈]**」。

   * 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，按一下資產名稱左側帶斜線的灰色倒圓角表徵圖。

## 手動取消發佈資產 {#manually-unpublishing-assets}

您可以手動取消發佈個別資產。取消發佈集時，例如色票集或 eCatalog，集 (或稱為「父項」) 本身會變成未發佈狀態。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

在使用者介面中，發佈的資產會在資產名稱左側以中心帶有白色勾選記號的綠色圓形圖示指出 (發佈的狀態)。取消發佈資產後，圖示會以斜線穿過資產變成灰色（取消發佈狀態）,

**手動取消發佈資產:**

1. 進行以下一項操作:

   * 在「格線檢視」、「清單檢視」或「詳細資料檢視」中，選取一或多個已發佈的資產。

      在全域導覽列上，按一下「**[!UICONTROL 檔案]** >**[!UICONTROL 未發佈]**」。

   * 在格點檢視、清單檢視或詳細資訊檢視中，按一下資產名稱左側的綠色圓形勾選記號圖示。

## 取得資產發佈操作記錄 {#getting-an-asset-s-publish-history}

資產上次發佈的日期顯示在面板頂部的詳細檢視中。您可以開啟詳細檢視中的「操作記錄和已發佈的伺服器」面板，取得關於發佈操作記錄的更多詳細資訊。在該面板中可以查看資產發佈時間以及發佈的目標伺服器。

## 重新發佈的資產和 CDN 延遲 {#republished-assets-and-cdn-delays}

Dynamic Media Classic資產是在內容傳遞網路(CDN)上分發。 CDN 是指聯成網路的電腦伺服器系統，這些伺服器以完全無障礙地的方式合作，將內容 (尤其是大型媒體內容) 傳送給終端使用者。在 CDN 系統中，網路內容儲存在整個網際網路的網路快取中 (稱為邊緣快取網路)。Web內容會從Web快取傳送給使用者，以加快傳遞速度。

使用者首次下載網頁時，這些資產即傳送到 CDN 網路快取伺服器。資產儲存在該伺服器上，當下次同一區域中有人存取該網頁時，可以更快地傳送快取的相同內容。內容傳送速度更快是因為其位置更接近終端使用者。CDN 提高了網頁顯示速度。它降低了中央伺服器上的頻寬要求，因為內容是從邊緣快取網路傳送，而不是從每個實體的中央伺服器傳送。

新發佈的Dynamic Media Classic內容可立即供一般使用者使用，並快速填入邊緣快取網路。 但重新發佈的內容 (與之前發佈到影像伺服器的影像完全同名的影像) 需要長達十個小時之後才會在 CDN 上更新。終端使用者看到的則是 CDN 網路上網路快取中的內容。因此，您的Dynamic Media Classic重新發佈的資產在10小時內不會對使用者顯示。

如果希望重新發佈的影像資產在可用前的延遲時間小於十個小時，可以清空 CDN 上的網路快取。清空這些網路快取可以從 CDN 網路快取中移除舊內容，並將其取代為最新發佈的資產。

若要排清快取，請在全域導覽列上按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 使CDN]**&#x200B;無效」。 所有已選取的檔案會從快取中移除。如果沒有可發佈資產，或者您不是公司管理員，則「從 CDN 移除」選項不可用。

>[!MORELIKETHIS]
>
>* [檢查工作檔案](checking-job-files.md)
* [編輯、刪除、暫停和繼續週期性工作](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

