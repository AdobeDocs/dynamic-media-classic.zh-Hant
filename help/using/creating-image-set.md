---
title: 建立影像集
description: 瞭解如何在Adobe Dynamic Media Classic中建立影像集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 0e1b2e9dcbee182f3ec0da53b56b5b8d3eb29cce
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 46%

---

# 建立影像集{#creating-an-image-set}

若要建立多重視圖影像集，您需要的影像必須能夠從不同視角顯示項目，或是能夠顯示相同項目的不同面相。目標是要向檢視者呈現項目的影像，讓他們確實瞭解項目外觀或功能。

## 建立影像集 {#create}

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 儲存後發佈]** 儲存前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

建立影像集時，Adobe會建議下列最佳作法並強制進行下列限制：

| 限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每個集的重複資產數 | 無重複專案 | 20‡ |
| 每組影像的最大數量 | 每組5至10個影像 | 1000 |

‡最佳實務是集合中不要有重複的資產。 單一資產的限製為20個重複專案。 如果您為該資產新增另一個重複專案（在該集合內），請求會傳回錯誤或忽略重複專案。

另請參閱 [Dynamic Media限制](/help/using/limitations.md).

**若要建立影像集：**

1. 進行以下一項操作:

   * **請先選取影像**  — 在「瀏覽」面板中，選取您想用於影像集的影像，前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**.

   * **從影像集畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**. 「影像集」畫面開啟。選取「資產庫」中的檔案夾，並將您要用於影像集的影像拖曳至「影像集」畫面。

1. 若要變更影像順序，請將影像拖曳至新位置。
1. 在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**，選取儲存影像集的資料夾，輸入影像集的名稱，然後選取 **[!UICONTROL 儲存]**.
1. 若要在影像集檢視器中檢視您的影像集，請選取 **[!UICONTROL 預覽]** 在「影像集」畫面上。 您可以在「影像集檢視器」中選取色票縮圖，以檢視其行為。

## 編輯影像集 {#editing-an-image-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響集合與設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員會保留其已發佈狀態。 在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要編輯影像集：**

1. 在「格點檢視」中，瀏覽至影像集，然後在影像下方選取 **[!UICONTROL 編輯]**.
1. 請執行下列任一動作:

   * 若要新增影像（已發佈或已取消發佈），請從新增資產中的資料夾將其拖曳至影像集的 **[!UICONTROL 檢視]** 頁面。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** （在工具列上）。
   * 若要重新排序影像，請將影像拖曳至新位置。

1. 完成集的編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**，為您的集合選取儲存資料夾，輸入集合名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除影像集 {#deleting-an-image-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要刪除影像集：**

1. 在「格點檢視」、「清單檢視」或「詳細資料檢視」中，選取一個或多個影像集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
