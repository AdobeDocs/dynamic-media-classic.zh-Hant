---
title: 建立回轉集
description: 了解如何在Adobe Dynamic Media Classic中建立回轉集。
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 50%

---

# 建立回轉集{#creating-a-spin-set}

若要建立有效的迴轉集，請確定正確拍攝影像。您可以選取「建置」按鈕並選擇「回轉集」，在Adobe Dynamic Media Classic中建立回轉集。 在「迴轉集」畫面中編輯迴轉集。

>[!NOTE]
>
>舊版Adobe Dynamic Media Classic未提供二維回轉集。 如果您在舊版Adobe Dynamic Media Classic中建立回轉集，必須先以不同名稱儲存一維回轉集，才能加以儲存。 選擇 **[!UICONTROL 另存新檔]** 在「回轉集」畫面中輸入新名稱，以便在Adobe Dynamic Media Classic中編輯。

## 迴轉集影像拍攝準則 {#guidelines-for-shooting-spin-set-images}

一般而言，旋轉集中的影像越多，影像旋轉效果就越好。 不過，在迴轉集中加入許多影像會增加影像的載入時間。Adobe Dynamic Media Classic建議拍攝影像以用於回轉集的這些准則：

* 至少在一維回轉集中使用8-12個影像，在二維回轉集中使用16-24個影像。
* 請使用不失真的格式；建議使用 TIFF 和 PNG。
* 為所有影像建立遮色片，這樣項目將顯示在純白色或其他高對比度背景上。也可以增加陰影。
* 確保產品細節非常明亮，且位於焦點上。
* 借助人體模型或時裝模特兒為流行服飾拍攝迴轉影像。人體模型通常是蒙面的（使用玻璃人體模型），或者在影像中顯示一個風格化的人體模型/裁縫。 通過定義角度數，可以建立模型回轉集上的回轉集。 在地板上用磁帶標籤每個角度，以便引導模型按照每個拍攝的方向進行步驟和查看。

## 建立回轉集 {#create}

在Adobe Dynamic Media Classic中製作或建立回轉集的順序非常重要。 根據您將影像拖放至「迴轉集」頁面中的格線時排列資產的順序，迴轉集會以特定的方向迴轉。因此，在產生器中以視覺方式顯示資產的順序，是當使用者移動滑鼠指標或移動手指時，資產的旋轉方式。

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 儲存後發佈]** 選項（儲存前）? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

當您建立回轉集時，Adobe會建議下列最佳作法並強制執行下列限制：

| 回轉集限制類型 | 最佳實務 | 限制 |
| --- | --- | --- |
| 每2D集的最大行/列數 | 每組12-18頁圖片 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

儲存迴轉集之後，可在「建置:迴轉集」頁面中使用「預覽」，以便在預設檢視器中查看迴轉集的顯示效果。

**建立迴轉集:**

1. 在 **[!UICONTROL 建置]** 下拉式功能表，選取 **[!UICONTROL 回轉集]**.
1. 在「迴轉集大小」對話框中，設定需要的列和儲存格數。

   若要構建一維迴轉集，僅選取一列。

   若要構建二維迴轉集，選取兩列或更多列。

1. 選擇 **[!UICONTROL 確定]**.
1. 將影像拖放到迴轉集畫面上的格線中。
1. 完成時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**.
1. 在「儲存」對話框中，選取一個檔案夾來儲存迴轉集。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選擇 **[!UICONTROL 儲存]**.

## 編輯回轉集 {#editing-a-spin-set}

無論您編輯已發佈的集或未發佈的集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 在保存編輯之前選中？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**編輯迴轉集:**

1. 選取回轉集的變換 **[!UICONTROL 編輯]** 按鈕。
1. 請執行下列任一動作:

   * **移除影像**  — 選取影像，然後選取 **[!UICONTROL 刪除]**.

   * **新增影像**  — 將影像拖曳至儲存格。

   * **重新排序列（二維回轉集）**  — 選取列選取器方塊（位於列左側），然後選取 **[!UICONTROL 向下移動行]** 或 **[!UICONTROL 上移行]**.

   * **新增列和儲存格**  — 在「行」框和「單元格」框中輸入一個數字，以確定每行的行數和單元格數。

1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 儲存]**，選擇儲存資料夾，輸入該集的名稱，然後選擇 **[!UICONTROL 儲存]**.

## 刪除回轉集 {#deleting-a-spin-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**刪除迴轉集:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個迴轉集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
