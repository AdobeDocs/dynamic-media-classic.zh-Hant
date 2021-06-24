---
title: 管理垃圾桶檔案夾
description: 了解如何管理垃圾桶資料夾。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic，資產管理
role: Business Practitioner
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 39%

---

# 管理垃圾桶檔案夾{#managing-the-trash-folder}

您從Dynamic Media Classic刪除的項目會移至垃圾桶資料夾。 已刪除的會保留在此資料夾中7天，直到被還原或永久刪除為止。 您可以按一下資產庫底部的&#x200B;**[!UICONTROL 清除]**&#x200B;圖示，並在清除資料夾頁面中檢視項目，以檢查已刪除的項目。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

從「垃圾筒」資料夾刪除項目，會永久刪除Dynamic Media Classic中的項目；從垃圾桶資料夾刪除的項目無法再還原。 如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶資料夾的資產仍會在Dynamic Media Classic上註冊。 如果您嘗試上傳的檔案名稱與「垃圾筒」資料夾中已刪除的檔案相同，Dynamic Media Classic會將您要上傳的資產視為重複資產。 因此，其名稱會附加數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 雖然項目已從您的Dynamic Media Classic資料夾中移除，但其ID無法指派給其他資產，因為它仍保留在垃圾桶資料夾中。 如果您嘗試上傳與垃圾桶資料夾中的檔案同名的資產，Dynamic Media Classic會將數字附加至資產名稱。
* 無法發佈項目。即使項目在您刪除時已標記為發佈，您也無法予以發佈。
* 項目會保留在「垃圾筒」資料夾中，直到還原、七天過後，或有人選擇&#x200B;**[!UICONTROL 清除垃圾筒]**&#x200B;命令。 七天之後，自動清除作業就會永久刪除項目。

## 從垃圾桶檔案夾中復原資產 {#restoring-assets-from-the-trash-folder}

並非刪除資產的人才能夠還原資產；任何人都可以從「垃圾桶」檔案夾中還原資產。還原的資產會放在其刪除來源的檔案夾中。如果這些資料夾已不存在，Dynamic Media Classic會重新建立這些資料夾，並將還原的資產放置在重新建立的資料夾中。

若要將資產從垃圾桶資料夾還原至從中刪除的資料夾，請執行下列動作：

1. 在「資產庫」面板底部，按一下&#x200B;**[!UICONTROL Trash]**&#x200B;圖示以開啟「 Trash」資料夾。
1. 選取您要還原的資產。
1. 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶還原]**」。

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。七天後就會從「垃圾桶」檔案夾中永久刪除資產。

若要從「垃圾筒」資料夾中永久刪除資產，請按一下&#x200B;**[!UICONTROL 垃圾筒]**&#x200B;圖示。 在垃圾桶資料夾頁面上，執行下列任一操作：

* **刪除個別資產**  — 選取您要永久刪除的資產，然後按一下「 **[!UICONTROL 檔案]**  >從 **[!UICONTROL 垃圾筒清除空白」]**。

* **刪除所有資產**  — 按一 **[!UICONTROL 下「檔案]**  >空 **[!UICONTROL 白垃圾桶」]**。

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)

