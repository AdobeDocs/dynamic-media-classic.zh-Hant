---
title: 管理垃圾桶檔案夾
seo-title: 管理垃圾桶檔案夾
description: 'null'
seo-description: 瞭解如何管理垃圾筒資料夾。
uuid: 3992a5b8-1919-4924-b07 d-7fb25565 fetter
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/managing_ assets
discoiquuid: 553c95fc -a41-4f06-af50-a62 bc1438149
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 管理垃圾桶檔案夾{#managing-the-trash-folder}

從 Scene7 Publishing System 中刪除的項目會移動到「垃圾桶」檔案夾。這些項目會在這個檔案夾中保留七天，直到還原或永久刪除為止。您可以選取「垃圾桶」圖示  (位於資產庫下方)，然後檢視「垃圾桶」檔案夾中的項目，即可檢查已刪除的項目。

所有使用者都可以將「垃圾桶」檔案夾中的項目還原到其刪除來源的檔案夾。所有使用者也都可以清空「垃圾桶」檔案夾中的所有內容。

如果從「垃圾桶」檔案夾中刪除項目，就會從 Scene7 Publishing System 中永久刪除該項目；從「垃圾桶」檔案夾中刪除的項目再也無法還原。如需設定在資產即將從「垃圾桶」中自動刪除時通知公司管理員的資訊，請參閱[應用程式一般設定](application-setup.md#general_settings)。

>[!NOTE]
>
>移動到「垃圾桶」檔案夾的資產，在 Scene7 Publishing System 上仍處於已註冊狀態。如果您嘗試上傳與「垃圾筒」檔案夾中已刪除檔案同名的檔案，Dynamic Media Classic會將您想要上傳的資產視為重復資產。因此，其名稱會附加數字。

## 關於垃圾桶檔案夾 {#about-the-trash-folder}

刪除檔案夾中的項目會將該項目放入「垃圾桶」檔案夾。刪除項目並將它移動到「垃圾桶」檔案夾時，會發生下列狀況:

* 雖然項目已從您的 Scene7 Publishing System 檔案夾中移除，但是只要它仍留在「垃圾桶」檔案夾中，其 ID 就無法指定給其它資產。如果您嘗試上傳與「垃圾筒」檔案夾中相同名稱的資產，Dynamic Media Classic會附加數字至資產名稱。
* 無法發佈項目。即使項目在您刪除時已標記為發佈，您也無法予以發佈。
* 項目會保留在「垃圾桶」檔案夾中，直到予以還原、經過七天，或是某人選擇「清空垃圾桶」命令為止。七天之後，自動清除作業就會永久刪除項目。

## 從垃圾桶檔案夾中復原資產 {#restoring-assets-from-the-trash-folder}

並非刪除資產的人才能夠還原資產；任何人都可以從「垃圾桶」檔案夾中還原資產。還原的資產會放在其刪除來源的檔案夾中。如果這些檔案夾已不存在，Scene7 Publishing System 就會予以重新建立，並將還原的資產放在重新建立的檔案夾中。

遵循下列步驟，即可將資產從「垃圾桶」檔案夾還原到其刪除來源的檔案夾:

1. 按一下「垃圾筒」圖示以開啓「垃圾筒」檔案夾。
1. 選取您要還原的資產。
1. 選擇「檔案 &gt; 從垃圾桶還原」。

## 永久刪除垃圾桶檔案夾中的資產 {#permanently-deleting-assets-in-the-trash-folder}

刪除「垃圾桶」檔案夾中的資產時，會永久刪除該資產。七天後就會從「垃圾桶」檔案夾中永久刪除資產。

若要永久刪除「垃圾桶」檔案夾中的資產，請選取「垃圾桶」圖示 ，以開啟「垃圾桶」檔案夾。然後刪除檔案夾中的個別資產或所有資產:

**刪除個別資產** 選取您要永久刪除的資產，然後按一下「檔案&gt;空從垃圾桶」。

**刪除所有資產** 按一下「檔案&gt;空垃圾筒」。

>[!MORELIKETHIS]
>
>* [刪除資產](moving-renaming-deleting-assets.md#delete_assets)

