---
title: 使用 Adobe Analytics 檢測套件來檢測檢視器
description: 瞭解如何使用Adobe Analytics儀器套件來測量檢視器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media經典
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# 使用 Adobe Analytics 檢測套件來檢測檢視器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics工具套件將HTML5檢視器與Adobe Analytics整合。

如果您使用預先定義的Dynamic MediaClassic HTML5檢視器預設集，它們已包含所有要傳送資料至Adobe Analytics的實作程式碼；您不需要進一步的工具。

## 從Dynamic Media經典網站設定Adobe Analytics追蹤{#set-up-adobe-analytics-tracking-from-scene-publishing-system}

對於所有HTML5檢視器，請將下列JavaScript™新增至HTML容器，通常位於&lt;head>元素中：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

其中`Dynamic Media Classic Company ID`設定為Dynamic Media經典公司名稱。 而`&preset`則為選用，除非公司預設集名稱不是`companypreset`。 在這種情況下，它可能是`companypreset-1, companypreset-2`，依此類推。 數字越高，表示預設集實體越新。若要判斷正確的公司預設值名稱，請按一下「複製URL ]**」，然後查看`preset=`參數以尋找公司預設值名稱。**[!UICONTROL 

繼續，現在新增將檢視器事件傳送至Adobe Analytics追蹤代碼的函式。

將`s7ComponentEvent()`函式新增至容器HTML（或JSP、ASPX或其他）:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函式名稱區分大小寫。 傳遞給`s7componentEvent`的唯一必需參數是最後一個：`eventData`。 其中`s7track()`在上述s_code.jsp中定義。 而`s7track`可處理每個事件的所有追蹤。 (若要進一步自訂傳輸到 Adobe Analytics 的資料，可在該區域執行此操作。)

## 啟用 HREF 和 ITEM 事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。將`&rolloverKey=`參數新增至影像地圖中的HREF值。
