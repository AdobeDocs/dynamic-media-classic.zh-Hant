---
title: 使用 PSD 檔案
description: 了解如何使用PSD檔案。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 41%

---

# 使用 PSD 檔案{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop檔案)最常用於AdobeDynamic Media Classic以建立範本。 上傳PSD檔案時，可以從檔案自動建立AdobeDynamic Media Classic範本（在「上傳」畫面上選取「建立範本」選項）。

AdobeDynamic Media Classic如果您使用檔案建立範本，則會從含有圖層的PSD檔案建立多個影像；它會為每個圖層建立一個影像。

## PSD 上載選項 {#psd-upload-options}

上載PSD檔案的選項位於「上載作業選項」對話框的「Photoshop選項」下。 您可以裁切檔案、選擇檔案的色彩設定檔、使用檔案來建立範本，以及選取錨點。

上載 PSD 檔案時可使用以下選項:

* **裁切選項**  — 位於裁切 **[!UICONTROL 選項下]**。選擇「修剪」以自動從PSD檔案的邊緣裁切空白；按一下&#x200B;**[!UICONTROL 手動]**&#x200B;以裁切PSD檔案的側：

   * **修剪**  — 選取「基於 **[!UICONTROL 修剪的」]** Onmenu，然後選擇「顏 **** 色」或「 **[!UICONTROL 透明度」]**。

      如果您選擇「色彩」選項，請選取「邊角」選單，並且選擇對所要裁切之色彩呈現最佳空白區域色彩的 PSD 邊角。

      拖動滑塊以指定從0到1的公差。 若要根據色彩修剪，請指定 0，如此僅會在完全符合您選取的 PDF 邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。要根據透明度進行修剪，請指定0隻在像素為透明時裁剪像素；接近1的數字使透明度更高。

   * **手動**  — 輸入要從影像的任一側或每側裁切的像素數。影像裁切的多寡取決於影像檔案的 ppi (每英吋像素) 設定。例如，如果影像顯示 150 ppi，而您在「上」、「右」、「下」及「左」文字方框中輸入「75」，則會從影像的每一側裁切半英吋。

* **色彩描述檔選項**  — 位於色彩描述檔 **[!UICONTROL 選項下方]**。

   * **預設色彩保存**

   * **保留原始顏色空間**  — 保留影像的原始顏色空間。

   * **「自訂自」>「轉換為」**  — 開啟功能表，供您選擇「轉換自」和「轉換為顏色空間」。您可以選擇標準的Photoshop色域，或上傳至AdobeDynamic Media Classic的色域。 請參閱[ICC 設定檔](/help/icc-profiles.md)。

* **Photoshop 選項**

   * **維護圖層**  — 將PSD中的圖層（如果有的話）分割為個別資產。資產圖層會維持與 PSD 相關聯。通過在「詳細視圖」中開啟PSD檔案並選取圖層面板，可以查看它們。 參閱檢視和編輯 PSD 檔案中的圖層。

   * **建立模板**  — 從PSD檔案中的圖層建立模板。

   * **擷取文字**  — 擷取文字，讓使用者能在檢視器中搜尋文字。

   * **將圖層擴展到背景大小**  — 將撕開的影像圖層的大小擴展到背景圖層的大小。

   * **圖層命名** - PSD檔案中的圖層會上傳為個別影像。若要在AdobeDynamic Media Classic中為這些影像命名，請從下列選項中選擇：

      * **圖層名稱**  — 在影像的圖層名稱后按照影像在PSD檔案中的圖層名稱命名。例如，在原始 PSD 檔案中名稱為 Price Tag 的圖層會變成名稱為 Price Tag 的影像。但是，如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱 (Background、Layer 1、Layer 2 等等)，則這些影像會以 PSD 檔案中的圖層編號命名，而非預設的圖層名稱。

      * **Photoshop和圖層號**  — 在PSD檔案中的圖層號後命名影像，忽略原始圖層名稱。影像會以 Photoshop 檔案名稱並附加圖層編號命名。例如，名為`Spring Ad.psd`的檔案的第二層名為`Spring Ad_2`，即使該檔案在Photoshop中具有非預設名稱亦然。

      * **Photoshop和圖層名稱**  — 在PSD檔案後面加上圖層名稱或圖層編號的影像名稱。如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。例如，名為`SpringAd`的PSD檔案中名為`Price Tag`的層名為`Spring Ad_Price Tag`。 名為「第2層」的預設層稱為`Spring Ad_2`。
   * **錨點**  — 指定如何將影像錨點到從PSD檔案生成的分層合成生成的模板中。預設的錨點為中心。無論替代影像的外觀比例為何，中心錨點允許替代影像以最佳方式填滿相同的空間。當參考範本並且使用替換參數時，取代此影像的不同長寬影像可有效的填滿相同的空間。如果您的應用程式需要將替代影像填滿範本中的配置空間，請變更為其他設定。


## 檢視和編輯 PSD 檔案中的圖層 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上載PSD時選擇了「維護圖層」選項，則AdobeDynamic Media Classic會將各個圖層拆分為資產。 通過在「詳細資訊視圖」的「瀏覽面板」中開啟檔案，可以查看和編輯屬於PSD檔案的資產層。

1. 按兩下「瀏覽」面板中的完整PSD檔案。 檔案在「詳細資訊視圖」中開啟。

   >[!NOTE]
   >
   >確定您開啟完整資產，而非 PSD 圖層其中的資產。

1. 按一下「**[!UICONTROL 層]**」。 所有圖層在「圖層」面板中皆會顯示為個別影像。
1. 按兩下某個圖層，然後執行下列任一操作：

   * 若要在圖層上建立影像映射，請按一下「影像映射」]**表徵圖。**[!UICONTROL (參閱[建立影像地圖](creating-image-maps.md#creating_image_maps))。
   * 要在圖層上建立縮放目標，請按一下「**[!UICONTROL 縮放目標]**」表徵圖。 (參閱[建立已導引縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom))。
   * 要裁切圖層，請按一下「**[!UICONTROL 裁切]**」表徵圖。 (參閱[裁切影像](cropping-image.md#cropping_an_image)。)
   * 要銳化圖層，請按一下「銳化」****。 (參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。)
   * 要調整圖層，請按一下&#x200B;**[!UICONTROL Adjust]**。 (參閱[調整影像](adjusting-image.md#adjusting_an_image)。)

1. 按一下「**[!UICONTROL 儲存]**」或「**[!UICONTROL 另存新檔]**」。
1. 若要檢視或編輯其他圖層，請按一下圖層預覽底部的箭頭。
1. 要退出「圖層詳細資訊視圖」，請按一下&#x200B;**[!UICONTROL 網格視圖]**&#x200B;表徵圖。
