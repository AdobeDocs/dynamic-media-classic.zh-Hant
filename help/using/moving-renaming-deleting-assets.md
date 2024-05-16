---
title: 移動、重新命名和刪除資產
description: 瞭解如何在Adobe Dynamic Media Classic中移動、重新命名和刪除資產。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 17%

---

# 移動、重新命名和刪除資產{#moving-renaming-and-deleting-assets}

您可以從「瀏覽」面板移動、重新命名和刪除資產。 此外，您也可以利用文字檔案同時刪除多項資產。

## 移動資產 {#move-assets}

您可以在「瀏覽」面板中將資產移至不同的資料夾。

**若要移動資產：**

1. 在「瀏覽」面板中選取一個或多個資產，然後執行下列任一項作業：

   * 在「資產庫」中顯示您要移動資產的資料夾，並將資產拖曳至資料夾。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 移動]**，請在「移動資產」視窗中選取資料夾，然後選取 **[!UICONTROL 移動]**.

## 重新命名資產 {#rename-assets}

1. 在「瀏覽」面板中選取資產，然後執行下列任一項作業：

   * 選取名稱，輸入新名稱，然後按 **[!UICONTROL 輸入]** 或選取遠離名稱。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新命名]**. 資產名稱會以反白顯示。輸入新名稱，然後按 **[!UICONTROL 輸入]**. 請勿輸入現有Adobe Dynamic Media Classic資產的名稱。

## 刪除資產 {#delete-assets}

您可以刪除「瀏覽」面板中選取的資產並刪除整個資料夾。 刪除的資產與檔案夾會移動到「垃圾桶」檔案夾，七天後就會永久刪除。

當您刪除資產時，衍生自該資產的所有資產也會一併刪除。 例如，刪除您已建立「縮放目標」的影像時，會一併刪除「縮放目標」與影像。

刪除資產時，也會永久刪除其中衍生的縮放影像、影像屬性及操作記錄項目。這些衍生項目不會與資產一同移動到「垃圾桶」檔案夾，也無法從「垃圾桶」中復原。

>[!IMPORTANT]
>
>大量刪除是一項大量作業。 請確定您是依序執行大量刪除，而非同時執行大量刪除作業。 Adobe建議您將刪除操作限製為每小時5000個或更少的資產刪除。 任何大於每小時5000的數字都可能導致速率限制。

**若要刪除資產：**

1. 請執行下列任一動作:

   * 若要刪除一或多個資產，請在「瀏覽」面板中選取資產，然後按下 **[!UICONTROL 刪除]** 或前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**.
   * 若要刪除資料夾，請在「資產庫」中選取該資料夾，然後選取 **[!UICONTROL 移除資料夾]**.

     刪除資料夾會刪除該資料夾、該資料夾中的所有資產及其子資料夾中的所有資產。

如果您刪除資產檔案的原因是要以相同名稱取代檔案，Adobe Dynamic Media Classic建議您覆寫資產檔案，而非刪除檔案。

## 利用文字檔案刪除多項資產 {#delete-multiple-assets-with-a-text-file}

若要在整個資產庫中一次刪除許多資產，您可以在文字檔中列出您要刪除的資產，並將清單提交至Adobe Dynamic Media Classic。

建立Adobe Dynamic Media Classic ID清單，並將其儲存為文字(.txt)檔案。 每個Adobe Dynamic Media Classic ID都必須有自己的行（後面接著強制傳回）。

建立清單之後，遵循下列步驟即可使用該清單刪除資產:

1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除資產清單]**.
1. 在 **[!UICONTROL 已刪除的資產清單]** 對話方塊中，輸入文字檔的路徑，其中包含您要刪除的資產清單。
1. 選取 **[!UICONTROL 刪除]**.

當您刪除含有文字檔的資產時，如果清單中不存在任何Adobe Dynamic Media Classic ID，則會顯示「無法驗證您清單中的這些專案：」訊息。 也會顯示專案清單。 不過，Adobe Dynamic Media Classic不會在作業頁面上產生錯誤。

>[!MORELIKETHIS]
>
>* [在瀏覽面板中選取資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [準備您的資產和資料夾以進行上傳](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [從垃圾桶資料夾中還原資產](trash-folder.md#restoring_assets_from_the_trash_folder)
