---
title: 管理設定
description: 瞭解如何設定Adobe Dynamic Media Classic的管理區域。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1969'
ht-degree: 33%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

管理設定螢幕用於管理Adobe Dynamic Media Classic用戶。 使用這些螢幕可讓用戶在Adobe Dynamic Media Classic工作，並通過電子郵件與用戶通信。

1. 要訪問「管理設定」選項，請轉到 **設定** > **個人設定** > **管理設定**。

## 使用者管理 {#user-administration}

所有Adobe Dynamic Media Classic用戶都被分配一個角色，確定他們對Adobe Dynamic Media Classic功能的權限和訪問權限。 管理員會決定不同角色和其對於所指派公司的責任。

通常，Adobe Dynamic Media Classic會配置第一組公司，並指派公司管理員。 然後，公司管理員設定並管理Adobe Dynamic Media Classic用戶。

Adobe Dynamic Media Classic支援多個用戶角色。 這些角色可以訪問為Adobe Dynamic Media Classic設立的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic用戶** 可以訪問他們被指派到的公司；不能履行任何管理職責。

**Adobe Dynamic Media Classic公司管理員** 只能查看和管理自己的公司。 公司管理員也可以執行所有管理功能，包含增加管理員和使用者。公司管理員可以將用戶添加到DMC公司管理員帳戶。 (此角色為預設使用者角色。)

添加用戶後，Adobe Dynamic Media Classic會向用戶發送歡迎電子郵件。 該消息包括密碼和Adobe Dynamic Media ClassicURL。

### 添加用戶或管理員 {#adding-a-user-or-administrator}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 選擇 **[!UICONTROL 添加]**。
1. 輸入要添加的用戶或管理員的姓名和電子郵件地址，然後選擇 **[!UICONTROL 下一個]**。

   >[!NOTE]
   >
   >撇號字元(`‘`)在電子郵件地址中不允許。

1. 要為用戶分配角色，請選擇「角色」選項。

   請參閱 [Adobe Dynamic Media Classic用戶角色和權限](administration-setup.md#user_administration)。

1. 要將用戶添加到公司，請選擇公司名稱。
1. 如果要將用戶添加到組（如果要添加媒體門戶用戶或參與者），請選擇 **[!UICONTROL 下一個]** 並添加用戶。
1. 選擇 **[!UICONTROL 保存]** 完成用戶設定。

   系統會在儲存之後出現提示訊息，問您是否要將使用者增加至其他公司。選擇 **[!UICONTROL 添加]** 的子菜單。

   所有新用戶都得到隨機生成的密碼；用戶首次登錄Adobe Dynamic Media Classic案頭應用程式時必須更改密碼。

   您增加新使用者後，新的使用者便會收到「歡迎」電子郵件。該電子郵件提供了臨時密碼並說明如何登錄Adobe Dynamic Media Classic。

   如果用戶未收到歡迎電子郵件，請讓他們轉到Adobe Dynamic Media Classic登錄頁(https://s7sps1.scene7.com)，然後選擇 **[!UICONTROL 忘記密碼]**。 已重設密碼並傳送新的電子郵件。如果使用者沒有收到電子郵件，也沒有在「垃圾郵件」資料夾中也發現，請聯絡「技術支援」。

   添加新媒體門戶用戶時，您還可以 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 用戶管理]**，然後選擇 **[!UICONTROL 上載用戶清單]** 並選擇一個不超過500個用戶的.csv檔案。

### 刪除使用者 {#deleting-a-user}

您可以通過使用戶無效從Adobe Dynamic Media Classic刪除用戶。 無效的使用者會從系統和所有帳戶中移除。

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 從清單中選擇用戶，然後選擇 **[!UICONTROL 編輯]**。
1. 取消選取「有效」。
1. 選擇 **[!UICONTROL 保存]**。

### 激活或停用用戶 {#activating-or-deactivating-users}

已停用的使用者將不再擁有進入「選取要存取的帳戶」選單上方列出之帳戶的權限。

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 在用戶清單中，選擇或取消選擇 **[!UICONTROL 活動]** 的子菜單。

### 編輯使用者資訊 {#editing-user-information}

您可以編輯的使用者資訊視您的管理員角色，以及您要編輯其資訊之使用者獲得指派的角色而定。顏色較暗 (不可用) 的選項無法編輯。

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 用戶管理]**。
1. 從清單中選擇用戶，然後選擇 **[!UICONTROL 編輯]**。
1. 選擇表中顯示您試圖修改權限或訪問權限的公司的條目，然後選擇 **[!UICONTROL 管理公司]**。
1. 選取使用者角色。
1. 如果要更改用戶的組成員身份（如果正在編輯或添加媒體門戶用戶或參與者），請選擇 **[!UICONTROL 下一個]** 並編輯組成員身份。
1. 選擇 **[!UICONTROL 保存]**。

