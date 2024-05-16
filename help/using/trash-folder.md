---
title: 管理垃圾桶資料夾
description: 瞭解如何管理垃圾桶資料夾。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# 管理垃圾桶資料夾{#managing-the-trash-folder}

您從Adobe Dynamic Media Classic刪除的專案會移至垃圾桶資料夾。 這些已刪除的專案會在此資料夾中保留七天，直到還原或永久刪除為止。 您可以選取 **[!UICONTROL 垃圾桶]** 圖示並檢視「垃圾筒」資料夾頁面中的專案。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

若從垃圾桶資料夾刪除專案，將會永久刪除Adobe Dynamic Media Classic中的專案；若從垃圾桶資料夾刪除專案，將無法再還原。 如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶資料夾的資產仍會在Adobe Dynamic Media Classic上註冊。 例如，假設您嘗試上傳的檔案名稱與垃圾桶資料夾中已刪除的檔案名稱相同。 Adobe Dynamic Media Classic會將您要上傳的資產視為重複資產。 在這種情況下，會在名稱后面附加一個數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 雖然專案已從您的Adobe Dynamic Media Classic資料夾中移除，但其ID無法指派給另一個資產，因為它仍保留在垃圾桶資料夾中。 如果您嘗試上傳與垃圾桶資料夾中檔案同名的資產，Adobe Dynamic Media Classic會在資產名稱后面附加數字。
* 無法發佈項目。即使項目在您刪除時已標記為發佈，您也無法予以發佈。
* 該專案會保留在垃圾桶資料夾中，直到它還原、7天過去或有人選擇 **[!UICONTROL 清空垃圾桶]** 命令。 七天之後，自動清除作業就會永久刪除項目。

## 從垃圾桶資料夾中還原資產 {#restoring-assets-from-the-trash-folder}

刪除資產的人不需要還原資產；任何人都可以從垃圾桶資料夾還原資產。 還原的資產會放在其刪除來源的檔案夾中。如果這些資料夾已不存在，Adobe Dynamic Media Classic會重新建立它們，而且還原的資產會放在重新建立的資料夾中。

若要將資產從垃圾桶資料夾還原至其被刪除的資料夾，請執行下列動作：

1. 在「資產庫」面板底部，選取 **[!UICONTROL 垃圾桶]** 圖示以開啟垃圾桶資料夾。
1. 選取您要還原的一個或多個資產。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶還原]**.

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。七天後就會從「垃圾桶」檔案夾中永久刪除資產。

您可以選取「 」，從「垃圾桶」資料夾中永久刪除資產 **[!UICONTROL 垃圾桶]** 圖示。 在「垃圾桶」資料夾頁面上，執行下列任一項作業：

* **刪除個別資產**：您可以永久刪除資產。 選取您想要的資產，然後按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶清空]**.

* **刪除所有資產**：前往 **[!UICONTROL 檔案]** > **[!UICONTROL 清空垃圾桶]**.

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)
