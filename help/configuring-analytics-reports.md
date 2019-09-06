---
title: 設定 Adobe Analytics 報告
seo-title: 設定 Adobe Analytics 報告
description: 'null'
seo-description: 瞭解如何設定Adobe Analytics報表。
uuid: bc210f68-dcb0-4e86-be04-0a8 b2117 ef2 a
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/adobe_ analytics_ tooling_ kit
discoiquuid: f4c8c2b3-cc95-416f-9a5 d-da81 c31 dfc2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 設定 Adobe Analytics 報告{#configuring-adobe-analytics-reports}

若要告知 Adobe Analytics 在 Adobe Analytics 報告中需要哪些資訊，請前往「Adobe Analytics 配置」畫面。在您設定報表後，此畫面會列出您需要的每個檢視器事件，包括對應的Adobe Analytics變數和動態媒體Classic變數。這些檢視器事件-Adobe Analytics變數-動態媒體Classic變數組合會決定哪些資訊會被回報。

除了將檢視器事件與變數相關聯之外，「Adobe Analytics 配置」畫面還提供用於啟用、編輯和刪除檢視器事件的工具。

>[!NOTE]
>
>每當您變更 Adobe Analytics 中的「Adobe Analytics 報告」設定時，請務必從 Adobe Scene7 Publishing System 中登入回到 Adobe Analytics，重新儲存您的 Adobe Analytics 組態設定，然後再重新發佈。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

請參閱[發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用「Adobe Analytics Configuration」畫面將檢視器事件與Adobe Analytics變數和動態媒體Classic變數關聯。對於每個檢視器事件，請選擇一個Adobe Analytics變數和一個Dynamic Media Classic變數。如需如何開啟「Adobe Analytics 配置」畫面的詳細資訊，請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**若要將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. 針對所需的檢視器事件，按一下「變數」欄下方的箭頭按鈕，即可顯示變數組選取器。

   請參閱[檢視器事件](configuring-analytics-reports.md#viewer_events)。

1. 新增動態媒體Classic變數。

   請參閱 [動態媒體Classic變數](configuring-analytics-reports.md#scene7_variables)。

1. 增加 Adobe Analytics 變數。
1. (選擇性) 若要增加其他變數組，請按一下「**增加**」。
1. 按一下&#x200B;**「儲存」**。

   按一下「儲存」後，檢視器事件、其Adobe Analytics變數及其動態媒體Classic變數會列在「Adobe Analytics Configuration」畫面中。

1. 在右下角按一下「**關閉**」。
1. 按一下「**發佈** &gt; **送出發佈**」，以執行「影像伺服」發佈。

   需要發佈，以便檢視器中包含的資訊可用於動態媒體Classic伺服器。

### 檢視器事件 {#viewer-events}

檢視器事件說明使用者使用Dynamic Media Classic檢視器執行的動作。當使用者起始特定動作，例如按一下縮圖或者開始或停止播放視訊時，檢視器會將事件連同與該事件相關聯的資料一起「廣播」到網頁。

下表描述可以增加到「Adobe Analytics 配置」畫面的檢視器事件。

| 檢視器事件 | HTML5 檢視器平台支援和檢視器 | 說明 |
|--- |--- |--- |
| LOAD | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 使用者啟動檢視器時。 |
| PAGE | **X** (eCatalog) | 使用者在 eCatalog 中翻頁時；使用者在目標縮放檢視器中按一下其他目標或色票時。 |
| SWAP | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 使用者按一下其他縮圖以檢視其他影像時。 |
| ITEM | **X** (eCatalog) | 當使用者在支援已定義滑鼠指向效果的影像地圖的檢視器中，將指標暫留在影像地圖上以讀取滑鼠指向效果文字時。 |
| HREF | **X** (eCatalog) | 當使用者在支援影像地圖的檢視器中，在影像地圖中按一下 URL 時。 |
| TARGET |  | 當使用者在目標縮放檢視器中，按一下縮放目標以縮放影像的一部分時。 |
| SEARCH |  | 當使用者在 eCatalog 中，執行關鍵字搜尋時。 |
| PLAY | **X** (視訊) | 當使用者在視訊檢視器中，按一下「播放」以開始播放視訊時。<br><br>**注意：** 如果您使用Adobe Analytics活動訊號型視訊報告，當您在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數映射至此檢視器事件。視訊心率可搭配立即可用的Dynamic Media Classic HTML Video和MixedMedia檢視器運作。此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X** (視訊) | 當使用者在視訊檢視器中，按一下「暫停」以暫停視訊時。<br><br>**注意：** 如果您使用Adobe Analytics活動訊號型視訊報告，當您在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數映射至此檢視器事件。視訊心率可搭配立即可用的Dynamic Media Classic HTML Video和MixedMedia檢視器運作。此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP | **X** (視訊) | 當使用者在視訊檢視器中，按一下「停止」以停止播放視訊時。<br><br>**注意：** 如果您使用Adobe Analytics活動訊號型視訊報告，當您在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數映射至此檢視器事件。視訊心率可搭配立即可用的Dynamic Media Classic HTML Video和MixedMedia檢視器運作。此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (視訊) | 在視訊檢視器中，使用者在觀看到視訊的 0%、25%、50%、75% 或 100% 時產生里程碑事件時。<br><br>**注意：** 如果您使用Adobe Analytics活動訊號型視訊報告，當您在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數映射至此檢視器事件。視訊心率可搭配立即可用的Dynamic Media Classic HTML Video和MixedMedia檢視器運作。此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH | X (彈出、縮放) | 此檢視器事件對應至 Scene7 Publishing System 中的「頁面」檢視器事件。 |
| ZOOM | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。<br> |
| PAN | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。<br> |
| SPIN | **X** (迴轉集) | Adobe Analytics 不會加以追蹤。<br> |


### Dynamic Media Classic變數 {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. 動態媒體Classic變數代表您可以取得報表的資料。例如，`searchTerm` 變數會列出在 eCatalog 搜尋中使用的關鍵字。

下表說明Dynamic Media Classic變數。

| Dynamic Media Classic變數 | 說明 |
|--- |:--- |
| asset | Scene7 Publishing System 的資產 ID 或視訊路徑檔案。 |
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

## 啟用、編輯和刪除檢視器事件 {#activating-editing-and-deleting-viewer-events}

可以在「Adobe Analytics 配置」畫面上啟用、編輯和刪除檢視器事件: 

**啓用** 按一下 **「啓用啓用** 」或「停用」以停用選取的檢視器事件。

**編輯** 選取檢視器事件，然後按一下 **「檢視/編輯** 變數灰色」按鈕。在Dynamic Media Classic變數和Adobe Analytics變數下拉式清單中，從各個個別清單中選擇不同的變數。如需詳細資訊，請參閱「指派Adobe Analytics變數至Dynamic Media Classic檢視器事件和變數」。

**刪除** 選取檢視器事件，然後按一下 **「檢視/編輯** 變數」灰色按鈕。按一下「**刪除**」。
