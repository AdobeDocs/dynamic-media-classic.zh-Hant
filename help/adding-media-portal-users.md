---
title: 添加和管理媒體門戶用戶
description: 瞭解如何添加和管理Adobe Dynamic Media Classic的媒體門戶用戶。
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 58%

---

# 添加和管理媒體門戶用戶{#adding-and-managing-media-portal-users}

身為管理員，您可以增加和管理使用者、決定使用者是否能夠變更密碼、編輯使用者資訊，以及上載使用者清單。這些工作都可以在「使用者管理」畫面上完成。要訪問此螢幕，請導航到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。

>[!NOTE]
>
>增加使用者之前，請先設定用來管理使用者的群組。如果您在增加使用者時，沒有為使用者指定一或多個群組，則 Media Portal 不會讓您增加使用者。有關詳細資訊，請參見 [建立和管理媒體門戶組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

## 管理媒體門戶密碼 {#handling-media-portal-passwords}

Media Portal 使用者、參與者及參與者 - 使用者都會收到「歡迎」電子郵件，其中含有您予以註冊時所使用的密碼。管理員可以決定 Media Portal 使用者是否能夠變更此密碼。

1. 導航到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 常規設定]**。
1. 在「一般設定」頁面上，選取或取消選取&#x200B;**[!UICONTROL 允許 Media Portal 使用者變更密碼]**。
1. 選擇 **[!UICONTROL 保存]**。

>[!NOTE]
>
>允許更改密碼的媒體門戶用戶可以通過選擇 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]** 和更改「個人設定」螢幕上的密碼。

## 添加媒體門戶用戶 {#adding-a-media-portal-user}

