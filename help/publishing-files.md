---
title: 發佈檔案
description: 「瞭解如何將資產發佈到Dynamic Media映像伺服器。 您可以一次性發佈資產，或安排Adobe Dynamic Media Classic按經常性計畫發佈資產。 發佈資產後，這些資產即可用來傳送。您可以從Adobe Dynamic Media Classic複製URL呼叫，並將其添加到您的網站或應用程式。」
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: f0e6d634587500877dbcd9e56bcfca105a6e6b9b
workflow-type: tm+mt
source-wordcount: '1726'
ht-degree: 48%

---

# 發佈檔案{#publishing-files}

您將資產發佈到Dynamic Media映像伺服器。 您可以一次性發佈資產，或安排Adobe Dynamic Media Classic按經常性計畫發佈資產。 發佈資產後，這些資產即可用來傳送。您可以複製來自Adobe Dynamic Media Classic的URL呼叫，並將它們添加到您的網站或應用程式。

Adobe Dynamic Media Classic現在支援通過HTTP/2傳輸所有影像和視頻。 即，可將影像或視頻的已發佈URL或嵌入代碼與接受託管資產的任何應用程式整合。 然後，該已發佈資產將通過HTTP/2協定交付。 這種傳送方法改進了瀏覽器和伺服器之間的通信方式，使您的所有Adobe Dynamic Media Classic資產都能得到更好的響應和載入時間。 請參閱 [HTTP2內容傳送常見問題](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic)。

## 上載後發佈 {#publish-after-uploading}

資產狀態一定是「已發佈」或「未發佈」。預設情況下，您上傳到Adobe Dynamic Media Classic的任何資產都會自動標籤為要發佈。

有關詳細資訊，請參見 [即時發佈通知PDF](/help/assets/rendering-instant-publish-notification.pdf)。

使用以下方法將資產標記為發佈:

* **[!UICONTROL 上載後發佈]**  — 在「上載」頁面底部附近，選擇 **[!UICONTROL 上載後發佈]**。 預設狀態是已選取。

* **[!UICONTROL 上載後發佈]**  — 在「作業選項」對話框中，選擇 **[!UICONTROL 上載後發佈]**。 預設狀態是已選取。

如果父項資產標記為發佈，則某些「子項」資產會自動標記為發佈。該表格列出自動標記為發佈的子項資產。

| 父項 (群組) 項目 | 子項 (成員) 項目 |
| --- | --- |
| 影像集 | 集內的影像。 |
| 色票集 | 集內的色票。 |
| 迴轉集 | 集內的影像。 |
| 範本 | 範本檔案、頁面和影像。 |

發佈衍生影像的父項影像時，衍生影像也會自動標示為發佈。衍生影像包括您使用影像編輯選項調整的影像。您可以在「構建和衍生」下的「詳細視圖」中查看這些派生影像。

## 建立發佈作業 {#creating-a-publish-job}

建立發佈作業以發佈已上載到Adobe Dynamic Media Classic伺服器的資產，但不想自動發佈這些資產。 您可以執行一次性發佈作業或計畫定期重複的作業。 Adobe Dynamic Media Classic公司提供高級發佈選項，用於發佈到特定伺服器，以及重新發佈已發佈的資產。

**建立發佈工作:**

