---
title: 設定影像預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定影像預設集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 34%

---

# 設定影像預設集{#setting-up-image-presets}

如同巨集，影像預設集是儲存於同一個名稱下的大小調整和格式指令的預先定義集合。若要瞭解影像預設集的運作方式，假設您的網站要求每個產品影像以兩種不同的大小顯示：500 × 500畫素和150 × 150畫素。 您可以建立兩個影像預設集，一個稱為「放大」，以500x500畫素顯示影像，另一個稱為「縮圖」，以150×150畫素顯示影像。 為了以「放大」和「縮圖」大小傳送影像，Dynamic Media影像伺服器會查詢「放大影像預設集」和「縮圖影像預設集」的定義。 接著，伺服器便會動態地按照每個影像預設集的大小和格式規格產生影像。

Adobe Dynamic Media Classic隨附數個「最佳實務」影像預設集，這些預設集已設定好供您使用。 管理員也可以建立影像預設集。 若要建立影像預設集，您可以從頭開始建立，也可以從現有預設集開始建立，並另存為新名稱。

從伺服器動態傳送時，縮小的影像可能會損失銳利度和細節。因此，每個影像預設集都含有格式控制項，以便在以特定大小傳送影像時將影像最佳化。這些控制項可確保影像在傳送至您的網站或應用程式時呈現銳利而清晰的影像。

## 建立影像預設集 {#creating-an-image-preset}

如果您是公司管理員，則可以建立自己的影像預設集。您可以建立影像預設集，或從Adobe Dynamic Media Classic提供的預設影像預設集開始、編輯預設集，然後以新名稱儲存。

**若要建立影像預設集：**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.

   您可以瀏覽至此畫面上的影像預設集名稱，以預覽現有影像預設集。選取影像預設集名稱時，「預覽」視窗中的範例影像會變更大小和外觀。

1. 進行以下一項操作:

   * **建立影像預設集**：選取 **[!UICONTROL 新增]**.
   * **編輯影像預設集**：瀏覽至最接近您要建立的影像預設集，然後選取 **[!UICONTROL 編輯]**.

1. 輸入影像預設集名稱。
1. 輸入寬度和高度的度量 (以像素為單位)。這些度量會決定影像傳送的大小。
1. 填入「增加預設集」或「編輯預設集」畫面。如需詳細資訊，請參閱[影像預設集選項](application-setup.md#image_preset_options)。

   Adobe Dynamic Media Classic建議從下列「最佳實務」選項開始：

   * **[!UICONTROL 格式]**：選擇JPEG或其他符合您要求的格式。 所有網頁瀏覽器都支援JPEG影像格式；它在小檔案大小和影像品質之間提供良好的平衡。 不過，JPEG影像使用有失真壓縮配置，如果壓縮設定太低，則會引入不想要的影像偽影。 因此，Adobe Dynamic Media Classic建議將壓縮品質（在滑杆上）設為75。 此設定提供了影像品質和小型檔案之間的良好平衡。

   * **[!UICONTROL 銳利化]**：請勿選取「銳利化」 (此銳利化濾鏡提供的控制力比 **[!UICONTROL 遮色片銳利化調整]** 設定)。

   * **[!UICONTROL 重新取樣模式]**：選擇 **[!UICONTROL 雙立方式]**.

   * **[!UICONTROL 遮色片銳利化調整]** (USM)：輸入下列設定：

   | 預設集類型 | 大小 | USM: 數量 | USM: 半徑 | USM: 臨界值 |
   | --- | --- | --- | --- | --- |
   | 交叉銷售 (迷你縮圖) | 75 × 75 | 1.5 | 0.8 | 5 |
   | 縮圖 | 150 × 150 | 1.1 | 1 | 5 |
   | 主影像 | 350 × 350 | 1 | 1 | 6 |
   | 放大 | 500 × 500 | 1.2 | 1.2 | 5 |

1. 選取 **[!UICONTROL 儲存]**.

Adobe Dynamic Media Classic建立影像預設集的「最佳實務」選項列於此處為一般建議；銳利化是高度主觀的。 這些「最佳實務」設定是以2000×2000主要影像為基礎；大型或小型主要檔案的設定可能不同。 如果要調整「不銳利化遮色片」設定，Adobe Dynamic Media Classic建議使用下列範圍：

* **[!UICONTROL 數量]**：介於 `.8` 和 `1.5`.

* **[!UICONTROL 半徑]**：介於 `.6` 和 `2`.

* **[!UICONTROL 臨界值]**：從 `1` 到 `6`.

若要刪除影像預設集，請在「影像預設集」畫面上選取它，然後選取「 」 **[!UICONTROL 刪除]**.

>[!MORELIKETHIS]
>
>* [建立和編輯影像預設集](application-setup.md#creating_and_editing_image_presets)
>* [影像預設集選項](application-setup.md#image_preset_options)
>* [根據影像預設集預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
