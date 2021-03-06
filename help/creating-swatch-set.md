---
title: 建立色票集
description: 了解如何在Adobe Dynamic Media Classic中建立色票集。
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: fe2aef174299366fc88309679ae29cc99e3d7f98
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 67%

---

# 建立色票集{#creating-a-swatch-set}

色票集允許使用者以不同色彩、圖樣或飾面檢視項目。若要使用色票建立色票集，需要具有要提供給使用者的每種不同色彩、圖樣或飾面的一個影像。還需要每種色彩、圖樣或飾面的一種色彩、圖樣或飾面色票。

例如，假定要使用不同色彩的標記顯示大寫字母的影像，標記為紅色、綠色和藍色。在這種情況下，需要同一大寫字母的三種快照。一個紅色標記快照，一個綠色標記快照，以及一個藍色標記快照。還需要紅色、綠色和藍色色票。顏色色板用作用戶在「色板集查看器」中選擇的縮略圖，以查看紅色、綠色或藍色的大寫。

## 建立色票集 {#create}

建立集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 儲存後發佈]** 選項（儲存前）? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 出版 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立色票集:**

1. 進行以下一項操作:

   * **首先選擇影像**  — 在「瀏覽」面板中，選取影像，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**.

   * **從「色票集」螢幕開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**. 從資產庫中選取檔案夾，並將影像拖曳到「色票集」頁面的「檢視」區段。

1. 將色票色彩、圖樣或飾面拖曳到「色票集」頁面上的「色票」預留位置方框中。

   確保拖曳到每個預留位置裡的色彩、圖樣或飾面色票代表相鄰影像的色彩、圖樣或飾面。

1. 若要變更色票集中影像的順序，請將影像拖曳到新位置。
1. 在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**，選擇儲存色板的資料夾「色板集」，輸入該集的名稱，然後選擇 **[!UICONTROL 提交]**.
1. 要在「色票集查看器」中查看色票集，請選擇 **[!UICONTROL 預覽]** 在「色票集」螢幕上。 您可以在「色票集查看器」中選擇色票縮略圖，以查看其行為。

## 編輯色票集 {#editing-a-swatch-set}

無論您編輯已發佈或未發佈的集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 已發佈集? | **[!UICONTROL 在之後發佈]** 儲存編輯前已選取儲存選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯色票集:**

1. 在「網格視圖」中，瀏覽到色票集，然後在影像下，選擇 **[!UICONTROL 編輯]**.
1. 請執行下列任一動作:

   * 若要加入影像 (已發佈或未發佈)，請將它從「增加資產」中的檔案夾拖曳到色票集的「**[!UICONTROL 檢視]**」頁面上。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** 的上界。
   * 若要重新排序影像，請將影像拖曳至新位置。

1. 完成集的編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**，選擇儲存資料夾，輸入該集的名稱，然後選擇 **[!UICONTROL 儲存]**.

## 刪除色票集 {#deleting-a-swatch-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除色票集:**

1. 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個色板集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