1. 在全局導航欄上，選擇 **[!UICONTROL 發佈]**。
1. 在「發佈」對話框中，選擇一次性或週期性發佈工作。

   請參閱 [建立一次性發佈作業](publishing-files.md#creating_a_one_time_publish_job) 和 [建立定期發佈作業](publishing-files.md#creating_a_recurring_publish_job)。

1. 輸入工作名稱。
1. 或者，顯示「進階」選項並選擇這些選項。

   請參閱[進階發佈選項](publishing-files.md#advanced_publish_options)。

1. 選擇 **[!UICONTROL 提交發佈]**。

Adobe Dynamic Media Classic跟蹤「工作」頁面上的發佈工作。 您可以在該頁面上檢閱發佈工作。

>[!NOTE]
>
>由於內容傳遞網路 (CDN) 上的網路快取機制，您重新發佈的資產 (以前曾經發佈) 並不會立即顯示在網站上。請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 建立一次性發佈作業 {#creating-a-one-time-publish-job}

通過選擇 **[!UICONTROL 一次性]** 的子菜單。

如果希望以後發佈作業，請在「發佈」頁中選擇 **[!UICONTROL 一次性]**，然後選擇 **[!UICONTROL 計畫以後]** 下拉。 使用日曆和時間滑塊選擇運行發佈作業的日期和時間。

### 建立定期發佈作業 {#creating-a-recurring-publish-job}

通過選擇 **[!UICONTROL 循環]** 的子菜單。

然後選擇「重複」選項 **[!UICONTROL 每日]**。 **[!UICONTROL 每週]**。 **[!UICONTROL 每月]**&#x200B;或 **[!UICONTROL 自定義]**，然後指定要重複發佈作業的時間。 Adobe Dynamic Media Classic提供日曆工具，用於安排定期發佈作業。 可以選擇 **[!UICONTROL 自定義]** 選項，並在規則文本欄位中輸入規則以描述自定義作業間隔。

請參閱 [建立自定義上載或發佈作業時間間隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)。

>[!NOTE]
>
>在「工作」頁面上會列出週期性發佈 (和上載) 工作。前往「工作」頁面的「已排程」標籤，可以編輯或刪除排程的工作。

### 進階發佈選項 {#advanced-publish-options}

您可以在「發佈」頁面上顯示「進階」選項，並選擇這些選項來處理發佈工作: 

* **[!UICONTROL 發佈到]**  — 要僅將資產發佈到特定伺服器，請選擇伺服器類型。

* **[!UICONTROL 發佈]**  — 預設情況下，Adobe Dynamic Media Classic僅發佈以前未發佈的新資產（「自上次發佈後新建」選項）。 但是，您可以選擇 **[!UICONTROL 完全發佈]** 還要發佈自上次發佈以來已更新或更改的資產。 選擇 **[!UICONTROL 包含搜索資料的完整]** 如果您正在發佈eCatalog，並且希望讀者能夠按關鍵字搜索它。

* **[!UICONTROL 作業運行方式]**  — 從清單中選擇用戶名。 可以在「工作」頁面上依使用者名稱排序工作。可以透過選擇名稱將發佈工作與使用者建立關聯。

**[!UICONTROL HTTP通知]**  — 輸入URL以觸發後續發佈作業。

請參閱 [將上載或發佈作業用作觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)。)

## 取消發佈作業 {#canceling-a-publish-job}

您可以取消進行中的發佈工作。此外，管理員還可以透過公司的「工作」頁面取消進行中的發佈工作。

要取消發佈作業，請轉到「作業」頁並選擇 **[!UICONTROL 取消]**。 在「工作」頁面的「已排程」標籤上，您可以取消選取或選取工作的「作用中」欄內之核取方框，以暫停或繼續工作。

>[!NOTE]
>
>取消發佈工作之後，其狀態變更為「正在停止」，直至達到一個安全的停止點。如果工作正從資料庫取得資料，則停止發佈工作可能會花費一些時間。

## 手動發佈資產 {#manually-publishing-assets}

您可以手動發佈個別資產，而不是建立發佈工作。發佈集 (例如影像集或最適化視訊集) 時，將會發佈該集內的集 (或稱為「父項」) 和所有成員 (或稱為「子項」)。

未發佈的資產在用戶介面中以灰色的圓形表徵圖表示，並在資產名稱左側以斜槓（未發佈狀態）。 發佈資產之後，圖示會變成綠色，並且在中心會有白色的勾選記號 (發佈的狀態)。

**手動發佈資產:**

1. 進行以下一項操作:

   * 在格點檢視、清單檢視或詳細資訊檢視中，用標準檔案選取方法來選取一或多個未發佈的資產。

      在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 發佈]**。

   * 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇資產名稱左側帶有斜槓的灰色倒圓角表徵圖。

## 手動取消發佈資產 {#manually-unpublishing-assets}

您可以手動取消發佈個別資產。取消發佈集時，例如色票集或 eCatalog，集 (或稱為「父項」) 本身會變成未發佈狀態。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

在使用者介面中，發佈的資產會在資產名稱左側以中心帶有白色勾選記號的綠色圓形圖示指出 (發佈的狀態)。取消發佈資產後，表徵圖會變為灰色，並在其上用斜線（未發佈狀態）,

**手動取消發佈資產:**

1. 進行以下一項操作:

   * 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個已發佈的資產。

      在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 取消發佈]**。

   * 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇資產名稱左側的捨入綠色複選標籤表徵圖。

## 獲取資產的發佈歷史記錄 {#getting-an-asset-s-publish-history}

上次發佈資產的日期顯示在面板頂部的詳細資訊視圖中。 通過開啟「詳細資訊視圖」中的「歷史記錄和已發佈伺服器」面板，可以獲取有關發佈歷史記錄的詳細資訊。 在該面板中可以查看資產發佈時間以及發佈的目標伺服器。

## 重新發佈的資產和 CDN 延遲 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic資產在內容分發網路(CDN)上分發。 CDN 是指聯成網路的電腦伺服器系統，這些伺服器以完全無障礙地的方式合作，將內容 (尤其是大型媒體內容) 傳送給終端使用者。在 CDN 系統中，網路內容儲存在整個網際網路的網路快取中 (稱為邊緣快取網路)。Web內容從Web快取被遞送給最終用戶，以便更快遞送。

使用者首次下載網頁時，這些資產即傳送到 CDN 網路快取伺服器。資產儲存在該伺服器上，當下次同一區域中有人存取該網頁時，可以更快地傳送快取的相同內容。內容傳送速度更快是因為其位置更接近終端使用者。CDN 提高了網頁顯示速度。它降低了中央伺服器上的頻寬要求，因為內容是從邊緣快取網路傳送，而不是從每個實體的中央伺服器傳送。

新發佈的Adobe Dynamic Media Classic內容可立即提供給最終用戶，並快速填充邊緣快取網路。 但重新發佈的內容 (與之前發佈到影像伺服器的影像完全同名的影像) 需要長達十個小時之後才會在 CDN 上更新。終端使用者看到的則是 CDN 網路上網路快取中的內容。因此，您的Adobe Dynamic Media Classic重新發佈的資產在十小時內不會出現在最終用戶面前。

如果希望重新發佈的影像資產在可用前的延遲時間小於十個小時，可以清空 CDN 上的網路快取。清空這些網路快取可以從 CDN 網路快取中移除舊內容，並將其取代為最新發佈的資產。

要刷新快取，請在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 無效CDN]**。 所有已選取的檔案會從快取中移除。如果沒有可發佈資產，或者您不是公司管理員，則「從 CDN 移除」選項不可用。

>[!MORELIKETHIS]
>
>* [檢查作業檔案](checking-job-files.md)
>* [編輯、刪除、暫停和恢復定期作業](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

