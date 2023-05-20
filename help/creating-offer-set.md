---
title: 建立聘用集
description: 瞭解如何在Adobe Dynamic Media Classic建立優惠集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 35%

---

# 建立聘用集 {#creating-an-offer-set}

您可以建立以下各種類型的提案集:

* 視訊
* 參數化範本
* 影像

對於模板，選擇 **[!UICONTROL 添加和預覽]**，然後設定您選擇的參數。 其它優惠集類型不包括參數，但您仍然可以通過選擇 **[!UICONTROL 預覽]** 並更改可用預設。

Adobe Dynamic Media Classic提供編輯和建立優惠集的工具。

>[!NOTE]
>
>在建立聘用集之前，請確保將要用於該集的所有資產發佈到Adobe Dynamic Media Classic。 請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

## 提案集的類型 {#types-of-offer-sets}

從以下類型的提案集中建立一個提案集:

* **影像**  — 您可以為優惠集組合影像。 每個影像都包括該集合中的不同報價。

* **影像模板**  — 您可以使用 **[!UICONTROL 生成]** >「模板基礎知識」命令。 透過參數，可交換出及自訂範本的各個組件 (文字框中的文字、不同的影像)。對於提案集，舉例來說，您可以使用範本參數在提案集中的同一影像上建立變體。有關建立和參數化影像模板的資訊，請參見 [建立模板參數](creating-template-parameters.md#creating_template_parameters)。

另請參閱 [模板基礎知識](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 培訓視頻。

* **視頻**  — 您可以為優惠集裝配視頻。 每個視訊是提案集中的一個不同提案。

## 使用參數化模板建立聘用集 {#creating-an-offer-set-with-a-parameterized-template}

建立提案集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 保存後發佈]** 選項，然後保存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**要使用參數化模板建立聘用集，請執行以下操作：**

1. 選擇模板或橫幅。
1. 轉到 **[!UICONTROL 生成]** > **[!UICONTROL Test和目標優惠集]**。

   「Test和目標優惠集」頁列出優惠集中的優惠。 清單中的第一項是物件。

1. 選擇對象並選擇 **[!UICONTROL 添加和預覽]**。

   頁面的左側列出了範本中的參數及參數值。

1. 變更參數值以建立提案。例如，在文字欄位中輸入不同文字、變更圖層大小、用一個影像交換另一個影像或者選擇不同的檢視器預設集。
1. 選擇 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存為**]** 保存要約作為要約集的一部分。

   「Test和目標優惠集」頁列出您建立的優惠。

1. 重複步驟 3 到 5 為提案集建立更多提案。
1. 完成後，靠近頁面右下角，確保 **[!UICONTROL 保存後發佈*]** 選中（預設）。
1. 選擇 **[!UICONTROL 關閉]**，輸入聘用集的名稱，然後選擇 **[!UICONTROL 保存]**。

在關閉「Test和目標優惠集」頁之前，請將優惠集推送到「Adobe Target標準/高級」。 請參閱 [將聘用集推送到Test(&amp;T)](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 建立包含影像或視頻的優惠集 {#creating-an-offer-set-with-images-or-videos}

建立提案集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 保存後發佈]** 選項，然後保存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**使用影像或視訊建立提案集:**

1. 為服務集組合影像或視頻。 從「Test和目標優惠集」螢幕或「網格視圖」或「清單視圖」中開始，然後使用以下方法之一：

   * **Test和目標優惠集螢幕**  — 轉到 **[!UICONTROL 生成]** > **[!UICONTROL Test和目標優惠集]**。 將影像或視訊拖放到畫面上。若要建立大小不同的視訊或影像，請拖入多個影像或視訊，然後逐一設定其大小。

   * **網格視圖或清單視圖**  — 選擇影像或視頻，然後轉到 **[!UICONTROL 生成]** > **[!UICONTROL Test和目標優惠集]**。

1. （可選）選擇影像或視頻並選擇 **[!UICONTROL 預覽]**。 在「預覽優惠」頁上，可以更改所選影像或視頻的大小和外觀。 或者，您可以更改優惠集中的所有影像或視頻。

   * 選擇預設集以變更影像或視訊的外觀和大小。
   * 要將您選擇的預設應用於聘用集中的所有聘用，請選擇 **[!UICONTROL 選擇「全部預設」]** 的子菜單。

   選擇 **[!UICONTROL 保存]** 保存對影像或視頻選項所做的更改。 然後選擇 **[!UICONTROL 關閉]** 返回「Test和目標優惠集」頁。

1. 完成為優惠集建立優惠並為不同影像選擇「影像預設」後，請確保 **[!UICONTROL 保存後發佈]** 選中（預設）。
1. 選擇 **[!UICONTROL 保存]** 並輸入聘用集的名稱，然後選擇 **[!UICONTROL 保存]**。

在關閉「Test和目標優惠集」頁之前，將優惠集推送至「Adobe Target標準/特優」。 請參閱 [將聘用集推送到Test(&amp;T)](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 編輯聘用集 {#editing-an-offer-set}

無論您編輯已發佈集還是未發佈集， **[!UICONTROL 保存後發佈]** 選項通過以下方式影響集和整合員：

| 已發佈集? | **[!UICONTROL 保存後發佈]** 的下界？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**要編輯聘用集，請執行以下操作：**

1. 要編輯聘用集，請在「網格視圖」或「清單視圖」中顯示聘用集，然後選擇其 **[!UICONTROL 編輯]** 滾動按鈕。
1. 在「Test和目標優惠集」頁中，執行下列任一操作：

   * **刪除優惠**  — 選擇優惠，然後選擇 **[!UICONTROL 刪除]** 從集中刪除優惠。
   * **添加優惠**  — 如何添加聘用取決於您正在使用的聘用集的類型：
      * **模板**  — 選擇 **[!UICONTROL 添加和預覽]**，並在「添加和預覽聘用」頁面上，建立其他聘用。
      * **影像和視頻**  — 將影像或視頻拖到「Test和目標優惠集」頁。

   >[!NOTE]
   >
   >您無法刪除與某個行銷活動相關的提案集。要刪除與市場活動關聯的優惠集，請先登錄Adobe Target標準/高級版並刪除市場活動關聯。 即使與市場活動取消關聯後，資產也只能從Adobe Dynamic Media Classic刪除，需要登錄到Adobe Target標準/特優，而不是從Adobe Target標準/特優中。

1. 編輯完成後，請在頁面右下角附近確保 **[!UICONTROL 保存後發佈]** 選中（預設）。
1. 選擇 **[!UICONTROL 保存]**，選擇儲存資料夾，輸入集的名稱，然後選擇 **[!UICONTROL 保存]**。

## 刪除聘用集 {#deleting-an-offer-set}

刪除提案集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**要刪除聘用集，請執行以下操作：**

1. 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個優惠集。
1. 在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **刪除**。

>[!MORELIKETHIS]
>
>* [建立範本參數](creating-template-parameters.md#creating_template_parameters)

