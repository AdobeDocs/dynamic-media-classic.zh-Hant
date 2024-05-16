---
title: 建立迴轉集
description: 瞭解如何在Adobe Dynamic Media Classic中建立迴轉集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 44%

---

# 建立迴轉集{#creating-a-spin-set}

若要建立有效的迴轉集，請確定正確拍攝影像。您可以選取「建立」按鈕並選擇「迴轉集」，在Adobe Dynamic Media Classic中建立迴轉集。 在「迴轉集」畫面中編輯迴轉集。

>[!NOTE]
>
>舊版Adobe Dynamic Media Classic未提供二維迴轉集。 如果您在舊版Adobe Dynamic Media Classic中建立迴轉集，則必須先以其他名稱儲存一維迴轉集。 選取 **[!UICONTROL 另存為]** 在「迴轉集」畫面中，輸入新名稱以便在Adobe Dynamic Media Classic中編輯。

## 迴轉集影像拍攝準則 {#guidelines-for-shooting-spin-set-images}

一般而言，迴轉集中的影像越多，影像旋轉效果就越好。 不過，在迴轉集中加入許多影像會增加影像的載入時間。Adobe Dynamic Media Classic建議您在拍攝要用於迴轉集的影像時遵循以下准則：

* 在一維迴轉集中最少使用 8 到 12 張影像，在二維迴轉集中最少使用 16 到 24 張影像。
* 請使用不失真的格式；建議使用 TIFF 和 PNG。
* 為所有影像建立遮色片，這樣項目將顯示在純白色或其他高對比度背景上。也可以增加陰影。
* 確保產品細節非常明亮，且位於焦點上。
* 借助人體模型或時裝模特兒為流行服飾拍攝迴轉影像。通常，人體模型會被遮罩（使用玻璃人體模型），或樣式化的人體模型/服裝模型會顯示在影像中。 您可以定義角度數來建立模型上的旋轉集。 在地板上用膠帶標籤每個角度，這樣您就可以引導模型步進，並檢視每個拍攝的方向。

## 建立迴轉集 {#create}

在Adobe Dynamic Media Classic中製作或建立迴轉集的順序很重要。 在將影像拖放至「迴轉集」頁面的格線時，根據您排序資產的方式，迴轉集會以特定方向迴轉。 因此，當使用者移動滑鼠指標或移動他們的手指（由左至右）時，資產在產生器中視覺顯示的順序就是資產的旋轉方式。

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 儲存後發佈]** 儲存前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

建立迴轉集時，Adobe會建議下列最佳作法並強制執行下列限制：

| 迴轉集限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每個2D集的最大列/欄數 | 每組12至18個影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/using/limitations.md).

儲存迴轉集之後，可在「建置:迴轉集」頁面中使用「預覽」，以便在預設檢視器中查看迴轉集的顯示效果。

**若要建立迴轉集：**

1. 在 **[!UICONTROL 建置]** 下拉式功能表，選取 **[!UICONTROL 迴轉集]**.
1. 在「迴轉集大小」對話框中，設定需要的列和儲存格數。

   若要構建一維迴轉集，僅選取一列。

   若要構建二維迴轉集，選取兩列或更多列。

1. 選取 **[!UICONTROL 確定]**.
1. 將影像拖放到迴轉集畫面上的格線中。
1. 完成時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 選取 **[!UICONTROL 儲存]**.
1. 在「儲存」對話框中，選取一個檔案夾來儲存迴轉集。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選取 **[!UICONTROL 儲存]**.

## 編輯迴轉集 {#editing-a-spin-set}

無論您是編輯已發佈集合還是未發佈集合， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響集合與設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員會保留其已發佈狀態。 在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**若要編輯迴轉集：**

1. 選取迴轉集的變換影像 **[!UICONTROL 編輯]** 按鈕。
1. 請執行下列任一動作:

   * **移除影像**：選取影像，然後選取 **[!UICONTROL 刪除]**.

   * **新增影像**：將影像拖曳至儲存格。

   * **重新排序列（二維迴轉集）**：選取列選擇器方塊（位於列左側），然後選取 **[!UICONTROL 將列下移]** 或 **[!UICONTROL 將列上移]**.

   * **新增列和儲存格**：在「列」方塊和「儲存格」方塊中輸入數字，以決定每列的列數和儲存格數。

1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除迴轉集

刪除集時，便會將集本身移到垃圾桶。不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**若要刪除迴轉集：**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個迴轉集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
