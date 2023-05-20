---
title: 移動、更名和刪除資產
description: 瞭解如何移動、更名和刪除Adobe Dynamic Media Classic的資產。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 741e31e64125a2dfe3f801480837ffbaf81767aa
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# 移動、更名和刪除資產{#moving-renaming-and-deleting-assets}

您可以從瀏覽面板中，移動、重新命名和刪除資產。此外，您也可以利用文字檔案同時刪除多項資產。

## 移動資產 {#move-assets}

您可以在瀏覽面板中，將資產移動到不同檔案夾。

**移動資產：**

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 在「資產庫」中顯示要將資產移動到的資料夾，並將資產拖動到該資料夾。
   * 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 移動]**，在「移動資產」窗口中選擇一個資料夾，然後選擇 **[!UICONTROL 移動]**。

## 重新命名資產 {#rename-assets}

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 選擇名稱，鍵入新名稱，然後按 **[!UICONTROL 輸入]** 或從名稱中選取。
   * 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 更名]**。 資產名稱會以反白顯示。輸入新名稱，然後按 **[!UICONTROL 輸入]**。 請確保不輸入現有Adobe Dynamic Media Classic資產的名稱。

## 刪除資產 {#delete-assets}

您可以在「瀏覽面板」中刪除選定的資產並刪除整個資料夾。 刪除的資產與檔案夾會移動到「垃圾桶」檔案夾，七天後就會永久刪除。

刪除資產時，也會刪除衍生的所有資產。例如，刪除您建立其縮放目標的影像時，也會同時刪除縮放目標。

刪除資產時，也會永久刪除其中衍生的縮放影像、影像屬性及操作記錄項目。這些衍生項目不會與資產一同移動到「垃圾桶」檔案夾，也無法從「垃圾桶」中復原。

>[!IMPORTANT]
>
>批量刪除是一項密集操作。 請確保按順序運行批量刪除操作，而不是作為併發、繁重的刪除操作。 Adobe建議將刪除操作限制為每小時刪除5000次或更少資產。 每小時超過5000的任何數字都可能導致速率限制。

**要刪除資產：**

1. 請執行下列任一動作:

   * 要刪除一個或多個資產，請在「瀏覽」面板中選擇資產，然後按 **[!UICONTROL 刪除]** 或轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**。
   * 要刪除資料夾，請在資產庫中選擇該資料夾，然後選擇 **[!UICONTROL 刪除資料夾]**。

      刪除資料夾會刪除資料夾、資料夾中的所有資產及其子資料夾中的所有資產。

Adobe Dynamic Media Classic建議覆蓋資產檔案，而不是刪除它們，如果刪除資產檔案的原因是用同名的另一個檔案替換它。

## 利用文字檔案刪除多項資產 {#delete-multiple-assets-with-a-text-file}

要在整個資產庫中同時刪除許多資產，您可以在文本檔案中列出要刪除的資產，並將清單提交Adobe Dynamic Media Classic。

建立Adobe Dynamic Media ClassicID清單，並將其另存為文本(.txt)檔案。 每個Adobe Dynamic Media ClassicID必須位於其自己的行上（後跟硬返回）。

建立清單之後，遵循下列步驟即可使用該清單刪除資產:

1. 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除資產清單]**。
1. 在「刪除資產清單」對話框中，瀏覽或鍵入包含要刪除的資產清單的文本檔案路徑。
1. 選擇 **[!UICONTROL 刪除]**。

當您刪除帶有文本檔案的資產時，如果清單中沒有任何Adobe Dynamic Media ClassicID，則會顯示消息「無法驗證清單中的這些條目：」。 還顯示條目清單。 但是，Adobe Dynamic Media Classic在「作業」頁上不會生成錯誤。

>[!MORELIKETHIS]
>
>* [在「瀏覽」面板中選擇資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [準備資產和資料夾以便上載](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [從垃圾資料夾還原資產](trash-folder.md#restoring_assets_from_the_trash_folder)

