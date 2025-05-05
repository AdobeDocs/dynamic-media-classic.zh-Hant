---
title: 裁切影像
description: 瞭解如何在Adobe Dynamic Media Classic中裁切影像。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# 裁切影像{#cropping-an-image}

您可以在Adobe Dynamic Media Classic中裁切影像。 系統會保留已裁切之影像的相關資訊，以便您將這類影像還原成原始狀態。您也可以裁切影像並以新名稱儲存裁切過的版本。

您可以裁切影像以移除周圍的空白區域，或是裁切影像區域。

>[!NOTE]
>
>裁切之後，您可以選取&#x200B;**[!UICONTROL 另存新檔]**，並以不同的名稱儲存裁切的影像版本。 在「另存新檔」視窗中，選取&#x200B;**[!UICONTROL 另存為新主要專案]**&#x200B;以儲存影像的第二個復本。 選取「**[!UICONTROL 另存為主要]**&#x200B;的新增檢視」，以便以不同的名稱儲存原始版本及其裁切版本。 選取&#x200B;**[!UICONTROL 取代原始檔案]**&#x200B;以刪除您從中裁切影像的原始檔案。 然後輸入影像的名稱，並選取&#x200B;**[!UICONTROL 提交]**。

## 裁切以移除影像周圍的空白區域 {#crop-to-remove-white-space-around-an-image}

您可以從影像邊緣裁切透明或純色的像素。

1. 若要裁切影像，請選取影像的滑鼠指向效果&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕，然後選取&#x200B;**[!UICONTROL 裁切]**，或在[詳細資訊]檢視的[瀏覽]面板中顯示該影像，然後選取&#x200B;**[!UICONTROL 裁切]**&#x200B;按鈕。
1. 在「裁切編輯器」頁面上，執行下列任一項作業：

   * 若要修剪色彩畫素，請移至&#x200B;**[!UICONTROL 修剪]** > **[!UICONTROL 色彩]**。 在&#x200B;**[!UICONTROL 依色彩自動裁切]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL 轉角]**&#x200B;功能表，並選擇要裁切掉的背景色彩轉角。 然後輸入從0到1的&#x200B;**[!UICONTROL 容許度]**&#x200B;設定。 設定為 0 只會在完全符合您選取的影像邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。選取&#x200B;**[!UICONTROL 裁切]**。
   * 若要修剪透明畫素，請移至&#x200B;**[!UICONTROL 修剪]** > **[!UICONTROL 透明]**。 在&#x200B;**[!UICONTROL 依透明度自動裁切]**&#x200B;對話方塊中，輸入從0到1的容許度設定。 0設定只會在畫素為透明時裁切畫素。 數值越接近 1，允許的透明度就越高。選取&#x200B;**[!UICONTROL 裁切]**。

1. 選取&#x200B;**[!UICONTROL 儲存]**。

>[!NOTE]
>
>若要在裁切影像後將其還原為原始狀態，請在[裁切編輯器]畫面中顯示該影像，並選取[重設]。**&#x200B;**

## 選取要裁切的區域 {#select-an-area-to-crop}

1. 若要裁切影像，請選取其滑鼠指向效果&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕，然後選擇&#x200B;**[!UICONTROL 裁切]**，或在[詳細資訊]檢視的[瀏覽]面板中顯示該影像，然後選取&#x200B;**[!UICONTROL 裁切]**。

1. 在「裁切編輯器」視窗中，將您不想裁切的影像部分放置在裁切方塊中。 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;並裁切影像後，方塊內顯示的內容將會保留。
1. 若要調整裁切區域，請執行下列其中一個動作:

   * 拖曳方塊某一側或邊角。按住Shift鍵拖曳以變更大小，但維持裁切方塊的外觀比例（形狀）。
   * 在「大小」方框中輸入像素度量。
   * 拖曳以移動裁切方塊。在方塊邊界內移動指標。顯示四向箭頭時，請將方塊拖曳至影像上的新位置。

1. 選取&#x200B;**[!UICONTROL 儲存]**。

>[!NOTE]
>
>若要在裁切影像後將其還原為原始狀態，請在[裁切編輯器]畫面中顯示該影像，並選取[重設]。**&#x200B;**

>[!MORELIKETHIS]
>
>* 在上傳時用於編輯影像的[選項](image-editing-options-upload.md#image-editing-options-at-upload)
>* [從PDF檔案裁切空白字元](pdfs.md#cropping_white_space_from_a_pdf_file)
>* 從PDF頁面兩側[裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)
