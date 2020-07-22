---
title: 移動、重新命名和刪除資產
seo-title: 移動、重新命名和刪除資產
description: 'null'
seo-description: 瞭解如何移動、重新命名和刪除資產。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 66%

---


# 移動、重新命名和刪除資產{#moving-renaming-and-deleting-assets}

您可以從瀏覽面板中，移動、重新命名和刪除資產。此外，您也可以利用文字檔案同時刪除多項資產。

## 移動資產 {#move-assets}

您可以在瀏覽面板中，將資產移動到不同檔案夾。

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 在資產庫中顯示您要將資產移動到哪個檔案夾，然後將資產拖曳到該檔案夾。
   * 選擇「檔案 > 移動」，在「移動資產」視窗中選取檔案夾，然後選取「移動」。

## 重新命名資產 {#rename-assets}

若要重新命名資產:

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 選取名稱，輸入新名稱，然後按 Enter 鍵或在名稱以外的位置按一下。
   * 選擇「檔案 > 重新命名」。資產名稱會以反白顯示。輸入新名稱，然後按 Enter 鍵。

請確定您不要輸入現有Dynamic Media Classic資產的名稱。

## 刪除資產 {#delete-assets}

您可以在瀏覽面板中刪除選取的資產，也可以刪除整個檔案夾。刪除的資產與檔案夾會移動到「垃圾桶」檔案夾，七天後就會永久刪除。

刪除資產時，也會刪除衍生的所有資產。例如，刪除您建立其縮放目標的影像時，也會同時刪除縮放目標。

>[!NOTE]
>
>刪除資產時，也會永久刪除其中衍生的縮放影像、影像屬性及操作記錄項目。這些衍生項目不會與資產一同移動到「垃圾桶」檔案夾，也無法從「垃圾桶」中復原。

1. 請執行下列任一動作:

   * 若要刪除一或多項資產，請在瀏覽面板中選取資產，然後按 Delete 鍵或選擇「檔案 > 刪除」。
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      刪除檔案夾會刪除該檔案夾、其中的所有資產，以及其子檔案夾中的所有資產。

>[!NOTE]
>
>如果您刪除資產檔案的原因是要以相同名稱取代另一個檔案，Dynamic Media Classic建議覆寫資產檔案，而非將其刪除。

## 利用文字檔案刪除多項資產 {#delete-multiple-assets-with-a-text-file}

若要在整個資產庫中一次刪除多個資產，您可以在文字檔案中列出要刪除的資產，並將清單送出至Dynamic Media Classic。

建立Dynamic Media Classic ID清單，並儲存為文字(.txt)檔案。 每個Dynamic Media Classic ID都必須位於其自己的行上（後面接著硬式傳回）。

建立清單之後，遵循下列步驟即可使用該清單刪除資產:

1. 選擇「檔案 > 刪除資產清單」。
1. 在「刪除資產清單」對話框中，瀏覽或輸入含有您要刪除之資產清單的文字檔案路徑。
1. 按一下「刪除」按鈕。

當您刪除包含文字檔的資產時，如果清單中沒有任何Dynamic Media Classic ID，則會顯示訊息，告知您Dynamic Media Classic是「無法驗證清單中的這些項目：」以及項目清單。 不過，Dynamic Media Classic不會在「工作」畫面上產生錯誤。

>[!MORELIKETHIS]
>
>* [在瀏覽面板中選取資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [準備要上載的資產和檔案夾](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [從垃圾桶檔案夾中復原資產](trash-folder.md#restoring_assets_from_the_trash_folder)

