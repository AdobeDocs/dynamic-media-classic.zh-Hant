---
title: 裁切影像
description: 了解如何裁切影像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic，資產管理
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 51%

---

# 裁切影像{#cropping-an-image}

您可以在Dynamic Media Classic中裁切影像。 系統會保留已裁切之影像的相關資訊，以便您將這類影像還原成原始狀態。您也可以裁切影像並以新名稱儲存裁切過的版本。

您可以裁切影像以移除周圍的空白區域，或是裁切影像區域。

>[!NOTE]
>
>裁切之後，您可以按一下「另存新檔」按鈕，以不同名稱儲存裁切過的影像版本。在「另存新檔」視窗中，選擇「另存為新的主檔案」，即可儲存影像的複本。按一下「主版的另存新檔」]**以不同名稱儲存原始版本及其裁切的版本。**[!UICONTROL &#x200B;按一下「**[!UICONTROL 取代原始檔案]**」以刪除您裁切影像的原始檔案。 然後輸入影像名稱，然後按一下&#x200B;**[!UICONTROL Submit]**。

## 裁切以移除影像周圍的空白區域 {#crop-to-remove-white-space-around-an-image}

您可以從影像邊緣裁切透明或純色的像素。

1. 要裁切影像，請按一下其滾動&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕並選擇&#x200B;**[!UICONTROL Crop]**，或在「瀏覽面板」的「詳細資訊」視圖中顯示該影像，然後按一下&#x200B;**[!UICONTROL Crop]**&#x200B;按鈕。
1. 在「裁切編輯器」頁面上，執行下列其中一項操作：

   * 要修剪顏色像素，請按一下&#x200B;**[!UICONTROL Trim]** > **[!UICONTROL Color]**。 此時會顯示「依照色彩自動裁切」對話框。按一下&#x200B;**[!UICONTROL Corner]**&#x200B;菜單，然後選擇背景顏色的角來裁切掉。 然後輸入從0到1的&#x200B;**[!UICONTROL 允差]**&#x200B;設定。 設定為 0 只會在完全符合您選取的影像邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。按一下&#x200B;**[!UICONTROL Crop]**&#x200B;按鈕。
   * 要修剪透明像素，請選擇按一下「**[!UICONTROL Trim]** > **[!UICONTROL Transparent]**」。 此時會顯示「依照透明度自動裁切」對話框。輸入容許度設定 (從 0 到 1)。0設定只會在像素為透明時裁切像素。 數值越接近 1，允許的透明度就越高。按一下「**[!UICONTROL 裁切]**」。

1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

>[!NOTE]
>
>要在裁切影像後將其恢復為原始狀態，請在「裁切編輯器」螢幕中顯示該影像，然後按一下&#x200B;**[!UICONTROL Reset]**。

## 選取要裁切的區域 {#select-an-area-to-crop}

1. 要裁切影像，請按一下其滾動&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕，然後選擇&#x200B;**[!UICONTROL 裁切]**，或在「詳細資訊」視圖的「瀏覽面板」中顯示該影像，然後按一下&#x200B;**[!UICONTROL 裁切]**。

1. 在「裁切編輯器」窗口中，將不想要裁切的影像部分置於裁切框中。 框內顯示的是當您按一下&#x200B;**[!UICONTROL Save]**&#x200B;並裁切影像時仍保留的內容。
1. 若要調整裁切區域，請執行下列其中一個動作:

   * 拖曳方塊某一側或邊角。拖曳時按住 Shift 鍵即可變更大小，但會維持裁切方塊的外觀比例 (形狀)。
   * 在「大小」方框中輸入像素度量。
   * 拖曳以移動裁切方塊。在方塊邊界內移動指標。顯示四向箭頭時，請將方塊拖曳至影像上的新位置。

1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

>[!NOTE]
>
>要在裁切影像後將其恢復為原始狀態，請在「裁切編輯器」螢幕中顯示該影像，然後按一下&#x200B;**[!UICONTROL Reset]**。

>[!MORELIKETHIS]
>
>* [上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)
* [從 PDF 檔案裁切空白區域](pdfs.md#cropping_white_space_from_a_pdf_file)
* [從 PDF 頁面邊緣裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

