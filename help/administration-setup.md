---
title: 管理設定
seo-title: 管理設定
description: 'null'
seo-description: 瞭解如何設定Dynamic Media Classic的管理區域。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 64%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

「管理設定」畫面是用於管理Dynamic Media Classic使用者。 使用這些畫面，讓使用者可在Dynamic Media Classic中工作，並透過電子郵件與使用者通訊。

1. 要訪問「管理設定」選項，請按一下「設定」**「設定」>「個人設定」**>「管理設定」**。******

## 使用者管理 {#user-administration}

所有Dynamic Media Classic使用者都會被指派角色，以決定其權限和對Dynamic Media Classic功能的存取權限。 管理員會決定不同角色和其對於所指派公司的責任。

通常，Dynamic Media Classic會設定第一組公司，並指派公司管理員。 然後，公司管理員會設定並管理Dynamic Media Classic使用者。

Dynamic Media Classic支援數個使用者角色。 這些角色可存取為Dynamic Media Classic所設定的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UserCan存取被指派給的公司；不能履行行政職責。

**Adobe Dynamic Media Classic公司管** 理員僅能檢視和管理其公司。公司管理員也可以執行所有管理功能，包含增加管理員和使用者。公司管理員可以將用戶添加到DMC公司管理員帳戶。 (此角色為預設使用者角色。)

新增使用者後，Dynamic Media Classic會傳送歡迎電子郵件訊息給使用者。 訊息包含密碼和Dynamic Media Classic URL。

### 增加使用者或管理員 {#adding-a-user-or-administrator}

1. 按一下「設定 > 應用程式設定 > 管理設定 > 使用者管理」。
1. 按一下「增加」。
1. 輸入您要增加的使用者或管理員名稱和電子郵件地址，然後按一下「下一步」。

   >[!NOTE]
   >
   >電子郵件地址裡不可使用撇號字元 (‘)。

