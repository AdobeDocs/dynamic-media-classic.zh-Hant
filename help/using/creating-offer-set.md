---
title: 建立優惠方案集
description: 瞭解如何在Adobe Dynamic Media Classic中建立優惠方案集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# 建立優惠方案集 {#creating-an-offer-set}

您可以建立下列任何型別的選件集：

* 視訊
* 參數化範本
* 影像

對於範本，請選取&#x200B;**[!UICONTROL 新增並預覽]**，然後設定您選擇的引數。 其他選件集型別不包含引數，但您仍可以透過選取&#x200B;**[!UICONTROL 預覽]**&#x200B;並變更可用的預設集來自訂這些引數。

Adobe Dynamic Media Classic提供編輯和建立選件集的工具。

>[!NOTE]
>
>建立選件集之前，請確定您將要用於選件集的所有資產發佈到Adobe Dynamic Media Classic。 請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

## 優惠方案集的型別 {#types-of-offer-sets}

從下列優惠方案集型別建立優惠方案集：

* **影像**：您可以組合選件集的影像。 每個影像在集中包含不同的選件。

* **影像範本**：您可以使用&#x200B;**[!UICONTROL 建置]** >範本基本概念命令，將Adobe Dynamic Media Classic中的影像範本引數化。 透過引數、範本的元件、文字框中的文字，以及不同的影像，都可以調出並自訂。 例如，針對優惠方案集，您可以使用範本引數在優惠方案集中的相同影像上建立變數。 如需建立與引數化影像範本的相關資訊，請參閱[建立範本引數](creating-template-parameters.md#creating_template_parameters)。

另請觀看[基本範本](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)訓練影片。

* **影片**：您可以組合選件集的影片。 每個視訊是提案集中的一個不同提案。

## 使用引數化範本建立選件集 {#creating-an-offer-set-with-a-parameterized-template}

當您建立選件集時，儲存&#x200B;**之後的** Publish選項會以下列方式影響該集和設定成員：

| 儲存前已選取儲存後&#x200B;**[!UICONTROL Publish]**&#x200B;選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要使用引數化範本建立提案集：**

1. 選取範本或橫幅。
1. 移至&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**。

   Test&amp;Target選件集頁面會列出選件集中的選件。 清單中的第一項是物件。

1. 選取物件並選取&#x200B;**[!UICONTROL 新增與預覽]**。

   頁面的左側列出了範本中的參數及參數值。

1. 變更參數值以建立提案。例如，在文字欄位中輸入不同的文字、變更圖層大小、將一個影像交換給另一個影像，或選擇不同的「檢視器預設集」。
1. 選取「**[!UICONTROL 儲存]**」或「**[!UICONTROL 另存新檔**]**」，將選件儲存為選件集的一部分。

   Test&amp;Target選件集頁面會列出您建立的選件。

1. 重複步驟 3 到 5 為提案集建立更多提案。
1. 完成時（在頁面的右下角附近），請確定已選取&#x200B;**[!UICONTROL 儲存Publish*]** （預設）。
1. 選取&#x200B;**[!UICONTROL 關閉]**，輸入選件集的名稱，然後選取&#x200B;**[!UICONTROL 儲存]**。

在關閉Test&amp;Target選件集頁面之前，請將選件集推送至Adobe Target Standard/Premium。 請參閱[將提案集推送至Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 使用影像或影片建立選件集 {#creating-an-offer-set-with-images-or-videos}

當您建立選件集時，儲存&#x200B;**之後的** Publish選項會以下列方式影響該集和設定成員：

| 儲存前已選取儲存後&#x200B;**[!UICONTROL Publish]**&#x200B;選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要建立包含影像或視訊的優惠方案集：**

1. 組合選件集的影像或視訊。 從「Test&amp;Target選件集」畫面或「格線檢視」或「清單檢視」開始，並使用下列其中一種方法：

   * **Test&amp;Target選件集畫面**：移至&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**。 將影像或視訊拖放到畫面上。若要建立大小不同的視訊或影像，請拖入多個影像或視訊，然後逐一設定其大小。

   * **格線檢視或清單檢視**：選取影像或視訊，然後前往&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**。

1. 選擇性地選取影像或視訊，然後選取&#x200B;**[!UICONTROL 預覽]**。 在「預覽選件」頁面上，您可以變更所選影像或視訊的大小和外觀。 或者，您可以變更選件集中的所有影像或視訊。

   * 選擇預設集以變更影像或視訊的外觀和大小。
   * 若要將您選擇的預設集套用至選件集中的所有選件，請選取&#x200B;**[!UICONTROL 選取預設集至全部]**&#x200B;核取方塊。

   選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存影像或視訊選件的變更。 然後選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回Test&amp;Target選件集頁面。

1. 完成建立選件集的選件並選擇不同影像的影像預設集後，請確定已選取&#x200B;**[!UICONTROL 儲存]**&#x200B;後的Publish （預設）。
1. 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;並輸入選件集的名稱，然後選取&#x200B;**[!UICONTROL 儲存]**。

在關閉Test&amp;Target選件集頁面之前，請將選件集推送至Adobe Target Standard/Premium。 請參閱[將提案集推送至Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 編輯優惠方案集 {#editing-an-offer-set}

不論您是編輯已發佈的集還是未發佈的集，**[!UICONTROL 儲存]**&#x200B;後的Publish選項都會影響該集和整合員，其影響方式如下：

| 已發佈集? | 在儲存編輯內容之前，是否已選取儲存&#x200B;**[!UICONTROL Publish]**&#x200B;選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員會保留其已發佈狀態。 在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要編輯提案集：**

1. 若要編輯選件集，請在網格檢視或清單檢視中顯示選件集，然後選取其&#x200B;**[!UICONTROL 編輯]**&#x200B;滑鼠指向效果按鈕。
1. 在Test&amp;Target選件集頁面中，執行下列任一項作業：

   * **移除選件**：選取選件，然後選取&#x200B;**[!UICONTROL 刪除]**，將選件從集移除。
   * **新增選件**：您新增選件的方式取決於您正在使用的選件集型別：
      * **範本**：選取「**[!UICONTROL 新增並預覽]**」，然後在「新增並預覽選件」頁面上建立另一個選件。
      * **影像和視訊**：將影像或視訊拖曳至Test&amp;Target選件集頁面。

   >[!NOTE]
   >
   >您無法刪除與行銷活動相關聯的優惠方案集。 若要刪除與行銷活動相關聯的優惠方案集，請先登入Adobe Target Standard/Premium並移除行銷活動關聯。 即使在與行銷活動解除關聯後，也只能從Adobe Dynamic Media Classic中刪除資產，這要求登入Adobe Target Standard/Premium，而不是從Adobe Target Standard/Premium中登入。

1. 當您完成編輯時（在頁面的右下角附近），請確定已選取儲存後的&#x200B;**[!UICONTROL Publish]** （預設）。
1. 選取&#x200B;**[!UICONTROL 儲存]**，選取儲存資料夾，輸入集合的名稱，然後選取&#x200B;**[!UICONTROL 儲存]**。

## 刪除優惠方案集 {#delet-an-offer-set}

刪除提案集時，便會將集本身移到垃圾桶。不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要刪除提案集：**

1. 在「網格檢視」、「清單檢視」或「詳細資料檢視」中，選取一個或數個選件集。
1. 在全域導覽列上，移至&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **刪除**。

>[!MORELIKETHIS]
>
>* [正在建立範本引數](creating-template-parameters.md#creating_template_parameters)
