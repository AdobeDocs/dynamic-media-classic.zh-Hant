---
title: 管理設定
description: 瞭解如何設定Adobe Dynamic Media Classic的管理區域。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: fc2138cc9fd08cb4ce7466724af03f0901edebf3
workflow-type: tm+mt
source-wordcount: '1995'
ht-degree: 29%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

「管理設定」畫面可用來管理Adobe Dynamic Media Classic使用者。 使用這些畫面可讓使用者在Adobe Dynamic Media Classic中工作，並透過電子郵件與其他使用者通訊。

1. 若要存取管理安裝程式選項，請移至&#x200B;**安裝程式** > **個人安裝程式** > **管理安裝程式**。

## 使用者管理 {#user-administration}

所有Adobe Dynamic Media Classic使用者都會獲得一個角色，該角色會決定其在Adobe Dynamic Media Classic中功能的許可權和存取權。 管理員會決定不同角色和其對於所指派公司的責任。

通常Adobe Dynamic Media Classic會設定第一組公司並指派公司管理員。 然後，公司管理員會設定和管理Adobe Dynamic Media Classic使用者。

Adobe Dynamic Media Classic支援多個使用者角色。 這些角色可以存取為Adobe Dynamic Media Classic設定的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic使用者**&#x200B;可以存取已指派給他們的公司；無法執行任何管理職責。

**Adobe Dynamic Media Classic公司管理員**&#x200B;只能檢視和管理自己的公司。 公司管理員也可以執行所有管理功能，包含增加管理員和使用者。公司管理員可將使用者新增至DMC公司管理員帳戶。 (此角色為預設使用者角色。)

新增使用者後，Adobe Dynamic Media Classic會傳送一封歡迎電子郵件給使用者。 此訊息包含密碼和Adobe Dynamic Media Classic URL。

### 新增使用者或管理員 {#adding-a-user-or-administrator}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**。
1. 選取&#x200B;**[!UICONTROL 新增]**。
1. 輸入您要新增的使用者或管理員的名稱和電子郵件地址，然後選取&#x200B;**[!UICONTROL 下一步]**。

   >[!NOTE]
   >
   >電子郵件地址中不允許使用單引號字元(`'`)。

