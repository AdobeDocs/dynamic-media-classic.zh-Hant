---
title: 設定影像預設
description: 瞭解如何在Adobe Dynamic Media Classic設定影像預設。
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 50%

---

# 設定影像預設{#setting-up-image-presets}

如同巨集，影像預設集是儲存於同一個名稱下的大小調整和格式指令的預先定義集合。要瞭解「影像預設」的工作原理，假設網站要求每個產品影像以兩種不同大小顯示：500 x 500像素和150 x 150像素。 您建立了兩個影像預設集，一個名為「放大」，以 500 x 500 像素顯示影像，另一個則名為「縮圖」，以 150 x 150 像素顯示影像。要以「放大」和「縮略圖」大小傳送影像，Dynamic Media影像伺服器會查找「放大影像預設」和「縮略圖影像預設」的定義。 接著，伺服器便會動態地按照每個影像預設集的大小和格式規格產生影像。

Adobe Dynamic Media Classic提供了幾個「最佳實踐」影像預設，這些預設已經為您設定，供您使用。 管理員也可以建立「影像預設」。 若要建立影像預設集，您可以從頭開始建立，也可以從現有預設集開始建立，並另存為新名稱。

從伺服器動態傳送時，縮小的影像可能會損失銳利度和細節。因此，每個影像預設集都含有格式控制項，以便在以特定大小傳送影像時將影像最佳化。傳送影像至網站或應用程式時，這些控制項能夠確保您的影像銳利且清晰。

## 建立影像預設 {#creating-an-image-preset}

如果您是公司管理員，則可以建立自己的影像預設集。您可以建立「影像預設」或以Adobe Dynamic Media Classic提供的預設「影像預設」開頭，編輯該預設，並用新名稱保存。

**建立影像預設集:**

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設]**。

   您可以瀏覽至此畫面上的影像預設集名稱，以預覽現有影像預設集。選取影像預設集名稱時，「預覽」視窗中的範例影像會變更大小和外觀。

1. 進行以下一項操作:

   * **建立影像預設**  — 選擇 **[!UICONTROL 添加]**。
   * **編輯影像預設**  — 瀏覽到最類似於要建立的影像預設，然後選擇 **[!UICONTROL 編輯]**。

1. 輸入影像預設集名稱。
1. 輸入寬度和高度的度量 (以像素為單位)。這些度量會決定影像傳送的大小。
1. 填入「增加預設集」或「編輯預設集」畫面。如需詳細資訊，請參閱[影像預設集選項](application-setup.md#image_preset_options)。

   Adobe Dynamic Media Classic建議從以下「最佳實踐」選項開始：

   * **[!UICONTROL 格式]**  — 選擇符合您要求的JPEG或其他格式。 所有網路瀏覽器皆支援 JPEG 影像格式；它在小型檔案和影像品質之間取得了良好的平衡。然而，JPEG 格式影像使用了會失真的壓縮配置，如果壓縮設定過低可能會導致不必要的影像不自然感。因此，Adobe Dynamic Media Classic建議將壓縮質量（滑塊上）設為75。 此設定提供了影像品質和小型檔案之間的良好平衡。

   * **[!UICONTROL 銳化]**  — 不選擇銳化(此銳化濾鏡提供的控制少於 **[!UICONTROL 反銳化掩碼]** )。

   * **[!UICONTROL 重新取樣模式]**  — 選擇 **[!UICONTROL 雙立方]**。

   * **[!UICONTROL 反銳化掩碼]** (USM) — 輸入以下設定：

   | 預設集類型 | 大小 | USM: 數量 | USM: 半徑 | USM: 臨界值 |
   | --- | --- | --- | --- | --- |
   | 交叉銷售 (迷你縮圖) | 75 x 75 | 1.5 | 0.8 | 5 |
   | 縮圖 | 150 x 150 | 1.1 | 1 | 5 |
   | 主影像 | 350 x 350 | 1 | 1 | 6 |
   | 放大 | 500 x 500 | 1.2 | 1.2 | 5 |

1. 選擇 **[!UICONTROL 保存]**。

此處列出的建立影像預設的Adobe Dynamic Media Classic「最佳實踐」選項是一般性建議；銳化是高度主觀的。 這些「最佳實踐」設定基於2000 x 2000主映像；大或小主檔案的設定可以不同。 如果要調整「反銳屏蔽」設定，Adobe Dynamic Media Classic建議使用以下範圍：

* **[!UICONTROL 金額]**  — 介於。8和1.5之間。

* **[!UICONTROL 半徑]**  — 介於。6和2之間。

* **[!UICONTROL 閾值]**  — 從1到6。

要刪除影像預設，請在「影像預設」螢幕上將其選中，然後選擇 **[!UICONTROL 刪除]**。

>[!MORELIKETHIS]
>
>* [建立和編輯影像預設集](application-setup.md#creating_and_editing_image_presets)
>* [影像預設集選項](application-setup.md#image_preset_options)
>* [根據影像預設預覽影像資源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

