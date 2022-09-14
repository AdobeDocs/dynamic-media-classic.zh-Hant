---
title: 建立影像集
description: 了解如何在Adobe Dynamic Media Classic中建立影像集。
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 59%

---

# 建立影像集{#creating-an-image-set}

若要建立多重視圖影像集，您需要的影像必須能夠從不同視角顯示項目，或是能夠顯示相同項目的不同面相。目標是要向檢視者呈現項目的影像，讓他們確實瞭解項目外觀或功能。

## 建立影像集 {#create}

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 儲存後發佈]** 選項（儲存前）? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

當您建立影像集時，Adobe會建議下列最佳作法並強制執行下列限制：

| 限制類型 | 最佳實務 | 限制 |
| --- | --- | --- |
| 每組重複資產數 | 無重複項目 | 20 |
| 每組影像的最大數量 | 每組5-10頁影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

**建立影像集:**

1. 進行以下一項操作:

   * **首先選擇影像**  — 在「瀏覽」面板中，選取您要用於影像集的影像，請前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**.

   * **從「影像集」螢幕開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**. 「影像集」畫面開啟。選取「資產庫」中的檔案夾，並將您要用於影像集的影像拖曳至「影像集」畫面。

1. 若要變更影像順序，請將影像拖曳至新位置。
1. 在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**，選擇儲存影像集的資料夾，輸入影像集的名稱，然後選擇 **[!UICONTROL 儲存]**.
1. 若要在「影像集檢視器」中查看影像集，請選取 **[!UICONTROL 預覽]** 在「影像集」螢幕上。 您可以在「影像集查看器」中選擇色板縮略圖，以查看其行為。

## 編輯影像集 {#editing-an-image-set}

無論您編輯已發佈或未發佈的集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 在保存編輯之前選中？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯影像集:**

1. 在「網格視圖」中，瀏覽到ImageSet，然後在影像下，選擇 **[!UICONTROL 編輯]**.
1. 請執行下列任一動作:

   * 若要加入影像 (已發佈或未發佈)，請將它從「增加資產」中的檔案夾拖曳到影像集的「**[!UICONTROL 檢視]**」頁面上。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** 的上界。
   * 若要重新排序影像，請將影像拖曳至新位置。

1. 完成集的編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**，為集選擇儲存資料夾，輸入集的名稱，然後選擇 **[!UICONTROL 儲存]**.

## 刪除影像集 {#deleting-an-image-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除影像集:**

1. 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個「影像集」。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
