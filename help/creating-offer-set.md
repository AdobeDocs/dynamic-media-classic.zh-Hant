---
title: 建立提案集
seo-title: 建立提案集
description: 'null'
seo-description: 瞭解如何建立選件集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adcc8f
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEVENDONDEMENT_ PK/categories/target_ classic_ integration
discoiquuid: 59b6437d-c21 e-4929-9291-3032db34565
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creating an offer set{#creating-an-offer-set}

您可以建立以下各種類型的提案集:

* 視訊
* 參數化範本
* 影像

For templates, click **Add and Preview**, then set the parameters you choose. 其他提案集類型不包括參數，但仍然可以進行自訂，方法是按一下「**預覽**」，然後變更可用預設集。

Dynamic Media Classic提供編輯工具以及建立選件集。

>[!NOTE]
>
>在建立選件集之前，請確定您已將所有要用於設為Scene Publishing System的資產發佈。請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

## 提案集的類型 {#types-of-offer-sets}

從以下類型的提案集中建立一個提案集:

**影像** 您可以組合選件集的影像。每個影像在集中包含不同的選件。

**影像範本** 您可以使用「建置&gt;範本基本概念」命令，在動態媒體Classic中參數化影像範本。透過參數，可交換出及自訂範本的各個組件 (文字框中的文字、不同的影像)。對於提案集，舉例來說，您可以使用範本參數在提案集中的同一影像上建立變體。有關建立及參數化影像範本的資訊，請參閱建立範本參數。

**影片** 您可以組合選件集的視訊。每個視訊是提案集中的一個不同提案。

## 使用參數化範本建立選件集 {#creating-an-offer-set-with-a-parameterized-template}

建立提案集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要使用參數化範本建立選件集**

1. 選取範本或橫幅。
1. Click **Build** &gt; **Target Classic Offer Set**.

   Target Classic選件集頁面會列出選件集中的選件。清單中的第一項是物件。

1. 選取物件，然後按一下「**增加與預覽**」。

   頁面的左側列出了範本中的參數及參數值。

1. 變更參數值以建立提案。例如，在文字欄位中輸入不同文字、變更圖層大小、用一個影像交換另一個影像或者選擇不同的檢視器預設集。
1. 按一下「**儲存**」或「**另存新檔**」將提案儲存為提案集的一部分。

   「Target Classic選件集」頁面會列出您建立的選件。

1. 重複步驟 3 到 5 為提案集建立更多提案。
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

在關閉Target Classic選件集頁面之前，請將選件設為Target Classic。See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## 使用影像或視訊建立提案集 {#creating-an-offer-set-with-images-or-videos}

建立提案集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**使用影像或視訊建立提案集**

1. 組合選件的影像或影片。從Target Classic選件集畫面或「格點檢視」或「清單檢視」中開始，並使用下列其中一種方法：

   **Target Classic選件集畫面** 按一下「建立&gt;目標Classic選件集」。將影像或視訊拖放到畫面上。若要建立大小不同的視訊或影像，請拖入多個影像或視訊，然後逐一設定其大小。

   **格線或清單檢視** 選取影像或影片，然後按一下「建置&gt;目標Classic選件集」。

1. 也可以選取影像或視訊，然後按一下「**預覽**」。在「預覽選件」頁面上，您可以變更所選影像或視訊的大小和外觀。或者，您可以變更選件集中的所有影像或影片。

   * 選擇預設集以變更影像或視訊的外觀和大小。
   * 按一下「將所選預設集套用於全部」核取方框，將所選預設集套用到提案集中的所有提案。
   按一下「**儲存**」以儲存您對影像或視訊提案的變更。Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. 按一下「**儲存**」然後輸入提案集的名稱，並按「**儲存**」。

關閉Target Classic選件集頁面之前，請將選件設為Target Classic。See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## 編輯提案集 {#editing-an-offer-set}

根據您編輯的是已發佈的集或未發佈的集，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有的設定成員會保留其發佈狀態。您在編輯期間新增的任何新設定成員都會保留其已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯提案集**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. 在Target Classic選件集頁面中，執行下列任一項作業：

   **移除提案**

   Select the offer, and then click **Delete** to remove an offer from the set.

   **增加提案**

   新增選件的方式取決於您使用的選件集類型：

   * Templates: Click **Add &amp; Preview**, and on the Add &amp; Preview Offers page, create another offer.
   * 影像和影片：將影像或視訊拖曳至Target Classic選件集頁面。
   ***注意**：您無法刪除與促銷活動相關聯的選件集。若要刪除與促銷活動相關聯的選件集，請登入Target Classic並先移除促銷活動關聯。Even after un-associating from a campaign, the asset can only be deleted from Scene7 Publishing System, requiring a login to Target Classic, and not from within Target Classic.*

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. 按一下「**儲存**」，選取存放區檔案夾，輸入集名稱，然後按「**儲存**」。

## 刪除提案集 {#deleting-an-offer-set}

刪除提案集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除提案集**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個提案集。
1. 在全域導覽列上，按一下「**檔案** &gt; **刪除** &gt; **刪除**」。

>[!MORELIKETHIS]
>
>* [建立範本參數](creating-template-parameters.md#creating_template_parameters)

