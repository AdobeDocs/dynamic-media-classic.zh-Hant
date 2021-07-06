---
title: 設定 Adobe Analytics 報告
description: 了解如何設定Adobe Analytics報表。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# 設定 Adobe Analytics 報告{#configuring-adobe-analytics-reports}

若要告知 Adobe Analytics 在 Adobe Analytics 報告中需要哪些資訊，請前往「Adobe Analytics 配置」畫面。設定報表後，此畫面會針對您想要了解的每個檢視器事件，列出對應的Adobe Analytics變數和Dynamic Media Classic變數。 這些檢視器事件 — Adobe Analytics變數 — Dynamic Media Classic變陣列合決定要回報的資訊。

除了將檢視器事件與變數建立關聯外，Adobe Analytics設定畫面也提供工具來啟用、編輯和刪除檢視器事件。

>[!NOTE]
>
>每當您在Adobe Analytics中變更Adobe Analytics報表設定時，請務必從Adobe Dynamic Media Classic登回Adobe Analytics，重新儲存Adobe Analytics組態設定，然後重新發佈。

請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

請參閱[發佈配置資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用Adobe Analytics設定畫面，將檢視器事件與Adobe Analytics變數和Dynamic Media Classic變數建立關聯。 對於每個檢視器事件，選擇一個Adobe Analytics變數和一個Dynamic Media Classic變數。 如需如何開啟「Adobe Analytics 配置」畫面的詳細資訊，請參閱[登入 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數的方式**

1. 在您從Dynamic Media Classic登入Adobe Analytics，並選取報表套裝後，在Adobe Analytics設定頁面的右表欄中，按一下&#x200B;**[!UICONTROL Enable]**&#x200B;啟動檢視器事件。
1. 針對所需的檢視器事件，按一下「變數」欄下方的箭頭按鈕，即可顯示變數組選取器。

   請參閱[檢視器事件](configuring-analytics-reports.md#viewer_events)。

1. 新增Dynamic Media Classic變數。

   請參閱[Dynamic Media Classic變數](configuring-analytics-reports.md#scene7_variables)。

1. 增加 Adobe Analytics 變數。
1. (選擇性) 若要增加其他變數組，請按一下「**增加**」。
1. 按一下&#x200B;**「儲存」**。

   按一下「儲存」後，檢視器事件、其Adobe Analytics變數及其Dynamic Media Classic變數會列在「Adobe Analytics設定」畫面中。

1. 在右下角按一下「**關閉**」。
1. 按一下「**發佈** > **送出發佈**」，以執行「影像伺服」發佈。

   必須發佈，才能在Dynamic Media Classic伺服器上使用檢視器中包含的資訊。

### 檢視器事件 {#viewer-events}

檢視器事件說明使用者使用Dynamic Media Classic檢視器執行的動作。 當使用者起始特定動作時，例如按一下縮圖或啟動或停止視訊時，檢視器會將事件「廣播」至網頁，以及與該事件相關聯的資料。

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
| PLAY | **X** (視訊) | 當使用者在視訊檢視器中，按一下「播放」以開始播放視訊時。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。視訊心率可搭配現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器運作。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| PAUSE | **X** (視訊) | 當使用者在視訊檢視器中，按一下「暫停」以暫停視訊時。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。視訊心率可搭配現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器運作。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| STOP | **X** (視訊) | 當使用者在視訊檢視器中，按一下「停止」以停止播放視訊時。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。視訊心率可搭配現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器運作。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| MILESTONE | **X**  (視訊) | 在視訊檢視器中，使用者在觀看到視訊的 0%、25%、50%、75% 或 100% 時產生里程碑事件時。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。視訊心率可搭配現成可用的Dynamic Media Classic HTML5視訊和MixedMedia檢視器運作。 此視訊播放器會產生可在 Adobe Analytics 視訊報告中檢視的追蹤資料。請參閱[啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md)。 |
| SWATCH | X (彈出、縮放) | 此檢視器事件已對應至Dynamic Media Classic中的PAGE檢視器事件。 |
| ZOOM | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。<br> |
| PAN | **X** (eCatalog、迴轉集、縮放) | Adobe Analytics 不會加以追蹤。<br> |
| SPIN | **X** (迴轉集) | Adobe Analytics 不會加以追蹤。<br> |


### Dynamic Media Classic變數 {#scene-variables}

對於「Adobe Analytics設定」畫面上的每個檢視器事件，選擇Adobe Analytics變數和&#x200B;*Dynamic Media Classic變數*。 Dynamic Media Classic變數代表您可為報表取得的資料。 例如，`searchTerm` 變數會列出在 eCatalog 搜尋中使用的關鍵字。

下表說明Dynamic Media Classic變數。

| Dynamic Media Classic變數 | 說明 |
|--- |:--- |
| asset | Dynamic Media傳統資產ID或視訊路徑檔案。 |
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

* ****
啟用按一 **** 下啟用以啟用或停 **** 用以停用選取的檢視器事件。

* ****
編輯選取檢視器事件，然後按一下 **[!UICONTROL 檢視/]** 編輯變數灰色按鈕。在「Dynamic Media傳統變數」和「Adobe Analytics變數」下拉式清單中，從各個清單中選擇不同的變數。 如需詳細資訊，請參閱將Adobe Analytics變數指派給Dynamic Media Classic檢視器事件和變數。

* ****
刪除選取檢視器事件，然後按一下「檢 **[!UICONTROL 視/]** 編輯變數」灰色按鈕。按一下「**[!UICONTROL 刪除]**」。
