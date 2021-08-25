---
title: 建立影像集
description: 了解如何在Dynamic Media Classic中建立影像集。
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 63%

---

# 建立影像集{#creating-an-image-set}

若要建立多重視圖影像集，您需要的影像必須能夠從不同視角顯示項目，或是能夠顯示相同項目的不同面相。目標是要向檢視者呈現項目的影像，讓他們確實瞭解項目外觀或功能。

## 建立影像集 {#create}

建立集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 在儲存選]** 項後發佈再儲存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立影像集:**

1. 進行以下一項操作:

   * **先選取影像**  — 在「瀏覽」面板中，選取您要用於影像集的影像，然後前往「 **[!UICONTROL 建立]**  >影 **[!UICONTROL 像集」]**。

   * **從「影像集」畫面** 開始 — 前往「 **[!UICONTROL 建置]**  > **[!UICONTROL 影像集」]**。「影像集」畫面開啟。選取「資產庫」中的檔案夾，並將您要用於影像集的影像拖曳至「影像集」畫面。

1. 若要變更影像順序，請將影像拖曳至新位置。
1. 在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇&#x200B;**[!UICONTROL 保存]**，選擇用於儲存影像集的資料夾，輸入該集的名稱，然後選擇&#x200B;**[!UICONTROL 保存]**。
1. 若要在「影像集查看器」中查看影像集，請在「影像集」螢幕上選擇「**[!UICONTROL 預覽]**」。 您可以在「影像集查看器」中選擇色板縮略圖，以查看其行為。

## 編輯影像集 {#editing-an-image-set}

無論您編輯已發佈或未發佈的集，**[!UICONTROL 儲存後發佈]**&#x200B;選項都會以下列方式影響集和設定成員：

| 已發佈集? | **[!UICONTROL 在儲存編輯]** 之前選取儲存選項後發佈？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯影像集:**

1. 在「網格」視圖中，瀏覽到ImageSet，然後在影像下，選擇&#x200B;**[!UICONTROL Edit]**。
1. 請執行下列任一動作:

   * 若要加入影像 (已發佈或未發佈)，請將它從「增加資產」中的檔案夾拖曳到影像集的「**[!UICONTROL 檢視]**」頁面上。
   * 若要移除影像，請選取該影像，然後選取工具列上的&#x200B;**[!UICONTROL Delete]**。
   * 若要重新排序影像，請將影像拖曳至新位置。

1. 完成集的編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇&#x200B;**[!UICONTROL 保存]**，為集選擇儲存資料夾，輸入集的名稱，然後選擇&#x200B;**[!UICONTROL 保存]**。

## 刪除影像集 {#deleting-an-image-set}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除影像集:**

1. 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個「影像集」。
1. 在全局導航欄上，轉至&#x200B;**[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**。
