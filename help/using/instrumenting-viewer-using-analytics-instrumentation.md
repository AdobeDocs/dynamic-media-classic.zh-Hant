---
title: 使用Adobe Analytics Instrumentation Kit檢測檢視器
description: 瞭解如何使用Adobe Dynamic Media Classic中的Adobe Analytics Instrumentation Kit檢測檢視器。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 596e4337002ebd67dd9f915a5ae63ae2a6e18437
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 15%

---

# 使用Adobe Analytics Instrumentation Kit檢測檢視器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit將HTML5檢視器與Adobe Analytics整合。

如果您使用任何預先定義的Adobe Dynamic Media Classic HTML5檢視器預設集，這些預設集已包含所有傳送資料至Adobe Analytics的實作程式碼。 您不需要新增任何進一步的檢測。

## 從Adobe Dynamic Media Classic設定Adobe Analytics追蹤 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

針對所有HTML5檢視器，新增下列JavaScript至HTML容器（通常在&lt;head>元素中）：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

其中`Adobe Dynamic Media Classic Company ID`設定為Adobe Dynamic Media Classic公司名稱。 而`&preset`是選擇性的。 如果公司預設集名稱不是`companypreset`，則不是選用名稱。 在這些情況下，它是`companypreset-1`、`companypreset-2`和更新版本。 數字越高，表示預設集實體越新。 若要判斷正確的公司預設集名稱，請選取&#x200B;**[!UICONTROL 複製URL]**，然後檢視`preset=`引數以尋找公司預設集名稱。

新增將檢視器事件傳輸至Adobe Analytics追蹤代碼的函式。

將`s7ComponentEvent()`函式新增至容器HTML （或JSP、ASPX或其他）：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函式名稱會區分大小寫。 唯一傳遞給`s7ComponentEvent`的必要引數是最後一個引數`eventData`。 其中`s7track()`定義於上述包含的s_code.jsp中。 及`s7track`處理每個事件的所有追蹤。 （您可以在此區域中進一步自訂傳輸至Adobe Analytics的資料。）

## 啟用HREF和ITEM事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。 在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。 將`&rolloverKey=`引數新增至影像地圖內的HREF值。
