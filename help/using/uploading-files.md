---
title: 上載檔案
description: 瞭解如何在Adobe Dynamic Media Classic中上傳檔案。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '3929'
ht-degree: 31%

---

# 上載檔案{#uploading-files}

在將資產檔案上傳至Adobe Dynamic Media Classic之前，請確定資產檔案已正確命名，且您的資料夾結構已依您想要的方式設定和組織。 您可以從Adobe Dynamic Media Classic提供的FTP站台上傳檔案，也可以直接從您的電腦或網路上傳檔案。 Adobe Dynamic Media Classic提供上傳檔案時最佳化檔案的選項。 如果您已安裝Adobe Dynamic Media Classic案頭應用程式，則可直接從案頭拖曳檔案和資料夾，即可將其上傳。 請參閱[應用程式一般設定](application-setup.md#general_settings)。

## 準備資產和資料夾以進行上傳 {#preparing-your-assets-and-folders-for-uploading}

將資產上傳至Adobe Dynamic Media Classic之前，請確定它們的格式和大小正確。 您也必須遵守資產命名的Adobe Dynamic Media Classic規則。 為檔案設定檔案夾組織和結構之前，請確定您可以輕鬆尋找和處理檔案。

### 支援的資產檔案格式 {#supported-asset-file-formats}

下表列出Adobe Dynamic Media Classic支援的資產檔案格式。 如需有關支援的Camera Raw檔案的資訊，請參閱 [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| 資產檔案格式 | 說明 |
| --- | --- |
| 音效資料 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 階層式樣式表 | CSS |
| 色彩設定檔 | ICC、ICM |
| 字型 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 影像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT (僅限Windows®)、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| Adobe Dynamic Media Classic影像製作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 視訊 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上載支援包含一個核取框，供您選取是否想要解壓縮檔案。

### Dynamic Media不支援的影像格式 {#unsupported-image-formats-dynamic-media}

下列清單說明點陣影像檔案格式的子型別 *not* 在Dynamic Media中支援。

另請參閱 [偵測Dynamic Media不支援的檔案格式](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* IDAT區塊大小大於100 MB的PNG檔案。
* PSB檔案。
* 不支援色彩空間不是CMYK、RGB、灰階或點陣圖的PSD檔案。 不支援DuoTone、Lab和索引色域。
* 位元深度大於16的PSD檔案。
* TIFF含有浮點資料的檔案。
* TIFF具有Lab色域的檔案。

### 資產類型 {#asset-types}

若要使用Adobe Dynamic Media Classic程式取得最佳結果，請務必使用建議的檔案格式和大小。 下表格列出了資產類型，其中一些資產類型具有常用資產的建議格式和檔案大小。

| 資產類型 | 描述/建議 |
| --- | --- |
| 音效資料 | 輸入音訊資產格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。 可以將音訊轉碼為以下格式: MP3、AAC 和 HE-AAC。 |
| 影像 (用於調整影像大小、縮放、影像集、迴轉集) | 最大大小的影像必須至少為2000畫素；最大大小的典型影像大小範圍是1500到2500畫素。 建議使用不失真的影像格式，包括 TIFF 和 PNG 檔案。 如果使用 JPEG 影像，請使用最高品質的設定。處理動畫GIF檔案的方式與其他靜態內容相同。 |
| eCatalog | 使用在Adobe Acrobat中建立的高解析度PDF檔案，或是儲存為「備妥」的AdobeCreative Suite應用程式。 PDF 包括所有需要的字型、影像、遮色片以及參照的圖形化元素，採用單頁、雙頁式跨頁或多頁格式。 透過按字母數字順序為檔案命名來排列頁面順序。 將 eCatalog 的所有 PDF 檔放於一個檔案夾中，以便上載。 您可以在上載時選取裁切選項，以便從 PDF 中移除修剪區域，包括裁切標記、對齊目標或色彩導表。 多數印刷就緒的 PDF 檔案採用 CMYK 色域，因此務必要獲得用於 PDF 檔案的 CMYK ICC 色彩設定檔。 |
| 範本 | 分層影像或版面設計，可以包括文字、影像和圖層。 可以將圖層、文字字串和屬性 (如色彩和大小) 參數化，從而可以自訂變數資料。 在範本中使用時的影像要求與其他影像相同。 在 Photoshop 或其他影像編輯程式中準備圖形。 採用 TIFF 或 PNG 格式將每個圖形儲存為平面化透明檔案。 確保影像解析度適合所要求的用途。 列印影像為300 ppi。 |
| 視訊 | Adobe Dynamic Media Classic支援以OGV和MP4格式儲存的視訊檔案。 您可以在上載時，將檔案轉碼為 MP4。請參閱[支援的資產檔案格式](#supported-static-file-formats)。 |
| 字型 | 已上傳TrueType、Type1 (僅限Windows®)、OpenType®字型和PhotoFonts。 |
| 影像 | 影像和分層影像檔案。 |
| 影像集和色票集 | 可以在檢視器中顯示的一組相關影像。 |
| ICC 設定檔 | 一種色彩設定檔，可用來將上傳的影像從來源色域轉換為不同的色域。 |
| 暈映 | 使用影像製作程式製作的影像和相關檔案。 |
| 內容檔案 | Adobe InDesign、Illustrator 或 Photoshop 內容檔案。 |
| FXG 檔案 | 與解析度無關的圖形格式檔案，可以用來建立能夠自訂的範本，以輸出進行列印、輸出到網路、電子郵件、桌面以及裝置。 |
| SVG 檔案 | 「影像伺服」伺服器可以演算的可擴放向量圖形檔案。 |
| XML 檔案 | 定義用於修改要求路徑和查詢部分之預處理規則的檔案。 |
| 階層式樣式表檔案。 | 上載用以自訂 HTML5 檢視器的 CSS 外觀。 |
| JavaScript 檔案 | JavaScript檔案用於viewer instrumentation以儲存帳戶資訊。 Adobe安全性建議僅針對使用不同網域進行傳送的使用者端帳戶使用此資產型別（以避免跨網站指令碼）。 |

>[!NOTE]
>
>當您將影像檔案和PDF上傳到Adobe Dynamic Media Classic時，系統將這些來源檔案轉換為PTIFF(金字塔TIFF)檔案。 這些PTIFF是稍後發佈至Dynamic Media影像伺服器的檔案。 Adobe Dynamic Media Classic使用「金字塔Tiff」檔案格式，因為它包含各種縮放比例，以便在使用Adobe Dynamic Media Classic縮放檢視器檢視時可快速縮放。

### 支援的靜態檔案格式 {#supported-static-file-formats}

Adobe Dynamic Media Classic支援多種靜態檔案格式。 靜態內容是以「原樣」發佈的任何資產，例如CSS、PDF、SVG和XML。

您可以發佈下列檔案類型:

* 動畫 GIF
* 音訊檔案
* CSS
* JavaScript (當公司設定了自己的網域時)
* 主要影片
* PDF(當PDF在上傳後標籤為發佈時，以避免交付現有eCatalog/PDF工作流程的所有PDF)
* PrX 視訊
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic不提供產生靜態內容預覽URL的選項。

### 檔案名稱要求 {#filename-requirements}

由於在檔案上載過程中將去除檔案名中的副檔名，因此系統不允許檔案使用相同的根名稱。在Adobe Dynamic Media Classic系統中，資產檔案名稱減去副檔名後，即為資產的資產ID。 因此，兩個資產不能同名。

請確定貴公司的所有使用者都瞭解這些檔案命名規則：

* 系統中不允許存在名稱完全相同的資產 ID。
* 資產ID名稱會區分大小寫。
* 最佳做法是確保資產 ID 不包含空格 (例如 black jacket.tif 和 blue jacket.jpg)。Adobe Dynamic Media Classic使用資產名稱來建構URL字串時，會對資產名稱中的空白進行ASCII編碼。 這些 ASCII 代碼不易理解，從而使 URL 更難讀取。
* 檔名中允許使用特定語言的字元，但不允許使用下列字元:

  \ ; / ? : @ &amp; = + $ , &#42; &quot; &lt; > | &#39; { } %

  如果檔名中包含一或多個上述字元，上載時會將其從檔案名稱移除。

通常，資產檔案名稱可以與其料號、產品SKU或其他名稱相同，如下所示：

| 項目 | 檔案名稱 | 資產 ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 檔案夾組織和結構 {#folder-organization-and-structure}

上傳內容至系統之前，先在Adobe Dynamic Media Classic中組織和建構內容的資料夾和子資料夾。 採用這種方式提前進行規劃主要有兩個好處:

* 透過FTP將內容上傳至Adobe Dynamic Media Classic時，您可以指示系統在上傳期間復寫您的資料夾結構。 如此一來，您的內容就會在Adobe Dynamic Media Classic中與在您電腦或網路上的資料夾和子資料夾中加以整理。 (若要在Adobe Dynamic Media Classic中復寫資料夾結構，請在透過FTP上傳資產時選取「包含子資料夾」選項。)
* 與在開始就使用經過仔細計畫的檔案夾結構相比，在檔案上載之後重新對系統內的檔案夾進行組織要困難得多。

您選擇在Adobe Dynamic Media Classic上儲存內容的資料夾命名方法和結構取決於貴組織的需求。 以下是一些檔案夾結構範例:

**以SKU為基礎**  — 資料夾會根據SKU或專案編號命名。 例如，為所有以 0、20、30 開頭的編號序列分別建立單獨的檔案夾。

**品牌型**  — 針對擁有多個品牌線的製造商和銷售其他公司品牌的銷售商，將檔案分割成不同品牌的產品資料夾。

**以專案為基礎**  — 根據轉出/放置日期或專案名稱來組織資料夾。 主要產生 eCatalog 的客戶喜歡使用這種方法。

**網站資料夾階層的映象**  — 此資料夾結構會映象網站的資料夾結構，例如產品類別的資料夾名稱為時。

## 關於上傳檔案 {#uploading-your-files}

您可以從桌面上載個別檔案，或是透過 FTP 上載檔案夾。如果您想要上傳超過100 MB的檔案或上傳整個資料夾和子資料夾，請選取 **透過FTP** 標籤。

Adobe Dynamic Media Classic會傳送電子郵件給您，以確認上傳工作開始和結束的時間，並通知您發生任何問題。

在大型上載工作期間（或緊接在其後），某些新專案可能會顯示「影像尚未最佳化」訊息。 出現此訊息是因為檔案尚未完全處理並新增至Adobe Dynamic Media Classic。 您可以稍後將這些檔案最佳化。另請參閱 [最佳化檔案](application-setup.md#optimize_files).

### 使用「從案頭」標籤上傳檔案 {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic案頭應用程式可讓您透過拖曳方式來上傳檔案和資料夾。

1. 在Adobe Dynamic Media Classic案頭應用程式中，於全域導覽列上選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面上，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在「上傳」頁面的左側，在 **[!UICONTROL 選取要上傳的檔案]** 區域，選取 **[!UICONTROL 瀏覽]** 以選取您要上傳的檔案或資料夾，然後選取 **[!UICONTROL 開啟]**.
1. 在上傳頁面的右側，在 **選擇資料夾目的地** 區域，導覽至您想要新增已上傳檔案或資料夾的目標資料夾。
1. （選擇性）在「上傳」頁面底部附近的「工作名稱」文字欄位中，輸入上傳工作的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統產生名稱。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 上傳後發佈]** 如果您想要自動發佈您上傳的資產。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「工作選項」對話方塊中也提供相同選項。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]** 如果您希望上傳的檔案以相同名稱取代現有檔案。 「工作選項」對話方塊中也提供相同選項。
此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.
1. 在「上傳」頁面的右下角附近，選取 **[!UICONTROL 工作選項]**，然後指定您想要的選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 提交上傳]**.
若要檢視上傳進度，請選取 **[!UICONTROL 工作]** 全域導覽列上。 您可以繼續在Adobe Dynamic Media Classic中工作，並隨時返回「工作」頁面來檢閱進行中的工作。 若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

### 使用「透過FTP」索引標籤上傳檔案 {#upload-files-using-via-ftp}

1. 登入特定地區的Adobe Dynamic Media Classic FTP網站。 使用管理員寄給您的 FTP 使用者名稱與密碼。
1. 在Adobe Dynamic Media Classic中的全域導覽列上，選取「 」 **[!UICONTROL 上傳]**.
1. 在上傳頁面上，選取 **[!UICONTROL 透過FTP]** 標籤。
1. 在「上傳」頁面的左側，在 **[!UICONTROL 選擇要上傳的FTP資料夾]** 區域，選擇要從中上傳檔案的FTP資料夾。
1. 在上傳頁面的右側，在 **[!UICONTROL 選擇AdobeDynamic Media資料夾目的地]** 區域，選擇Adobe Dynamic Media Classic中的目的地資料夾。
1. （選擇性）在「上傳」頁面底部附近的「工作名稱」文字欄位中，輸入上傳工作的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統產生名稱。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 上傳後發佈]** 如果您想要自動發佈您上傳的資產。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「工作選項」對話方塊中也提供相同選項。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]** 如果您希望上傳的檔案以相同名稱取代現有檔案。 「工作選項」對話方塊中也提供相同選項。
此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.
1. 選擇性；只有當您按一下 **[!UICONTROL 透過FTP]** 標籤。 在上傳頁面底部附近，選取 **[!UICONTROL 上傳時解壓縮Zip或Tar檔案]** 如果您想從上傳的ZIP或TAR檔案中自動解壓縮所有檔案。 「工作選項」對話方塊中也提供相同選項。
1. 在「上傳」頁面的右下角附近，選取 **[!UICONTROL 工作選項]**，然後指定您想要的選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 提交上傳]**.

   若要檢視上傳進度，請在全域導覽列上選取 **[!UICONTROL 工作]**. 「工作」頁面隨即出現，並顯示上載的進度。您可以繼續在Adobe Dynamic Media Classic中工作，並隨時返回「工作」頁面來檢閱進行中的工作。

