---
title: 處理 PSD 檔案
seo-title: 處理 PSD 檔案
description: 'null'
seo-description: 瞭解如何使用PSD檔案。
uuid: 5836b660-6bca-46e7-ab39-1a31 d1 e0 cff2
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/master_ files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbb67ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 處理 PSD 檔案{#working-with-psd-files}

PSD(Photoshop Document檔案)通常用於Dynamic Media Classic中以建立範本。當您上傳PSD檔案時，可以從檔案自動建立Dynamic Media Classic範本(選取「上傳」畫面上的「建立範本」選項)。

如果您使用檔案來建立範本，則 SPS 會從含有圖層的 PSD 檔案建立多個影像；它會為每個圖層建立一個影像。

## PSD 上載選項 {#psd-upload-options}

用來上載 PSD 檔案的選項位於「上載工作選項」的「Photoshop 選項」之下。您可以裁切檔案、選擇檔案的色彩設定檔、使用檔案來建立範本，以及選取錨點。

上載 PSD 檔案時可使用以下選項:

**裁切(** 位於「裁切選項」下)。選擇「修剪」以自動從 PSD 檔案邊緣裁切空白區域；選擇「手動」以裁切 PSD 檔案的邊緣:

**修剪** ：選取「以裁切為基礎的修剪」功能表，然後選擇「顏色」或「透明度」。

如果您選擇「色彩」選項，請選取「邊角」選單，並且選擇對所要裁切之色彩呈現最佳空白區域色彩的 PSD 邊角。

拖曳滑桿以指定容許度 (從 0 到 1):

若要根據色彩修剪，請指定 0，如此僅會在完全符合您選取的 PDF 邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。

若要根據透明度修剪，請指定 0，如此僅會在完全為透明時才會裁切像素；數值越接近 1，允許的透明度就越高。

**手動** 輸入影像的任何一側或每一側裁切的像素數目。影像裁切的多寡取決於影像檔案的 ppi (每英吋像素) 設定。例如，如果影像顯示 150 ppi，而您在「上」、「右」、「下」及「左」文字方框中輸入「75」，則會從影像的每一側裁切半英吋。

**色彩描述檔** (位於顏色描述檔選項下)。選擇一個選項:

**轉換為sRGB(預設)** 轉換為sRGB(標準紅色綠色藍色)。sRGB 是在網頁上顯示影像時建議使用的色域。

**保留原始顏色空間** 保留影像的原始色域。

**自訂從&gt;「開啓** 」功能表，您可以選擇「轉換自」和「轉換為色域」。您可以選擇標準 Photoshop 色域，或是上載至 SPS 的色域。請參閱ICC 設定檔。

**維護圖層** 將PSD中的圖層取代為個別資產。資產圖層會維持與 PSD 相關聯。在詳細檢視中開啟 PSD 檔案，然後選取圖層面板，即可予以檢視。參閱檢視和編輯 PSD 檔案中的圖層。

**建立範本** 從PSD檔案中的圖層建立範本。

**擷取文字** 擷取文字，讓使用者可以搜尋檢視器中的文字。

**將圖層延伸至背景大小** 將擷取的影像圖層大小擴展至背景圖層的大小。

**PSD檔案中的圖層命名** 圖層會上傳為個別影像。在 Scene7 Publishing System 中選擇要命名這些影像的選項:

**圖層名稱** ：在PSD檔案中的圖層名稱之後命名影像。例如，在原始 PSD 檔案中名稱為 Price Tag 的圖層會變成名稱為 Price Tag 的影像。但是，如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱 (Background、Layer 1、Layer 2 等等)，則這些影像會以 PSD 檔案中的圖層編號命名，而非預設的圖層名稱。

**Photoshop和圖層編號** 會在PSD檔案中的圖層編號後面加上影像名稱，忽略原始圖層名稱。影像會以 Photoshop 檔案名稱並附加圖層編號命名。例如，即使圖層在 Photoshop 中沒有預設名稱，但是檔案名稱為 Spring Ad.psd 的第二個圖層會被命名為 Spring Ad_2。

**Photoshop和圖層名稱** 在PSD檔案後面加上影像，後面接著圖層名稱或圖層編號。如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。例如，在 PSD 檔案 SpringAd 中名稱為 Price Tag 的圖層會命名為 Spring Ad_Price Tag。預設名稱為 Layer 2 的圖層會命名為 Spring Ad_2。

**錨點** 指定影像錨定在範本中的錨點，這些範本是由PSD檔案產生的圖層構圖所產生。預設的錨點為中心。無論替代影像的外觀比例為何，中心錨點允許替代影像以最佳方式填滿相同的空間。當參考範本並且使用替換參數時，取代此影像的不同長寬影像可有效的填滿相同的空間。如果您的應用程式需要將替代影像填滿範本中的配置空間，請變更為其他設定。

## 檢視和編輯 PSD 檔案中的圖層 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上傳PSD時選取「維護圖層」選項，Dynamic Media Classic會將個別圖層擷取到資產中。您可以在瀏覽面板中以詳細檢視開啟檔案，以檢視和編輯 PSD 檔案所屬的資產圖層。

1. 在瀏覽面板中按兩下完整的 PSD 檔案，以在詳細檢視中開啟該檔案。

   ***附註**：請確定您開啓了完整資產，而非PSD圖層。*

1. 按一下「圖層」以開啟「圖層」面板。所有圖層在「圖層」面板中皆會顯示為個別影像。
1. 按兩下圖層將其開啟，然後執行下列任一動作:

   * 按一下「影像地圖」圖示即可在圖層上建立影像地圖。(參閱[建立影像地圖](creating-image-maps.md#creating_image_maps))。
   * 按一下「縮放目標」圖示即可在圖層上建立縮放目標。(參閱[建立已導引縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom))。
   * 按一下「裁切」圖示來裁切圖層。(參閱[裁切影像](cropping-image.md#cropping_an_image)。)
   * 按一下「銳利化」以銳利化圖層。(參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。)
   * 按一下「調整」以調整圖層。(參閱[調整影像](adjusting-image.md#adjusting_an_image)。)

1. 按一下「儲存」或「另存新檔」。
1. 若要檢視或編輯其他圖層，請按一下圖層預覽底部的箭頭。
1. 若要結束圖層的詳細檢視，請按一下「格點檢視」圖示。

