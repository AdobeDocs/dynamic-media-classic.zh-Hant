---
title: 快速入門： Media Portal
description: Media Portal簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速啟動和執行Media Portal技術和管理。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 45%

---

# 快速入門： Media Portal{#quick-start-media-portal}

Media Portal可讓公司輕鬆取得、控制資產，並將核准的資產發佈給外部合作夥伴和管道，以及公司的內部使用者。 這個以瀏覽器為基礎的「自助式」環境為Media Portal使用者提供由管理員控制的Adobe Dynamic Media Classic資產「檢視」，方便他們以公司核准的格式存取、瀏覽、搜尋、預覽和匯出資產。

身為管理員，您可以控制使用者在 Media Portal 中檢視、存取和使用資產的方式。此外，您可以自訂Media Portal介面，以符合您的網站和品牌。 您可以在Media Portal介面中指定字型、字型顏色、字型大小，以及合併商標元素（例如標誌）。

請參閱下列訓練影片：

* [Media Portal概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Media Portal導覽1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Media Portal導覽2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

下列快速入門旨在協助您快速上手並執行Media Portal管理。 在每個步驟結束時，選取主題連結以瞭解更多資訊。

## 1. 瞭解 Media Portal 使用者角色

Media Portal使用者分為三種角色：使用者、貢獻者和使用者貢獻者。 每個角色都可以執行不同的工作組合。例如，參與者可以重新命名和刪除檔案和檔案夾，但使用者不能執行這些工作。瞭解不同角色，可讓您在增加使用者時，知道應賦予他們哪些責任。

請參閱[Media Portal 使用者角色](media-portal-user-roles.md#media_portal_user_roles)。

## 2. 建立群組以管理使用者

群組可決定使用者有權存取的檔案夾與檔案、使用者可對這些檔案夾與檔案執行哪些動作，以及可使用哪些影像預設集。身為管理員，您的首要工作就是建立群組。針對每個群組決定其成員能夠存取的檔案夾、檔案及影像預設集。同時將讀取、寫入及刪除權限授與群組成員。這些權限可決定成員是否能夠瀏覽、編輯、重新命名和刪除他們有權存取的檔案夾與檔案。

請參閱[建立和管理Media Portal群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

## 3. 增加使用者

增加使用者時，可以為使用者指定角色 (使用者、參與者或使用者 - 參與者)。您也可以將使用者指派給一或多個群組。 為了加速增加使用者的程序，您可以使用 CSV 檔案的形式上載使用者清單。新使用者會收到「歡迎」電子郵件以及登入 Media Portal 的指示。

請參閱[新增及管理Media Portal使用者](adding-media-portal-users.md#adding_and_managing_media_portal_users)。

## 4. 管理 FTP 帳戶

您可以有與Media Portal關聯的個別FTP帳戶。 它們可以對應至您Adobe Dynamic Media Classic帳戶中的特定資料夾。 這種功能表示，您可以允許使用者透過個別的 FTP 帳戶將數位資產上載至您的帳戶中。

請參閱[管理FTP帳戶](ftp-accounts.md#managing_ftp_accounts)。

>[!NOTE]
>
>只有Media Portal管理員可以管理這些FTP帳戶。 此外，只有具有「Media Portal 參與者 - 使用者」或「Media Portal 參與者」角色的使用者，才能夠上載檔案。

請參閱[Media Portal 使用者角色](media-portal-user-roles.md#media_portal_user_roles)。

## 5. 指定匯出選項

Media Portal使用者匯出檔案時，可以重新格式化檔案並匯出原始主要檔案（如果您授予他們執行此作業的許可權）。 身為管理員，您可以決定使用者匯出檔案的方式。

請參閱[指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

## 6. 建立影像預設集

影像預設集是預先定義設定的集合。 這些設定可變更匯出影像時的尺寸、影像品質、格式、解析度及其他外觀方面。 您可以建立影像預設集，來控制使用者匯出影像時，對影像重新格式化的方式。

請參閱[建立和啟用影像預設集](creating-enabling-image-presets.md#creating_and_enabling_image_presets)。

## 7. 建立中繼資料預設集與使用者定義的中繼資料欄位

中繼資料會說明並識別檔案。 它可用來搜尋及組織資產。 您可以建立中繼資料預設集，以確保您正確輸入中繼資料，並填入任何需要資料的中繼資料欄位。 中繼資料預設集是預先定義的一組中繼資料項目。您也可以建立能夠以唯一方式說明您處理之檔案的中繼資料欄位。

請參閱[更有效地使用中繼資料](making-efficient-metadata.md#making_more_efficient_use_of_metadata)。

## 8.自訂Media Portal

Media Portal樣式設定可讓您使用公司的標誌和顏色來包裝Media Portal頁面。 使用樣式設定將您的公司品牌置於Media Portal上。

請參閱[自訂Media Portal頁面](customizing-media-portal-screen.md#customizing_the_media_portal_screen)