### 篩選和排序使用者清單 {#filtering-and-sorting-the-user-list}

您可以篩選並排序使用者清單，以找出使用者。不論在「選取要存取的帳戶」選單中選取了哪些帳戶，您管理之所有帳戶中的所有使用者都會顯示在「使用者」清單中。

可以使用以下用戶清單篩選技術：

* **按組篩選**  — 選擇 **[!UICONTROL 按組]** 的子菜單。

* **按用戶角色篩選**  — 選擇 **[!UICONTROL 按用戶角色]** 的子菜單。

* **按欄位名稱篩選**  — 選擇 **[!UICONTROL 啟用按欄位篩選]**。 然後選擇 **[!UICONTROL 按欄位名稱]** 菜單，選擇用於篩選清單的列，然後選擇「篩選字元」菜單並選擇字母。 該清單按您選擇的字母在其中一列上過濾。 要查看完整清單，請取消選擇 **[!UICONTROL 啟用按欄位篩選]** 的雙曲餘切值。

* **篩選無效用戶**  — 取消選擇 **[!UICONTROL 包含無效]**。 搜尋結果只會顯示系統中的使用者。已從系統和您管理的帳戶中刪除無效用戶。

* **按列標題排序**  — 選擇一個標題，按所有用戶的狀態、按名字、姓氏或電子郵件的字母順序、按用戶角色或按有效/無效狀態對其進行排序。

