---
title: 管理設定
description: 了解如何設定Adobe Dynamic Media Classic的管理區域。
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

「管理設定」畫面可用於管理Adobe Dynamic Media Classic使用者。 使用這些畫面，讓使用者能在Adobe Dynamic Media Classic中工作，並透過電子郵件與使用者通訊。

1. 要訪問「管理設定」選項，請轉至 **設定** > **個人設定** > **管理設定**.

## 使用者管理 {#user-administration}

所有Adobe Dynamic Media Classic使用者都獲派角色，決定其Adobe Dynamic Media Classic功能的權限和存取權限。 管理員會決定不同角色和其對於所指派公司的責任。

通常，Adobe Dynamic Media Classic會設定第一組公司，並指派公司管理員。 然後，公司管理員會設定並管理Adobe Dynamic Media Classic使用者。

Adobe Dynamic Media Classic支援數個使用者角色。 這些角色可存取為Adobe Dynamic Media Classic設定的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic使用者** 可以訪問被分配給的公司；不能執行任何管理職責。

**Adobe Dynamic Media Classic公司管理員** 只能檢視和管理自己的公司。 公司管理員也可以執行所有管理功能，包含增加管理員和使用者。公司管理員可以將用戶添加到DMC公司管理員帳戶。 (此角色為預設使用者角色。)

新增使用者後，Adobe Dynamic Media Classic會傳送歡迎電子郵件給使用者。 訊息包含密碼和Adobe Dynamic Media Classic URL。

### 添加用戶或管理員 {#adding-a-user-or-administrator}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 選擇 **[!UICONTROL 新增]**.
1. 輸入要添加的用戶或管理員的名稱和電子郵件地址，然後選擇 **[!UICONTROL 下一個]**.

   >[!NOTE]
   >
   >撇號字元(`‘`)在電子郵件地址中不允許。

