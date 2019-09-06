---
title: 使用 Adobe Analytics 檢測套件來檢測檢視器
seo-title: 使用 Adobe Analytics 檢測套件來檢測檢視器
description: 'null'
seo-description: 瞭解如何使用Adobe Analytics工具套件來檢測檢視器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/adobe_ analytics_ tooling_ kit
discoiquuid: a2824244-1755-42de-a167-42afe117 cf038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 使用 Adobe Analytics 檢測套件來檢測檢視器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics工具套件，將HTML檢視器與Adobe Analytics整合。

如果您使用任何預先定義的Dynamic Media Classic HTML檢視器預設集，請注意，它們已包含傳送資料至Adobe Analytics所需的所有實作代碼—您不需要進一步進行檢測。

## 從 Scene7 Publishing System 設定 Adobe Analytics 追蹤 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

對於所有HTML檢視器，請將下列JavaScript新增至HTML容器，通常位於&lt; head&gt;元素中：

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

將 `Company` 設定為 SPS 公司名稱。`&preset` 是選擇性的，除非公司預設集名稱不是 `companypreset`。In such cases, it could be `companypreset-1, companypreset-2`, and so on. 數字越高，表示預設集實體越新。To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

您現在要繼續增加一個函數，以便將檢視器事件傳輸到 Adobe Analytics 追蹤程式碼。

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函數名稱會區分大小寫。The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` is defined in s_ code. jsp included.`s7track` 控制每個事件的所有追蹤。(若要進一步自訂傳輸到 Adobe Analytics 的資料，可在該區域執行此操作。)

## 啟用 HREF 和 ITEM 事件 {#enabling-href-and-item-events}

可以透過影像地圖編輯，在檢視器中啟用 HREF (滑鼠指向) 和 ITEM (滑鼠按一下/輕觸) 事件。在與檢視器內容相關聯的影像地圖中定義 HREF 和 ITEM 識別名稱。Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
