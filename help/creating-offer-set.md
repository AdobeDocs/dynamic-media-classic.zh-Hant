---
title: 建立提案集
seo-title: 建立提案集
description: 'null'
seo-description: 瞭解如何建立選件集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 57%

---


# Creating an offer set{#creating-an-offer-set}

您可以建立以下各種類型的提案集:

* 視訊
* 參數化範本
* 影像

對於模板，按一下「添加並預覽」，然後設定您選擇的參數。 ****&#x200B;其他提案集類型不包括參數，但仍然可以進行自訂，方法是按一下「**預覽**」，然後變更可用預設集。

Dynamic Media Classic提供編輯和建立選件集的工具。

>[!NOTE]
>
>在建立選件集之前，請務必發佈您要用於該集合的所有資產，並設定為Dynamic Media Classic。 請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

## 提案集的類型 {#types-of-offer-sets}

從以下類型的提案集中建立一個提案集:

* **影**
像您可以組合選件集的影像。每張影像在集合中包含不同的選件。

* **影像**
範本您可以使用「建立>範本基礎」命令，在Dynamic Media Classic中參數化影像範本。透過參數，可交換出及自訂範本的各個組件 (文字框中的文字、不同的影像)。對於提案集，舉例來說，您可以使用範本參數在提案集中的同一影像上建立變體。有關建立及參數化影像範本的資訊，請參閱建立範本參數。

* **視**
訊您可以組合選件集的視訊。每個視訊是提案集中的一個不同提案。

## 使用參數化範本{#creating-an-offer-set-with-a-parameterized-template}建立選件集

建立提案集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要建立包含參數化範本的選件集**

1. 選取範本或橫幅。
1. 按一下「**建置** > **Test&amp;Target 提案集**」。

   「Test&amp;Target選件集」頁面會列出選件集中的選件。 清單中的第一項是物件。

1. 選取物件，然後按一下「**增加與預覽**」。

   頁面的左側列出了範本中的參數及參數值。

1. 變更參數值以建立提案。例如，在文字欄位中輸入不同文字、變更圖層大小、用一個影像交換另一個影像或者選擇不同的檢視器預設集。
1. 按一下「**儲存**」或「**另存新檔**」將提案儲存為提案集的一部分。

   「Test&amp;Target選件集」頁面會列出您建立的選件。

1. 重複步驟 3 到 5 為提案集建立更多提案。
1. 完成時，在頁面右下角附近，請確定已選取「儲存後發佈」（預設）。****
1. 按一下「關閉」，輸入選件集的名稱，然後按一下「儲存」。********

在您關閉「Test&amp;Target選件集」頁面之前，請將選件集推送至Target Standard/Premium。 請參閱[將提案集發送到 Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 使用影像或視訊建立提案集 {#creating-an-offer-set-with-images-or-videos}

建立提案集時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**使用影像或視訊建立提案集**

1. 為選件集組合影像或視訊。 從Test&amp;Target選件集畫面或「格線檢視」或「清單檢視」中開始，然後使用下列其中一種方法：

   * **Test&amp;Target選件集螢幕按**
一下 **[!UICONTROL 建置> Test&amp;Target選件集]**。將影像或視訊拖放到畫面上。若要建立大小不同的視訊或影像，請拖入多個影像或視訊，然後逐一設定其大小。

   * **格線或清單**
檢視選取影像或視訊，然後按一 **[!UICONTROL 下「建立> Test&amp;Target選件集」]**。

1. 也可以選取影像或視訊，然後按一下「**預覽**」。在「預覽選件」頁面上，您可以變更所選影像或視訊的大小和外觀。 或者，您可以變更選件集中的所有影像或影片。

   * 選擇預設集以變更影像或視訊的外觀和大小。
   * 按一下「將所選預設集套用於全部」核取方框，將所選預設集套用到提案集中的所有提案。

   按一下「**儲存**」以儲存您對影像或視訊提案的變更。然後按一下「**關閉**」回到「Test&amp;Target 提案集」頁面。

1. 完成為選件集建立選件並選擇「影像預設集」以建立不同影像後，請確定已選取「儲存後發佈」（預設）。****
1. 按一下「**儲存**」然後輸入提案集的名稱，並按「**儲存**」。

在關閉「Test&amp;Target選件集」頁面之前，請將選件集推送至Target Standard/Premium。 請參閱[將提案集發送到 Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 編輯提案集 {#editing-an-offer-set}

根據您編輯的是已發佈的集或未發佈的集，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員將保留其已發佈狀態。在編輯期間添加的任何新整合員都將保留其已發佈或未發佈狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯提案集**

1. 若要編輯選件集，請在「格線檢視」或「清單檢視」中顯示選件集，然後按一下其&#x200B;**編輯**&#x200B;變換按鈕。
1. 在「Test&amp;Target選件集」頁面中，執行下列任一動作：

   * **移除選件選**
擇選件，然後按一下 
**刪** 除以從集合中移除選件。
   * **新增選**
件新增選件的方式取決於您使用的選件集類型：
   * **範本**
點按 
**新增與預覽**，並在「新增與預覽選件」頁面上建立另一個選件。
   * **影像和視**
訊將影像或視訊拖曳至Test&amp;Target選件集頁面。
   >[!NOTE]
   >
   >您無法刪除與某個行銷活動相關的提案集。若要刪除與促銷活動關聯的選件集，請先登入Target Standard/Premium，然後移除促銷活動關聯。 即使從促銷活動取消關聯後，資產也只能從Dynamic Media Classic刪除，需要登入Target Standard/Premium，而不是從Target Standard/Premium中。

1. 編輯完成後，在頁面右下角附近，請確定已選取「儲存後發佈」（預設）。****
1. 按一下「**儲存**」，選取存放區檔案夾，輸入集名稱，然後按「**儲存**」。

## 刪除提案集  {#deleting-an-offer-set}

刪除提案集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**刪除提案集**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個提案集。
1. 在全域導覽列上，按一下「**檔案** > **刪除** > **刪除**」。

>[!MORELIKETHIS]
>
>* [建立範本參數](creating-template-parameters.md#creating_template_parameters)

