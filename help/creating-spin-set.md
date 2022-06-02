---
title: 建立旋轉集
description: 瞭解如何在Adobe Dynamic Media Classic建立旋轉集。
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 54%

---

# 建立旋轉集{#creating-a-spin-set}

若要建立有效的迴轉集，請確定正確拍攝影像。通過選擇「生成」按鈕並選擇「旋轉集」，可以在Adobe Dynamic Media Classic建立旋轉集。 在「迴轉集」畫面中編輯迴轉集。

>[!NOTE]
>
>以前版本的Adobe Dynamic Media Classic沒有提供二維自旋集。 如果在以前版本的Adobe Dynamic Media Classic中建立了旋轉集，則不能先以其他名稱保存一維旋轉集。 選擇 **[!UICONTROL 另存為]** 在「旋轉集」螢幕中，輸入新名稱，以便在Adobe Dynamic Media Classic編輯。

## 迴轉集影像拍攝準則 {#guidelines-for-shooting-spin-set-images}

通常，迴轉集中的影像越多，影像的旋轉效果越好。不過，在迴轉集中加入許多影像會增加影像的載入時間。Adobe Dynamic Media Classic建議在旋轉集中拍攝影像的以下准則：

* 至少在一維自旋集中使用8-12個影像，在二維自旋集中使用16-24個影像。
* 請使用不失真的格式；建議使用 TIFF 和 PNG。
* 為所有影像建立遮色片，這樣項目將顯示在純白色或其他高對比度背景上。也可以增加陰影。
* 確保產品細節非常明亮，且位於焦點上。
* 借助人體模型或時裝模特兒為流行服飾拍攝迴轉影像。通常，人體模型要麼被蒙版（使用玻璃人體模型），要麼在影像中顯示一個風格化的人體模型/服裝。 透過定義角度的數目，可以建立模特兒迴轉集。用底板上的磁帶標籤每個角度，以便引導模型按照每個鏡頭的方向進行步驟和查看。

## 建立旋轉集 {#create}

旋轉集在Adobe Dynamic Media Classic創作或建立的順序非常重要。 根據您將影像拖放至「迴轉集」頁面中的格線時排列資產的順序，迴轉集會以特定的方向迴轉。因此，在生成器中直觀顯示資產的順序是當用戶移動其滑鼠指針或移動其手指時資產如何旋轉。

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 保存後發佈]** 選項，然後保存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

>[!NOTE]
>
>建立「旋轉集」時，Adobe建議使用以下最佳實踐准則和強制限制。
>
>* 每2D旋轉集的最大行/列數
   > 
   >   * 最佳做法：1000
   >   * 強制限制：1000


儲存迴轉集之後，可在「建置:迴轉集」頁面中使用「預覽」，以便在預設檢視器中查看迴轉集的顯示效果。

**建立迴轉集:**

1. 在 **[!UICONTROL 生成]** 下拉菜單，選擇 **[!UICONTROL 旋轉集]**。
1. 在「迴轉集大小」對話框中，設定需要的列和儲存格數。

   若要構建一維迴轉集，僅選取一列。

   若要構建二維迴轉集，選取兩列或更多列。

1. 選擇 **[!UICONTROL 確定]**。
1. 將影像拖放到迴轉集畫面上的格線中。
1. 完成時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 選擇 **[!UICONTROL 保存]**。
1. 在「儲存」對話框中，選取一個檔案夾來儲存迴轉集。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選擇 **[!UICONTROL 保存]**。

## 編輯旋轉集 {#editing-a-spin-set}

無論您編輯已發佈集還是未發佈集， **[!UICONTROL 保存後發佈]** 選項通過以下方式影響集和整合員：

| 已發佈集? | **[!UICONTROL 保存後發佈]** 的下界？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**編輯迴轉集:**

1. 選擇「旋轉集」的翻轉 **[!UICONTROL 編輯]** 按鈕
1. 請執行下列任一動作:

   * **刪除影像**  — 選擇影像，然後選擇 **[!UICONTROL 刪除]**。

   * **添加影像**  — 將影像拖到單元格中。

   * **對行重新排序（二維旋轉集）**  — 選擇行選擇器框（位於行左側），然後選擇 **[!UICONTROL 下移行]** 或 **[!UICONTROL 上移行]**。

   * **添加行和單元格**  — 在「行」框和「單元格」框中輸入一個數字，以確定每行中的行數和單元格數。

1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 保存]**，選擇儲存資料夾，輸入集的名稱，然後選擇 **[!UICONTROL 保存]**。

## 刪除旋轉集 {#deleting-a-spin-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**刪除迴轉集:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個迴轉集。
1. 在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**。
