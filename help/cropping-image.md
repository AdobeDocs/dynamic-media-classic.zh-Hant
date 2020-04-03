---
title: 裁切影像
seo-title: 裁切影像
description: 'null'
seo-description: 瞭解如何裁切影像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
translation-type: tm+mt
source-git-commit: b8d245bfc8375966af314ed95e81a519c5ee6c24

---


# 裁切影像{#cropping-an-image}

您可以在 Scene7 Publishing System 中裁切影像。系統會保留已裁切之影像的相關資訊，以便您將這類影像還原成原始狀態。您也可以裁切影像並以新名稱儲存裁切過的版本。

您可以裁切影像以移除周圍的空白區域，或是裁切影像區域。

>[!NOTE]
>
>裁切之後，您可以按一下「另存新檔」按鈕，以不同名稱儲存裁切過的影像版本。在「另存新檔」視窗中，選擇「另存為新的主檔案」，即可儲存影像的複本。選擇「另存為主影像的額外視圖」，以不同名稱儲存原始版本與裁切過的版本。選擇「取代原始檔案」，即可刪除已裁切之影像的原始檔案。接著輸入影像的名稱，然後選取「送出」按鈕。

## 裁切以移除影像周圍的空白區域 {#crop-to-remove-white-space-around-an-image}

您可以從影像邊緣裁切透明或純色的像素。

1. 若要裁切影像，請按一下它的滑鼠指向「編輯」按鈕，然後選擇「裁切」，或是在瀏覽面板中，以詳細檢視顯示影像，然後按一下「裁切」按鈕 。「裁切編輯器」畫面開啟。
1. 進行以下一項操作:

   * 若要修剪顏色像素，請選取「修剪」選單並選擇「顏色」。此時會顯示「依照色彩自動裁切」對話框。選取「邊角」選單，然後選擇要裁切掉的具有背景色彩的邊角。接著輸入「容許度」設定 (從 0 到 1)。設定為 0 只會在完全符合您選取的影像邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。選取「裁切」按鈕。
   * 若要修剪透明像素，請選取「修剪」選單並選擇「透明」。此時會顯示「依照透明度自動裁切」對話框。輸入容許度設定 (從 0 到 1)。設定為 0 只會在完全為透明時才會裁切像素。數值越接近 1，允許的透明度就越高。選取「裁切」按鈕。

1. 按一下&#x200B;**「儲存」**。

>[!NOTE]
>
>完成裁切後若要將影像還原至原始狀態，請在「裁切編輯器」畫面中顯示影像，然後選取「重設」按鈕。

## 選取要裁切的區域 {#select-an-area-to-crop}

1. To crop an image, click its rollover Edit button and choose **Crop**, or display it in the Browse Panel in Detail view and click **Crop**.

1. 在「裁切編輯器」視窗中，將您不想裁切的影像部分置於裁切方塊中。 What appears inside the box remains when you click **Save** and crop the image.
1. 若要調整裁切區域，請執行下列其中一個動作:

   * 拖曳方塊某一側或邊角。拖曳時按住 Shift 鍵即可變更大小，但會維持裁切方塊的外觀比例 (形狀)。
   * 在「大小」方框中輸入像素度量。
   * 拖曳以移動裁切方塊。在方塊邊界內移動指標。顯示四向箭頭時，請將方塊拖曳至影像上的新位置。

1. 按一下&#x200B;**「儲存」**。

>[!NOTE]
>
>完成裁切後若要將影像還原至原始狀態，請在「裁切編輯器」畫面中顯示影像，然後選取「重設」按鈕。

>[!MORELIKETHIS]
>
>* [上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)
>* [從 PDF 檔案裁切空白區域](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [從 PDF 頁面邊緣裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

