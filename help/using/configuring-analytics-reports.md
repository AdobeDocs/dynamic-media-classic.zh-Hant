---
title: 設定Adobe Analytics報表
description: 瞭解如何在Adobe Dynamic Media Classic中設定Adobe Analytics報表。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 21%

---

# 設定Adobe Analytics報表{#configuring-adobe-analytics-reports}

若要告訴Adobe Analytics您想在Adobe Analytics報表中取得哪些資訊，請前往Adobe Analytics設定畫面。 依照您的設定報告，此畫面會針對您想取得資訊的每個檢視器事件，列出相對應的Adobe Analytics變數和Adobe Dynamic Media Classic變數。 這些檢視器事件 — Adobe Analytics變數 — Adobe Dynamic Media Classic變陣列合會決定要報告的資訊。

除了將檢視器事件與變數建立關聯以外， Adobe Analytics設定畫面還提供啟用、編輯和刪除檢視器事件的工具。

>[!NOTE]
>
>當您在Adobe Analytics中變更Adobe Analytics報表設定時，請務必從Adobe Dynamic Media Classic中重新登入Adobe Analytics、重新儲存Adobe Analytics組態設定，然後重新發佈。

請參閱[登入Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

請參閱[Publish組態資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用Adobe Analytics設定畫面將檢視器事件與Adobe Analytics變數和Adobe Dynamic Media Classic變數建立關聯。 請為每個檢視器事件選擇一個Adobe Analytics變數和一個Adobe Dynamic Media Classic變數。 如需有關開啟Adobe Analytics設定畫面的指示，請參閱[登入Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**若要將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數：**

1. 當您從Dynamic Media Classic登入Adobe Analytics並選取報表套裝後，請在Adobe Analytics設定頁面的右側表格欄中，選取「**[!UICONTROL 啟用]**」以啟動檢視器事件。
1. 在「變數」欄下，選取所需檢視器事件的箭頭按鈕，以顯示變數配對選擇器。

   請參閱[檢視器事件](configuring-analytics-reports.md#viewer_events)。

1. 新增Adobe Dynamic Media Classic變數。

   請參閱[Adobe Dynamic Media Classic變數](configuring-analytics-reports.md#scene7_variables)。

1. 增加 Adobe Analytics 變數。
1. （選擇性）若要新增其他變陣列，請選取&#x200B;**[!UICONTROL 新增]**。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

   選取&#x200B;**[!UICONTROL 儲存]**&#x200B;後，檢視器事件、其Adobe Analytics變數及其Adobe Dynamic Media Classic變數會列在Adobe Analytics設定畫面中。

1. 在右下角，選取&#x200B;**[!UICONTROL 關閉]**。
1. 移至&#x200B;**[!UICONTROL Publish]** > **[!UICONTROL 提交Publish]**&#x200B;以執行影像伺服發佈。

   發佈是必要的，如此檢視器中包含的資訊才能在Adobe Dynamic Media Classic伺服器上使用。

### 檢視器事件 {#viewer-events}

檢視器事件說明使用者使用Dynamic Media Classic檢視器執行的動作。 當使用者起始動作（例如選取縮圖或啟動或停止視訊）時，檢視器會將事件「廣播」至網頁。 也會推送與該事件相關聯的資料。

下表說明可新增至Adobe Analytics設定畫面的檢視器事件。

| 檢視器事件 | HTML5 檢視器平台支援和檢視器 | 說明 |
| --- | --- | --- |
| LOAD | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 當使用者啟動檢視器時 |
| PAGE | **X** (eCatalog) | 在eCatalogs中，當使用者轉動頁面時；在目標縮放檢視器中，當使用者選取不同的目標或色票時。 |
| SWAP | **X** (eCatalog、彈出、迴轉集、視訊、縮放) | 當使用者選擇不同的縮圖來檢視不同的影像時。 |
| ITEM | **X** (eCatalog) | 當使用者在支援已定義滑鼠指向效果的影像地圖的檢視器中，將指標暫留在影像地圖上以讀取滑鼠指向效果文字時。 |
| HREF | **X** (eCatalog) | 在支援「影像地圖」的檢視器中，當使用者在「影像地圖」中選取URL時。 |
| TARGET | | 在目標縮放檢視器中，使用者選取縮放目標以縮放至影像的一部分時。 |
| SEARCH | | 當使用者在 eCatalog 中，執行關鍵字搜尋時。 |
| PLAY | **X** (視訊) | 在視訊檢視器中，當使用者選取「播放」開始播放視訊時。<br><br>**注意：**&#x200B;如果您使用Adobe Analytics心率式視訊報告，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 視訊播放器會產生追蹤資料，以便在Adobe Analytics視訊報表中檢視。 請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| PAUSE | **X** (視訊) | 在視訊檢視器中，當使用者選取&#x200B;**[!UICONTROL 暫停]**&#x200B;以凍結視訊時。<br><br>**注意：**&#x200B;如果您使用Adobe Analytics心率式視訊報告，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 視訊播放器會產生追蹤資料，以便在Adobe Analytics視訊報表中檢視。 請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| STOP | **X** (視訊) | 在視訊檢視器中，當使用者選取&#x200B;**[!UICONTROL 停止]**&#x200B;以停止播放視訊時。<br><br>**注意：**&#x200B;如果您使用Adobe Analytics心率式視訊報告，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 視訊播放器會產生追蹤資料，以便在Adobe Analytics視訊報表中檢視。 請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| MILESTONE | **X** (視訊) | 在視訊檢視器中，使用者在觀看到視訊的 0%、25%、50%、75% 或 100% 時產生里程碑事件時。<br><br>**注意：**&#x200B;如果您使用Adobe Analytics心率式視訊報告，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 視訊播放器會產生追蹤資料，以便在Adobe Analytics視訊報表中檢視。 請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| SWATCH | **X** (彈出、縮放) | 此檢視器事件對應至Adobe Dynamic Media Classic中的頁面檢視器事件。 |
| ZOOM | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。 |
| PAN | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。 |
| SPIN | **X** (迴轉集) | Adobe Analytics 不會加以追蹤。 |

### Adobe Dynamic Media Classic變數 {#scene-variables}

針對Adobe Analytics設定畫面上的每個檢視器事件，選擇一個Adobe Analytics變數及一個&#x200B;*Adobe Dynamic Media Classic變數*。 Adobe Dynamic Media Classic變數代表您可針對報表取得的資料。 例如，`searchTerm`變數會列出用於eCatalog搜尋的關鍵字。

下表說明Adobe Dynamic Media Classic變數：

| Adobe Dynamic Media Classic變數 | 說明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic資產ID或視訊路徑檔案。 |
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

## 啟動、編輯和刪除檢視器事件 {#activating-editing-and-deleting-viewer-events}

可以在「Adobe Analytics 配置」畫面上啟用、編輯和刪除檢視器事件: 

* **啟動**：選取&#x200B;**[!UICONTROL 啟用]**&#x200B;以啟動或&#x200B;**[!UICONTROL 停用]**&#x200B;以停用選取的檢視器事件。

* **編輯**：選取檢視器事件並選取&#x200B;**[!UICONTROL 檢視/編輯]**&#x200B;變數灰色按鈕。 在Adobe Dynamic Media Classic變數和Adobe Analytics變數下拉式清單中，從各個清單選擇不同的變數。 如需詳細資訊，請參閱[將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables)。

* **刪除**：選取檢視器事件，然後選取&#x200B;**[!UICONTROL 檢視/編輯]**&#x200B;變數灰色按鈕。 選取&#x200B;**[!UICONTROL 刪除]**。