若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

## 上載工作選項對話方塊 {#upload-options}

上傳檔案時，您可以在「上傳工作選項」對話方塊中選擇以下選項：

* **工作**  — 選取 **[!UICONTROL 工作]** 以選擇影響整個上載工作的選項。

  您也可以選擇 *預設* 使用上傳作業的選項 **[!UICONTROL 預設上傳選項]** 對話方塊。 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 預設上傳選項]**，然後設定您想要的預設選項。

   * **[!UICONTROL 時間]**  — 只有當您選取 **[!UICONTROL 透過FTP]** 標籤。
      * **[!UICONTROL 一次性]**  — 指定執行一次的上傳工作。 選項包括：
         * **[!UICONTROL 現在]**  — 選取後立即執行上載工作 **[!UICONTROL 儲存]** 在「上載工作選項」對話方塊中，然後選取 **[!UICONTROL 提交上傳]** （在上傳頁面上）。
         * **[!UICONTROL 排程供日後使用]**  — 選取您要執行上載工作的年、月、日和時間（以15分鐘為增量）。
      * **[!UICONTROL 週期性]**  — 指定每日、每週或每月執行的上傳工作。 或者，根據您自己的規格自訂上載工作。
         * **[!UICONTROL 每日]**  — 設定每天要執行工作的時間。 如果您希望工作只在星期一到星期五執行，請選取 **[!UICONTROL 僅限工作日]**.
         * **[!UICONTROL 每週]**  — 選擇您想要執行工作的一週中的特定日和時間。
         * **[!UICONTROL 每月]**  — 選擇您想要執行工作的特定日期（當月或當週某日），包括開始時間。
         * **[!UICONTROL 自訂]**  — 根據您自己的規格自訂上載或發佈工作時間間隔。 另請參閱 [建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL 上傳後發佈]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。 選取此選項即可自動發佈您上載的資產。當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「上載」頁面上也有此選項。

   * **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。 如果您要以上載的檔案來取代現有同名檔案，請選取此選項。「上載」頁面上也有此選項。 此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.

   * **[!UICONTROL 上傳時解壓縮Zip或Tar檔案]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。
