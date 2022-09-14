---
title: 管理垃圾桶資料夾
description: 了解如何管理垃圾桶資料夾。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# 管理垃圾桶資料夾{#managing-the-trash-folder}

從Adobe Dynamic Media Classic刪除的項目會移至垃圾桶資料夾。 已刪除的會保留在此資料夾中7天，直到被還原或永久刪除為止。 您可以按一下 **[!UICONTROL 垃圾]** 圖示（位於資產庫底部），並在「垃圾桶」資料夾頁面中檢視項目。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

從垃圾桶資料夾刪除項目會永久刪除Adobe Dynamic Media Classic中的項目；從垃圾桶資料夾刪除的項目無法再還原。 如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶資料夾的資產仍會在Adobe Dynamic Media Classic上註冊。 如果您嘗試上傳的檔案名稱與「垃圾筒」資料夾中已刪除的檔案相同，Adobe Dynamic Media Classic會將您要上傳的資產視為重複資產。 因此，其名稱會附加數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 雖然項目已從您的Adobe Dynamic Media Classic資料夾中移除，但其ID無法指派給其他資產，因為該資產仍保留在垃圾桶資料夾中。 如果您嘗試上傳與垃圾桶資料夾中的檔案同名的資產，Adobe Dynamic Media Classic會在資產名稱中附加數字。
* 無法發佈項目。即使項目在您刪除時已標記為發佈，您也無法予以發佈。
* 項目會保留在垃圾桶資料夾中，直到還原、七天過後，或有人選擇 **[!UICONTROL 清除垃圾]** 命令。 七天之後，自動清除作業就會永久刪除項目。

## 從清除資料夾還原資產 {#restoring-assets-from-the-trash-folder}

刪除資產的人不需要將資產還原；任何人都可以從垃圾桶資料夾還原資產。 還原的資產會放在其刪除來源的檔案夾中。如果這些資料夾已不存在，Adobe Dynamic Media Classic會重新建立這些資料夾，並將還原的資產放置在重新建立的資料夾中。

若要將資產從垃圾桶資料夾還原至從中刪除的資料夾，請執行下列動作：

1. 在「資產庫」面板底部，選取 **[!UICONTROL 垃圾]** 圖示以開啟「垃圾筒」資料夾。
1. 選取您要還原的資產或資產。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶還原]**.

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。七天後就會從「垃圾桶」檔案夾中永久刪除資產。

若要從垃圾桶資料夾永久刪除資產，請選取 **[!UICONTROL 垃圾]** 表徵圖。 在垃圾桶資料夾頁面上，執行下列任一操作：

* **刪除個別資產**  — 選取您要永久刪除的資產，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 清空]**.

* **刪除所有資產**  — 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 空白垃圾]**.

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)