1. 若要將角色指派給使用者，請選擇角色選項。

   請參閱[Adobe Dynamic Media Classic使用者角色和許可權](administration-setup.md#user_administration)。

1. 若要新增使用者至公司，請選取公司名稱。
1. 如果您想要將使用者新增至群組（如果您正在新增Media Portal使用者或貢獻者），請選取&#x200B;**[!UICONTROL 下一步]**&#x200B;並新增使用者。
1. 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以完成使用者設定。

   系統會在儲存之後出現提示訊息，問您是否要將使用者增加至其他公司。若要將使用者新增至公司，請選取&#x200B;**[!UICONTROL 新增]**。

   所有新使用者都會獲得隨機產生的密碼；使用者在第一次登入Adobe Dynamic Media Classic案頭應用程式時需要變更密碼。

   您增加新使用者後，新的使用者便會收到「歡迎」電子郵件。此電子郵件會提供暫時密碼，並說明如何登入Adobe Dynamic Media Classic。

   如果使用者未收到歡迎電子郵件，請讓他們前往Adobe Dynamic Media Classic登入頁面(https://s7sps1.scene7.com)，然後選取&#x200B;**[!UICONTROL 忘記我的密碼]**。 已重設密碼並傳送新的電子郵件。如果使用者沒有收到電子郵件，也沒有在「垃圾郵件」資料夾中也發現，請聯絡「技術支援」。

   新增Media Portal使用者時，您也可以前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 使用者管理]**，然後選取&#x200B;**[!UICONTROL 上傳使用者清單]**，並選取包含不多於500名使用者的.csv檔案。

### 刪除使用者 {#delet-a-user}

您可以讓使用者無效以從Adobe Dynamic Media Classic中刪除使用者。 無效的使用者會從系統和所有帳戶中移除。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**。
1. 從清單中選取使用者，然後選取&#x200B;**[!UICONTROL 編輯]**。
1. 取消選取「有效」。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

### 啟用或停用使用者 {#activating-or-deactivating-users}

已停用的使用者將不再擁有進入「選取要存取的帳戶」選單上方列出之帳戶的權限。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**。
1. 在使用者清單中，選取或取消選取使用者名稱旁的&#x200B;**[!UICONTROL Active]**&#x200B;選項。

### 編輯使用者資訊 {#editing-user-information}

您可以編輯的使用者資訊視您的管理員角色，以及您要編輯其資訊之使用者獲得指派的角色而定。顏色較暗 (不可用) 的選項無法編輯。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**。
1. 從清單中選取使用者，然後選取&#x200B;**[!UICONTROL 編輯]**。
1. 在表格中選取顯示您嘗試修改許可權或存取之公司的專案，然後選取&#x200B;**[!UICONTROL 管理公司]**。
1. 選取使用者角色。
1. 如果您想要變更使用者的群組成員資格（如果您正在編輯或新增Media Portal使用者或貢獻者），請選取[下一步] ****&#x200B;並編輯群組成員資格。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

### 篩選和排序使用者清單 {#filtering-and-sorting-the-user-list}

您可以篩選並排序使用者清單，以找出使用者。不論在「選取要存取的帳戶」選單中選取了哪些帳戶，您管理之所有帳戶中的所有使用者都會顯示在「使用者」清單中。

您可以使用下列使用者清單篩選技術：

* **依群組篩選**：選取&#x200B;**[!UICONTROL 依群組]**&#x200B;功能表，並選擇選項以將清單縮小至群組中的使用者。

* **依使用者角色篩選**：選取&#x200B;**[!UICONTROL 依使用者角色]**&#x200B;功能表，並選擇選項以將清單縮小至不同型別的使用者或管理員。

* **依欄位名稱篩選**：選取&#x200B;**[!UICONTROL 啟用依欄位篩選]**。 接著選取&#x200B;**[!UICONTROL 依欄位名稱]**&#x200B;功能表，選擇欄以篩選清單，然後選取「篩選字元」功能表並選擇字母。 清單會依您選取的字母在其中一個欄上篩選。 若要檢視完整清單，請取消選取&#x200B;**[!UICONTROL 啟用依欄位篩選]**&#x200B;選項。

* **篩選出無效的使用者**：取消選取&#x200B;**[!UICONTROL 包含無效]**。 搜尋結果只會顯示系統中的使用者。已從您管理的系統和帳戶中刪除無效的使用者。

* **依欄標題排序**：選取標題，依狀態依名字、姓氏或電子郵件的字母順序排序所有使用者。 或者，依使用者角色或有效/無效狀態排序。

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

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 頻寬和儲存空間 {#bandwidth-storage}

Adobe Dynamic Media Classic管理員可以為他們管理的公司產生頻寬、儲存空間和其他型別的報表。 這些報告可在「頻寬與儲存」頁面上取得。

若要開啟此頁面，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。 展開&#x200B;**[!UICONTROL 管理設定]**，然後選取&#x200B;**[!UICONTROL 頻寬與儲存空間]**。

### 報告類型 {#types-of-reports}

下表說明可從「頻寬與儲存」頁面產生的報表：

| 報告 | 資訊 | 使用 |
| --- | --- | --- |
| 頻寬 | | <!-- CQDOC-22504 --> **重要**：不再支援[頻寬]索引標籤。 雖然頻寬資料仍會顯示在UI中，但頻寬資料無法使用，而且所有值都會顯示為`0`。 |
| 存放區 | 存放區使用情況 | 追蹤公司上傳的資料量。 |
| 影像內容 | 顯示依請求型別和子型別劃分的點選總數和影像傳送數量。 | 追蹤不同影像型別（包括非視訊資產的量度）的請求數和數量。<!-- CQDOC-22504 --> |
| 網域 | 特定網域的 URL 要求數量 | 根據特定公司之影像要求的網域來追蹤影像使用情況。(Adobe Dynamic Media Classic可為每個帳戶提供一個以上的網域。 如需更多資訊，請聯絡技術支援。) |
| 視訊串流 | 串流視訊的頻寬使用情況 | 追蹤公司在特定日期範圍的串流視訊使用情況，以判斷流量模式。 |
| 視訊內容 | 不同視訊的播放時間 | 判定哪些是檢視最多和檢視最少的視訊。 |

「影像內容」報告提供了有關下列影像類型要求的資訊:

* **影像要求**：影像要求。

* **縮圖要求**：檢視器中色票或替代影像的要求。

* **遮罩要求**：要求影像傳回灰階遮罩。

* **檢視器並排要求**：檢視器載入的影像要求。

* **VNT物件要求**：傳回影像的影像演算要求，在要求的暈映中有指定的物件。

* **VNT資訊要求**：傳回有關要求的暈映資訊的影像演算要求。

>[!NOTE]
>
>「視訊串流」報告僅適用於串流視訊。它不會追蹤漸進式影片的觀看情形。

### 產生報表 {#generating-a-report}

若要產生頻寬、存放區、影像內容、網域、視訊串流或視訊內容報告:

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 展開[管理設定]，然後選取&#x200B;**[!UICONTROL 頻寬與儲存空間]**。
1. 選取索引標籤： **[!UICONTROL 頻寬]**、**[!UICONTROL 儲存空間]**、**[!UICONTROL 影像內容]**、**[!UICONTROL 網域]**、**[!UICONTROL 視訊串流]**&#x200B;或&#x200B;**[!UICONTROL 視訊內容]**。

   請參閱[「報告類型」](administration-setup.md#types_of_reports)。

### 以不同方式檢視資料 {#viewing-data-in-different-ways}

在「頻寬和存放區」頁面產生報告後，您可以選擇檢視資訊選項。您可以選擇資訊呈現方式、在圖表或資料格線中檢視資訊，以及指定擷取資訊的時段。在「資料」視圖中，您也可以排序資訊和重新排序欄。

* **在圖表或資料網格中檢視資料**：選取&#x200B;**[!UICONTROL 圖表檢視]**&#x200B;可檢視圖表中的資料；選取&#x200B;**[!UICONTROL 資料檢視]**&#x200B;可在資料網格中檢視資料。

* **選擇報表簡報型別**：在[報表型別]功能表中，選取&#x200B;**[!UICONTROL 摘要]**、**[!UICONTROL 每日]**&#x200B;或&#x200B;**[!UICONTROL 每月]**，以摘要形式、依日期或依月份組織資料。 並非所有報告都提供此選項。

* **指定時段**：選擇選項以定義報表的時段，然後在定義時段後選取&#x200B;**[!UICONTROL 更新]**：

* **預先定義期間**：在預先定義報表功能表上，選擇一個選項。 例如，選擇「上月」可擷取前一個月的資料。

* **自訂時段**：在預先定義的報表功能表中，選取&#x200B;**[!UICONTROL 自訂]**。 然後在&#x200B;**[!UICONTROL 開始月份]** （或&#x200B;**[!UICONTROL 開始日期]**）功能表上選擇一個日期，並在「月數」 （或「天數」）功能表上選擇一個日期。 對於「網域」和「視訊內容報告」，您可以選擇特定開始和結束日期，以擷取報告資訊。

* **排序資料（僅限資料檢視）**：排序資料行中的資訊。 選取欄的標題。 再次選取「 」可依遞減順序排序。

* **重新排列欄（僅限資料檢視）**：若要將欄移至資料格線上的不同位置，請拖曳其標題。

### 匯出和列印報告 {#exporting-and-printing-reports}

產生報告後，您便可以匯出其資料，以用於試算表和其它應用程式。您也可以列印報告。

* **匯出報表資料**：在資料檢視中，視需要排序和排列資料。 然後開啟&#x200B;**[!UICONTROL 匯出]**&#x200B;功能表並選擇格式： **[!UICONTROL 以Tab分隔]**、**[!UICONTROL 以逗號分隔]**&#x200B;或&#x200B;**[!UICONTROL HTML格式]**。 資料會以您選擇的格式複製到剪貼簿。 您現在可以將資料貼上試算表或應用程式。

* **列印報告**：選取&#x200B;**[!UICONTROL 列印]**，在[列印]對話方塊中選擇您想要的選項，然後選取&#x200B;**[!UICONTROL 確定]**。

## 影像錯誤 {#image-errors}

Adobe Dynamic Media Classic管理員可以產生影像錯誤報告。 「影像錯誤」報告會針對您目前登入的公司，提供過去 24 小時內 20 個最常見的影像錯誤清單。若要產生「影像錯誤」報表，請執行下列動作：

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 展開管理設定，然後選取&#x200B;**[!UICONTROL 影像錯誤]**。
1. (選擇性) 執行下列任一項作業:

   * 若要依標題資訊排序錯誤，請選取標題。 根據預設，錯誤會按照出現次數由最高至最低排序。
   * 將游標移至錯誤的「回應」欄位，即可查看特定錯誤訊息。
   * 若要檢視影像或反向連結網頁的連結，請將游標移至URL欄位或反向連結欄位上。
   * 若要複製實際影像的連結，請選取&#x200B;**[!UICONTROL URL複製URL]**。 您可以在瀏覽器視窗中貼上此連結，以前往影像並調查錯誤。
   * 若要複製反向連結網頁的連結，請選取&#x200B;**[!UICONTROL 反向連結複製URL]**。

顯示的錯誤適用於您目前登入的公司。 每個錯誤都包含下列資訊:

* **影像識別碼**：違規影像的識別碼。

* **時間**：在過去24小時內，第一次回報錯誤到上次回報錯誤的時間範圍。

* **計數**：影像上報告的錯誤數。

* **回應**：特定錯誤訊息。 錯誤為 4xx 或 5xx。

* **URL**：列出Adobe Dynamic Media Classic上的影像URL。

* **Referrer**：指定初始要求來源網站的URL。 反向連結可以是任何具有影像連結的網站。

顯示的錯誤都屬於您目前所登入的公司。
