---
title: 移動、重新命名和刪除資產
description: 了解如何移動、重新命名和刪除資產。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic，資產管理
role: Business Practitioner
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 44%

---

# 移動、重新命名和刪除資產{#moving-renaming-and-deleting-assets}

您可以從瀏覽面板中，移動、重新命名和刪除資產。此外，您也可以利用文字檔案同時刪除多項資產。

## 移動資產 {#move-assets}

您可以在瀏覽面板中，將資產移動到不同檔案夾。

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 在資產庫中顯示您要將資產移動到哪個檔案夾，然後將資產拖曳到該檔案夾。
   * 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 移動]**」，在「移動資產」窗口中選擇資料夾，然後選擇「**[!UICONTROL 移動]**」。

## 重新命名資產 {#rename-assets}

1. 在瀏覽面板中選取資產，並執行下列任一項作業:

   * 選擇名稱，鍵入新名稱，然後按&#x200B;**[!UICONTROL Enter]**&#x200B;或按一下離開名稱。
   * 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 更名]**」。 資產名稱會以反白顯示。輸入新名稱，然後按&#x200B;**[!UICONTROL Enter]**。

請務必不要輸入現有Dynamic Media Classic資產的名稱。

## 刪除資產 {#delete-assets}

您可以刪除「瀏覽」面板中選取的資產，並刪除整個資料夾。 刪除的資產與檔案夾會移動到「垃圾桶」檔案夾，七天後就會永久刪除。

刪除資產時，也會刪除衍生的所有資產。例如，刪除您建立其縮放目標的影像時，也會同時刪除縮放目標。

>[!NOTE]
>
>刪除資產時，也會永久刪除其中衍生的縮放影像、影像屬性及操作記錄項目。這些衍生項目不會與資產一同移動到「垃圾桶」檔案夾，也無法從「垃圾桶」中復原。

1. 請執行下列任一動作:

   * 若要刪除一或多個資產，請在「瀏覽」面板中選取資產，然後按&#x200B;**[!UICONTROL Delete]**&#x200B;或按一下&#x200B;**[!UICONTROL File]** > **[!UICONTROL Delete]**。
   * 若要刪除資料夾，請在「資產庫」中選取資料夾，然後按一下「移除資料夾&#x200B;]**」。**[!UICONTROL 

      刪除資料夾會刪除資料夾、資料夾中的所有資產及其子資料夾中的所有資產。

>[!NOTE]
>
>Dynamic Media Classic建議您覆寫資產檔案，而非刪除資產檔案，前提是您刪除資產檔案的原因是以相同的名稱取代另一個檔案。

## 利用文字檔案刪除多項資產 {#delete-multiple-assets-with-a-text-file}

若要在整個資產資料庫中一次刪除多個資產，您可以在文字檔案中列出您要刪除的資產，並將清單提交至Dynamic Media Classic。

建立Dynamic Media Classic ID清單並儲存為文字(.txt)檔案。 每個Dynamic Media Classic ID必須各行（後面接著硬式傳回）。

建立清單之後，遵循下列步驟即可使用該清單刪除資產:

1. 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 刪除資產清單]**」。
1. 在「刪除資產清單」對話方塊中，瀏覽或輸入包含您要刪除資產清單之文字檔案的路徑。
1. 按一下「**[!UICONTROL 刪除]**」。

當您刪除包含文字檔的資產時，如果清單中沒有任何Dynamic Media Classic ID，則會顯示「無法驗證清單中的這些項目：」訊息和項目清單。 不過，Dynamic Media Classic不會在「工作」頁面上產生錯誤。

>[!MORELIKETHIS]
>
>* [在瀏覽面板中選取資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
* [準備要上載的資產和檔案夾](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
* [從垃圾桶檔案夾中復原資產](trash-folder.md#restoring_assets_from_the_trash_folder)

