---
title: 增加和管理 Media Portal 使用者
seo-title: 增加和管理 Media Portal 使用者
description: 'null'
seo-description: 瞭解如何新增和管理Media Portal使用者
uuid: 96d4103c-6428-4ce1-b9 e4-231599304f27
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PK/categories/media_ Portal
discoiquuid: 5e933045-cce1 a-41b9-ba8 b-2151c396 b7 a
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 增加和管理 Media Portal 使用者{#adding-and-managing-media-portal-users}

身為管理員，您可以增加和管理使用者、決定使用者是否能夠變更密碼、編輯使用者資訊，以及上載使用者清單。這些工作都可以在「使用者管理」畫面上完成。若要存取這個畫面，請按一下「**設定** &gt; **應用程式設定** &gt; **管理設定** &gt; **使用者管理**」。

>[!NOTE]
>
>增加使用者之前，請先設定用來管理使用者的群組。如果您在增加使用者時，沒有為使用者指定一或多個群組，則 Media Portal 不會讓您增加使用者。如需詳細資訊，請參閱[建立和管理 Media Portal 群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

## 處理 Media Portal 密碼 {#handling-media-portal-passwords}

Media Portal 使用者、參與者及參與者 - 使用者都會收到「歡迎」電子郵件，其中含有您予以註冊時所使用的密碼。管理員可以決定 Media Portal 使用者是否能夠變更此密碼。

1. 按一下「**設定** &gt; **Media Portal 設定** &gt; **一般設定**」。
1. 在「一般設定」頁面上，選取或取消選取&#x200B;**允許 Media Portal 使用者變更密碼**。
1. 按一下「**儲存**」。

>[!NOTE]
>
>可以變更密碼的 Media Portal 使用者，可以按一下「**設定** &gt; **個人設定**」，並在「個人設定」畫面上更改密碼，以進行此動作。

## 增加 Media Portal 使用者 {#adding-a-media-portal-user}

1. 按一下「**設定** &gt; **應用程式設定** &gt; **管理設定** &gt; **使用者管理**」。
1. 在「使用者管理」頁面上，按一下「**增加**」。
1. 在「增加使用者」對話框的「使用者資訊」面板中，輸入使用者的「名字」、「姓氏」和「電子郵件地址」，然後按&#x200B;**下一步**。
1. 在「公司/角色」面板的「公司」下拉式清單中，選取該使用者的一或多個公司。
1. 在「角色」清單中，選取一個 Media Portal 角色，然後按&#x200B;**下一步**。

   請參閱[Media Portal 使用者角色](media-portal-user-roles.md#media_portal_user_roles)。

1. 在「存取群組」面板中，選取一或多個群組。

   請參閱[建立和管理 Media Portal 群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

1. (選擇性) 按一下「**電子郵件設定**」可選擇與預設設定不同的電子郵件設定。

   請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。

1. 按一下「**增加使用者**」。

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
| 使用者角色 | MediaPortorTaleMediaPortalTalUserMediaPremiertorContributorMediaPrepertoruser |
| 群組 | 為每個使用者指定的一或多個帳戶群組的清單 (以逗號分隔)。您可以透過為帳戶名稱添加字首以指定群組，並以正斜線 (/) 區隔之。例如，若 PortalCo 為帳戶而 IT 為 PortalCo 帳戶內的群組，則為「PortalCo/IT」。 |

下列範例試算表示範如何配置 CSV 檔案:

| 名字 | 姓氏 | 電子郵件 | 密碼 | 使用者角色 | 群組 |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | 歡迎 | Media Portal 管理員 | PortalCo/IT,PortalCo/Admin |
| Kevin | Marks | `kevinm@myco.com` | 歡迎 | Media Portal 使用者 | PortalCo/MktgGroup, PortalCo/test |


### 上載 CSV 檔案 {#uploading-the-csv-file}

1. 開啟「使用者管理設定」畫面。
1. 按一下「**上載使用者清單**」。
1. 在「選取要上載的檔案」對話框中選取 CSV 檔案，然後按一下「**開啟**」。

清單中的每個使用者都會自動增加到指定的群組中。系統會將「歡迎」電子郵件傳送給每個使用者。

>[!NOTE]
如果 CSV 檔案的格式不正確，則會出現下列錯誤訊息:「處理上載的 CSV 檔案時發生錯誤。請檢查檔案內容是否為有效資料。」 此外，如果 CSV 包含現有的 IP 或 IPS 使用者，該使用者就不會增加到「使用者清單」中。

## 產生 Media Portal 使用者的可選取清單 {#generating-a-selectable-list-of-media-portal-users}

您可以在彈出式視窗中，顯示 Media Portal 使用者的名稱與電子郵件地址。這份清單有助您剪下並貼上使用者名稱與位址，在 Media Portal 以外使用。

1. 按一下「**設定** &gt; **應用程式設定** &gt; **管理設定** &gt; **使用者管理**」。
1. 在「**依使用者角色**」下拉式清單中，選擇 Media Portal 使用者角色的名稱，然後按一下「**重新整理**」，即可顯示某一類 Media Portal 使用者的名稱。
1. 按一下「**彈出式清單**」，即可開啟彈出式視窗。您可以複製和貼上這份清單。

## 設定 Media Portal 使用者的「歡迎」電子郵件 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新增 Media Portal 使用者、參與者及參與者 - 使用者時，可以傳送「歡迎」電子郵件。您可以設定此電子郵件訊息，或告訴Dynamic Media Classic不要傳送它。

1. 選擇「**設定** &gt; **應用程式設定** &gt; **管理設定** &gt; **使用者管理**」。
1. In the User Administration Setup screen, click **Email Settings**.
1. 在「電子郵件設定」對話框中，指定下列任一設定:

   **傳送電子郵件** ：如果您不想透過電子郵件通知新使用者，請取消選取此選項。

   **預設密碼** 輸入新使用者的暫時密碼，或將欄位留空，使動態媒體Classic產生隨機密碼。系統會在使用者首次登入時，要求使用者變更密碼。

   **取代URL** ：如果您的使用者透過不同的URL存取動態媒體Classic，請輸入與預設值不同的URL。

## 其它使用者管理任務 {#other-user-management-tasks}

從「使用者管理設定」畫面開始，您也可以執行下列工作:

**篩選並排序使用者清單** 篩選Media Portal使用者清單以找出使用者。請參閱篩選和排序使用者清單。

**刪除使用者** 從清單刪除使用者。請參閱刪除使用者。

**啓用和停用使用者** 暫停使用者存取資料夾。請參閱啟用和停用使用者。

**編輯使用者資訊** 輸入使用者的最新資訊。請參閱編輯使用者資訊。

**建立使用者定義欄位** 建立自訂、使用者定義的中繼資料欄位，以協助組織Scene Publishing System中的資產。這些欄位也可視需要啟用或停用。

請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。