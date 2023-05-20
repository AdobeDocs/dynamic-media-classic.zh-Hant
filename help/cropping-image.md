---
title: 裁切影像
description: 學習如何在Adobe Dynamic Media Classic裁剪影像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# 裁切影像{#cropping-an-image}

你可以在Adobe Dynamic Media Classic拍攝圖片。 系統會保留已裁切之影像的相關資訊，以便您將這類影像還原成原始狀態。您也可以裁切影像並以新名稱儲存裁切過的版本。

您可以裁切影像以移除周圍的空白區域，或是裁切影像區域。

>[!NOTE]
>
>裁剪後，可以選擇 **[!UICONTROL 另存為]** 並以其他名稱保存影像的裁剪版本。 在「另存為」窗口中，選擇 **[!UICONTROL 另存為新首頁]** 保存影像的第二個副本。 選擇 **[!UICONTROL 另存為主視圖]** 因此，可以使用其他名稱保存原始版本及其裁剪版本。 選擇 **[!UICONTROL 替換原始]** 刪除從中剪切影像的原始檔案。 然後輸入影像的名稱，然後選擇 **[!UICONTROL 提交]**。

## 裁切以移除影像周圍的空白區域 {#crop-to-remove-white-space-around-an-image}

您可以從影像邊緣裁切透明或純色的像素。

1. 要裁剪影像，請選擇其滾動影像 **[!UICONTROL 編輯]** 按鈕，然後選擇 **[!UICONTROL 裁剪]**，或在「詳細資訊視圖」的「瀏覽面板」中顯示，然後選擇 **[!UICONTROL 裁剪]** 按鈕
1. 在「裁剪編輯器」頁上，執行下列操作之一：

   * 要裁切顏色像素，請轉到 **[!UICONTROL 修剪]** > **[!UICONTROL 顏色]**。 在 **[!UICONTROL 按顏色自動裁剪]** 對話框，選擇 **[!UICONTROL 角]** ，然後選擇要裁剪的背景顏色的角。 然後輸入 **[!UICONTROL 容差]** 從0到1。 設定為 0 只會在完全符合您選取的影像邊角顏色時才會裁切像素。數值越接近 1，允許的色彩差異就越大。選擇 **[!UICONTROL 裁剪]**。
   * 要修剪透明像素，請轉到 **[!UICONTROL 修剪]** > **[!UICONTROL 透明]**。 在 **[!UICONTROL 按透明度自動裁剪]** 對話框，輸入0到1的公差設定。 0設定僅在像素為透明時才會裁剪像素。 數值越接近 1，允許的透明度就越高。選擇 **[!UICONTROL 裁剪]**。

1. 選擇 **[!UICONTROL 保存]**。

>[!NOTE]
>
>要在剪切影像後將影像恢復為原始狀態，請在「裁剪編輯器」螢幕中顯示影像並選擇 **[!UICONTROL 重置]**。

## 選取要裁切的區域 {#select-an-area-to-crop}

1. 要裁剪影像，請選擇其滾動影像 **[!UICONTROL 編輯]** 按鈕 **[!UICONTROL 裁剪]**，或在「詳細資訊視圖」的「瀏覽面板」中顯示，然後選擇 **[!UICONTROL 裁剪]**。

1. 在「裁剪編輯器」窗口中，將不想裁剪的影像部分放在裁剪框中。 框內顯示的任何內容都是在您選擇 **[!UICONTROL 保存]** 並裁剪影像。
1. 若要調整裁切區域，請執行下列其中一個動作:

   * 拖曳方塊某一側或邊角。拖曳時按住 Shift 鍵即可變更大小，但會維持裁切方塊的外觀比例 (形狀)。
   * 在「大小」方框中輸入像素度量。
   * 拖曳以移動裁切方塊。在方塊邊界內移動指標。顯示四向箭頭時，請將方塊拖曳至影像上的新位置。

1. 選擇 **[!UICONTROL 保存]**。

>[!NOTE]
>
>要在剪切影像後將影像恢復為原始狀態，請在「裁剪編輯器」螢幕中顯示影像並選擇 **[!UICONTROL 重置]**。

>[!MORELIKETHIS]
>
>* [上載時影像編輯的選項](image-editing-options-upload.md#image-editing-options-at-upload)
>* [從PDF檔案裁剪空白](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [從PDF頁的側面裁剪](pdfs.md#cropping_from_the_sides_of_pdf_pages)

