---
title: Publish檔案
description: 瞭解如何將資產發佈至Dynamic Media影像伺服器。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# Publish檔案{#publishing-files}

您將資產發佈至Dynamic Media影像伺服器。 您可以單次發佈資產，或安排Adobe Dynamic Media Classic按照週期性排程發佈資產。 發佈資產後，這些資產即可用來傳送。您可以複製Adobe Dynamic Media Classic的URL呼叫，並將其新增至您的網站或應用程式。

Adobe Dynamic Media Classic現在支援透過HTTP/2傳送所有影像和視訊。 也就是說，影像或視訊的已發佈URL或內嵌程式碼可整合至任何接受託管資產的應用程式。 該已發佈資產使用HTTP/2通訊協定來傳送。 此傳送方式可改善瀏覽器和伺服器的通訊方式，讓您的所有Adobe Dynamic Media Classic資產獲得更好的回應和載入時間。 請參閱[HTTP2傳送內容常見問答集](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-65/content/assets/dynamic/http2)。

## 上載後發佈 {#publish-after-uploading}

資產狀態一定是「已發佈」或「未發佈」。依預設，您上傳至Adobe Dynamic Media Classic的任何資產都會自動標示為發佈。

如需詳細資訊，請參閱[即時Publish通知PDF](/help/using/assets/rendering-instant-publish-notification.pdf)。

使用這些技巧來標籤要發佈的資產：

* **[!UICONTROL 上傳後的Publish]**：在上傳頁面上，靠近底部，選取&#x200B;**[!UICONTROL 上傳後的Publish]**。 預設狀態是已選取。

