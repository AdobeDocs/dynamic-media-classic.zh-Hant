---
title: 管理垃圾資料夾
description: 瞭解如何管理垃圾資料夾。
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

# 管理垃圾資料夾{#managing-the-trash-folder}

您從Adobe Dynamic Media Classic刪除的項目將移到垃圾資料夾。 刪除的內容將保留在此資料夾中七天，直到它們被還原或永久刪除。 通過按一下 **[!UICONTROL 垃圾]** 表徵圖，並查看「垃圾資料夾」頁面中的項目。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

從垃圾資料夾中刪除項目會永久刪除來自Adobe Dynamic Media Classic的項目；無法再還原從垃圾資料夾中刪除的項。 如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>已移動到垃圾資料夾的資產仍在Adobe Dynamic Media Classic註冊。 如果您嘗試上載與垃圾資料夾中已刪除檔案同名的檔案，Adobe Dynamic Media Classic會將要上載的資產視為重複資產。 因此，其名稱會附加數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 儘管該項目已從您的Adobe Dynamic Media Classic資料夾中刪除，但當其ID保留在「垃圾」資料夾中時，無法將其ID分配給其他資產。 如果嘗試上載與「垃圾」資料夾中的檔案同名的資產，Adobe Dynamic Media Classic會在資產名稱中附加數字。
* 無法發佈項目。即使項目在您刪除時已標記為發佈，您也無法予以發佈。
* 該項目將保留在「垃圾」資料夾中，直到其恢復、七天過去或有人選擇 **[!UICONTROL 清理垃圾]** 的子菜單。 七天之後，自動清除作業就會永久刪除項目。

## 從垃圾資料夾還原資產 {#restoring-assets-from-the-trash-folder}

刪除資產的人無需恢復；任何人都可以從垃圾資料夾中恢復資產。 還原的資產會放在其刪除來源的檔案夾中。如果這些資料夾不再存在，Adobe Dynamic Media Classic會重新建立它們，並將還原的資產放置在重新建立的資料夾中。

要將資產從垃圾資料夾還原到從中刪除這些資產的資料夾，請執行以下操作：

1. 在「資產庫」面板的底部，選擇 **[!UICONTROL 垃圾]** 表徵圖以開啟「垃圾」資料夾。
1. 選擇要恢復的資產。
1. 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾箱恢復]**。

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。七天後就會從「垃圾桶」檔案夾中永久刪除資產。

要從「垃圾」資料夾中永久刪除資產，請選擇 **[!UICONTROL 垃圾]** 表徵圖 在「垃圾資料夾」頁上，執行下列任一操作：

* **刪除單個資產**  — 選擇要永久刪除的資產，然後轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾中清空]**。

* **刪除所有資產**  — 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 空垃圾]**。

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)

