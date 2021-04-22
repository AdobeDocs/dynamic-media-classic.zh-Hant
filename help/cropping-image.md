---
title: 裁切影像
description: 瞭解如何裁切影像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media經典，資產管理
role: Business Practitioner
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 51%

---

# 裁切影像{#cropping-an-image}

您可以在Dynamic Media經典中裁切影像。 系統會保留已裁切之影像的相關資訊，以便您將這類影像還原成原始狀態。您也可以裁切影像並以新名稱儲存裁切過的版本。

您可以裁切影像以移除周圍的空白區域，或是裁切影像區域。

>[!NOTE]
>
>裁切之後，您可以按一下「另存新檔」按鈕，以不同名稱儲存裁切過的影像版本。在「另存新檔」視窗中，選擇「另存為新的主檔案」，即可儲存影像的複本。按一下&#x200B;**[!UICONTROL Save As Addition View Of Master]**&#x200B;以不同的名稱保存原始版本及其裁切版本。 按一下「取代原稿」，刪除影像裁切的原始檔案。 ****&#x200B;然後輸入影像的名稱，然後按一下「送出」。****

## 裁切以移除影像周圍的空白區域 {#crop-to-remove-white-space-around-an-image}

您可以從影像邊緣裁切透明或純色的像素。

1. 若要裁切影像，請按一下其滑鼠指向效果&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕並選擇&#x200B;**[!UICONTROL 裁切]**，或在「詳細資料」檢視的「瀏覽面板」中顯示影像，然後按一下「裁切&#x200B;**[!UICONTROL 裁切]**&#x200B;按鈕。
1. 在「裁切編輯器」頁面上，執行下列任一項作業：

   * 要修剪顏色像素，請按一下「修剪&#x200B;**** > **[!UICONTROL 顏色]**」。 此時會顯示「依照色彩自動裁切」對話框。按一下&#x200B;**[!UICONTROL Corner]**&#x200B;功能表，並選擇背景顏色的角落以裁切掉。 然後輸入從0到1的&#x200B;**[!UICONTROL 公差]**&#x200B;設定。 設定為 0 只會在完全符合您選取的影像邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。按一下&#x200B;**[!UICONTROL 裁切]**&#x200B;按鈕。
   * 要修剪透明像素，請按一下「修剪&#x200B;**** > **[!UICONTROL 透明]**」。 此時會顯示「依照透明度自動裁切」對話框。輸入容許度設定 (從 0 到 1)。0設定僅會在像素是透明的時候裁切像素。 數值越接近 1，允許的透明度就越高。按一下&#x200B;**[!UICONTROL 裁切]**。

1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

>[!NOTE]
>
>若要在裁切影像後將影像還原為原始狀態，請在裁切編輯器畫面中顯示影像，然後按一下「重設」。****

## 選取要裁切的區域 {#select-an-area-to-crop}

1. 若要裁切影像，請按一下其變換&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕，然後選擇&#x200B;**[!UICONTROL 裁切]**，或在「詳細資料」檢視的「瀏覽面板」中顯示影像，然後按一下裁切&#x200B;**[!UICONTROL 裁切]**。

1. 在「裁切編輯器」視窗中，將您不想裁切的影像部分置於裁切方塊中。 顯示在方塊中的是當您按一下「儲存」並裁切影像時仍保留的項目。****
1. 若要調整裁切區域，請執行下列其中一個動作:

   * 拖曳方塊某一側或邊角。拖曳時按住 Shift 鍵即可變更大小，但會維持裁切方塊的外觀比例 (形狀)。
   * 在「大小」方框中輸入像素度量。
   * 拖曳以移動裁切方塊。在方塊邊界內移動指標。顯示四向箭頭時，請將方塊拖曳至影像上的新位置。

1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

>[!NOTE]
>
>若要在裁切影像後將影像還原為原始狀態，請在裁切編輯器畫面中顯示影像，然後按一下「重設」。****

>[!MORELIKETHIS]
>
>* [上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)
>* [從 PDF 檔案裁切空白區域](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [從 PDF 頁面邊緣裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

