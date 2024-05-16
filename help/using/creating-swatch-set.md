---
title: 建立色票集
description: 瞭解如何在Adobe Dynamic Media Classic中建立色票集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# 建立色票集{#creating-a-swatch-set}

色票集允許使用者以不同色彩、圖樣或飾面檢視項目。若要使用色票建立色票集，需要具有要提供給使用者的每種不同色彩、圖樣或飾面的一個影像。還需要每種色彩、圖樣或飾面的一種色彩、圖樣或飾面色票。

例如，假定要使用不同色彩的標記顯示大寫字母的影像，標記為紅色、綠色和藍色。在這種情況下，需要同一大寫字母的三種快照。一個紅色標記快照，一個綠色標記快照，以及一個藍色標記快照。還需要紅色、綠色和藍色色票。色票可作為縮圖，供使用者在色票集檢視器中選取，以檢視紅色計費、綠色計費或藍色計費的次數上限。

## 建立色票集 {#create}

建立集合時， **儲存後發佈** 選項會以下列方式影響集合與設定成員：

| **[!UICONTROL 儲存後發佈]** 儲存前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 出版 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要建立色票集：**

1. 進行以下一項操作:

   * **請先選取影像**：在「瀏覽」面板中，選取影像，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**.

   * **從色票集畫面開始**：前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**. 從資產庫中選取檔案夾，並將影像拖曳到「色票集」頁面的「檢視」區段。

1. 將色票色彩、圖樣或飾面拖曳到「色票集」頁面上的「色票」預留位置方框中。

   確保拖曳到每個預留位置裡的色彩、圖樣或飾面色票代表相鄰影像的色彩、圖樣或飾面。

1. 若要變更色票集中影像的順序，請將影像拖曳到新位置。
1. 在頁面的右下角附近，確認 **[!UICONTROL 儲存後發佈]** 已選取（預設）。
1. 選取 **[!UICONTROL 儲存]**，選取要儲存色票集的資料夾，輸入色票集名稱，然後選取 **[!UICONTROL 提交]**.
1. 若要在色票集檢視器中檢視您的色票集，請選取 **[!UICONTROL 預覽]** 在「色票集」畫面上。 您可以在「色票集檢視器」中選取色票縮圖，以檢視其行為。

## 編輯色票集 {#editing-a-swatch-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響集合與設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 是否要先儲存選取的選項，再儲存您的編輯？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈。 |
| 是 | 否 | 已發佈 | 現有整合員會保留其已發佈狀態。 在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈。 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要編輯色票集：**

1. 在「格點檢視」中，瀏覽至「色票集」，然後在影像下方選取 **[!UICONTROL 編輯]**.
1. 請執行下列任一動作:

   * 若要新增影像（已發佈或已取消發佈），請將其從「新增資產」中的資料夾拖曳至色票集的 **[!UICONTROL 檢視]** 頁面。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** （在工具列上）。
   * 若要重新排序影像，請將影像拖曳至新位置。

1. 當您完成編輯頁面右下角附近的集合時，請確定 **[!UICONTROL 儲存後發佈]** 已選取（預設）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除色票集

刪除集時，便會將集本身移到垃圾桶。不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要刪除色票集：**

1. 在「格點檢視」、「清單檢視」或「詳細資料檢視」中，選取一個或多個「色票集」。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
