---
title: 設定影像預設集
description: 了解如何設定影像預設集。
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic，影像預設集
role: Business Practitioner
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 66%

---

# 設定影像預設集{#setting-up-image-presets}

如同巨集，影像預設集是儲存於同一個名稱下的大小調整和格式指令的預先定義集合。為了瞭解影像預設集如何運作，假設您的網站需要將每個產品影像以兩種不同大小顯示: 500 x 500 像素和 150 x 150 像素。您建立了兩個影像預設集，一個名為「放大」，以 500 x 500 像素顯示影像，另一個則名為「縮圖」，以 150 x 150 像素顯示影像。為了以「放大」和「縮圖」大小傳送影像，Dynamic Media影像伺服器會查找放大影像預設集和縮圖影像預設集的定義。 接著，伺服器便會動態地按照每個影像預設集的大小和格式規格產生影像。

Dynamic Media Classic隨附數個已設定供您使用的「最佳實務」影像預設集。 管理員也可以建立新的影像預設集。若要建立影像預設集，您可以從頭開始建立，也可以從現有預設集開始建立，並另存為新名稱。

從伺服器動態傳送時，縮小的影像可能會損失銳利度和細節。因此，每個影像預設集都含有格式控制項，以便在以特定大小傳送影像時將影像最佳化。傳送影像至網站或應用程式時，這些控制項能夠確保您的影像銳利且清晰。

## 建立影像預設集 {#creating-an-image-preset}

如果您是公司管理員，則可以建立自己的影像預設集。您可以建立新的影像預設集，或從Dynamic Media Classic提供的預設影像預設集開始、編輯，然後以新名稱儲存。

**建立影像預設集:**

1. 按一下「**設定** > **影像預設集**」。

   您可以瀏覽至此畫面上的影像預設集名稱，以預覽現有影像預設集。選取影像預設集名稱時，「預覽」視窗中的範例影像會變更大小和外觀。

1. 進行以下一項操作:

   * **建立影像預**
設集按一下新增。

   * **編輯影像預**
設集瀏覽至最像您要建立的影像預設集，然後按一下「編輯」。

1. 輸入影像預設集名稱。
1. 輸入寬度和高度的度量 (以像素為單位)。這些度量會決定影像傳送的大小。
1. 填入「增加預設集」或「編輯預設集」畫面。如需詳細資訊，請參閱[影像預設集選項](application-setup.md#image_preset_options)。

   Dynamic Media Classic建議從以下「最佳實務」選項開始：

   * ****
格式選擇JPEG或其它符合您要求的格式。所有網頁瀏覽器都支援JPEG影像格式；它在小檔案大小和影像品質之間提供良好的平衡。但是，JPEG格式影像使用有損壓縮方案，如果壓縮設定太低，則該壓縮方案會引入不想要的影像偽影。因此，Dynamic Media Classic建議將壓縮品質（在滑桿上）設為75。 此設定在影像品質和檔案大小之間取得良好的平衡。

   * ****
銳利化請勿選取「銳利化」（此銳利化濾鏡提供的控制力比「銳利化遮色片」設定少）。

   * **重新**
示例模式選擇雙立方。

   * **遮色片銳利化(USM)選**
項輸入此處顯示的設定：
   | 預設集類型 | 大小 | USM: 數量 | USM: 半徑 | USM: 臨界值 |
   |--- |--- |--- |--- |--- |
   | 交叉銷售 (迷你縮圖) | 75 x 75 | 1.5 | 0.8 | 5 |
   | 縮圖 | 150 x 150 | 1.1 | 1 | 5 |
   | 主影像 | 350 x 350 | 1 | 1 | 6 |
   | 放大 | 500 x 500 | 1.2 | 1.2 | 5 |

1. 按一下&#x200B;**「儲存」**。

此處所列的Dynamic Media Classic建立影像預設集的「最佳實務」選項為一般建議；銳利化是高度主觀的。 這些「最佳實踐」設定是基於 2000 x 2000 主影像；更大或更小主影像的設定則可能有所不同。如果您要調整「遮色片銳利化」設定，Dynamic Media Classic建議以下範圍：

* ****
金額介於。8和1.5之間。

* ****
Radius介於。6和2之間。

* ****
臨界值1-6。

若要刪除影像預設集，請在「影像預設集」畫面上加以選取，然後選取「刪除」按鈕。

>[!MORELIKETHIS]
>
>* [建立和編輯影像預設集](application-setup.md#creating_and_editing_image_presets)
* [影像預設集選項](application-setup.md#image_preset_options)
* [依據影像預設集來預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

