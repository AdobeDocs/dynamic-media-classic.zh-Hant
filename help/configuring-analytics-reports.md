---
title: 配置Adobe Analytics報告
description: 瞭解如何在Adobe Dynamic Media Classic配置Adobe Analytics報告。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 27%

---

# 配置Adobe Analytics報告{#configuring-adobe-analytics-reports}

要在Adobe Analytics報告中告訴Adobe Analytics您想要哪些資訊，請轉到Adobe Analytics配置螢幕。 配置報告後，此螢幕將列出您需要有關每個查看器事件的相應Adobe Analytics變數和Adobe Dynamic Media Classic變數的資訊。 這些查看器事件 — Adobe Analytics變數 — Adobe Dynamic Media Classic變數組合確定報告的資訊。

除了將查看器事件與變數關聯外，「Adobe Analytics配置」螢幕還提供用於激活、編輯和刪除查看器事件的工具。

>[!NOTE]
>
>無論何時更改Adobe Analytics內的Adobe Analytics報告設定，請確保從Adobe Dynamic Media Classic內重新登錄到Adobe Analytics，重新保存Adobe Analytics配置設定，然後重新發佈。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

請參閱 [發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 將Adobe Analytics變數分配給Adobe Dynamic Media Classic查看器事件和變數 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用「Adobe Analytics配置」螢幕將查看器事件與Adobe Analytics變數和Adobe Dynamic Media Classic變數關聯。 對於每個查看器事件，選擇一個Adobe Analytics變數和一個Adobe Dynamic Media Classic變數。 如需如何開啟「Adobe Analytics 配置」畫面的詳細資訊，請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**要將Adobe Analytics變數分配給Adobe Dynamic Media Classic查看器事件和變數：**

1. 從Adobe Dynamic Media Classic內登錄到Adobe Analytics並在「Adobe Analytics配置」頁面的右表列中選擇報告套件後，通過選擇 **[!UICONTROL 啟用]**。
1. 在「變數」列下，通過為所需的查看器事件選擇箭頭按鈕來顯示變數對選擇器。

   請參閱[檢視器事件](configuring-analytics-reports.md#viewer_events)。

1. 添加Adobe Dynamic Media Classic變數。

   請參閱 [Adobe Dynamic Media Classic變數](configuring-analytics-reports.md#scene7_variables)。

1. 增加 Adobe Analytics 變數。
1. （可選）要添加另一個變數對，請選擇 **[!UICONTROL 添加]**。
1. 選擇 **[!UICONTROL 保存]**。

   選擇後 **[!UICONTROL 保存]**，查看器事件、其Adobe Analytics變數及其Adobe Dynamic Media Classic變數將列在「Adobe Analytics配置」螢幕中。

1. 在右下角，選擇 **[!UICONTROL 關閉]**。
1. 轉到 **[!UICONTROL 發佈]** > **[!UICONTROL 提交發佈]** 運行Image Serving發佈。

   發佈是必要的，以便查看器中包含的資訊可在Adobe Dynamic Media Classic伺服器上找到。

### 檢視器事件 {#viewer-events}

查看器事件描述用戶對Adobe Dynamic Media Classic查看器執行的操作。 當用戶啟動某種動作時，例如選擇縮略圖或啟動或停止視頻，觀看者將事件「廣播」到網頁，以及與該事件相關聯的資料。

下表介紹了可添加到「Adobe Analytics配置」螢幕的查看器事件。

| 檢視器事件 | HTML5 檢視器平台支援和檢視器 | 說明 |
| --- | --- | --- |
| LOAD | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 用戶啟動查看器時 |
| PAGE | **X** (eCatalog) | 在eCatalogs中，當用戶翻頁時；在目標縮放查看器中，當用戶選擇不同的目標或顏色樣本時。 |
| SWAP | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 當用戶選擇不同的縮略圖以查看不同的影像時。 |
| ITEM | **X** (eCatalog) | 當使用者在支援已定義滑鼠指向效果的影像地圖的檢視器中，將指標暫留在影像地圖上以讀取滑鼠指向效果文字時。 |
| HREF | **X** (eCatalog) | 在支援影像映射的查看器中，當用戶在影像映射中選擇URL時。 |
| TARGET |  | 在目標縮放查看器中，當用戶選擇縮放目標以縮放到影像的一部分時。 |
| SEARCH |  | 當使用者在 eCatalog 中，執行關鍵字搜尋時。 |
| PLAY | **X** (視訊) | 在視頻查看器中，當用戶選擇「播放」開始播放視頻時。<br><br>**注：** 如果您使用基於Adobe Analytics心跳的視頻報告，則在Adobe Dynamic Media Classic配置Adobe Analytics時，無需將任何變數映射到此查看器事件。 Video Heartbat可與開箱即用的Adobe Dynamic Media ClassicHTML5視頻和MixedMedia觀看器配合使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱 [啟用Adobe Analytics視頻報告](enabling-analytics-video-reports.md)。 |
| PAUSE | **X** (視訊) | 在視頻查看器中，當用戶選擇 **[!UICONTROL 暫停]** 凍結視頻。<br><br>**注：** 如果您使用基於Adobe Analytics心跳的視頻報告，則在Adobe Dynamic Media Classic配置Adobe Analytics時，無需將任何變數映射到此查看器事件。 Video Heartbat可與開箱即用的Adobe Dynamic Media ClassicHTML5視頻和MixedMedia觀看器配合使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱 [啟用Adobe Analytics視頻報告](enabling-analytics-video-reports.md)。 |
| STOP | **X** (視訊) | 在視頻查看器中，當用戶選擇 **[!UICONTROL 停止]** 停止播放視頻。<br><br>**注：** 如果您使用基於Adobe Analytics心跳的視頻報告，則在Adobe Dynamic Media Classic配置Adobe Analytics時，無需將任何變數映射到此查看器事件。 Video Heartbat可與開箱即用的Adobe Dynamic Media ClassicHTML5視頻和MixedMedia觀看器配合使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱 [啟用Adobe Analytics視頻報告](enabling-analytics-video-reports.md)。 |
| MILESTONE | **X**  (視訊) | 在視訊檢視器中，使用者在觀看到視訊的 0%、25%、50%、75% 或 100% 時產生里程碑事件時。<br><br>**注：** 如果您使用基於Adobe Analytics心跳的視頻報告，則在Adobe Dynamic Media Classic配置Adobe Analytics時，無需將任何變數映射到此查看器事件。 Video Heartbat可與開箱即用的Adobe Dynamic Media ClassicHTML5視頻和MixedMedia觀看器配合使用。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱 [啟用Adobe Analytics視頻報告](enabling-analytics-video-reports.md)。 |
| SWATCH | **X** (彈出、縮放) | 此查看器事件映射到Adobe Dynamic Media Classic的PAGE查看器事件。 |
| ZOOM | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。 |
| PAN | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。 |
| SPIN | **X** (迴轉集) | Adobe Analytics 不會加以追蹤。 |

### Adobe Dynamic Media Classic變數 {#scene-variables}

對於「Adobe Analytics配置」螢幕上的每個查看器事件，選擇一個Adobe Analytics變數和 *Adobe Dynamic Media Classic變數*。 Adobe Dynamic Media Classic變數表示可為報表獲取的資料。 例如，`searchTerm` 變數會列出在 eCatalog 搜尋中使用的關鍵字。

下表介紹了Adobe Dynamic Media Classic變數：

| Adobe Dynamic Media Classic變數 | 說明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic資產ID或視頻路徑檔案。 |
| viewerId | 指定給各個不同檢視器類型的任一編號。 |
| pageLabel | 在 eCatalog 中，檢視器顯示的頁面。 |
| label | 標籤值 (字串)。 |
| frame | 影像集內的頁面或頁面參照。 |
| rollover_keyRaw | 完整的 HREF 值，不僅是已處理部分。 |
| rollover_keyProc | 在影像地圖中參照的項目 ID (對 href 和 item 事件有效)。 |
| searchTerm | 在 eCatalog 搜尋中使用的字詞。 |
| timeStamp | 在視訊檢視器中選擇的「播放」、「停止」和「暫停」。 |
| progress | 完成的里程碑事件的百分比。 |
| targetId | ID 值 (數值)。 |

## 激活、編輯和刪除查看器事件 {#activating-editing-and-deleting-viewer-events}

可以在「Adobe Analytics 配置」畫面上啟用、編輯和刪除檢視器事件: 

* **激活**  — 選擇 **[!UICONTROL 啟用]** 激活或 **[!UICONTROL 禁用]** 停用選定的查看器事件。

* **編輯**  — 選擇查看器事件並選擇 **[!UICONTROL 檢視/編輯]** 變數灰色按鈕。 在「Adobe Dynamic Media Classic變數」和「Adobe Analytics變數」下拉清單中，從每個相應的清單中選擇不同的變數。 有關詳細資訊，請參見 [將Adobe Analytics變數分配給Adobe Dynamic Media Classic查看器事件和變數](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables)。

* **刪除**  — 選擇查看器事件，然後選擇 **[!UICONTROL 檢視/編輯]** 變數灰色按鈕。 選擇 **[!UICONTROL 刪除]**。
