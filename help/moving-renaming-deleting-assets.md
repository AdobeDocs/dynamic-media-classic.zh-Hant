---
title: 移動、重新命名和刪除資產
description: 了解如何在Adobe Dynamic Media Classic中移動、重新命名和刪除資產。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 33%

---

# 移動、重新命名和刪除資產{#moving-renaming-and-deleting-assets}

您可以從瀏覽面板中，移動、重新命名和刪除資產。此外，您也可以利用文字檔案同時刪除多項資產。

## 移動資產 {#move-assets}

您可以在瀏覽面板中，將資產移動到不同檔案夾。

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 在「資產資料庫」中顯示您要將資產移至的資料夾，並將資產拖曳至資料夾。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 移動]**，在「移動資產」視窗中選取資料夾，然後選取 **[!UICONTROL 移動]**.

## 重新命名資產 {#rename-assets}

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 選取名稱，輸入新名稱，然後按 **[!UICONTROL 輸入]** 或從名稱中選取「離開」。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新命名]**. 資產名稱會以反白顯示。輸入新名稱，然後按 **[!UICONTROL 輸入]**.

請確定您不要輸入現有Adobe Dynamic Media Classic資產的名稱。

## 刪除資產 {#delete-assets}

您可以刪除「瀏覽」面板中選取的資產，並刪除整個資料夾。 刪除的資產與檔案夾會移動到「垃圾桶」檔案夾，七天後就會永久刪除。

刪除資產時，也會刪除衍生的所有資產。例如，刪除您建立其縮放目標的影像時，也會同時刪除縮放目標。

>[!NOTE]
>
>刪除資產時，也會永久刪除其中衍生的縮放影像、影像屬性及操作記錄項目。這些衍生項目不會與資產一同移動到「垃圾桶」檔案夾，也無法從「垃圾桶」中復原。

1. 請執行下列任一動作:

   * 若要刪除一或多個資產，請在「瀏覽」面板中選取資產，然後按 **[!UICONTROL 刪除]** 或前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**.
   * 若要刪除資料夾，請選取「資產資料庫」中的資料夾，然後選取 **[!UICONTROL 刪除資料夾]**.

      刪除資料夾會刪除資料夾、資料夾中的所有資產及其子資料夾中的所有資產。

>[!NOTE]
>
>如果您刪除資產檔案的原因是要以相同名稱取代資產檔案，Adobe Dynamic Media Classic建議您覆寫資產檔案，而非將其刪除。

## 利用文字檔案刪除多項資產 {#delete-multiple-assets-with-a-text-file}

若要在整個資產資料庫中一次刪除多個資產，您可以在文字檔案中列出您要刪除的資產，並將清單提交至Adobe Dynamic Media Classic。

建立Adobe Dynamic Media Classic ID清單並儲存為文字(.txt)檔案。 每個Adobe Dynamic Media Classic ID必須各行（後面接著硬式傳回）。

建立清單之後，遵循下列步驟即可使用該清單刪除資產:

1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除資產清單]**.
1. 在「刪除資產清單」對話方塊中，瀏覽或輸入包含您要刪除資產清單之文字檔案的路徑。
1. 選擇 **[!UICONTROL 刪除]**.

當您刪除含有文字檔的資產時，如果清單中沒有任何Adobe Dynamic Media Classic ID，則會顯示「無法驗證清單中的這些項目：」訊息。 項目清單也隨即顯示。 不過，Adobe Dynamic Media Classic不會在「工作」頁面上產生錯誤。

>[!MORELIKETHIS]
>
>* [在「瀏覽」面板中選取資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [準備資產和資料夾以便上傳](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [從清除資料夾還原資產](trash-folder.md#restoring_assets_from_the_trash_folder)