1. 要向用戶分配角色，請選擇角色選項。

   請參閱 [Adobe Dynamic Media Classic使用者角色和權限](administration-setup.md#user_administration).

1. 若要新增使用者至公司，請選取公司名稱。
1. 如果您想要將使用者新增至群組（如果您要新增Media Portal使用者或貢獻者），請選取 **[!UICONTROL 下一個]** 並添加用戶。
1. 選擇 **[!UICONTROL 儲存]** 以完成使用者設定。

   系統會在儲存之後出現提示訊息，問您是否要將使用者增加至其他公司。選擇 **[!UICONTROL 新增]** 如果您想要將使用者新增至公司。

   所有新用戶都獲得隨機生成的密碼；用戶首次登錄Adobe Dynamic Media Classic案頭應用程式時必須更改密碼。

   您增加新使用者後，新的使用者便會收到「歡迎」電子郵件。電子郵件提供暫時密碼，並說明如何登入Adobe Dynamic Media Classic。

   如果使用者未收到歡迎電子郵件，請讓他們前往Adobe Dynamic Media Classic登入頁面(https://s7sps1.scene7.com)，然後選取 **[!UICONTROL 忘記密碼]**. 已重設密碼並傳送新的電子郵件。如果使用者沒有收到電子郵件，也沒有在「垃圾郵件」資料夾中也發現，請聯絡「技術支援」。

   新增Media Portal使用者時，您也可以前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 使用者管理]**，然後選取 **[!UICONTROL 上傳使用者清單]** ，並選取不超過500個使用者的.csv檔案。

### 刪除使用者 {#deleting-a-user}

您可以將使用者設為無效，以從Adobe Dynamic Media Classic中刪除使用者。 無效的使用者會從系統和所有帳戶中移除。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 從清單中選取使用者，然後選取 **[!UICONTROL 編輯]**.
1. 取消選取「有效」。
1. 選擇 **[!UICONTROL 儲存]**.

### 啟用或停用使用者 {#activating-or-deactivating-users}

已停用的使用者將不再擁有進入「選取要存取的帳戶」選單上方列出之帳戶的權限。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 在使用者清單中，選取或取消選取 **[!UICONTROL 作用中]** 選項。

### 編輯使用者資訊 {#editing-user-information}

您可以編輯的使用者資訊視您的管理員角色，以及您要編輯其資訊之使用者獲得指派的角色而定。顏色較暗 (不可用) 的選項無法編輯。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 從清單中選取使用者，然後選取 **[!UICONTROL 編輯]**.
1. 在表格中選取顯示您嘗試修改權限或存取之公司的項目，然後選取 **[!UICONTROL 管理公司]**.
1. 選取使用者角色。
1. 如果您想要變更使用者的群組成員資格（如果您正在編輯或新增Media Portal使用者或貢獻者），請選取 **[!UICONTROL 下一個]** 和編輯群組成員資格。
1. 選擇 **[!UICONTROL 儲存]**.

### 篩選和排序使用者清單 {#filtering-and-sorting-the-user-list}

您可以篩選並排序使用者清單，以找出使用者。不論在「選取要存取的帳戶」選單中選取了哪些帳戶，您管理之所有帳戶中的所有使用者都會顯示在「使用者」清單中。

您可以使用下列使用者清單篩選技術：

* **依群組篩選**  — 選取 **[!UICONTROL 按組]** ，然後選擇選項將清單縮小到組中的用戶。

* **依使用者角色篩選**  — 選取 **[!UICONTROL 按用戶角色]** ，然後選擇一個選項，將清單縮小到不同類型的用戶或管理員。

* **依欄位名稱篩選**  — 選擇 **[!UICONTROL 啟用按欄位篩選]**. 然後選取 **[!UICONTROL 按欄位名稱]** ，選擇用於篩選清單的列，然後選擇「篩選字元」菜單並選擇字母。 清單會依您選取的字母，在其中一欄中篩選。 若要查看完整清單，請取消選取 **[!UICONTROL 啟用按欄位篩選]** 選項。

* **過濾無效用戶**  — 取消選擇 **[!UICONTROL 包含無效]**. 搜尋結果只會顯示系統中的使用者。已從您管理的系統和帳戶中刪除無效用戶。

* **按列標題排序**  — 選擇一個標題，按用戶的狀態、按名字、姓氏或電子郵件的字母順序、按用戶角色或按有效/無效狀態對所有用戶進行排序。

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

Adobe Dynamic Media Classic管理員可為所管理的公司產生頻寬、儲存和其他類型的報表。 「頻寬和儲存」頁上提供了這些報告。

若要開啟此頁面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**. 展開 **[!UICONTROL 管理設定]**，然後選取 **[!UICONTROL 頻寬和儲存]**.

### 報告類型 {#types-of-reports}

下表介紹了可從「頻寬和儲存」頁生成的報告：

| 報告 | 資訊 | 使用 |
|:--- |:--- |:--- |
| 頻寬 | 公司所使用的頻寬 | 追蹤公司在特定日期範圍的頻寬使用情況，以判斷流量模式。 |
| 存放區 | 存放區使用情況 | 追蹤由公司上載的資料量。 |
| 影像內容 | 特定類型的影像要求數量 | 追蹤要求數量以及不同影像類型的容量。 |
| 網域 | 特定網域的 URL 要求數量 | 根據特定公司之影像要求的網域來追蹤影像使用情況。(Adobe Dynamic Media Classic可為每個帳戶提供多個網域。 如需更多資訊，請聯絡技術支援。) |
| 視訊串流 | 串流視訊的頻寬使用情況 | 追蹤公司在特定日期範圍的串流視訊使用情況，以判斷流量模式。 |
| 視訊內容 | 不同視訊的播放時間 | 判定哪些是檢視最多和檢視最少的視訊。 |

「影像內容」報告提供了有關下列影像類型要求的資訊:

* **影像要求**  — 要求影像。

* **縮圖請求**  — 請求檢視器中的色票或替代影像。

* **遮罩請求**  — 請求影像返回灰階蒙版。

* **檢視器圖磚請求**  — 檢視器載入的影像要求。

* **Vnt物件要求**  — 影像呈現請求，這些請求會傳回包含請求暈映中指定物件的影像。

* **Vnt資訊請求**  — 影像呈現請求，可傳回請求的暈映資訊。

>[!NOTE]
>
>「視訊串流」報告僅適用於串流視訊。它不會追蹤漸進式視訊的檢視。

### 產生報表 {#generating-a-report}

若要產生頻寬、存放區、影像內容、網域、視訊串流或視訊內容報告:

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 展開「管理設定」，然後選取 **[!UICONTROL 頻寬和儲存]**.
1. 選擇頁簽： **[!UICONTROL 頻寬]**, **[!UICONTROL 儲存]**, **[!UICONTROL 影像內容]**, **[!UICONTROL 網域]**, **[!UICONTROL 視訊串流]**，或 **[!UICONTROL 視訊內容]**.

   請參閱[「報告類型」](administration-setup.md#types_of_reports)。

### 以不同方式檢視資料 {#viewing-data-in-different-ways}

在「頻寬和存放區」頁面產生報告後，您可以選擇檢視資訊選項。您可以選擇資訊呈現方式、在圖表或資料格線中檢視資訊，以及指定擷取資訊的時段。在「資料」視圖中，您也可以排序資訊和重新排序欄。

* **在圖表或資料網格中查看資料**  — 選擇 **[!UICONTROL 圖表視圖]** 查看圖表中的資料；選取 **[!UICONTROL 資料檢視]** 在資料網格中查看資料。

* **選擇報表簡報類型**  — 在「報表類型」功能表中，選取 **[!UICONTROL 摘要]**, **[!UICONTROL 每日]**，或 **[!UICONTROL 每月]** 以摘要形式、日或月來組織資料。 並非所有報告都提供此選項。

* **指定時段**  — 選擇選項以定義報表的時段，然後選取 **[!UICONTROL 更新]** 定義時段後：

* **預先定義的時段**  — 在預先定義的報表功能表中，選擇一個選項。 例如，選擇「上月」可擷取前一個月的資料。

* **自訂時段**  — 在預先定義的報表功能表中，選取 **[!UICONTROL 自訂]**. 然後在 **[!UICONTROL 開始月份]** (或 **[!UICONTROL 開始日期]**)功能表和月數（或天數）功能表上的日期。 對於「網域」和「視訊內容報告」，您可以選擇特定開始和結束日期，以擷取報告資訊。

* **排序資料（僅限資料檢視）**  — 要排序列的資訊，請選擇列的標題。 再次選取，以降序排序。

* **重新排列列（僅限資料視圖）**  — 要將列移動到資料網格上的其他位置，請拖動其標題。

### 匯出和列印報表 {#exporting-and-printing-reports}

產生報告後，您便可以匯出其資料，以用於試算表和其它應用程式。您也可以列印報告。

* **匯出報表資料**  — 在資料檢視中，視需要排序和排列資料。 然後開啟 **[!UICONTROL 匯出]** ，然後選擇格式： **[!UICONTROL 分隔標籤]**, **[!UICONTROL 逗號分隔]**，或 **[!UICONTROL HTML格式]**. 資料會以您所選的格式複製到剪貼簿。 您現在可以將資料貼上試算表或應用程式。

* **列印報表**  — 選擇 **[!UICONTROL 列印]**，在「打印」對話框中選擇所需的選項，然後選擇 **[!UICONTROL 確定]**.

## 影像錯誤 {#image-errors}

Adobe Dynamic Media Classic管理員可產生影像錯誤報表。 「影像錯誤」報告會針對您目前登入的公司，提供過去 24 小時內 20 個最常見的影像錯誤清單。若要產生「影像錯誤」報表，請執行下列動作：

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 展開「管理設定」，然後選取 **[!UICONTROL 影像錯誤]**.
1. (選擇性) 執行下列任一項作業:

   * 要按標題資訊排序錯誤，請選擇標題。 根據預設，錯誤會按照出現次數由最高至最低排序。
   * 將游標移至錯誤的「回應」欄位，即可查看特定錯誤訊息。
   * 若要查看影像或反向連結網頁的連結，請將游標移至URL欄位或反向連結欄位上。
   * 若要將連結複製到實際影像，請選取 **[!UICONTROL URL複製URL]**. 您可以在瀏覽器視窗中貼上此連結，以前往影像並調查錯誤。
   * 若要將連結複製到反向連結網頁，請選取 **[!UICONTROL 反向連結複製URL]**.

顯示的錯誤是針對您目前登入的公司。 每個錯誤都包含下列資訊:

* **影像ID**  — 違規影像的ID。

* **時間**  — 在過去24小時內，首次報告錯誤至上次報告錯誤的時間範圍。

* **計數**  — 影像上報告的錯誤數。

* **回應**  — 特定錯誤訊息。 錯誤為 4xx 或 5xx。

* **URL**  — 列出Adobe Dynamic Media Classic上影像的URL。

* **反向連結**  — 指定初始請求來自的網站URL。 參照者可能是任何連結至該影像的網站。

顯示的錯誤都屬於您目前所登入的公司。