* **[!UICONTROL 上傳後的Publish]**：在[工作選項]對話方塊中，選取[上傳後的&#x200B;**[!UICONTROL Publish]]**。 預設狀態是已選取。

如果父項資產標記為發佈，則某些「子項」資產會自動標記為發佈。此表格列出自動標示為要發佈的子資產。

| 父項 (群組) 項目 | 子項 (成員) 項目 |
| --- | --- |
| 影像集 | 集內的影像。 |
| 色票集 | 集內的色票。 |
| 迴轉集 | 集內的影像。 |
| 範本 | 範本檔案、頁面和影像。 |

衍生影像在發佈其父影像時，也會自動標示為發佈。 衍生影像包括您使用影像編輯選項調整的影像。您可以在「建置和衍生物」下的「詳細檢視」中看到這些衍生影像。

## 建立發佈工作 {#creating-a-publish-job}

建立發佈工作以發佈您已上傳至Adobe Dynamic Media Classic伺服器，但尚未自動發佈的資產。 您可以執行一次性發佈工作或排程定期重複的工作。 Adobe Dynamic Media Classic提供進階發佈選項，可用於發佈至特定伺服器，以及重新發佈已發佈資產的選項。

**若要建立發佈工作：**

1. 在全域導覽列上，選取&#x200B;**[!UICONTROL Publish]**。
1. 在「發佈」對話方塊中，選擇您要單次或循環發佈工作。

   請參閱[建立一次性發佈工作](publishing-files.md#creating_a_one_time_publish_job)和[建立循環發佈工作](publishing-files.md#creating_a_recurring_publish_job)。

1. 輸入工作名稱。
1. 或者，顯示「進階」選項並選擇這些選項。

   請參閱[進階發佈選項](publishing-files.md#advanced_publish_options)。

1. 選取&#x200B;**[!UICONTROL 提交Publish]**。

Adobe Dynamic Media Classic會追蹤「工作」頁面上的發佈工作。 您可以在該頁面上檢閱發佈工作。

>[!NOTE]
>
>您重新發佈的Assets （之前已發佈）不會立即出現在您的網站上，因為內容傳遞網路(CDN)上有網頁快取機制。 請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 建立一次性發佈工作 {#creating-a-one-time-publish-job}

在[發佈]頁面上選取&#x200B;**[!UICONTROL 一次性]**&#x200B;選項，以建立一次性的發佈工作。

如果您希望發佈工作稍後進行，請在[發佈]頁面中選取&#x200B;**[!UICONTROL 單次]**。 從下拉式清單中，選取&#x200B;**[!UICONTROL 排程稍後]**。 使用「行事曆」和「時間」滑桿來選取執行發佈工作的日期和時間。

### 建立週期性發佈工作 {#creating-a-recurring-publish-job}

在[發佈]頁面上選取&#x200B;**[!UICONTROL Recurring]**，以建立循環發佈工作。

接著選擇&#x200B;**[!UICONTROL 每日]**、**[!UICONTROL 每週]**、**[!UICONTROL 每月]**&#x200B;或&#x200B;**[!UICONTROL 自訂]**&#x200B;重複選項，然後指定您要發佈工作重複的時間。 Adobe Dynamic Media Classic提供用於排程週期性發佈工作的行事曆工具。 您可以選取&#x200B;**[!UICONTROL 自訂]**&#x200B;選項，並在「規則」文字欄位中輸入規則來說明自訂工作間隔。

請參閱[建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)。

>[!NOTE]
>
>在「工作」頁面上會列出週期性發佈 (和上載) 工作。前往「工作」頁面的「已排程」標籤，可以編輯或刪除排程的工作。

### 進階發佈選項 {#advanced-publish-options}

您可以在「發佈」頁面上顯示「進階」選項，並選擇這些選項來處理發佈工作：

* **[!UICONTROL Publish To]**：若要僅將資產發佈至特定伺服器，請選擇伺服器型別。

* **[!UICONTROL Publish]**：依預設，Adobe Dynamic Media Classic只會發佈新資產，而且是以前未發佈的資產(上次使用Publish後新增的選項)。 不過，您可以選取&#x200B;**[!UICONTROL 完整Publish]**，這樣您也可以發佈自上次發佈以來已更新或變更的資產。 如果您要發佈eCatalog且希望讀者能依關鍵字進行搜尋，請選取&#x200B;**[!UICONTROL 完整包含搜尋資料]**。

* **[!UICONTROL 以]**&#x200B;執行工作：從清單中選擇使用者名稱。 可以在「工作」頁面上依使用者名稱排序工作。透過選擇名稱，您可以將發佈工作與使用者建立關聯。

**[!UICONTROL HTTP通知]**：輸入URL以觸發後續的發佈工作。

請參閱[使用上載或發佈工作做為觸發程式](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)。)

## 取消發佈工作 {#canceling-a-publish-job}

您可以取消進行中的發佈工作。 此外，管理員還可以透過公司的「工作」頁面取消進行中的發佈工作。

若要取消發佈工作，請移至[工作]頁面並選取[取消]。**&#x200B;** 在「工作」頁面的「已排程」頁簽中，您可以取消選取或選取工作之「作用中」資料欄中的核取方塊，來暫停或繼續工作。

>[!NOTE]
>
>取消發佈工作後，其狀態會變更為「正在停止」，直到工作達到可以安全停止的時間點為止。 如果發佈工作正在從資料庫取得資料，則停止發佈工作可能需要一些時間。

## 手動Publish資產 {#manually-publishing-assets}

您可以手動發佈個別資產，而不是建立發佈工作。當您發佈影像集或最適化視訊集等集時，集（或「父項」）與該集內的所有成員（或「子項」）都會發佈。

未發佈的資產會在使用者介面中以灰色圓形圖示表示，在資產名稱的左側會有斜線（未發佈狀態）。 發佈資產之後，圖示會變成綠色，並且在中心會有白色的勾選記號 (發佈的狀態)。

**若要手動發佈資產：**

1. 進行以下一項操作:

   * 在格點檢視、清單檢視或詳細資訊檢視中，用標準檔案選取方法來選取一或多個未發佈的資產。

     在全域導覽列上，前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL Publish]**。

   * 在「格點檢視」、「清單檢視」或「詳細資料檢視」中，選取資產名稱左邊具有斜線的灰色圓形圖示。

## 手動取消發佈資產 {#manually-unpublishing-assets}

您可以手動取消發佈個別資產。當您取消發佈色票集或eCatalog等色票集時，該集（或「父項」）本身會進入取消發佈狀態。 不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

已發佈的資產會在使用者介面中以綠色圓形圖示表示，中央會有白色勾號（已發佈狀態），位於資產名稱左側。 取消發佈資產後，圖示會變成灰色，並加上斜線（取消發佈狀態）。

**若要手動取消發佈資產：**

1. 進行以下一項操作:

   * 在「網格檢視」、「清單檢視」或「詳細資料檢視」中，選取一或多個已發佈的資產。

     在全域導覽列上，前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 取消發佈]**。

   * 在「格點檢視」、「清單檢視」或「詳細資料檢視」中，選取資產名稱左側的圓形綠色勾號圖示。

## 取得資產的發佈歷史記錄 {#getting-an-asset-s-publish-history}

資產上次發佈的日期會顯示在「詳細資料檢視」的面板頂端。 您可以在「詳細資訊」檢視中開啟「歷程記錄和已發佈的伺服器」面板，以取得有關發佈歷程記錄的詳細資訊。 在該面板中可以查看資產發佈時間以及發佈的目標伺服器。

## 重新發佈的資產和 CDN 延遲 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic資產在內容傳遞網路(CDN)上分發。 CDN 是指聯成網路的電腦伺服器系統，這些伺服器以完全無障礙地的方式合作，將內容 (尤其是大型媒體內容) 傳送給終端使用者。在CDN系統中，網頁內容會儲存在網際網路上的網頁快取中（稱為邊緣快取網路）。 網頁內容會從網頁快取傳送給一般使用者，以加快傳送速度。

第一次下載網頁時，資產會傳送到CDN網頁快取伺服器。 此伺服器會儲存這些快取內容，以便下次同一區域中的某人存取網頁時，相同快取內容可以更快傳送。 內容傳送速度更快是因為其位置更接近終端使用者。CDN可加快網頁顯示速度。 它降低了中央伺服器上的頻寬要求，因為內容是從邊緣快取網路傳送，而不是從每個實體的中央伺服器傳送。

使用者可立即取得新發佈的Adobe Dynamic Media Classic內容，並快速填入邊緣快取網路。 然而，新重新發佈的內容（即名稱與先前發佈至影像伺服器的影像相同的影像）在CDN上最多十小時內不會更新。 一般使用者會看到CDN網路上網頁快取的內容。 因此，您的Adobe Dynamic Media Classic重新發佈資產不會在十小時內向一般使用者顯示。

如果您希望新重新發佈的影像資產在十小時延遲前就可供使用，您可以清除CDN上的網路快取。 清除這些網頁快取會從CDN網頁快取中移除舊內容，並將其取代為您最近發佈的資產。

若要清除快取，請在全域導覽列上，前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 使CDN失效]**。 所有已選取的檔案會從快取中移除。如果沒有可發佈資產，或者您不是公司管理員，則「從 CDN 移除」選項不可用。

>[!MORELIKETHIS]
>
>* [檢查工作檔案](checking-job-files.md)
>* [編輯、刪除、暫停並繼續週期性工作](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
