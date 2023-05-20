---
title: 使用PSD檔案
description: 瞭解如何處理Adobe Dynamic Media Classic的PSD檔案。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# 使用PSD檔案{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop文檔檔案)在Adobe Dynamic Media Classic最常用於建立模板。 上載PSD檔案時，可以自動從檔案建立Adobe Dynamic Media Classic模板（選擇「上載」螢幕上的「建立模板」選項）。

Adobe Dynamic Media Classic會使用檔案建立模板，從包含圖層的PSD檔案建立多個影像；它為每個圖層建立一個影像。

## PSD 上載選項 {#psd-upload-options}

上載PSD檔案的選項位於「上載作業選項」對話框的「Photoshop選項」下。 您可以裁切檔案、選擇檔案的色彩設定檔、使用檔案來建立範本，以及選取錨點。

上載 PSD 檔案時可使用以下選項:

* **裁剪選項**  — 位於 **[!UICONTROL 裁剪選項]**。 選擇 **[!UICONTROL 修剪]** 自動從PSD檔案邊緣裁剪空白；選擇 **[!UICONTROL 手動]** 裁剪PSD檔案的邊：

   * **[!UICONTROL 修剪]**  — 選擇 **[!UICONTROL 基於]** ，然後選擇 **[!UICONTROL 顏色]** 或 **[!UICONTROL 透明度]**。
   如果選擇 **[!UICONTROL 顏色]** 選項，選擇「拐角」菜單，然後選擇PSD的拐角，該顏色最能代表要裁剪的空白顏色。

   拖動滑塊以指定0到1的公差。 若要根據色彩修剪，請指定 0，如此僅會在完全符合您選取的 PDF 邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。要基於透明度進行裁切，請指定0以僅在像素為透明時裁剪像素；接近1的數字允許更透明。

   * **[!UICONTROL 手動]**  — 輸入要從影像的任何一側或每一側裁剪的像素數。 影像裁切的多寡取決於影像檔案的 ppi (每英吋像素) 設定。例如，如果影像顯示150 ppi，而您在「頂部」、「右側」、「底部」和「左側」文本框中輸入75，則輸入0.5。 從影像的每側裁切。


* **顏色配置檔案選項**  — 位於 **[!UICONTROL 顏色配置檔案選項]**。

   * **[!UICONTROL 預設色彩保存]**

   * **[!UICONTROL 保留原始顏色空間]**  — 保留影像的原始顏色空間。

   * **[!UICONTROL 自定義自]** > **[!UICONTROL 至]**  — 開啟菜單，以便選擇「轉換自」和「轉換至」顏色空間。 您可以選擇標準的Photoshop色彩空間或上載到Adobe Dynamic Media Classic的色彩空間。 請參閱[ICC 設定檔](/help/icc-profiles.md)。

* **Photoshop 選項**

   * **[!UICONTROL 維護層]**  — 將PSD中的層（如果有）拆分為單個資產。 資產圖層會維持與 PSD 相關聯。可通過在「詳細資訊視圖」中開啟PSD檔案並選擇層面板來查看它們。 參閱檢視和編輯 PSD 檔案中的圖層。

   * **[!UICONTROL 建立模板]**  — 從PSD檔案中的層建立模板。

   * **[!UICONTROL 提取文本]**  — 提取文本，以便用戶可以在查看器中搜索文本。

   * **[!UICONTROL 將圖層擴展到背景大小]**  — 將撕開的影像圖層的大小擴展到背景圖層的大小。

   * **[!UICONTROL 層命名]** -PSD檔案中的圖層將作為單獨的影像上載。 要在Adobe Dynamic Media Classic命名這些映像，請從以下選項中選擇：

      * **[!UICONTROL 層名稱]**  — 在PSD檔案中將影像命名為圖層名稱。 例如，在原始 PSD 檔案中名稱為 Price Tag 的圖層會變成名稱為 Price Tag 的影像。但是，如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱（背景、第1層、第2層等），則這些影像將以其在PSD檔案中的圖層編號命名。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshop和層號]**  — 在PSD檔案中將影像命名為圖層編號，忽略原始圖層名稱。 影像會以 Photoshop 檔案名稱並附加圖層編號命名。例如，檔案的第二層 `Spring Ad.psd` 命名 `Spring Ad_2` 即使在Photoshop有個非預設名稱。

      * **[!UICONTROL Photoshop和層名]**  — 將影像命名為PSD檔案後面的圖層名稱或圖層編號。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。例如，名為 `Price Tag` 在名為 `SpringAd` 命名 `Spring Ad_Price Tag`。 調用預設名為「層2」的層 `Spring Ad_2`。
   * **[!UICONTROL 錨點]**  — 指定如何將影像定位到從PSD檔案生成的分層合成生成的模板中。 預設的錨點為中心。無論替代影像的外觀比例為何，中心錨點允許替代影像以最佳方式填滿相同的空間。當參考範本並且使用替換參數時，取代此影像的不同長寬影像可有效的填滿相同的空間。如果您的應用程式需要將替代影像填滿範本中的配置空間，請變更為其他設定。


## 查看和編輯PSD檔案中的層 {#viewing-and-editing-layers-in-a-psd-file}

如果在上載PSD時選擇了「維護層」選項，則Adobe Dynamic Media Classic會將各個層拆分為資產。 通過在「詳細視圖」的「瀏覽面板」中開啟檔案，可以查看和編輯屬於PSD檔案的資產層。

>[!NOTE]
>
>Adobe Dynamic Media Classic在嵌套圖層組中支援多達五個級別。

1. 按兩下「瀏覽面板」中的完整PSD檔案。 檔案在「詳細資訊視圖」(Detail View)中開啟。

   >[!NOTE]
   >
   >確定您開啟完整資產，而非 PSD 圖層其中的資產。

1. 選擇 **[!UICONTROL 層]**。 所有圖層在「圖層」面板中皆會顯示為個別影像。
1. 按兩下某個圖層並執行下列任一操作：

   * 要在圖層上建立影像映射，請選擇 **[!UICONTROL 影像映射]** 表徵圖 (請參閱 [建立影像映射](creating-image-maps.md#creating_image_maps)。)
   * 要在圖層上建立縮放目標，請選擇 **[!UICONTROL 縮放目標]** 表徵圖 (請參閱 [為引導縮放建立縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。)
   * 要裁剪圖層，請選擇 **[!UICONTROL 裁剪]** 表徵圖 (請參閱 [裁剪影像](cropping-image.md#cropping_an_image)。)
   * 要銳化圖層，請選擇 **[!UICONTROL 銳化]**。 (請參閱 [銳化影像](sharpening-image.md#sharpening_an_image)。)
   * 要調整圖層，請選擇 **[!UICONTROL 調整]**。 (請參閱 [調整影像](adjusting-image.md#adjusting_an_image)。)

1. 選擇 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存為]**。
1. 要查看或編輯其他層，請在層預覽底部選取一個箭頭。
1. 要退出層「細節視圖」(Detail View)，請選擇 **[!UICONTROL 網格視圖]** 表徵圖
