---
title: 建立迴轉集
description: 了解如何建立回轉集。
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic，檢視器，回轉集
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 66%

---

# 建立迴轉集{#creating-a-spin-set}

若要建立有效的迴轉集，請確定正確拍攝影像。您可以在Dynamic Media Classic中建立回轉集，方法是選取「建置」按鈕並選擇「回轉集」。 在「迴轉集」畫面中編輯迴轉集。

>[!NOTE]
>
>舊版Dynamic Media Classic未提供二維回轉集。 如果您在舊版Dynamic Media Classic中建立回轉集，必須先以不同名稱儲存一維回轉集，才能加以儲存。 在「回轉集」畫面中按一下「另存新檔」 ，然後輸入新名稱，以便在Dynamic Media Classic中編輯。

## 迴轉集影像拍攝準則 {#guidelines-for-shooting-spin-set-images}

通常，迴轉集中的影像越多，影像的旋轉效果越好。不過，在迴轉集中加入許多影像會增加影像的載入時間。Dynamic Media Classic建議拍攝影像以用於回轉集的准則：

* 至少在一維回轉集中使用8-12個影像，在二維回轉集中使用16-24個影像。
* 請使用不失真的格式；建議使用 TIFF 和 PNG。
* 為所有影像建立遮色片，這樣項目將顯示在純白色或其他高對比度背景上。也可以增加陰影。
* 確保產品細節非常明亮，且位於焦點上。
* 借助人體模型或時裝模特兒為流行服飾拍攝迴轉影像。人體模型通常是蒙面的（使用玻璃人體模型），或者在影像中顯示一個風格化的人體模型/裁縫。 透過定義角度的數目，可以建立模特兒迴轉集。在地面上放置膠帶來標記每個角度，為模特兒提供指示，使其腳步和目光都朝向每個鏡頭的方向。

## 建立迴轉集 {#create}

在Dynamic Media Classic中製作或建立回轉集的順序非常重要。 根據您將影像拖放至「迴轉集」頁面中的格線時排列資產的順序，迴轉集會以特定的方向迴轉。因此，在產生器中以視覺方式顯示資產的順序，是當使用者移動滑鼠指標或移動手指時，資產的旋轉方式。

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 在儲存選]** 項後發佈再儲存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

儲存迴轉集之後，可在「建置:迴轉集」頁面中使用「預覽」，以便在預設檢視器中查看迴轉集的顯示效果。

**建立迴轉集:**

1. 在「**[!UICONTROL 建置]**」下拉式選單中，按一下「**[!UICONTROL 迴轉集]**」。
1. 在「迴轉集大小」對話框中，設定需要的列和儲存格數。

   若要構建一維迴轉集，僅選取一列。

   若要構建二維迴轉集，選取兩列或更多列。

1. 按一下&#x200B;**[!UICONTROL 「確定」]**。
1. 將影像拖放到迴轉集畫面上的格線中。
1. 完成時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。
1. 在「儲存」對話框中，選取一個檔案夾來儲存迴轉集。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

## 編輯迴轉集 {#editing-a-spin-set}

無論您編輯已發佈的集還是未發佈的集，**[!UICONTROL 儲存後發佈]**&#x200B;選項都會以下列方式影響集和整合員：

| 已發佈集? | **[!UICONTROL 在儲存編輯]** 之前選取儲存選項後發佈？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**編輯迴轉集:**

1. 按一下迴轉集的滑鼠指向效果「**[!UICONTROL 編輯]**」按鈕。
1. 請執行下列任一動作:

   * **移除影像**  — 選取影像，然後按一下「刪 **[!UICONTROL 除」]**。

   * **新增影像**  — 將影像拖曳至儲存格。

   * **重新排序列（二維回轉集）**  — 按一下列選取器方塊（位於列左側），然後按一下 **[!UICONTROL 下]** 移列或 **[!UICONTROL 上移列]**。

   * **新增列和儲存格**  — 在「列」方塊和「儲存格」方塊中輸入數字，以決定每列的列數和儲存格數。

1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 按一下「**[!UICONTROL 儲存]**」，選取存放區檔案夾，輸入集名稱，然後按「**[!UICONTROL 儲存]**」。

## 刪除迴轉集 {#deleting-a-spin-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually-publishing-assets)和[手動取消發佈資產](publishing-files.md#manually-unpublishing-assets)。

**刪除迴轉集:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個迴轉集。
1. 在全域導覽列上，按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**」。
