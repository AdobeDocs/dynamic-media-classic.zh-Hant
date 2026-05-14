---
title: 管理FTP帳戶
description: 瞭解如何在Adobe Dynamic Media Classic中管理FTP帳戶。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 95c7d403-7206-4158-b8ad-6091b24b5077
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:36.235Z'
TQID: 'https://experienceleague.adobe.com/6fNfI7Na3jeDys307id5U9nIt-DeWCmfwtIzsb0G73I'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 239
ht-degree: 52%

---

# 管理FTP帳戶{#managing-ftp-accounts}

只有 Media Portal 管理員才能夠管理 FTP 帳戶。 此外，只有角色為&#x200B;*Media Portal參與者 — 使用者*&#x200B;或&#x200B;*Media Portal參與者*&#x200B;的使用者才能上傳數位資產。

請記住，您可以透過「管理設定」中的「使用者管理」頁面來啟用或停用現有的 Media Portal 使用者。

請參閱[啟用或停用使用者](administration-setup.md#activating_or_deactivating_users)。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 媒體入口網站]** > **[!UICONTROL FTP帳戶]**。
1. 在「新增 FTP 帳戶」頁面的「FTP 帳戶使用者名稱」下拉式清單中，選取使用者。

   如果未列出使用者，您必須透過管理設定將他們新增為Media Portal管理員、Media Portal投稿人 — 使用者或Media Portal投稿人。 增加含有適當角色的使用者之後，他們的使用者名稱便會出現在下拉式清單中。

   請參閱[新增Media Portal使用者](adding-media-portal-users.md#adding_a_media_portal_user)。

1. 在「密碼」和「確認」欄位中，輸入 FTP 帳戶的密碼。
1. 選取&#x200B;**[!UICONTROL 儲存]**，將帳戶新增至[現有帳戶]資料表。

   若要上載媒體資產，您需要列於「現有帳戶」表格中的「FTP 帳戶使用者名稱」，以及指定給該帳戶的密碼。

   請參閱[上傳檔案](uploading-files.md#uploading_files)。

## 刪除現有的FTP帳戶 {#deleting-an-existing-ftp-account}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 媒體入口網站]** > **[!UICONTROL FTP帳戶]**。
1. 在「新增 FTP 帳戶」頁面的「現有帳戶」表格中，選取您要移除的 FTP 帳戶。
1. 選取&#x200B;**[!UICONTROL 刪除]**。
