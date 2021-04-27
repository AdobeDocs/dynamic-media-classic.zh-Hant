---
title: 使用 PSD 檔案
description: 瞭解如何使用PSD檔案。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media經典，資產管理
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 45%

---

# 使用 PSD 檔案{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop檔案檔)最常用於Dynamic Media經典中建立模板。 上傳PSD檔案時，您可以從檔案自動建立Dynamic Media經典範本（選取「上傳」畫面上的「建立範本」選項）。

Dynamic Media·Classic從PSD檔案建立多張影像，若您使用該檔案建立範本，則可建立圖層；它會為每個圖層建立一個影像。

## PSD 上載選項 {#psd-upload-options}

上傳PSD檔案的選項位於「上傳工作選項」對話方塊中的「Photoshop選項」下。 您可以裁切檔案、選擇檔案的色彩設定檔、使用檔案來建立範本，以及選取錨點。

上載 PSD 檔案時可使用以下選項:

* **裁切選項** -位於「裁切 **[!UICONTROL 選項」下]**。選擇「修剪」，從PSD檔案的邊緣自動裁切空白；按一下&#x200B;**[!UICONTROL Manual]**&#x200B;以裁切PSD檔案的側面：

   * **修剪** -選擇「基於 **[!UICONTROL 修剪去除」]** 的菜單，然後選擇「顏 **** 色」 **[!UICONTROL 或「透明度]**」。

      如果您選擇「色彩」選項，請選取「邊角」選單，並且選擇對所要裁切之色彩呈現最佳空白區域色彩的 PSD 邊角。

      拖動滑塊以指定0到1的公差。 若要根據色彩修剪，請指定 0，如此僅會在完全符合您選取的 PDF 邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。若要根據透明度進行修剪，請指定0以僅在像素為透明時裁切像素；接近1的數字使得透明度更高。

   * **手動** -輸入要從影像的任一側或每側裁切的像素數。影像裁切的多寡取決於影像檔案的 ppi (每英吋像素) 設定。例如，如果影像顯示 150 ppi，而您在「上」、「右」、「下」及「左」文字方框中輸入「75」，則會從影像的每一側裁切半英吋。

* **色彩描述檔選項** -位於「色彩描 **[!UICONTROL 述檔選項」下]**。

   * **預設色彩保存**

   * **保留原始色域** -保留影像的原始色域。

   * **「自訂自>至** -」開啟功能表，讓您選擇「轉換自」和「轉換至顏色空間」。您可以選擇標準的Photoshop色域或您上傳至Dynamic Media經典的色域。 請參閱[ICC 設定檔](/help/icc-profiles.md)。

* **Photoshop 選項**

   * **維護圖層** -將PSD中的圖層（如果有的話）分割為個別資產。資產圖層會維持與 PSD 相關聯。在詳細檢視中開啟 PSD 檔案，然後選取圖層面板，即可予以檢視。參閱檢視和編輯 PSD 檔案中的圖層。

   * **建立範本** -從PSD檔案中的圖層建立範本。

   * **摘取文字** -摘取文字，讓使用者在檢視器中搜尋文字。

   * **將圖層延伸至背景大小** -將擷取的影像圖層的大小延伸至背景圖層的大小。

   * **圖層命名** - PSD檔案中的圖層會上傳為個別影像。若要在Dynamic Media經典中命名這些影像，請從下列選項中選擇：

      * **圖層名稱** -在PSD檔案中的圖層名稱之後命名影像。例如，在原始 PSD 檔案中名稱為 Price Tag 的圖層會變成名稱為 Price Tag 的影像。但是，如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱 (Background、Layer 1、Layer 2 等等)，則這些影像會以 PSD 檔案中的圖層編號命名，而非預設的圖層名稱。

      * **Photoshop和圖層編號** -在PSD檔案中將影像命名為圖層編號之後，忽略原始圖層名稱。影像會以 Photoshop 檔案名稱並附加圖層編號命名。例如，名為`Spring Ad.psd`的檔案的第二層名為`Spring Ad_2`，即使它在Photoshop具有非預設名稱。

      * **Photoshop和圖層名稱** -將影像命名為PSD檔案後面的影像，後面接著圖層名稱或圖層編號。如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。例如，在名為`SpringAd`的PSD檔案中，名為`Price Tag`的層名為`Spring Ad_Price Tag`。 預設名為Layer 2的層稱為`Spring Ad_2`。
   * **錨點** -指定如何將影像錨定在範本中，範本是從PSD檔案產生的圖層構圖產生。預設的錨點為中心。無論替代影像的外觀比例為何，中心錨點允許替代影像以最佳方式填滿相同的空間。當參考範本並且使用替換參數時，取代此影像的不同長寬影像可有效的填滿相同的空間。如果您的應用程式需要將替代影像填滿範本中的配置空間，請變更為其他設定。


## 檢視和編輯 PSD 檔案中的圖層 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上傳PSD時選取了「維護圖層」選項，Dynamic Media經典會將個別圖層撕成資產。 您可以在瀏覽面板中以詳細檢視開啟檔案，以檢視和編輯 PSD 檔案所屬的資產圖層。

1. 連按兩下「瀏覽面板」中的完整PSD檔案。 檔案在「詳細資訊」(Detail)視圖中開啟。

   >[!NOTE]
   >
   >確定您開啟完整資產，而非 PSD 圖層其中的資產。

1. 按一下「**[!UICONTROL 圖層]**」。 所有圖層在「圖層」面板中皆會顯示為個別影像。
1. 連按兩下圖層，然後執行下列任一動作：

   * 若要在圖層上建立影像地圖，請按一下「影像地圖」圖示。 ****(參閱[建立影像地圖](creating-image-maps.md#creating_image_maps))。
   * 要在圖層上建立縮放目標，請按一下&#x200B;**[!UICONTROL 縮放目標]**&#x200B;表徵圖。 (參閱[建立已導引縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom))。
   * 要裁切圖層，請按一下「裁切」表徵圖。 ****(參閱[裁切影像](cropping-image.md#cropping_an_image)。)
   * 要銳利化圖層，請按一下「銳利化」。 ****(參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。)
   * 要調整圖層，請按一下「調整」。 ****(參閱[調整影像](adjusting-image.md#adjusting_an_image)。)

1. 按一下「**[!UICONTROL 儲存]**」或「**[!UICONTROL 另存新檔]**」。
1. 若要檢視或編輯其他圖層，請按一下圖層預覽底部的箭頭。
1. 要退出「圖層詳細資訊」視圖，請按一下「網格視圖」表徵圖。****
