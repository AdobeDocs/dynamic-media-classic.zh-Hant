---
title: 使用 Adobe Analytics 檢測套件來檢測檢視器
description: 瞭解如何使用Adobe Analytics Instrumentation Kit來測量檢視器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 36%

---


# 使用 Adobe Analytics 檢測套件來檢測檢視器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit將HTML5檢視器與Adobe Analytics整合。

如果您使用任何預先定義的Dynamic Media Classic HTML5檢視器預設集，請注意，這些預設集已包含傳送資料至Adobe Analytics所需的所有實作程式碼，您不需要進一步的工具。

## 從Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}設定Adobe Analytics追蹤

對於所有HTML5檢視器，請將下列JavaScript新增至HTML容器，通常位於&lt;head>元素中：

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` 設為Dynamic Media Classic公司名稱。`&preset` 為可選項，除非公司預設集名稱不 `companypreset`是。在這種情況下，它可能是`companypreset-1, companypreset-2`，依此類推。 數字越高，表示預設集實體越新。若要判斷正確的公司預設值名稱，請按一下「複製URL **」，然後查看`preset=`參數以尋找公司預設值名稱。**

您現在要繼續增加一個函數，以便將檢視器事件傳輸到 Adobe Analytics 追蹤程式碼。

將`s7ComponentEvent()`函式新增至容器HTML（或JSP、ASPX或其他）:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函數名稱會區分大小寫。傳遞給`s7componentEvent`的唯一必需參數是最後一個：`eventData`。 `s7track()` 定義於上述s_code.jsp中。`s7track` 處理每個事件的所有追蹤。(若要進一步自訂傳輸到 Adobe Analytics 的資料，可在該區域執行此操作。)

## 啟用 HREF 和 ITEM 事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。將`&rolloverKey=`參數新增至影像地圖中的HREF值。
