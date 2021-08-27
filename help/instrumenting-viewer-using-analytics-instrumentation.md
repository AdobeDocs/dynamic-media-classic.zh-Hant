---
title: 使用Adobe Analytics Instrumentation Kit檢測查看器
description: 了解如何使用AdobeDynamic Media Classic中的Adobe Analytics Instrumentation Kit來檢測檢視器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# 使用Adobe Analytics Instrumentation Kit檢測查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit將HTML5檢視器與Adobe Analytics整合。

如果您使用任何預先定義的AdobeDynamic Media Classic HTML5檢視器預設集，這些預設集已包含要將資料傳送至Adobe Analytics的所有實作程式碼；您無需進一步檢測。

## 從AdobeDynamic Media Classic設定Adobe Analytics追蹤 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

對於所有HTML5檢視器，請將下列JavaScript新增至HTML容器，通常位於&lt;head>元素中：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

其中`Adobe Dynamic Media Classic Company ID`設為AdobeDynamic Media Classic公司名稱。 而`&preset`是選用項目，除非公司預設集名稱不是`companypreset`。 在這種情況下，可能是`companypreset-1, companypreset-2`，以此類推。 數字越高，表示預設集實體越新。若要判斷正確的公司預設集值名稱，請選取「**[!UICONTROL 複製URL]**」 ，然後查看`preset=`參數以尋找公司預設集名稱。

繼續，現在新增將檢視器事件傳輸至Adobe Analytics追蹤程式碼的函式。

將`s7ComponentEvent()`函式新增至容器HTML（或JSP、ASPX或其他）:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函式名稱區分大小寫。 傳遞至`s7componentEvent`的唯一必要參數是最後一個：`eventData`。 其中`s7track()`定義於上述s_code.jsp中。 而`s7track`則處理每個事件的所有追蹤。 (若要進一步自訂傳輸到 Adobe Analytics 的資料，可在該區域執行此操作。)

## 啟用HREF和項目事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。將`&rolloverKey=`參數新增至影像映射內的HREF值。
