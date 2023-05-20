---
title: 使用Adobe Analytics儀表套件對查看器進行儀表
description: 瞭解如何使用Adobe Dynamic Media Classic的Adobe Analytics儀器套件來測試查看器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# 使用Adobe Analytics儀表套件對查看器進行儀表{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics儀器套件將HTML5查看器與Adobe Analytics整合。

如果您使用任何預定義的Adobe Dynamic Media ClassicHTML5查看器預設，它們已經包含了向Adobe Analytics發送資料的所有實現代碼；您不需要進一步的工具。

## 在Adobe Dynamic Media Classic建立Adobe Analytics跟蹤 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

對於所有HTML5查看器，將以下JavaScript添加到HTML容器中，通常在 &lt;head> 元素：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

位置 `Adobe Dynamic Media Classic Company ID` 設定為Adobe Dynamic Media Classic公司名稱。 和 `&preset` 是可選的，除非公司預設名稱不是 `companypreset`。 在這種情況下， `companypreset-1, companypreset-2`等等。 數字越高，表示預設集實體越新。要確定正確的公司預設值名稱，請選擇 **[!UICONTROL 複製URL]** ，然後看 `preset=`參數，以查找公司預設名稱。

繼續，現在添加將查看器事件傳輸到Adobe Analytics跟蹤代碼的函式。

添加 `s7ComponentEvent()` 函式到容器HTML（或JSP、或ASPX或其他）:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函式名稱區分大小寫。 傳遞給的唯一參數 `s7componentEvent`最後一個是必需的： `eventData`。 位置 `s7track()` 在上面包括的s_code.jsp中定義。 和 `s7track` 處理每個事件的所有跟蹤。 (若要進一步自訂傳輸到 Adobe Analytics 的資料，可在該區域執行此操作。)

## 啟用HREF和ITEM事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。添加 `&rolloverKey=` 影像映射中HREF值的參數。