如果您想要自動從上傳的ZIP或TAR檔案解壓縮所有檔案，請選取此選項。 「工作選項」對話方塊中也提供相同選項。

   * **[!UICONTROL 包含子資料夾]**  — 僅當您選取 **[!UICONTROL 透過FTP]** 標籤。
如果您要一併上載檔案夾及其子檔案夾，請選取此選項。您上傳的資料夾及其子資料夾的名稱會自動在Adobe Dynamic Media Classic中輸入。

   * **[!UICONTROL 處理中繼資料檔案]**  — 僅當您選取 **[!UICONTROL 透過FTP]** 標籤。 如果要上載 Tab 字元分隔檔案或 XML 檔案以將中繼資料增加到多個資產中，可以選取該選項。請參閱[匯入中繼資料 (透過 FTP)](viewing-adding-exporting-metadata.md#import-metadata)。

* **裁切選項**  — 若要自動裁切影像中的空白畫素，請開啟 **[!UICONTROL 裁切]** 功能表，選取 **[!UICONTROL 手動]**，並在「上」、「右」、「下」和「左」文字欄位中輸入畫素度量，從側面裁切。 您也可以選取 **[!UICONTROL Trim]** 在「裁切」選單上，選擇下列選項：

   * **[!UICONTROL 修剪依據]**  — 選擇根據顏色或透明度裁切：
      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 接著選取「邊角」選單，然後選擇含有最能代表您要裁切之空白區域色彩的影像邊角。依據色彩修剪: 指定為 0 時，則僅當像素與您在影像邊角中所選取色彩完全相符時才會裁切像素。數值越接近 1，允許的色彩差異就越大。
      * **[!UICONTROL 透明度]**  — 選擇 **[!UICONTROL 透明度]** 選項。
根據透明度裁剪：指定0可裁切透明畫素；數字越接近1則透明度越高。
      * **[!UICONTROL 容許度]**  — 拖曳滑桿以指定從0到1的公差。

* **色彩設定檔選項**  — 當您建立用於Adobe Dynamic Media Classic動態傳送的最佳化檔案時，請選擇色彩轉換：

   * **[!UICONTROL 預設色彩儲存]**  — 當影像包含色域資訊時，維持來源影像色彩；沒有色彩轉換。 幾乎所有影像目前都已內嵌適當的色彩設定檔。不過，如果 CMYK 來源影像沒有內嵌色彩設定檔，其色彩就會轉換為 sRGB (標準三原色) 色域。sRGB 是在網頁上顯示影像時建議使用的色域。
   * **[!UICONTROL 保留原始色域]**  — 保留原始顏色，在擷取至Adobe Dynamic Media Classic時不會進行任何顏色轉換。 對於沒有內嵌色彩設定檔的影像，處理影像要求所需的任何色彩轉換都是使用在「發佈」設定中設定的預設色彩設定檔來完成。 這些色彩設定檔並不總是與使用此選項建立的檔案中的色彩一致。 因此，最好使用「預設色彩保存」選項。
   * **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**  — 開啟功能表，讓您選擇 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 色域。 這個進階選項會覆蓋來源檔案內嵌的任何色彩資訊。只有在您要提交的所有影像包含不正確或遺失色彩設定檔資料時，才選取此選項。

* **影像編輯選項**  — 您可以保留影像中的剪裁&lt;>遮色片，並選擇色彩設定檔。
另請參閱 [上傳時影像微調選項](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript®選項**  — 您可以點陣化PostScript®檔案、裁切檔案、保留透明背景、選擇解析度，以及選擇色域。
另請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop選項**  — 您可以從Adobe® Photoshop®檔案建立範本、維護圖層、指定圖層的命名方式、擷取文字，以及指定影像錨定到範本的方式。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

* **PDF選項**  — 您可以點陣化檔案、擷取搜尋字詞和連結、自動產生eCatalog、設定解析度，以及選擇色域。
請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

* **Illustrator選項**  — 您可以點陣化Adobe Illustrator®檔案、保留透明背景、選擇解析度以及選擇色域。
另請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO選項**  — 您可以選擇視訊預設集，將視訊檔案轉碼。
另請參閱 [使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **其他中繼資料**  — 輸入說明您要上傳之檔案的關鍵字。 用逗號分隔關鍵字。使用關鍵字使搜尋資產變得更容易。另請參閱 [執行進階搜尋](searching-assets.md#conducting_an_advanced_search). 另請參閱 [上傳關鍵字](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) 訓練影片。

* **批次集預設集**  — 如果要從上傳的檔案建立影像集、迴轉集或色票集，請選取 **[!UICONTROL 作用中]** 欄中選取您要使用的預設集。 可以選取多個預設集。可以在「應用程式設定」/「批次集預設集」頁面中建立預設集。請參閱[批次集預設集](application-setup.md#batch_set_presets)。

* **進階**  — 請參閱 [上載後執行其他工作](uploading-files.md#follow-an-upload-with-another-job).

## 上載後執行其他工作 {#follow-an-upload-with-another-job}

使用FTP上傳專案時，您可以排程後續工作，以便在上傳完成時開始。 如果排程開始其他工作，您在此排程的工作會在它們之後排入佇列。

新工作會將通知傳送至您指定的地址，以便觸發該位置的代碼。 該後續發佈工作所使用的名稱與上載工作相同，但在開頭加有文字 *Pub_*。

**上載後執行其他工作:**

1. 選取 **[!UICONTROL 上傳]**，然後選取 **[!UICONTROL 透過FTP]** 標籤。
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 工作選項]**.
1. 在「上載工作選項」對話方塊中，展開 **[!UICONTROL 進階]** 區段。
1. 從下列選項中選擇一項 **[!UICONTROL 上載後執行其他工作]** 下拉式清單：

   * 無
   * HTTP 要求
   * 影像伺服發佈
   * 影像演算發佈
   * 視訊發佈

1. 指定 HTTP 位址。
1. 指定您是否只想在上傳檔案時執行。
1. 指出希望在每次完成該工作時執行要求，還是僅當檔案發佈後執行該要求。

   >[!NOTE]
   >
   >定期排程的工作有時會導致未發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產資料夾](asset-folders.md#working_with_asset_folders)
>* [處理週期性上傳和發佈工作](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
