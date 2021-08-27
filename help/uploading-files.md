---
title: 上載檔案
description: 了解如何在AdobeDynamic Media Classic中上傳檔案。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '3866'
ht-degree: 34%

---

# 上載檔案{#uploading-files}

在將資產檔案上傳至AdobeDynamic Media Classic之前，請確定資產檔案的名稱正確，而且您的資料夾結構是依照您想要的方式設定和組織。 您可以從AdobeDynamic Media Classic提供的FTP站台或直接從您的電腦或網路上傳檔案。 AdobeDynamic Media Classic提供上傳檔案時最佳化檔案的選項。 如果您安裝了AdobeDynamic Media Classic案頭應用程式，則可以直接從案頭拖曳檔案和資料夾，以便上傳檔案和資料夾。 請參閱[應用程式一般設定](application-setup.md#general_settings)。

## 準備資產和資料夾以便上傳 {#preparing-your-assets-and-folders-for-uploading}

在將資產上傳至AdobeDynamic Media Classic之前，請確定其格式和大小正確。 您也必須遵循AdobeDynamic Media Classic的資產命名規則。 為檔案設定檔案夾組織和結構之前，請確定您可以輕鬆尋找和處理檔案。

### 支援的資產檔案格式 {#supported-asset-file-formats}

下表列出AdobeDynamic Media Classic支援的資產檔案格式。 有關支援的Camera Raw檔案的資訊，請參閱[https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html)。

| 資產檔案格式 | 說明 |
| --- | --- |
| 音效資料 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 階層式樣式表 | CSS |
| 色彩設定檔 | ICC、ICM |
| 字型 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 影像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT(僅限Windows®)、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| AdobeDynamic Media Classic影像製作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 視訊 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上載支援包含一個核取框，供您選取是否想要解壓縮檔案。

### Dynamic Media不支援的影像格式 {#unsupported-image-formats-dynamic-media}

下列清單說明Dynamic Media支援的點陣影像檔案格式的子類型，這些格式為&#x200B;*not*。

另請參閱[偵測不支援的Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)檔案格式。

* IDAT區塊大小大於100 MB的PNG檔案。
* PSB檔案。
* 不支援使用CMYK、RGB、灰度或點陣圖以外的顏色空間的PSD檔案。 不支援DuoTone、Lab和索引色空間。
* 位深度大於16的PSD檔案。
* 具有浮點資料的TIFF檔案。
* 具有Lab色域的TIFF檔案。

### 資產類型 {#asset-types}

若要使用Adobe Dynamic Media Classic程式達到最佳效果，請務必使用建議的檔案格式和大小。 下表格列出了資產類型，其中一些資產類型具有常用資產的建議格式和檔案大小。

| 資產類型 | 描述/建議 |
| --- | --- |
| 音效資料 | 輸入音訊資產格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。 可以將音訊轉碼為以下格式: MP3、AAC 和 HE-AAC。 |
| 影像 (用於調整影像大小、縮放、影像集、迴轉集) | 影像長度必須至少為2000像素；一般影像大小範圍為最大的1500到2500像素。 建議使用不失真的影像格式，包括 TIFF 和 PNG 檔案。 如果使用 JPEG 影像，請使用最高品質的設定。動畫GIF檔案的處理方式與其他靜態內容相同。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 應用程式中建立並儲存為「印刷就緒」的高解析度 PDF 檔案。 PDF 包括所有需要的字型、影像、遮色片以及參照的圖形化元素，採用單頁、雙頁式跨頁或多頁格式。 透過按字母數字順序為檔案命名來排列頁面順序。 將 eCatalog 的所有 PDF 檔放於一個檔案夾中，以便上載。 您可以在上載時選取裁切選項，以便從 PDF 中移除修剪區域，包括裁切標記、對齊目標或色彩導表。 多數印刷就緒的 PDF 檔案採用 CMYK 色域，因此務必要獲得用於 PDF 檔案的 CMYK ICC 色彩設定檔。 |
| 範本 | 分層影像或版面設計，可以包括文字、影像和圖層。 可以將圖層、文字字串和屬性 (如色彩和大小) 參數化，從而可以自訂變數資料。 在範本中使用時的影像要求與其他影像相同。 在 Photoshop 或其他影像編輯程式中準備圖形。 採用 TIFF 或 PNG 格式將每個圖形儲存為平面化透明檔案。 確保影像解析度適合所要求的用途。 打印影像為300 ppi。 |
| 視訊 | AdobeDynamic Media Classic支援以OGV和MP4格式儲存的視訊檔案。 您可以在上載時，將檔案轉碼為 MP4。請參閱[支援的資產檔案格式](#supported-static-file-formats)。 |
| 字型 | 上載的TrueType、Type1(僅限Windows®)、OpenType®字型和PhotoFonts。 |
| 影像 | 影像和分層影像檔案。 |
| 影像集和色票集 | 可以在檢視器中顯示的一組相關影像。 |
| ICC 設定檔 | 色彩設定檔，可以用來將上載的影像從來源色域轉換為其他色域。 |
| 暈映 | 使用影像製作程式製作的影像以及相關檔案。 |
| 內容檔案 | Adobe InDesign、Illustrator 或 Photoshop 內容檔案。 |
| FXG 檔案 | 與解析度無關的圖形格式檔案，可以用來建立能夠自訂的範本，以輸出進行列印、輸出到網路、電子郵件、桌面以及裝置。 |
| SVG 檔案 | 「影像伺服」伺服器可以演算的可擴放向量圖形檔案。 |
| XML 檔案 | 定義用於修改要求路徑和查詢部分之預處理規則的檔案。 |
| 階層式樣式表檔案。 | 上載用以自訂 HTML5 檢視器的 CSS 外觀。 |
| JavaScript 檔案 | JavaScript檔案用於檢視器檢測以保留帳戶資訊。 Adobe安全性建議僅針對傳送時使用個別網域的用戶端帳戶使用此資產類型（以避免跨網站指令碼）。 |

>[!NOTE]
>
>當您上傳影像檔案和PDF以AdobeDynamic Media Classic時，系統會將這些來源檔案轉換為P-TIFF（金字塔TIFF）檔案。 這些P-TIFF是稍後發佈至Dynamic Media影像伺服器的檔案。 AdobeDynamic Media Classic使用金字塔Tiff檔案格式，因為它包含各種縮放比例，在使用AdobeDynamic Media Classic縮放檢視器檢視時可快速縮放。

### 支援的靜態檔案格式 {#supported-static-file-formats}

AdobeDynamic Media Classic支援多種靜態檔案格式。 靜態內容是任何「原樣」發佈的資產，例如CSS、PDF、SVG和XML。

您可以發佈下列檔案類型:

* 動畫 GIF
* 音訊檔案
* CSS
* JavaScript (當公司設定了自己的網域時)
* 主視訊
* PDF（上傳後將PDF標示為發佈時，為了避免傳送現有eCatalog/PDF工作流程的所有PDF）
* PrX 視訊
* SVG
* XML
* ZIP

AdobeDynamic Media Classic不提供產生靜態內容預覽URL的選項。

### 檔案名稱要求 {#filename-requirements}

由於在檔案上載過程中將去除檔案名中的副檔名，因此系統不允許檔案使用相同的根名稱。在AdobeDynamic Media Classic系統中，資產檔案名稱減去副檔名會變成資產的資產ID。 因此，兩個資產不能同名。

確保貴公司的所有使用者都瞭解以下檔案命名規則: 

* 系統中不允許存在名稱完全相同的資產 ID。
* 資產ID名稱會區分大小寫。
* 最佳做法是確保資產 ID 不包含空格 (例如 black jacket.tif 和 blue jacket.jpg)。AdobeDynamic Media Classic ASCII使用資產名稱來建構URL字串時，會對資產名稱中的空白字元進行編碼。 這些 ASCII 代碼不易理解，從而使 URL 更難讀取。
* 檔名中允許使用特定語言的字元，但不允許使用下列字元:

   \ ;/ ? :@ &amp; = + $ 、 * &quot; &lt; > | &#39; { } %

   如果檔名中包含一或多個上述字元，上載時會將其從檔案名稱移除。

通常，資產檔案名稱可以與其項目編號、產品SKU或其他名稱相同，如下所示：

| 項目 | 檔案名稱 | 資產 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 檔案夾組織和結構 {#folder-organization-and-structure}

在將內容上傳至系統之前，先在Adobe Dynamic Media Classic中組織並建構內容的資料夾和子資料夾。 採用這種方式提前進行規劃主要有兩個好處:

* 透過FTP將內容上傳至AdobeDynamic Media Classic時，可以指示系統在上傳期間複製資料夾結構。 這樣，您的內容就會組織在與您電腦或網路相同的Adobe Dynamic Media Classic資料夾和子資料夾中。 (若要在Dynamic Media ClassicAdobe中複製資料夾結構，請在透過FTP上傳資產時選取「包含子資料夾」選項。)
* 與在開始就使用經過仔細計畫的檔案夾結構相比，在檔案上載之後重新對系統內的檔案夾進行組織要困難得多。

您在Dynamic Media ClassicAdobe上儲存內容時選擇的資料夾命名方法和結構，會視貴組織的需求而定。 以下是一些檔案夾結構範例:

**SKU型**  — 資料夾的名稱是根據SKU或項目編號。例如，為所有以 0、20、30 開頭的編號序列分別建立單獨的檔案夾。

**以品牌為基礎**  — 對於擁有多個品牌線的製造商和從其他公司推銷其他品牌的零售商，請將檔案分割為以不同品牌命名的產品資料夾。

**專案**  — 資料夾會根據轉出/下拉日期或專案名稱組織。主要產生 eCatalog 的客戶喜歡使用這種方法。

**網站資料夾階層的鏡像**  — 此資料夾結構會鏡像網站的資料夾結構，例如，針對產品類別，資料夾命名為。

## 關於上傳檔案 {#uploading-your-files}

您可以從桌面上載個別檔案，或是透過 FTP 上載檔案夾。如果要上傳超過100 MB的檔案或上傳整個資料夾和子資料夾，請選擇「**VIA FTP**」頁簽。

AdobeDynamic Media Classic會傳送電子郵件給您，確認上傳作業的開始和結束時間，並通知您任何問題。

在大型上傳作業期間（或緊接在之後），某些新項目可能會顯示「影像尚未最佳化」訊息。 此訊息會出現，因為檔案尚未完全處理，且已新增至AdobeDynamic Media Classic。 您可以稍後將這些檔案最佳化。請參閱[最佳化檔案](application-setup.md#optimize_files)。

### 使用「從案頭」頁簽上傳檔案 {#upload-files-using-sps-desktop-application}

AdobeDynamic Media Classic案頭應用程式可讓您透過拖曳上傳檔案和資料夾。

1. 在Adobe的Dynamic Media Classic案頭應用程式中，在全局導航欄上，選擇&#x200B;**[!UICONTROL Upload]**。
1. 在「上載」頁上，選擇「從案頭&#x200B;]**」頁簽。**[!UICONTROL 
1. 在「上載」頁的左側，在&#x200B;**[!UICONTROL 選擇要上載的檔案]**&#x200B;區域中，選擇&#x200B;**[!UICONTROL 瀏覽]**&#x200B;以選擇要上載的檔案或資料夾，然後選擇&#x200B;**[!UICONTROL 開啟]**。
1. 在「上載」頁的右側，在&#x200B;**選擇資料夾目標**&#x200B;區域中，導航到要添加上載檔案或資料夾的目標資料夾。
1. （可選）在「上傳」頁面底部的「作業名稱」文字欄位中，輸入上傳作業的新名稱。 或者，您只需使用Dynamic Media Classic提供的預設系統產生名稱即可。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （選用）如果您想要自動發佈上傳的資產，請在「上傳」頁面底部附近選取「**[!UICONTROL 上傳後發佈」。]**&#x200B;當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」對話框中也提供了相同的選項。
1. （可選）在「上傳」頁面底部附近，選擇「在任何資料夾中覆寫」（無論副檔名&#x200B;]**），如果要上傳的檔案以相同名稱取代現有檔案，請選擇相同的基本資產名稱。**[!UICONTROL 「作業選項」對話框中也提供了相同的選項。
此選項的名稱可能不同，具體取決於**[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**&#x200B;中的設定。
1. 在「上傳」頁面的右下角附近，選擇&#x200B;**[!UICONTROL 「作業選項」]**，然後指定您要的選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載作業選項」對話框中，選擇&#x200B;**[!UICONTROL Save]**。
1. 在「上傳」頁面的右下角，選取「**[!UICONTROL 提交上傳]**」。
若要查看上傳進度，請選取全域導覽列上的**[!UICONTROL 工作]**。 您可以繼續使用Adobe Dynamic Media Classic，並隨時返回「工作」頁面，以檢閱進行中的工作。 若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

### 使用「透過FTP」索引標籤上傳檔案 {#upload-files-using-via-ftp}

1. 登入您特定地區專屬的AdobeDynamic Media Classic FTP站台。 使用管理員寄給您的 FTP 使用者名稱與密碼。
1. 在AdobeDynamic Media Classic中，在全域導覽列上，選取&#x200B;**[!UICONTROL Upload]**。
1. 在「上傳」頁面上，選取&#x200B;**[!UICONTROL VIA FTP]**&#x200B;標籤。
1. 在「上傳」頁面的左側，在&#x200B;**[!UICONTROL 選擇「要上傳的FTP資料夾」區域中，選擇要從中上傳檔案的FTP資料夾。]**
1. 在「上傳」頁面的右側，在&#x200B;**[!UICONTROL 選擇AdobeDynamic Media資料夾目的地]**&#x200B;區域中，選擇AdobeDynamic Media Classic中的目的地資料夾。
1. （可選）在「上傳」頁面底部的「作業名稱」文字欄位中，輸入上傳作業的新名稱。 或者，您只需使用Dynamic Media Classic提供的預設系統產生名稱即可。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （選用）如果您想要自動發佈上傳的資產，請在「上傳」頁面底部附近選取「**[!UICONTROL 上傳後發佈」]**。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」對話框中也提供了相同的選項。
1. （可選）在「上傳」頁面底部附近，選擇「在任何資料夾中覆寫」（無論副檔名&#x200B;]**），如果要上傳的檔案以相同名稱取代現有檔案，請選擇相同的基本資產名稱。**[!UICONTROL 「作業選項」對話框中也提供了相同的選項。
此選項的名稱可能不同，具體取決於**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**&#x200B;中的設定。
1. 可選；只有在您按一下&#x200B;**[!UICONTROL VIA FTP]**&#x200B;標籤時才可用。 如果要自動從上傳的ZIP或TAR檔案中擷取所有檔案，請在「上傳」頁面底部附近選取「**[!UICONTROL 在上傳時解壓縮Zip或Tar檔案」]**。 「作業選項」對話框中也提供了相同的選項。
1. 在「上傳」頁面的右下角附近，選擇&#x200B;**[!UICONTROL 「作業選項」]**，然後指定您要的選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載作業選項」對話框中，選擇&#x200B;**[!UICONTROL Save]**。
1. 在「上傳」頁面的右下角，選取「**[!UICONTROL 提交上傳]**」。

   要查看上傳的進度，請在全局導航欄上，選擇&#x200B;**[!UICONTROL Jobs]**。 「工作」頁面隨即出現，並顯示上載的進度。您可以繼續使用Adobe Dynamic Media Classic，並隨時返回「工作」頁面，以檢閱進行中的工作。

若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

## 上載作業選項對話框 {#upload-options}

上傳檔案時，您可以在「上傳作業選項」對話方塊中選擇下列選項：

* **作業**  — 選擇 **** 作業以選擇影響整個上載作業的選項。

   您也可以使用「一般設定」中的「預設上傳選項」對話方塊，選擇&#x200B;*預設*&#x200B;選項，以上傳作業。 ****&#x200B;前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]**，然後設定您想要的預設選項。

   * **[!UICONTROL 當]**  — 只有在您選取「透過FTP」索引標籤時，才 **[!UICONTROL 能]** 使用此選項。
      * **[!UICONTROL 一次性]**  — 指定執行一次的上傳工作。選項包括：
         * **[!UICONTROL 現在]**  — 在您選取「儲存上傳工作選項」對話方塊，然後選取「上傳」頁 **** 面上的「提交上傳」後，立 **[!UICONTROL 即]** 執行上傳工作。
         * **[!UICONTROL 排程稍後]**  — 選取您要上傳工作執行的年、月、日和時間（以15分鐘為增量單位）。
      * **[!UICONTROL 循環]**  — 指定每日、每週或每月執行的上傳工作。或者，根據您自己的規格自訂上傳工作。
         * **[!UICONTROL 每日]**  — 設定您要每天執行工作的時間。如果希望作業僅在星期一到星期五運行，請選擇&#x200B;**[!UICONTROL 僅工作日]**。
         * **[!UICONTROL 每週]**  — 選擇要作業執行的一週中的特定日期和時間。
         * **[!UICONTROL 每月]**  — 選擇要工作執行的月份特定日或一週中的某天，包括開始時間。
         * **[!UICONTROL 自訂]**  — 根據您自己的規格自訂上傳或發佈工作時間間隔。請參閱[建立自訂上傳或發佈作業時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **[!UICONTROL 上傳後發佈]**  — 如果您選取「從案頭」標籤 **[!UICONTROL 或]** 「透過FTP」標 **[!UICONTROL 簽，即]** 可使用。選取此選項即可自動發佈您上載的資產。當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「上載」頁面上也有此選項。

   * **[!UICONTROL 在任何資料夾中覆寫相同的基本資產名稱（無論副檔名為何）]**  — 如果您選取「從案頭」標籤或「 **[!UICONTROL 透]** 過FTP」標籤，即 **[!UICONTROL 可]** 使用。如果您要以上載的檔案來取代現有同名檔案，請選取此選項。「上載」頁面上也有此選項。 此選項的名稱可能不同，具體取決於&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**&#x200B;中的設定。

   * **[!UICONTROL 上傳時解壓縮Zip或Tar檔案]**  — 如果您選取「從案頭」標籤 **[!UICONTROL 或]** 「透過FTP」標 **[!UICONTROL 簽，即]** 可使用。如果您想從上傳的ZIP或TAR檔案自動解壓縮所有檔案，請選取此選項。 「作業選項」對話框中也提供了相同的選項。

   * **[!UICONTROL 包含子資料夾]**  — 只有在您選取了VIA FTP索引標籤 **[!UICONTROL 時才]** 可用。如果您要一併上載檔案夾及其子檔案夾，請選取此選項。您上傳的資料夾及其子資料夾名稱會在AdobeDynamic Media Classic中自動輸入。

   * **[!UICONTROL 處理中繼資料檔案]**  — 只有在您選取「透過FTP」索引標 **[!UICONTROL 簽時]** 才可用。如果要上載 Tab 字元分隔檔案或 XML 檔案以將中繼資料增加到多個資產中，可以選取該選項。請參閱[匯入中繼資料 (透過 FTP)](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁切OPTIONS**  — 若要自動從影像裁切空白像素，請開啟「拖 **** 放」功能表、選 **[!UICONTROL 取「手動」]**，然後在「上」、「右」、「下」和「左」文字欄位中輸入像素測量，以便從側邊裁切。您也可以在「裁切」功能表中選取&#x200B;**[!UICONTROL Trim]**，然後選擇下列選項：

   * **[!UICONTROL 根據]** 修剪掉 — 選擇根據顏色或透明度裁切：
      * **[!UICONTROL 顏色]**  — 選擇顏色選項。接著選取「邊角」選單，然後選擇含有最能代表您要裁切之空白區域色彩的影像邊角。依據色彩修剪: 指定為 0 時，則僅當像素與您在影像邊角中所選取色彩完全相符時才會裁切像素。數值越接近 1，允許的色彩差異就越大。
      * **[!UICONTROL 透明度]**  — 選擇「透 **** 明度」選項。根據透明度進行修剪：指定0，只有在像素為透明時才裁切像素；接近1的數字使透明度更高。
      * **[!UICONTROL 公差]**  — 拖動滑塊以指定從0到1的公差。

* **色彩描述檔OPTIONS**  — 當您建立用於AdobeDynamic Media Classic動態傳送的最佳化檔案時，請選擇色彩轉換：

   * **[!UICONTROL 預設顏色保留]**  — 每當影像包含顏色空間資訊時，都保持源影像的顏色；沒有顏色轉換。幾乎所有影像目前都已內嵌適當的色彩設定檔。不過，如果 CMYK 來源影像沒有內嵌色彩設定檔，其色彩就會轉換為 sRGB (標準三原色) 色域。sRGB 是在網頁上顯示影像時建議使用的色域。
   * **[!UICONTROL 保留原始色域]**  — 在擷取至AdobeDynamic Media Classic時，保留原始色域而不進行任何顏色轉換。對於沒有內嵌色彩描述檔的影像，處理影像要求所需的任何色彩轉換，都是使用「發佈」設定中設定的預設色彩描述檔來完成。 這些顏色配置檔案不一定與使用此選項建立的檔案中的顏色一致。 因此，最好使用「預設色彩保存」選項。
   * **[!UICONTROL 自訂自]**  >  **[!UICONTROL 至]**  — 開啟功能表，供您選擇「轉換自」 **[!UICONTROL 和「]**  **[!UICONTROL 轉換]** 為顏色」空間。這個進階選項會覆蓋來源檔案內嵌的任何色彩資訊。只有當您提交的所有影像包含不正確或缺少顏色配置檔案資料時，才選擇此選項。

* **影像編輯選項**  — 可以保留影像 &lt;> 中的剪裁遮色片，並選擇顏色配置檔案。請參閱上傳](image-editing-options-upload.md#image-editing-options-at-upload)時的[影像微調選項。

* **PostScript®選項**  — 您可以柵格化PostScript®檔案、裁切檔案、維護透明背景、選擇解析度，以及選擇顏色空間。請參閱[使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **Photoshop選項**  — 您可以從Adobe® Photoshop®檔案建立範本、維護圖層、指定圖層的命名方式、擷取文字，以及指定影像錨記至範本的方式。請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

* **PDF選項**  — 您可以柵格化檔案、擷取搜尋字詞和連結、自動產生eCatalog、設定解析度，以及選擇顏色空間。請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

* **Illustrator選項**  — 您可以柵格化Adobe Illustrator®檔案、維護透明背景、選擇解析度，以及選擇顏色空間。請參閱[使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEO選項**  — 您可以透過選擇視訊預設集來轉換視訊檔案。請參閱[使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他中繼資料**  — 輸入描述您要上傳之檔案的關鍵字。用逗號分隔關鍵字。使用關鍵字使搜尋資產變得更容易。請參閱[執行進階搜尋](searching-assets.md#conducting_an_advanced_search)。

* **批集預設**  — 如果要從上傳的檔案建立影像集、回轉集或色票集，請為要使 **** 用的預設集選擇「活動」列。可以選取多個預設集。可以在「應用程式設定」/「批次集預設集」頁面中建立預設集。請參閱[批次集預設集](application-setup.md#batch_set_presets)。

* **進階**  — 請參 [閱使用其他工作執行上傳](uploading-files.md#follow-an-upload-with-another-job)。

## 上載後執行其他工作 {#follow-an-upload-with-another-job}

使用FTP上傳項目時，您可以排程後續工作，以在上傳完成時開始。 如果已排程其他作業開始，您在此排程的作業會排入佇列。

新工作將向您指定的位址傳送一則通知，以觸發該位置的程式碼。該後續發佈工作所使用的名稱與上載工作相同，但在開頭加有文字 *Pub_*。

**上載後執行其他工作:**

1. 選取「**[!UICONTROL 上傳]**」，然後選取「**[!UICONTROL VIA FTP]**」標籤。
1. 在「上傳」頁面的右下角，選擇「作業選項」****。
1. 在「上載作業選項」對話框中，展開&#x200B;**[!UICONTROL ADVANCED]**&#x200B;部分。
1. 從&#x200B;**[!UICONTROL 「以其他作業上傳」下拉式清單中選擇下列其中一項：]**

   * 無
   * HTTP 要求
   * 影像伺服發佈
   * 影像演算發佈
   * 視訊發佈

1. 指定 HTTP 位址。
1. 指定是否只在上傳檔案時執行。
1. 指出希望在每次完成該工作時執行要求，還是僅當檔案發佈後執行該要求。

   >[!NOTE]
   >
   >定期排程的作業有時會導致未發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產資料夾](asset-folders.md#working_with_asset_folders)
>* [處理循環上傳和發佈作業](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上傳或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

