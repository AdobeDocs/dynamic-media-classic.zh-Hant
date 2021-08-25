---
title: 建立優惠方案集
description: 了解如何在Dynamic Media Classic中建立優惠方案集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 38%

---

# 建立優惠方案集 {#creating-an-offer-set}

您可以建立以下各種類型的提案集:

* 視訊
* 參數化範本
* 影像

對於模板，選擇&#x200B;**[!UICONTROL 添加並預覽]**，然後設定您選擇的參數。 其他選件集類型不包含參數，但您仍可以選取&#x200B;**[!UICONTROL 預覽]**&#x200B;並變更可用的預設集來自訂參數。

Dynamic Media Classic提供編輯和建立優惠方案集的工具。

>[!NOTE]
>
>建立優惠方案集之前，請務必發佈您要用於該集的所有資產，並設為Dynamic Media Classic。 請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

## 提案集的類型 {#types-of-offer-sets}

從以下類型的提案集中建立一個提案集:

* **影像**  — 您可以組合選件集的影像。每個影像在集合中包含不同的選件。

* **影像範本**  — 您可以使用「建置>範本基本概念」命令，以參數化Dynamic Media Classic中的影像範本。透過參數，可交換出及自訂範本的各個組件 (文字框中的文字、不同的影像)。對於提案集，舉例來說，您可以使用範本參數在提案集中的同一影像上建立變體。有關建立及參數化影像範本的資訊，請參閱建立範本參數。

* **影片**  — 您可以為優惠方案集組合影片。每個視訊是提案集中的一個不同提案。

## 使用參數化範本建立選件集 {#creating-an-offer-set-with-a-parameterized-template}

建立提案集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 在儲存選]** 項後發佈再儲存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要使用參數化範本建立選件集：**

1. 選取範本或橫幅。
1. 前往&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target選件集]**。

   Test&amp;Target選件集頁面會列出選件集中的選件。 清單中的第一項是物件。

1. 選擇對象並選擇&#x200B;**[!UICONTROL 添加和預覽]**。

   頁面的左側列出了範本中的參數及參數值。

1. 變更參數值以建立提案。例如，在文字欄位中輸入不同文字、變更圖層大小、用一個影像交換另一個影像或者選擇不同的檢視器預設集。
1. 選取&#x200B;**[!UICONTROL Save]**&#x200B;或&#x200B;**[!UICONTROL Save As**]** ，將選件儲存為選件集的一部分。

   「Test&amp;Target選件集」頁面會列出您建立的選件。

1. 重複步驟 3 到 5 為提案集建立更多提案。
1. 完成後，在頁面右下角附近，確定已選取「儲存後發佈」*]**（預設）。**[!UICONTROL 
1. 選擇&#x200B;**[!UICONTROL 關閉]**，輸入選件集的名稱，然後選擇&#x200B;**[!UICONTROL 保存]**。

在關閉「Test&amp;Target選件集」頁面之前，請先將選件集推送至Adobe Target Standard/Premium。 請參閱[將提案集發送到 Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 建立包含影像或影片的優惠方案集 {#creating-an-offer-set-with-images-or-videos}

建立提案集時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| **[!UICONTROL 在儲存選]** 項後發佈再儲存？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**使用影像或視訊建立提案集:**

1. 為選件集組合影像或影片。 在「Test&amp;Target選件集」畫面或「格線檢視」或「清單檢視」中開始，然後使用下列其中一種方法：

   * **Test&amp;Target選件集畫面**  — 前往「 **[!UICONTROL 建置]**  >  **[!UICONTROL Test&amp;Target選件集」]**。將影像或視訊拖放到畫面上。若要建立大小不同的視訊或影像，請拖入多個影像或視訊，然後逐一設定其大小。

   * **格線檢視或清單檢視**  — 選取影像或影片，然後前往 **[!UICONTROL 「建置]**  >  **[!UICONTROL Test&amp;Target選件集」]**。

1. 或者，選擇影像或視頻，然後選擇&#x200B;**[!UICONTROL 預覽]**。 在「預覽選件」頁面上，您可以變更所選影像或視訊的大小和外觀。 或者，您可以變更選件集中的所有影像或影片。

   * 選擇預設集以變更影像或視訊的外觀和大小。
   * 若要將您選擇的預設套用至選件集中的所有選件，請選取「選取全部的預設集」核取方塊。****

   選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您對影像或視訊選件所做的變更。 然後選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回Test&amp;Target選件集頁面。

1. 完成為選件集建立選件並選擇不同影像的影像預設集後，請確定已選取儲存&#x200B;]**後發佈（預設）。**[!UICONTROL 
1. 選擇&#x200B;**[!UICONTROL Save]**&#x200B;並輸入選件集的名稱，然後選擇&#x200B;**[!UICONTROL Save]**。

在關閉「Test&amp;Target選件集」頁面之前，請將選件集推送至Adobe Target Standard/Premium。 請參閱[推送選件集至Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 編輯優惠方案集 {#editing-an-offer-set}

無論您編輯已發佈的集還是未發佈的集，**[!UICONTROL 儲存後發佈]**&#x200B;選項都會以下列方式影響集和整合員：

| 已發佈集? | **[!UICONTROL 在儲存編輯]** 之前選取儲存選項後發佈？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要編輯優惠方案集：**

1. 若要編輯選件集，請顯示「格線」檢視或「清單」檢視中的選件集，然後選取其&#x200B;**[!UICONTROL Edit]**&#x200B;變換按鈕。
1. 在「Test&amp;Target選件集」頁面中，執行下列任一操作：

   * **移除選件**  — 選取選件，然後選取「刪 **** 除」以從集中移除選件。
   * **新增選件**  — 新增選件的方式取決於您使用的選件集類型：
      * **範本**  — 選取 **[!UICONTROL 新增和預覽]**，然後在新增和預覽選件頁面上建立另一個選件。
      * **影像和影片**  — 將影像或影片拖曳至Test&amp;Target選件集頁面。

   >[!NOTE]
   >
   >您無法刪除與某個行銷活動相關的提案集。若要刪除與促銷活動相關聯的選件集，請登入Adobe Target Standard/Premium，並先移除促銷活動關聯。 即使從促銷活動取消關聯後，資產也只能從Dynamic Media Classic中刪除，需要登入Adobe Target Standard/Premium，而不能從Adobe Target Standard/Premium中刪除。

1. 完成編輯時，在頁面右下角附近，確定已選取「儲存後發佈」 ****（預設）。
1. 選擇&#x200B;**[!UICONTROL 保存]**，選擇儲存資料夾，輸入該集的名稱，然後選擇&#x200B;**[!UICONTROL 保存]**。

## 刪除優惠方案集 {#deleting-an-offer-set}

刪除提案集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要刪除優惠方案集：**

1. 在「網格視圖」、「清單視圖」或「詳細資訊視圖」中，選擇一個或多個選件集。
1. 在全局導航欄上，轉至&#x200B;**[!UICONTROL File]** > **[!UICONTROL Delete]** > **Delete**。

>[!MORELIKETHIS]
>
>* [建立範本參數](creating-template-parameters.md#creating_template_parameters)

