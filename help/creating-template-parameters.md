---
title: 建立範本參數
description: 了解如何在Adobe Dynamic Media Classic中建立範本參數。
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 59%

---

# 建立範本參數{#creating-template-parameters}

您可以透過參數盡可能靈活地使用範本；可以透過參數來動態自訂範本影像。您可以決定範本中要包括哪些文字圖層和影像圖層，以及每個圖層中要顯示哪些參數。例如，要吸引對正在銷售的產品的注意，可以建立「銷售時」文本層。 日後可以移除「特價出售」參數來移除該圖層，但仍保留範本影像的其餘部分。

建立範本參數時，實際上是宣告要在 URL 字串中呼叫範本的哪些部分。使用參數結構的 URL 會在 URL 字串中列出相關項目。透過列出的參數，您可以按照範本影像從影像伺服器動態結構的方式來建立自訂結果， 從而變更動態範本 (因為您可以呼叫 URL 中的部分或全部參數)。

在文字圖層參數中，還可以將文字字串設定為連結到資料庫值的動態欄位。將文字連結到資料庫的功能非常有用 (例如在促銷活動中)。您可以自訂範本影像，使其顯示用戶端或客戶姓名。您也可以將文字層參數連結至價格資料庫，以顯示範本影像中項目的價格。

您可以多次參考一個參數。對參數對話框中的每個命令使用下拉式方框，以選取符合該特定命令的任何參數。例如，所有大小參數都可用於`size=`命令。 可以將參數參照再分配給已存在於下拉式方框中的任何參數，並重新命名為下拉式方框中不存在的名稱。在後一種情況下，名稱必須是唯一的。 否則，錯誤會指出參數存在。 刪除參數參照時，如果參照未在其他任何位置被引用，則參數將從URL中刪除。 當更改文本參數的預設值時，該參數的所有引用都會更新。 您可以在圖層表格、範本轉譯和URL中看到更新。 通過調整控制滑塊大小或在屬性面板中鍵入值來更改圖層屬性時，會更新參數值，並更新參數的所有引用。 例如，如果使用一個參數對兩個圖層的大小進行了參數化，則在變更其中一個圖層大小時，兩個圖層的大小均會更新。在您預覽範本並變更參數時，該參數的所有參照均會更新。

另請參閱[範本基本知識](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)訓練影片。

## 參數化圖層 {#parameterizing-a-layer}

對於範本中的每個圖層，請根據以下步驟建立範本參數:

1. 在「圖層」清單中，選取要建立參數的圖層名稱旁邊的「參數」按鈕 。將開啟「參數」畫面。它會列出圖層上每個參數的名稱、值及類型。
1. 對於要包括在範本影像中的每個參數，選取其名稱旁邊的「開啟」選項。
1. 選擇&#x200B;**[!UICONTROL 關閉]**&#x200B;退出「參數」螢幕。

>[!NOTE]
>
>可以在「參數」畫面中重新命名參數。重新命名參數使得參數更易於在 URL 字串中識別，且更易於作為資料庫值使用。要更名參數，請選擇其&#x200B;**[!UICONTROL On]**&#x200B;選項，選擇其名稱，並在「名稱」欄位中輸入新名稱。

若要查看已為範本建立的參數清單，請在「範本」畫面上選取「參數摘要」按鈕。將開啟「參數摘要」畫面。它會列出每個圖層的名稱，如果已為圖層建立參數，則還會顯示參數名稱和參數值。

## 建立動態文字參數 {#creating-dynamic-text-parameters}

對於文本層，還可以將文本字串設定為連結到資料庫值的動態欄位。 請遵循下列步驟︰

1. 在「範本」畫面上，選取要為其建立動態文字參數的文字圖層名稱旁邊的「參數」按鈕 。「參數」(Parameters)頁面隨即開啟。
1. 選取文字屬性(textAttr)名稱旁的&#x200B;**[!UICONTROL On]**&#x200B;選項。
1. 在「參數」螢幕中選擇&#x200B;**[!UICONTROL Text]**&#x200B;頁簽。
1. 選擇&#x200B;**[!UICONTROL 添加參數]**。 將顯示預設的參數名稱。選取該名稱並覆蓋鍵入新名稱，可以取代此名稱。目前鍵入的文字字串將成為參數的新名稱。
1. 選擇&#x200B;**[!UICONTROL 關閉]**&#x200B;以關閉「參數」頁。

若要使參數名稱使用資料庫值，請將以下字串附加到範本 URL:

```as3
?$_2(parameter name)=(database value)
```

參數名稱被資料庫欄位或Java™代碼中的名稱替換，該代碼指示例如項目的當前價格或客戶名稱。