1. 導航到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 在「用戶管理」頁上，選擇 **添加**。
1. 在「添加用戶」對話框的「用戶資訊」面板中，輸入用戶的名字、姓氏和電子郵件地址，然後選擇 **[!UICONTROL 下一個]**。
1. 在「公司/角色」面板的「公司」下拉式清單中，選取該使用者的一或多個公司。
1. 在角色清單中，選擇介質門戶角色，然後選擇 **[!UICONTROL 下一個]**。

   請參閱[Media Portal 使用者角色](media-portal-user-roles.md#media_portal_user_roles)。

1. 在「存取群組」面板中，選取一或多個群組。

   請參閱 [建立和管理媒體門戶組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

1. （可選）選擇 **[!UICONTROL 電子郵件設定]** 選擇與預設設定不同的電子郵件設定。

   請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。

1. 選擇 **[!UICONTROL 添加用戶]**。

增加使用者之後，Media Portal 會將「歡迎」電子郵件傳送給該使用者。該訊息含有臨時密碼與 Media Portal URL。

## 上載 Media Portal 使用者清單 {#uploading-a-media-portal-user-list}

如果您要增加數個使用者，則可以上載使用者清單。使用者會自動增加到目前選取的帳戶中。

將使用者清單建立為含有使用者資訊的 CSV (逗號分隔值) 檔案。上載清單之後，清單中的使用者就會與指定的群組指派一起自動增加到帳戶中。系統會將「歡迎」電子郵件傳送給每個新使用者，其中包含 Media Portal 的連結與臨時密碼。

### 建立 CSV 檔案 {#creating-the-csv-file}

建立符合下列格式與欄位的 CSV 檔案 (filename.csv)。檔案的第一列必須包含此表格列出的欄標題；您可以視需要排序這些欄。所有欄都是必要欄。

| 欄名稱 | 說明 |
|--- |--- |
| 名字 | 名字。 |
| 姓氏 | 姓氏。 |
| 電子郵件 | 有效的電子郵件地址。 |
| 密碼 | 區分大小寫的密碼字串。 |
| 使用者角色 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| 群組 | 為每個使用者指定的一或多個帳戶群組的清單 (以逗號分隔)。您可以透過為帳戶名稱添加字首以指定群組，並以正斜線 (/) 區隔之。例如，若 PortalCo 為帳戶而 IT 為 PortalCo 帳戶內的群組，則為「PortalCo/IT」。 |

下列範例試算表示範如何配置 CSV 檔案:

| 名字 | 姓氏 | 電子郵件 | 密碼 | 使用者角色 | 群組 |
|--- |--- |--- |--- |--- |--- |
| 草原 | 凱特 | `prairiek@company.com` | 歡迎 | Media Portal 管理員 | PortalCo/IT,PortalCo/Admin |
| 里克 | 布魯 | `rickb@myco.com` | 歡迎 | Media Portal 使用者 | PortalCo/MktgGroup, PortalCo/test |

### 上載 CSV 檔案 {#uploading-the-csv-file}

1. 開啟「使用者管理設定」畫面。
1. 選擇 **[!UICONTROL 上載用戶清單]**。
1. 在「選擇要上載的檔案」對話框中，選擇CSV檔案，然後選擇 **[!UICONTROL 開啟]**。

清單中的每個使用者都會自動增加到指定的群組中。系統會將「歡迎」電子郵件傳送給每個使用者。

>[!NOTE]
>
>如果 CSV 檔案的格式不正確，則會出現下列錯誤訊息:「處理上載的 CSV 檔案時發生錯誤。請檢查檔案內容是否為有效資料。」 此外，如果 CSV 包含現有的 IP 或 IPS 使用者，該使用者就不會增加到「使用者清單」中。

## 產生 Media Portal 使用者的可選取清單 {#generating-a-selectable-list-of-media-portal-users}

您可以在彈出式視窗中，顯示 Media Portal 使用者的名稱與電子郵件地址。這份清單有助您剪下並貼上使用者名稱與位址，在 Media Portal 以外使用。

1. 導航到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 在 **[!UICONTROL 按用戶角色]** 下拉清單，選擇媒體門戶用戶角色的名稱，然後選擇 **[!UICONTROL 刷新]** 顯示一個類媒體門戶用戶的名稱。
1. 選擇 **[!UICONTROL 彈出清單]**。 複製並貼上此清單。

## 設定 Media Portal 使用者的「歡迎」電子郵件 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新增 Media Portal 使用者、參與者及參與者 - 使用者時，可以傳送「歡迎」電子郵件。您可以配置此電子郵件或告訴Adobe Dynamic Media Classic不要發送它。

1. 導航到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 在「用戶管理設定」螢幕中，選擇 **[!UICONTROL 電子郵件設定]**。
1. 在「電子郵件設定」對話框中，指定下列任一設定:

   * **[!UICONTROL 發送電子郵件]**  — 如果不想通過電子郵件通知新用戶您已註冊，請取消選擇此選項。

   * **[!UICONTROL 預設密碼]**  — 為新用戶輸入臨時密碼，或將欄位留空以使Adobe Dynamic Media Classic生成隨機密碼。 用戶首次登錄時被要求更改密碼。

   * **[!UICONTROL 替換URL]**  — 如果用戶通過其他URL訪問Adobe Dynamic Media Classic，則輸入與預設URL不同的URL。

## 其它使用者管理任務 {#other-user-management-tasks}

從「使用者管理設定」畫面開始，您也可以執行下列工作:

* **[!UICONTROL 篩選和排序用戶清單]**  — 篩選媒體門戶用戶清單以查找用戶。

* **[!UICONTROL 刪除用戶]**  — 從清單中刪除用戶。

* **[!UICONTROL 激活和停用用戶]**  — 暫停用戶訪問資料夾。

* **[!UICONTROL 編輯用戶資訊]**  — 輸入有關用戶的最新資訊。

* **[!UICONTROL 建立用戶定義的欄位]**  — 建立自定義的、用戶定義的元資料欄位，以便它們能夠幫助您組織Adobe Dynamic Media Classic的資產。 這些欄位也可視需要啟用或停用。

請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。
