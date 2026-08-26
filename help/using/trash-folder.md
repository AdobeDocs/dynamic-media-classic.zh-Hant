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
autotag-review: '2026-05-13T20:15:24.015Z'
TQID: 'https://experienceleague.adobe.com/5XOu6T0n7zssUzXgQXushja4DJBSHs8-0-2h2Ao1L20'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 6da2e49f8dde8d9bbedb1d4264f34d52548d0d6c
workflow-type: tm+mt
source-wordcount: 562
ht-degree: 24%

---

# 管理垃圾桶資料夾{#managing-the-trash-folder}

您從Adobe Dynamic Media Classic刪除的專案會移至垃圾桶資料夾。 這些已刪除的專案會在此資料夾中保留七天，直到還原或永久刪除為止。 您可以選取資產庫底部的&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;圖示，並檢視「垃圾桶」資料夾頁面中的專案，以檢查已刪除的專案。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。 所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

若從垃圾桶資料夾刪除專案，將會永久刪除Adobe Dynamic Media Classic中的專案；若從垃圾桶資料夾刪除專案，將無法再還原。 如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶資料夾的Assets仍可在Adobe Dynamic Media Classic上註冊。 例如，假設您嘗試上傳的檔案名稱與垃圾桶資料夾中已刪除的檔案名稱相同。 Adobe Dynamic Media Classic會將您要上傳的資產視為重複資產。 在這種情況下，會在名稱后面附加一個數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。 刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 雖然專案已從您的Adobe Dynamic Media Classic資料夾中移除，但其ID無法指派給另一個資產，因為它仍保留在垃圾桶資料夾中。 如果您嘗試上傳與垃圾桶資料夾中檔案同名的資產，Adobe Dynamic Media Classic會在資產名稱后面附加一個數字。
* 無法發佈項目。 即使專案在您刪除時標籤為發佈，它也不會發佈。
* 專案會保留在垃圾桶資料夾中，直到還原為止、過了七天或有人選擇&#x200B;**[!UICONTROL 清空垃圾桶]**&#x200B;命令。 七天後，自動刪除操作會永久刪除專案。

## 從垃圾桶資料夾中還原資產 {#restoring-assets-from-the-trash-folder}

刪除資產的人不需要還原資產；任何人都可以從垃圾桶資料夾還原資產。 還原的資產會放在其刪除來源的檔案夾中。 如果這些資料夾已不存在，Adobe Dynamic Media Classic會重新建立它們，而且還原的資產會放在重新建立的資料夾中。

若要將資產從垃圾桶資料夾還原至其被刪除的資料夾，請執行下列動作：

1. 在「資產庫」面板底部，選取&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;圖示以開啟「垃圾桶」資料夾。
1. 選取您要還原的一個或多個資產。
1. 移至&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶還原]**。

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。 七天後就會從「垃圾桶」檔案夾中永久刪除資產。

您可以選取&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;圖示，從「垃圾桶」資料夾中永久刪除資產。 在「垃圾桶」資料夾頁面上，執行下列任一項作業：

* **刪除個別資產**：您可以永久刪除資產。 選取您想要的資產，然後按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶清空]**。

* **正在刪除所有資產**：移至&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 清空垃圾桶]**。

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)
