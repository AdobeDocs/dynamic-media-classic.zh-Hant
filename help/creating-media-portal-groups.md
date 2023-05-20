---
title: 建立和管理媒體門戶組
description: 瞭解如何在Adobe Dynamic Media Classic建立和管理媒體門戶組。
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 56%

---

# 建立和管理媒體門戶組{#creating-and-managing-media-portal-groups}

*群組*&#x200B;的設計可協助您管理 Media Portal 使用者。使用者必須是至少一個有權存取資產的群組的成員。您增加使用者時，可將使用者指定給一或多個群組。這樣一來，您就會將已指定給該群組的檔案夾存取權授與該使用者。您也可以選擇要讓群組使用哪些影像預設集。

## 使用組限制對資料夾、資產和影像預設的訪問 {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

若要在不同層級授與存取權限，請建立群組。針對每個群組，您可以指定不同檔案夾與檔案夾中資產的讀取、寫入及刪除權限。此外，您還可以決定要讓群組使用哪些影像預設集。接著將使用者指定給群組。使用者可以是一或多個群組的成員。群組的概念可讓您靈活地為整體內容中的有限集合指定存取權。

如果您沒有具體為資產或資料夾授予組權限，則該資產或資料夾將繼承您分配給其父資料夾（資料夾層次結構中位於其上方的資料夾）的權限。 如果要確保某個檔案夾中的所有下層檔案夾都繼承相同權限，請將權限授與該父級檔案夾。

>[!NOTE]
>
>使用者可以隸屬於多個群組。如果使用者所屬的群組對於某個檔案夾擁有不同存取權限，則會將最高存取權授與該使用者。

## 增加群組 {#adding-a-group}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 組]**。
1. 選擇 **[!UICONTROL 添加]**。
1. 在「添加組」對話框中，在「組名」框中輸入組的名稱，然後選擇 **[!UICONTROL 添加組]**。
1. 您也可以選取使用者名稱旁的方框，將該使用者增加到新群組。
1. 如果要立即指定訪問權限，請選擇 **[!UICONTROL 資產訪問權限]** ，然後指定所需的選項。

   請參閱[為群組建立資產存取權限](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group)。

1. 如果要選擇組可用的影像預設，請選擇 **[!UICONTROL 影像預設訪問權限]** ，然後選擇組可以使用的影像預設。

   請參閱[為群組選擇影像預設集存取權限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。

1. 選擇 **[!UICONTROL 關閉]**。

## 為群組建立資產存取權限 {#establishing-asset-access-permissions-for-a-group}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 組]**。
1. 在「群組清單」頁面上，執行下列其中一個動作:

   * 要添加組並指定權限，請選擇 **[!UICONTROL 添加]**。 在「添加組」對話框中，輸入組的名稱，選擇 **[!UICONTROL 添加組]**，並將用戶添加到組。
   * 要編輯組的權限，請選擇組，然後選擇 **[!UICONTROL 編輯]**。

1. 在「添加組」或「編輯組」對話框中，選擇 **[!UICONTROL 資產訪問權限]** 頁籤。 標籤右側提供的方框可用來建立檔案夾與資產的讀取、寫入及刪除權限。您可以在左窗格中，展開和收合檔案夾與子檔案夾。
1. 若要為檔案夾或個別資產指定權限，請在左窗格中選取檔案夾。檔案夾內容會顯示在右窗格中。接著，在右窗格中選取相應檔案或檔案夾的方框，即可為群組指定權限。

   這個表格會將不同工作對映到讀取、寫入及刪除權限。

   | 工作 | 已讀 | 寫入 | 刪除 |
   | --- | --- | --- | --- |
   | 瀏覽檔案夾與檔案 | X |  |  |
   | 編輯檔案 (裁切、銳利化、調整) |  | X |  |
   | 變更檔案名稱 |  | X |  |
   | 將檔案移至其他檔案夾 |  | X |  |
   | 重新命名檔案 |  | X |  |
   | 刪除檔案 |  |  | X |

1. 選擇 **[!UICONTROL 關閉]**。

>[!NOTE]
>
>選取方框後便會建立存取權。將權限指定給檔案夾時，也會將該檔案夾的權限指定給其子檔案夾與其中的所有檔案。不過，您可以針對個別子檔案夾與資產檔案指定不同權限。

## 為群組選擇影像預設集存取權限 {#choosing-image-preset-access-permissions-for-a-group}

如果要指定群組成員在透過 Media Portal 匯出資產時，可以使用哪些影像預設集，請為群組選擇影像預設集存取權限。

另請參閱 [指定媒體門戶用戶可用的導出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

**要為組選擇「影像預設」訪問權限：**

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 組]**。
1. 在「群組清單」頁面上，執行下列其中一個動作:

   * 要添加組並指定可用的影像預設，請選擇 **[!UICONTROL 添加]**。 在「添加組」對話框中，輸入組的名稱，選擇 **[!UICONTROL 添加組]**，並將用戶添加到組。
   * 要編輯組的「影像預設」選項，請選擇組，然後選擇 **[!UICONTROL 編輯]**。

1. 在「添加組」或「編輯組」對話框中，選擇 **[!UICONTROL 影像預設訪問權限]** 頁籤。
1. 要指定媒體門戶用戶在導出資產時可以使用的預設，請選擇或取消選擇「影像預設」。
1. 選擇 **[!UICONTROL 關閉]**。

## 編輯和刪除群組 {#edit-and-delete-groups}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 組]**。
1. 在「群組清單」頁面上，選取某個群組，然後加以編輯或刪除。

   **編輯組**  — 選擇 **[!UICONTROL 編輯]**，然後在「編輯組」對話框中選擇選項。

   **刪除組**  — 選擇 **[!UICONTROL 刪除]**。