如果您有多位使用者，則可以選取「清單大小上限」選單並選擇數量，來限制清單大小。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 頻寬和儲存 {#bandwidth-storage}

Adobe Dynamic Media Classic管理員可以為所管理的公司生成頻寬、儲存和其他類型的報告。 這些報告可在「頻寬和儲存」頁面上找到。

要開啟此頁面，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。 展開 **[!UICONTROL 管理設定]**，然後選擇 **[!UICONTROL 頻寬和儲存]**。

### 報告類型 {#types-of-reports}

下表介紹了可以從「頻寬和儲存」頁生成的報告：

| 報告 | 資訊 | 使用 |
|:--- |:--- |:--- |
| 頻寬 | 公司所使用的頻寬 | 追蹤公司在特定日期範圍的頻寬使用情況，以判斷流量模式。 |
| 存放區 | 存放區使用情況 | 追蹤由公司上載的資料量。 |
| 影像內容 | 特定類型的影像要求數量 | 追蹤要求數量以及不同影像類型的容量。 |
| 網域 | 特定網域的 URL 要求數量 | 根據特定公司之影像要求的網域來追蹤影像使用情況。(Adobe Dynamic Media Classic可以為每個帳戶提供多個域。 如需更多資訊，請聯絡技術支援。) |
| 視訊串流 | 串流視訊的頻寬使用情況 | 追蹤公司在特定日期範圍的串流視訊使用情況，以判斷流量模式。 |
| 視訊內容 | 不同視訊的播放時間 | 判定哪些是檢視最多和檢視最少的視訊。 |

「影像內容」報告提供了有關下列影像類型要求的資訊:

* **映像請求**  — 映像請求。

* **縮略圖請求**  — 在查看器中請求色板或替代影像。

* **掩碼請求**  — 請求返回灰階蒙版的影像。

* **查看器平鋪請求**  — 由查看器載入的影像請求。

* **Vnt對象請求**  — 影像呈現請求，該請求返回在請求的小節中具有指定對象的影像。

* **Vnt資訊請求**  — 影像呈現請求返回與所請求的小節相關的資訊。

>[!NOTE]
>
>「視訊串流」報告僅適用於串流視訊。它不會追蹤漸進式視訊的檢視。

### 生成報告 {#generating-a-report}

若要產生頻寬、存放區、影像內容、網域、視訊串流或視訊內容報告:

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 展開管理設定，然後選擇 **[!UICONTROL 頻寬和儲存]**。
1. 選擇頁籤： **[!UICONTROL 頻寬]**。 **[!UICONTROL 儲存]**。 **[!UICONTROL 影像內容]**。 **[!UICONTROL 域]**。 **[!UICONTROL 視頻流]**&#x200B;或 **[!UICONTROL 視頻內容]**。

   請參閱[「報告類型」](administration-setup.md#types_of_reports)。

### 以不同方式查看資料 {#viewing-data-in-different-ways}

在「頻寬和存放區」頁面產生報告後，您可以選擇檢視資訊選項。您可以選擇資訊呈現方式、在圖表或資料格線中檢視資訊，以及指定擷取資訊的時段。在「資料」視圖中，您也可以排序資訊和重新排序欄。

* **查看圖表或資料網格中的資料**  — 選擇 **[!UICONTROL 圖表視圖]** 在圖表中查看資料；選擇 **[!UICONTROL 資料視圖]** 查看資料網格中的資料。

* **選擇報表演示文稿類型**  — 在「報告類型」菜單上，選擇 **[!UICONTROL 摘要]**。 **[!UICONTROL 每日]**&#x200B;或 **[!UICONTROL 每月]** 以摘要形式、按天或按月組織資料。 並非所有報告都提供此選項。

* **指定時段**  — 選擇選項以定義報表的期間，然後選擇 **[!UICONTROL 更新]** 定義時間期後：

* **預定義的時間段**  — 在「預定義報表」菜單中，選擇一個選項。 例如，選擇「上月」可擷取前一個月的資料。

* **自定義時段**  — 在「預定義報表」菜單上，選擇 **[!UICONTROL 自定義]**。 然後選擇日期 **[!UICONTROL 開始月份]** 或 **[!UICONTROL 開始日期]**)菜單和「月數」（或「日數」）菜單上的日期。 對於「網域」和「視訊內容報告」，您可以選擇特定開始和結束日期，以擷取報告資訊。

* **對資料排序（僅限資料視圖）**  — 要對列的資訊進行排序，請選擇列的標題。 再次選擇以降序排序。

* **重新排列列（僅資料視圖）**  — 要將列移動到資料網格上的其他位置，請拖動其標題。

### 導出和打印報告 {#exporting-and-printing-reports}

產生報告後，您便可以匯出其資料，以用於試算表和其它應用程式。您也可以列印報告。

* **導出報表資料**  — 在「資料」視圖中，根據需要對資料進行排序和排列。 然後開啟 **[!UICONTROL 導出]** 的子菜單。 **[!UICONTROL 制表符分隔]**。 **[!UICONTROL 逗號分隔]**&#x200B;或 **[!UICONTROL HTML格式]**。 資料將以您選擇的格式複製到剪貼簿。 您現在可以將資料貼上試算表或應用程式。

* **打印報表**  — 選擇 **[!UICONTROL 打印]**，在「打印」對話框中選擇所需的選項，然後選擇 **[!UICONTROL 確定]**。

## 影像錯誤 {#image-errors}

Adobe Dynamic Media Classic管理員可以生成映像錯誤報告。 「影像錯誤」報告會針對您目前登入的公司，提供過去 24 小時內 20 個最常見的影像錯誤清單。要生成「Image Error（映像錯誤）」報告，請執行以下操作：

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 展開管理設定，然後選擇 **[!UICONTROL 影像錯誤]**。
1. (選擇性) 執行下列任一項作業:

   * 要按標題資訊對錯誤排序，請選擇標題。 根據預設，錯誤會按照出現次數由最高至最低排序。
   * 將游標移至錯誤的「回應」欄位，即可查看特定錯誤訊息。
   * 要查看指向影像或引用者網頁的連結，請將游標移到URL欄位或引用者欄位上。
   * 要將連結複製到實際影像，請選擇 **[!UICONTROL URL複製URL]**。 您可以在瀏覽器視窗中貼上此連結，以前往影像並調查錯誤。
   * 要將連結複製到引用者網頁，請選擇 **[!UICONTROL 引用者複製URL]**。

顯示的錯誤針對您當前登錄的公司。 每個錯誤都包含下列資訊:

* **影像ID**  — 違規影像的ID。

* **時間**  — 最近24小時內第一次報告錯誤到上次報告錯誤的時間範圍。

* **計數**  — 映像上報告的錯誤數。

* **響應**  — 特定錯誤消息。 錯誤為 4xx 或 5xx。

* **URL**  — 列出Adobe Dynamic Media Classic上影像的URL。

* **引用者**  — 指定初始請求來自的網站的URL。 參照者可能是任何連結至該影像的網站。

顯示的錯誤都屬於您目前所登入的公司。
