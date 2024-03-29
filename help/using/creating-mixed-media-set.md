---
title: 建立混合媒體集
description: 瞭解如何在Adobe Dynamic Media Classic中建立混合媒體集。
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 76%

---

# 建立混合媒體集{#creating-a-mixed-media-set}

當您要在一次呈現中結合多種類型的檢視器時，請建立混合媒體集。請確定檔案、影像集、色票集和迴轉集可發佈，再將它們增加至混合媒體集。

![混合媒體集](/help/using/assets/mm_mixed_media_set.png)

## 建立混合媒體集 {#create-a-mixed-media-set}

建立集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立混合媒體集:**

1. 前往 **[!UICONTROL 建置]** > **[!UICONTROL 混合媒體集]**.
1. 將視訊、影像集、迴轉集和色票從資產庫拖曳至「混合媒體集」畫面。

   >[!NOTE]
   >
   >混合媒體集不支援檔案名稱包含下列任何字元的資產： `( ) { }`.

1. 請執行下列任一動作:

   * 若要增加音軌，請將音訊檔案從資產庫拖曳至「音軌」方框。音軌會在顯示影像時播放， 並在播放視訊時停止。
   * 若要變更媒體集的順序，請將其拖曳至「混合媒體集」畫面上的新位置。媒體集在畫面上的順序會決定使用者在混合媒體集檢視器中看到的順序 (由左至右)。
   * (選擇性) 若要在檢視器中增加自訂縮圖以代表視訊，請將影像檔案從資產庫拖曳至「縮圖」預留位置方框。

1. 在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**.
1. 選取儲存混合媒體集的資料夾，然後輸入該集的名稱。
1. 選取 **[!UICONTROL 儲存]**.

   若要檢視您的組合影像集在影像集檢視器中的外觀，請選取 **[!UICONTROL 預覽]**.

## 編輯混合媒體集 {#edit-a-mixed-media-set}

您可以編輯混合媒體集。如果您要在混合媒體集內編輯，請將其單獨開啟、編輯，然後儲存。編輯的內容會顯示在混合媒體集中。

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 已發佈集? | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯混合媒體集:**

1. 選取混合媒體集的變換 **[!UICONTROL 編輯]** 按鈕。
1. 請執行下列任一動作:

   * 若要移除專案，請選取專案並選取 **[!UICONTROL 刪除]**.
   * 若要重新排序項目，請將其拖曳至新位置。

1. 完成集的編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]** 或 **[!UICONTROL 另存為]**.

## 刪除混合媒體集 {#deleting-a-mixed-media-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除混合媒體集:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個混合媒體集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
