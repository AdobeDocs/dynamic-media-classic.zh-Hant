---
title: 上載檔案
seo-title: 上載檔案
description: 'null'
seo-description: 瞭解如何上傳檔案。
uuid: b3025f84-4f28-4276-bc9 c-f0 c0 c2 a26 e12
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
discoiquuid: b2bc3bf9-e313-481a-8670-c3 debide21 b1 a
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# Uploading files{#uploading-files}

將資產檔案上載到 Scene7 Publishing System 之前，確保資產檔案命名正確，並且檔案夾結構的建立及組織符合要求。 您可以從Dynamic Media Classic提供的FTP站台或直接從電腦或網路上傳檔案。Dynamic Media Classic提供在上傳檔案時最佳化檔案的選項。如果安裝了 Adobe Scene7 Publishing System 桌面應用程式，可以採用直接從桌面拖曳的方式來上載檔案和檔案夾。 (請參閱[應用程式一般設定](application-setup.md#general_settings)。)

## 準備要上載的資產和檔案夾 {#preparing-your-assets-and-folders-for-uploading}

在將資產上載至 Scene7 Publishing System 之前，確保資產的格式和大小正確。 您也必須觀察命名資產的動態媒體Classic規則。為檔案設定檔案夾組織和結構之前，請確定您可以輕鬆尋找和處理檔案。

### 支援的資產檔案格式 {#supported-asset-file-formats}

此表格列出 Scene7 Publishing System 支援的資產檔案格式。 For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| 資產檔案格式 | 說明 |
|--- |--- |
| 音效資料 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 階層式樣式表 | CSS |
| 色彩設定檔 | ICC、ICM |
| 字型 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 影像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT (僅限 Windows)、TIF、TIFF |
| InDesign | INDD、INDT |
| MS Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| 動態媒體Classic影像製作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 視訊 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上載支援包含一個核取框，供您選取是否想要解壓縮檔案。

### 資產類型 {#asset-types}

若要使用Dynamic Media Classic平台達到最佳結果，請務必使用建議的檔案格式和大小。下表格列出了資產類型，其中一些資產類型具有常用資產的建議格式和檔案大小。

| 資產類型 | 描述/建議 |
|--- |--- |
| 音效資料 | 輸入音訊資產格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。 可以將音訊轉碼為以下格式: MP3、AAC 和 HE-AAC。 |
| 影像 (用於調整影像大小、縮放、影像集、迴轉集) | 影像的最大尺寸必須至少為 2000 像素；典型影像大小最大尺寸範圍在 1500 到 2500 像素之間。 建議使用不失真的影像格式，包括 TIFF 和 PNG 檔案。 如果使用 JPEG 影像，請使用最高品質的設定。Animate GIF檔案的處理方式與其他靜態內容相同。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 應用程式中建立並儲存為「印刷就緒」的高解析度 PDF 檔案。 PDF 包括所有需要的字型、影像、遮色片以及參照的圖形化元素，採用單頁、雙頁式跨頁或多頁格式。 透過按字母數字順序為檔案命名來排列頁面順序。 將 eCatalog 的所有 PDF 檔放於一個檔案夾中，以便上載。 您可以在上載時選取裁切選項，以便從 PDF 中移除修剪區域，包括裁切標記、對齊目標或色彩導表。 多數印刷就緒的 PDF 檔案採用 CMYK 色域，因此務必要獲得用於 PDF 檔案的 CMYK ICC 色彩設定檔。 |
| 範本 | 分層影像或版面設計，可以包括文字、影像和圖層。 可以將圖層、文字字串和屬性 (如色彩和大小) 參數化，從而可以自訂變數資料。 在範本中使用時的影像要求與其他影像相同。 在 Photoshop 或其他影像編輯程式中準備圖形。 採用 TIFF 或 PNG 格式將每個圖形儲存為平面化透明檔案。 確保影像解析度適合所要求的用途。 準備列印的影像應為 300 ppi。 |
| 視訊 | Dynamic Media Classic支援儲存在OGV和MP格式中的視訊檔案。您可以在上傳時將檔案轉換為MP格式。請參閱 [支援的資產檔案格式](#supported-static-file-formats)。 |
| 字型 | 上載的 TrueType、Type1 (僅 Windows)、OpenType 字型以及 PhotoFont |
| 影像 | 影像和分層影像檔案。 |
| 影像集和色票集 | 可以在檢視器中顯示的一組相關影像。 |
| ICC 設定檔 | 色彩設定檔，可以用來將上載的影像從來源色域轉換為其他色域。 |
| 暈映 | 使用「影像創作」程式創作的影像及相關的檔案。 |
| 內容檔案 | Adobe InDesign、Illustrator 或 Photoshop 內容檔案。 |
| FXG 檔案 | 與解析度無關的圖形格式檔案，可以用來建立能夠自訂的範本，以輸出進行列印、輸出到網路、電子郵件、桌面以及裝置。 |
| SVG 檔案 | 「影像伺服」伺服器可以演算的可擴放向量圖形檔案。 |
| XML 檔案 | 定義用於修改要求路徑和查詢部分之預處理規則的檔案。 |
| 階層式樣式表檔案。 | 上載用以自訂 HTML5 檢視器的 CSS 外觀。 |
| JavaScript 檔案 | 編寫檢視器時用於保存帳戶資訊的 Javascript 檔案。 Adobe Security 僅推薦將該檔用於使用單獨網域進行傳送 (以避免跨網站編寫指令碼) 的用戶端帳戶。 |

>[!NOTE]
>
>將影像檔案和 PDF 上載至 SPS 時，系統將這些來源檔案轉換為 P-TIFF (金字塔 TIFF) 檔案。 這些P-TIFF是稍後發佈至動態媒體影像伺服器的檔案。Dynamic Media Classic使用Dynamid TIFF檔案格式，因為它包含多種縮放比例，可在使用Dynamic Media Classic縮放檢視器檢視時快速縮放。

### 支援的靜態檔案格式 {#supported-static-file-formats}

Dynamic Media Classic支援數種靜態檔案格式。靜態內容是任何發佈「as-is」的資產，例如CSS、PDF、SVG、XML等。

您可以發佈下列檔案類型:

* 動畫 GIF
* 音訊檔案
* CSS
* JavaScript (當公司設定了自己的網域時)
* 主視訊
* PDF (當 PDF 在上載後被特別標記為發佈時，以避免傳送現有 eCatalog/PDF 工作流程的所有 PDF)
* PrX 視訊
* SVG
* XML
* ZIP

Dynamic Media Classic不提供產生靜態內容預覽URL的選項。

### 檔案名稱要求 {#filename-requirements}

由於在檔案上載過程中將去除檔案名中的副檔名，因此系統不允許檔案使用相同的根名稱。在Dynamic Media Classic系統中，資產檔案名稱減去檔案名稱副檔名會變成資產的資產ID。因此，兩個資產不能同名。

確保貴公司的所有使用者都瞭解以下檔案命名規則: 

* 系統中不允許存在名稱完全相同的資產 ID。
* 資產 ID 的名稱區分大小寫。
* 最佳做法是確保資產 ID 不包含空格 (例如 black jacket.tif 和 blue jacket.jpg)。當資產名稱使用資產名稱建構URL字串時，動態媒體Classic ASCII會在資產名稱中空白空格。這些 ASCII 代碼不易理解，從而使 URL 更難讀取。
* 檔名中允許使用特定語言的字元，但不允許使用下列字元:

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   如果檔名中包含一或多個上述字元，上載時會將其從檔案名稱移除。

在多數情況下，資產檔名可以與其項目編號、產品 SKU 或其他名稱相同，例如:

| 項目 | 檔案名稱 | 資產 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 檔案夾組織和結構 {#folder-organization-and-structure}

請先在 Scene7 Publishing System 中組織內容的檔案夾及子檔案並建立其結構，然後再將內容上載至系統。採用這種方式提前進行規劃主要有兩個好處:

* 在透過 FTP 將內容上載至 SPS 時，可以通知系統在上載期間複製檔案夾結構。這樣，在 SPS 中您的內容所在的檔案夾和子檔案夾，就與其在您電腦或網路上所在的檔案夾和子檔案夾相同。(要在 SPS 中複製您的檔案夾結構，在透過 FTP 上載資產時，選取「包含子檔案夾」選項。)
* 與在開始就使用經過仔細計畫的檔案夾結構相比，在檔案上載之後重新對系統內的檔案夾進行組織要困難得多。

您選擇用來在 Scene7 Publishing System 上儲存內容的檔案夾命名方法和結構取決於貴組織的需求。以下是一些檔案夾結構範例:

**SKU** 型資料夾是根據SKU或項目編號命名。例如，為所有以 0、20、30 開頭的編號序列分別建立單獨的檔案夾。

**以品牌為基礎** 的製造商，擁有多種品牌線條和零售商，行銷其他公司的其他品牌，將檔案區隔為不同品牌的產品資料夾。

**專案** 型資料夾會根據轉出/放置日期或專案名稱進行組織。主要產生 eCatalog 的客戶喜歡使用這種方法。

**網站資料夾階層的鏡像** 此檔案夾結構反映了網站的檔案夾結構，並使用例如產品類別的檔案夾。

## 關於上傳檔案 {#uploading-your-files}

您可以從桌面上載個別檔案，或是透過 FTP 上載檔案夾。If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

如果您安裝Scene Publishing System桌面應用程式，可以直接從桌面拖曳檔案和檔案夾至目的地上傳資料夾。

Scene7 Publishing System 會在您的上載工作開始和結束時向您傳送一封電子郵件進行確認，並將任何問題通知給您。

執行大批量上載工作期間 (或隨後)，有些新項目可能顯示「尚未最佳化影像」訊息。此訊息會出現，因為檔案尚未完整處理並新增至SPS。您可以稍後將這些檔案最佳化。(請參閱[最佳化檔案](application-setup.md#optimize_files)。)

### 使用FROM桌面標籤上傳檔案 {#upload-files-using-sps-desktop-application}

Scene7 Publishing System Desktop 應用程式允許以拖曳方式上載檔案和檔案夾。

1. 在 Scene7 Publishing System Desktop 應用程式中，按一下全域導覽列中的「**上載**」。
1. On the Upload page, click the **FROM DESKTOP** tab.
1. 在「上傳」頁面的左側，在 **「選取檔案用於上傳的檔案」** 中，按一下 **「瀏覽** 」以選取您要上傳的檔案或資料夾，然後按一下 **「開啓**」。
1. 在「上傳」頁面的右側，在 **「選擇檔案夾目的地** 」區域中，瀏覽至您想要新增已上傳檔案或資料夾的目標檔案夾。
1. (可選)在「上傳」頁面底部附近，在 **「工作名稱** 」欄位中指定上傳工作的新名稱。或者，您只需使用SPS提供的預設系統產生名稱。工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. (可選)在「上載」頁面底部，如果您要自動發佈上傳的資產，請選取 **「上載** 後發佈」。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。請注意，此相同選項也可在「工作選項」對話框中使用。
1. (可選)在「上傳」頁面底部，如果您要上傳檔案以取代同名的現有檔案，請在任何檔案夾中選取 **「覆寫」，而不考慮副** 資產。請注意，此相同選項也可在「工作選項」對話框中使用。
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話框中，按一下「**儲存**」。
1. 在「上傳」頁面右下角，按一下 **「送出上傳**」。
若要查看上載進度，按一下全域導覽列中的「**工作**」。您可以在 Scene7 Publishing System 中繼續工作，並隨時返回「工作」頁面檢閱進行中的工作。若要取消進行中的上載工作，請選取「持續時間」旁邊的「**取消**」按鈕。

### 使用FIA FTP標籤上傳檔案 {#upload-files-using-via-ftp}

1. 登入特定地區專屬的Dynamic Media Classic FTP站台。使用管理員寄給您的 FTP 使用者名稱與密碼。
1. 在Dynamic Media Classic中，在全域導覽列上，按一下 **「上傳**」。
1. On the Upload page, click the **VIA FTP** tab.
1. 在「上傳」頁面的左側，在 **「選擇FTP檔案夾for上傳」** 區域中，選擇要上傳檔案的FTP檔案夾。
1. 在「上傳」頁面右側，在 **「選擇SPS檔案夾目的地** 」區域中，選擇Scene Publishing System的目的地檔案夾。
1. (可選)在「上傳」頁面底部附近，在 **「工作名稱** 」欄位中指定上傳工作的新名稱。或者，您只需使用SPS提供的預設系統產生名稱。工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. (可選)在「上傳後」頁面底部，如果您想要自動發佈上傳的資產，請選取 **** 「上載後發佈」。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。請注意，此相同選項也可在「工作選項」對話框中使用。
1. (可選)在「上傳」頁面底部，如果您要上傳檔案以取代同名的現有檔案，請在任何檔案夾中選取 **「覆寫」，而不考慮副** 資產。請注意，此相同選項也可在「工作選項」對話框中使用。
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. (可選；只有在您按下 **「上傳FTP** 」標籤時才可使用)，如果 **您想要自動從上傳的ZIP或TAR檔案中擷取所有檔案，請選取「上傳** 時解壓縮Zip」或「Tar Files on Upload」(解除壓縮郵遞區號)。請注意，此相同選項也可在「工作選項」對話框中使用。
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話框中，按一下「**儲存**」。
1. 在「上傳」頁面右下角，按一下 **「送出上傳**」。

   若要查看上載進度，請按一下全域導覽列中的「**工作**」。「工作」頁面隨即出現，並顯示上載的進度。您可以在 Scene7 Publishing System 中繼續工作，並隨時返回「工作」頁面檢閱進行中的工作。

若要取消進行中的上載工作，請按一下「持續時間」旁邊的「**取消**」。

## 上傳工作選項對話方塊 {#upload-options}

上傳檔案時，您可以從「上載工作選項」對話方塊中的下列選項中選擇：

* **工作** —按一下 **「工作** 」，選擇影響整個上傳工作的選項。

   請注意，您也可以使用 *一般* 設定中的「 **預設上傳選項」** 對話方塊，選擇上傳工作的預設選項。按一下 **「設定&gt;應用程式設定&gt;一般設定&gt;預設上傳選項**」，然後設定您想要的預設選項。

   * **** 當— **只有** 當您選取 **「通過FTP** 」標籤時，才可使用「When」選項。
      * **一次性** -指定一次執行的上載工作。選項包括：
         * **** 現在—按一下「上傳工作選項」對話方塊中 **的「儲存」** ，然後按一下「上傳」頁面上的 **「提交上傳** 」，即可立即執行上傳工作。
         * **稍後排程** ：選取您要執行上傳工作的年、月、日和時間(以15分鐘為單位)。
      * **週期性** —指定每日、每周或每月執行的上載工作。或者，依您自己的規格自訂上傳工作。
         * **每日** —設定您希望每日工作執行的時間。如果您希望工作只有星期一到星期五，請選取「僅 **限工作日」**。
         * **每周** —選擇您要執行工作的周和時間的特定日期。
         * **每月** —選擇一個月中的某一天或一周中的某天(包括您希望工作執行的開始時間)。
         * **自訂** —依您自己的規格自訂上傳或發佈工作時間間隔。請參閱[建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **上傳後發佈** —如果您選取 **「FROM Desktop** 」標籤或 **「FIA FTP** 」索引標籤，則可使用此選項。選取此選項即可自動發佈您上載的資產。當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「上載」頁面上也有此選項。

   * **在任何檔案夾中覆寫相同的基本資產名稱，不論副檔名** 為何—如果您選取 **「FROM Desktop** 」標籤或 **「FIA FTP** 」索引標籤，則可使用此選項。如果您要以上載的檔案來取代現有同名檔案，請選取此選項。「上載」頁面上也有此選項。 The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.

   * **在上傳時解壓縮郵遞區號或Tar檔案** ：如果您選取 **「FROM Desktop** 」標籤或 **「FIA FTP** 」索引標籤，則可使用此選項。
如果您要自動從上傳的ZIP或TAR檔案中擷取所有檔案，請選取此選項。請注意，此相同選項也可在「工作選項」對話框中使用。

   * **包含子檔案夾** —只有在您選取 **「通過FTP** 」標籤時才可用。
如果您要一併上載檔案夾及其子檔案夾，請選取此選項。在 SPS 中會自動輸入您上載的檔案夾及其子檔案夾的名稱。

   * **流程中繼資料檔案** —只有當您選取 **「通過FTP** 」標籤時才可用。如果要上載 Tab 字元分隔檔案或 XML 檔案以將中繼資料增加到多個資產中，可以選取該選項。請參閱[匯入中繼資料 (透過 FTP)](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁切選項** —若要自動裁切影像的空格像素，請開啓「裁切」功能表、選擇「手動」，然後在「頂端」、「右側」、「底部」和「左側」欄位中輸入像素度量，以便從兩側裁切。您也可以從「裁切」選單中選擇「修剪」並選擇以下選項:

   * **修剪為根據** —選擇是否根據顏色或透明度進行裁切：

      * **色彩** —選擇「顏色」選項。接著選取「邊角」選單，然後選擇含有最能代表您要裁切之空白區域色彩的影像邊角。

         依據色彩修剪: 指定為 0 時，則僅當像素與您在影像邊角中所選取色彩完全相符時才會裁切像素。數值越接近 1，允許的色彩差異就越大。

      * **透明度** —選擇「透明度」選項。

         依據透明度修剪: 指定為 0 時，則僅當像素完全透明時裁切像素；數值越接近 1，允許的透明度就越高。

      * **容許度** —拖曳滑桿以指定到1的容許度。

* **色彩描述檔選項** —當您建立用於動態媒體Classic動態傳送的最佳化檔案時，可選擇色彩轉換：

   * **預設色彩保留** —每當影像包含色域資訊時，仍會保留來源影像色彩；沒有色彩轉換。幾乎所有影像目前都已內嵌適當的色彩設定檔。不過，如果 CMYK 來源影像沒有內嵌色彩設定檔，其色彩就會轉換為 sRGB (標準三原色) 色域。sRGB 是在網頁上顯示影像時建議使用的色域。

   * **保留原始色域** —在擷取到Scene Publishing System時，不會將原始顏色轉換為任何顏色。至於沒有內嵌色彩設定檔的影像，則會使用「發佈」中設定的預設色彩設定檔進行任何必要的色彩轉換，以利處理影像請求。這些色彩設定檔可能和以此選項建立的檔案中的色彩不一致。因此，最好使用「預設色彩保存」選項。

   * **自訂自&gt;到開啓選單，您可以選擇「轉換自」和「轉換為色域」。**&#x200B;這個進階選項會覆蓋來源檔案內嵌的任何色彩資訊。只有當您送出的所有影像包含不正確或遺失的色彩描述檔資料時，才應該選取此選項。

* **影像編輯選項** —您可以保留影像中的剪裁&lt;&gt;遮色片，並選擇顏色描述檔。
請參閱[上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)。

* **PostScript選項** —您可以點陣化PostScript®檔案、裁切檔案、維護透明背景、選擇解析度並選擇色域。
請參閱[使用 PostScript 和 Illustrator 檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **PHOTOSHOP選項** —您可以從Adobe® Photoshop®檔案建立範本、保留圖層、指定圖層的命名方式、擷取文字，以及指定影像錨定到範本中的方式。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

* **PDF選項** —您可以點陣化檔案、擷取搜尋字詞和連結、自動產生eCatalog、設定解析度，以及選擇色域。
請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

* **ILLUSTRATOR選項** —您可以點陣化Adobe Illustrator®檔案、維護透明背景、選擇解析度並選擇色域。
請參閱[使用 PostScript 和 Illustrator 檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVideo選項** —您可以選擇影片預設集來轉碼影片檔案。
請參閱[使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他中繼資料** —輸入描述您將上傳之檔案的關鍵字。用逗號分隔關鍵字。使用關鍵字使搜尋資產變得更容易。請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

* **批次集預設集** —如果您想要建立「影像集」、「多軸回轉集」或上傳的檔案中的色票集，請針對您要使用的預設集按一下「作用中」欄。可以選取多個預設集。可以在「應用程式設定」/「批次集預設集」頁面中建立預設集。請參閱[批次集預設集](application-setup.md#batch_set_presets)。

* **Advanced** -請參閱 [與其他工作](uploading-files.md#follow-an-upload-with-another-job)一起上傳。

## 上載後執行其他工作 {#follow-an-upload-with-another-job}

使用 FTP 上載項目時，可以安排一個後續工作在上載完成後立即開始執行。(如果有其他工作排程在此時開始，您在此處排程的工作將在佇列中排在其他工作的後面。)

新工作將向您指定的位址傳送一則通知，以觸發該位置的程式碼。該後續發佈工作所使用的名稱與上載工作相同，但在開頭加有文字 *Pub_*。

**上載後執行其他工作**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. 在「上傳工作選項」對話方塊中，展開 **「進階」** 區段。
1. 從「追隨上傳 **」中選擇下列其中一個工作** 下拉式清單：

   * 無
   * HTTP 要求
   * 影像伺服發佈
   * 影像演算發佈
   * 視訊發佈

1. 指定 HTTP 位址。
1. 指定是否只有在上傳檔案時才要執行。
1. 指出希望在每次完成該工作時執行要求，還是僅當檔案發佈後執行該要求。

   >[!NOTE]
   >
   >定期排程的工作不會導致發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產檔案夾](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

