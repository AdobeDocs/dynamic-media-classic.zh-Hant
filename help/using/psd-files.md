---
title: 使用PSD檔案
description: 瞭解如何在Adobe Dynamic Media Classic中使用PSD檔案。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 21%

---

# 使用PSD檔案{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD (Photoshop檔案檔案)最常用於Adobe Dynamic Media Classic中建立範本。 上傳PSD檔案時，您可以從檔案自動建立Adobe Dynamic Media Classic範本（在「上傳」畫面上選取「建立範本」選項）。

如果您使用包含圖層的PSD檔案來建立範本，Adobe Dynamic Media Classic會從該檔案建立多個影像；它會為每個圖層建立一個影像。

## PSD 上載選項 {#psd-upload-options}

上傳PSD檔案的選項位於「上傳工作選項」對話方塊中的「Photoshop選項」下。 您可以裁切檔案、選擇檔案的色彩設定檔、使用檔案來建立範本，以及選取錨點。

上載 PSD 檔案時可使用以下選項:

* **裁切選項**：位於 **[!UICONTROL 裁切選項]**. 選取 **[!UICONTROL Trim]** 因此您可以從PSD檔案的邊緣自動裁切空白字元。 選取 **[!UICONTROL 手動]** 裁切PSD檔案的側邊：

   * **[!UICONTROL Trim]**：選取 **[!UICONTROL 修剪依據]** 功能表，然後選擇 **[!UICONTROL 顏色]** 或 **[!UICONTROL 透明度]**.

  如果您選擇 **[!UICONTROL 顏色]** 選項，選取「轉角」功能表，然後選取最能代表您要裁切之空白顏色的PSD轉角。

  拖曳滑桿以指定從0到1的公差。 若要根據色彩修剪，請指定 0，如此僅會在完全符合您選取的 PDF 邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。若要根據透明度進行裁剪，請指定0以裁切透明畫素；接近1的數字可提供更高的透明度。

   * **[!UICONTROL 手動]**：輸入要從影像任何一側或每側裁切的畫素數。 影像裁切的多寡取決於影像檔案的 ppi (每英吋像素) 設定。例如，假設影像顯示150 ppi。 然後在「上」、「右」、「下」和「左」文字方塊中輸入75。 影像每一面都會被裁切，0.5英吋。

* **色彩設定檔選項**：位於 **[!UICONTROL 色彩設定檔選項]**.

   * **[!UICONTROL 預設色彩儲存]**

   * **[!UICONTROL 保留原始色域]**：保留影像的原始色域。

   * **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**：開啟選單，讓您能夠選擇「轉換自」和「轉換至」色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。 請參閱[ICC 設定檔](/help/using/icc-profiles.md)。

* **Photoshop選項**

   * **[!UICONTROL 保留圖層]**：將PSD中的圖層（如果有的話）擷取至個別資產。 資產圖層會維持與 PSD 相關聯。您可以在「詳細資料檢視」中開啟PSD檔案，並選取圖層面板來檢視它們。 請參閱在PSD檔案中檢視和編輯圖層。

   * **[!UICONTROL 建立範本]**：從PSD檔案中的圖層建立範本。

   * **[!UICONTROL 擷取文字]**：擷取文字，讓使用者可在檢視器中搜尋文字。

   * **[!UICONTROL 將圖層延伸至背景大小]**：將擷取的影像圖層大小延伸至背景圖層的大小。

   * **[!UICONTROL 圖層命名]**：PSD檔案中的圖層會以個別影像上傳。 若要在Adobe Dynamic Media Classic中命名這些影像，請從下列選項中選擇：

      * **[!UICONTROL 圖層名稱]**：將影像命名為PSD檔案中的圖層名稱。 例如，在原始 PSD 檔案中名稱為 Price Tag 的圖層會變成名稱為 Price Tag 的影像。不過，如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱（「背景」、「圖層1」、「圖層2」等等），則會以影像在PSD檔案中的圖層編號來命名影像。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshop和圖層編號]**：將影像命名為PSD檔案中的圖層編號，忽略原始圖層名稱。 影像會以 Photoshop 檔案名稱並附加圖層編號命名。例如，檔案的第二層，稱為 `Spring Ad.psd` 已命名 `Spring Ad_2` 即使它在Photoshop中有非預設名稱。

      * **[!UICONTROL Photoshop和圖層名稱]**：在PSD檔案後面加上圖層名稱或圖層編號來命名影像。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。例如，名為 `Price Tag` 在名為的PSD檔案中 `SpringAd` 已命名 `Spring Ad_Price Tag`. 系統會呼叫預設名稱為「圖層2」的圖層 `Spring Ad_2`.

   * **[!UICONTROL 錨點]**：指定如何在範本中錨定影像，這些範本是從PSD檔案產生的圖層構成中產生的。 預設的錨點為中心。無論取代影像的外觀比例為何，置中錨點都可讓取代影像最能填滿相同的空間。 當參考範本並且使用替換參數時，取代此影像的不同長寬影像可有效的填滿相同的空間。如果您的應用程式需要將替代影像填滿範本中的配置空間，請變更為其他設定。

## 在PSD檔案中檢視和編輯圖層 {#viewing-and-editing-layers-in-a-psd-file}

如果您選取選項 **[!UICONTROL 保留圖層]** 當您上傳PSD時，Adobe Dynamic Media Classic會將個別的圖層擷取至資產。 您可以在「詳細資料檢視」的「瀏覽面板」中開啟檔案，以檢視和編輯屬於PSD檔案的資產圖層。

>[!NOTE]
>
>Adobe Dynamic Media Classic在巢狀圖層群組中最多可支援五個層級。

1. 在「瀏覽」面板中按兩下完整PSD檔案。 檔案會在「詳細資料檢視」中開啟。

   >[!NOTE]
   >
   >確定您開啟完整資產，而非 PSD 圖層其中的資產。

1. 選取 **[!UICONTROL 圖層]**. 所有圖層在「圖層」面板中皆會顯示為個別影像。
1. 按兩下圖層並執行下列任一項作業：

   * 若要在圖層上建立影像地圖，請選取 **[!UICONTROL 影像地圖]** 圖示。 (請參閱 [建立影像地圖](creating-image-maps.md#creating_image_maps).)
   * 若要在圖層上建立縮放目標，請選取 **[!UICONTROL 縮放目標]** 圖示。 (請參閱 [建立引導式縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * 若要裁切圖層，請選取 **[!UICONTROL 裁切]** 圖示。 (請參閱 [裁切影像](cropping-image.md#cropping_an_image).)
   * 若要銳利化圖層，請選取 **[!UICONTROL 銳利化]**. (請參閱 [銳利化影像](sharpening-image.md#sharpening_an_image).)
   * 若要調整圖層，請選取 **[!UICONTROL 調整]**. (請參閱 [調整影像](adjusting-image.md#adjusting_an_image).)

1. 選取 **[!UICONTROL 儲存]** 或 **[!UICONTROL 另存為]**.
1. 若要檢視或編輯不同的圖層，請選取圖層預覽底部的箭頭。
1. 若要結束圖層的「細節檢視」，請選取 **[!UICONTROL 格點檢視]** 圖示。