1. 選擇要指派給該使用者的「角色」選項。

   請參閱[動態媒體經典使用者角色和權限](administration-setup.md#user_administration)。

1. 選取公司名稱以將使用者增加至公司。
1. 如果您要將使用者增加至群組 (如果您要增加「Media Portal」使用者或參與者)，請按一下「下一步」然後增加使用者。
1. 按一下「儲存」以完成使用者設定。

   系統會在儲存之後出現提示訊息，問您是否要將使用者增加至其他公司。若您要將使用者增加至公司，請按一下「增加」。

   所有新用戶都會獲得隨機生成的密碼；使用者第一次登入Dynamic Media Classic時，必須變更密碼。

   您增加新使用者後，新的使用者便會收到「歡迎」電子郵件。電子郵件提供了臨時密碼，並說明如何登入 Scene7 Publishing System。

   如果使用者未收到歡迎電子郵件，請他們前往Dynamic Media Classic登入頁面(https://s7sps1.scene7.com)，然後按一下「忘記我的密碼」。 已重設密碼並傳送新的電子郵件。如果使用者沒有收到電子郵件，也沒有在「垃圾郵件」資料夾中也發現，請聯絡「技術支援」。

   若要新增「Media Portal」使用者，您也可以前往「設定 > 應用程式設定 > 使用者管理」，然後按一下「上載使用者清單」並選取內含不超過 500 名使用者的 .csv 檔案。

### 刪除使用者 {#deleting-a-user}

您可以將使用者設為無效，從Dynamic Media Classic中刪除。 無效的使用者會從系統和所有帳戶中移除。

1. 按一下「**設定** > **應用程式設定** > **管理設定** > **使用者管理**」。
1. 從清單中選取使用者，然後按一下「**編輯**」。
1. 取消選取「有效」。
1. 按一下&#x200B;**「儲存」**。

### 啟用或停用使用者  {#activating-or-deactivating-users}

已停用的使用者將不再擁有進入「選取要存取的帳戶」選單上方列出之帳戶的權限。

1. 按一下「**設定** > **應用程式設定** > **管理設定** > **使用者管理**」。
1. 在使用者清單中，選取或取消選取使用者名稱旁的「作用中」選項。

### 編輯使用者資訊  {#editing-user-information}

您可以編輯的使用者資訊視您的管理員角色，以及您要編輯其資訊之使用者獲得指派的角色而定。顏色較暗 (不可用) 的選項無法編輯。

1. 前往&#x200B;**設定** > **應用程式設定**> **管理設定** > **使用者管理**。
1. 選取使用者，然後按一下「**編輯**」。
1. 在您要修改公司權限或存取的顯示表格中，選取輸入項目，然後按一下「管理公司」連結。
1. 選取使用者角色。
1. 如果您要更改使用者的群組成員資格 (如果您要編輯或增加「Media Portal」使用者或參與者)，請按一下「下一步」然後編輯群組成員資格。
1. 按一下&#x200B;**「儲存」**。

### 篩選和排序使用者清單  {#filtering-and-sorting-the-user-list}

您可以篩選並排序使用者清單，以找出使用者。不論在「選取要存取的帳戶」選單中選取了哪些帳戶，您管理之所有帳戶中的所有使用者都會顯示在「使用者」清單中。

您可以使用下列使用者清單篩選技巧:

**依群組篩** 選選取依群組功能表，然後選擇選項將清單縮小至群組中的使用者。

**依使用者角** 色篩選選取依使用者角色功能表，並選擇選項將清單縮小為不同類型的使用者或管理員。

**依欄位名稱篩** 選選取「啟用依欄位篩選」選項。然後選取「依欄位名稱」選單、選擇篩選清單的欄，然後選取「篩選字元」選單並選擇一個字母。清單會依您選擇的字母列出其中一個欄。取消選取「啟用依欄位篩選」選項，即可查看完整清單。

**篩選無效的使** 用者取消選取「包含無效」選項。搜尋結果只會顯示系統中的使用者。已從系統和您所管理的帳戶中刪除無效的使用者。

**依欄標題排** 序按一下標題，可依使用者的狀態、依名字、姓氏或電子郵件的字母順序、依使用者角色或有效／無效狀態來排序所有使用者。

如果您有多位使用者，則可以選取「清單大小上限」選單並選擇數量，來限制清單大小。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 頻寬與存放區  {#bandwidth-storage}

Dynamic Media Classic管理員可以為所管理的公司產生頻寬、儲存空間和其他類型的報表。 您可以在「頻寬和存放區」畫面取得這些報告。

若要開啟此畫面，請按一下「設定 > 個人設定」。展開「管理設定」，然後按一下「頻寬與存放區」。

### 報告類型  {#types-of-reports}

下列表格描述了您可以從「頻寬與存放區」畫面產生的報告:

| 報告 | 資訊 | 使用 |
|:--- |:--- |:--- |
| 頻寬 | 公司所使用的頻寬 | 追蹤公司在特定日期範圍的頻寬使用情況，以判斷流量模式。 |
| 存放區 | 存放區使用情況 | 追蹤由公司上載的資料量。 |
| 影像內容 | 特定類型的影像要求數量 | 追蹤要求數量以及不同影像類型的容量。 |
| 網域 | 特定網域的 URL 要求數量 | 根據特定公司之影像要求的網域來追蹤影像使用情況。(Dynamic Media Classic可為每個帳戶提供多個網域。 如需更多資訊，請聯絡技術支援。) |
| 視訊串流 | 串流視訊的頻寬使用情況 | 追蹤公司在特定日期範圍的串流視訊使用情況，以判斷流量模式。 |
| 視訊內容 | 不同視訊的播放時間 | 判定哪些是檢視最多和檢視最少的視訊。 |


「影像內容」報告提供了有關下列影像類型要求的資訊:

**影像** 請求影像請求。

**檢視** 器中色票或替代影像的縮圖Requests。

**將RequestRequests** 遮色片遮色片遮色為傳回灰色比例的影像。

**檢視器平** 鋪請求檢視器載入的影像請求。

**Vnt物件請** 求影像演算請求，可傳回在請求的暈映中具有指定物件的影像。

**Vnt Info** Request影像演算要求傳回所要求暈映的相關資訊。

>[!NOTE]
>
>「視訊串流」報告僅適用於串流視訊。它不會追蹤漸進式視訊的檢視。

### 產生報告  {#generating-a-report}

若要產生頻寬、存放區、影像內容、網域、視訊串流或視訊內容報告:

1. 選擇「設定 > 個人設定」。
1. 展開「管理設定」，然後按一下「頻寬與存放區」。
1. 按一下標籤:「頻寬」、「存放區」、「影像內容」、「網域」、「視訊串流」或「視訊內容」。

   請參閱[「報告類型」](administration-setup.md#types_of_reports)。

### 以不同方式檢視資料  {#viewing-data-in-different-ways}

在「頻寬和存放區」頁面產生報告後，您可以選擇檢視資訊選項。您可以選擇資訊呈現方式、在圖表或資料格線中檢視資訊，以及指定擷取資訊的時段。在「資料」視圖中，您也可以排序資訊和重新排序欄。

**在圖表或資料格線中檢視資** 料按一下圖表檢視選項以檢視圖表中的資料；按一下「資料檢視」選項，以檢視資料格線中的資料。

**選擇報表簡報類** 型在「報表類型」功能表上，選擇「摘要」、「每日」或「每月」，以匯總形式、依日或依月組織資料。並非所有報告都提供此選項。

**指定時段選** 擇選項以定義報表的時段，然後在定義時段後按一下更新：

**預先定義的時** 段在「預先定義報表」功能表上，選擇選項。例如，選擇「上月」可擷取前一個月的資料。

**自訂時** 段在預先定義的報表功能表上，選擇自訂。然後在「開始月份」(或「開始日期」) 選單上選擇日期，並在「月數」(或「天數」) 選單上選擇日期。對於「網域」和「視訊內容報告」，您可以選擇特定開始和結束日期，以擷取報告資訊。

**排序資料（僅限資料檢視）** 若要排序欄的資訊，請按一下欄的標題。再按一下就會以遞減的順序排序。

**重新排列列（僅限資料視圖）** 要將列移動到資料網格上的不同位置，請拖動其標題。

### 匯出和列印報告 {#exporting-and-printing-reports}

產生報告後，您便可以匯出其資料，以用於試算表和其它應用程式。您也可以列印報告。

**匯出報表** 資料在「資料」檢視中，視需要排序及排列資料。然後開啟「匯出」選單，並選擇格式:「Tab 字元分隔」、「逗號分隔」或「HTML 格式」。資料會依您選擇的格式複製到剪貼簿。您現在可以將資料貼上試算表或應用程式。

**列印報** 表按一下列印，在列印對話方塊中選擇您要的選項，然後按一下確定。

## 影像錯誤 {#image-errors}

Dynamic Media Classic管理員可產生「影像錯誤」報表。 「影像錯誤」報告會針對您目前登入的公司，提供過去 24 小時內 20 個最常見的影像錯誤清單。遵循下列步驟即可產生影像錯誤報告。

1. 按一下「設定 > 個人設定」。
1. 展開「管理設定」，然後按一下「影像錯誤」。
1. (選擇性) 執行下列任一項作業:

   * 按一下標題，依標題資訊排序錯誤。根據預設，錯誤會按照出現次數由最高至最低排序。
   * 將游標移至錯誤的「回應」欄位，即可查看特定錯誤訊息。
   * 將游標移至「URL」欄位或「參照者」欄位，即可查看影像連結或參照者網頁。
   * 按一下 URL 的「複製 URL」，即可複製實際影像連結。您可以在瀏覽器視窗中貼上此連結，以前往影像並調查錯誤。
   * 按一下參照者的「複製 URL」，即可複製參照者網頁連結。

顯示的錯誤都屬於您目前所登入的公司。每個錯誤都包含下列資訊:

**違規** 影像的影像IDID。

**時** 間過去24小時內首次報告錯誤到上次報告錯誤的時間範圍。

**計** 數影像上報告的錯誤數。

**回** 應特定錯誤訊息。錯誤為 4xx 或 5xx。

**URL** 列出Scene 7上影像的URL。

**反** 向連結指定初始請求來源之網站的URL。參照者可能是任何連結至該影像的網站。

顯示的錯誤都屬於您目前所登入的公司。
