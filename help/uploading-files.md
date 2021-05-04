---
title: 上載檔案
description: 瞭解如何上傳檔案。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media經典，資產管理
role: Business Practitioner
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3833'
ht-degree: 37%

---

# Uploading files{#uploading-files}

在將資產檔案上傳至Dynamic Media經典之前，請確定資產檔案的命名正確，以及您的檔案夾結構是以您想要的方式設定和組織。 您可以從Dynamic MediaClassic提供的FTP網站或直接從電腦或網路上傳檔案。 Dynamic Media經典提供在上傳檔案時最佳化檔案的選項。 如果您安裝了AdobeDynamic Media經典案頭應用程式，則可以直接從案頭拖曳檔案和檔案夾，以上傳檔案和檔案夾。 請參閱[應用程式一般設定](application-setup.md#general_settings)。

## 準備要上載的資產和檔案夾 {#preparing-your-assets-and-folders-for-uploading}

在上傳資產至Dynamic Media經典之前，請確定資產的格式和大小正確。 您還必須遵守Dynamic Media經典規則來命名資產。 為檔案設定檔案夾組織和結構之前，請確定您可以輕鬆尋找和處理檔案。

### 支援的資產檔案格式 {#supported-asset-file-formats}

下表列出了Dynamic Media經典支援的資產檔案格式。 有關支援的Camera Raw檔案的資訊，請參見[https://www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en)。

| 資產檔案格式 | 說明 |
|--- |--- |
| 音效資料 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 階層式樣式表 | CSS |
| 色彩設定檔 | ICC、ICM |
| 字型 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 影像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT（僅限Windows®）、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| Dynamic Media經典影像製作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 視訊 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上載支援包含一個核取框，供您選取是否想要解壓縮檔案。

### Dynamic Media{#unsupported-image-formats-dynamic-media}中不支援的影像格式

下列清單說明在Dynamic Media支援的&#x200B;*not*&#x200B;點陣影像檔案格式的子類型。

另請參見[檢測Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)不支援的檔案格式。

* IDAT區塊大小大於100 MB的PNG檔案。
* PSB檔案。
* 不支援色域不是CMYK、RGB、灰階或點陣圖的PSD檔案。 不支援DuoTone、Lab和索引色域。
* 位元深度大於16的PSD檔案。
* 具有浮點資料的TIFF檔案。
* 具有Lab色域的TIFF檔案。

### 資產類型 {#asset-types}

若要使用Dynamic Media經典(Leassic)程式取得最佳效果，請務必使用建議的檔案格式和大小。 下表格列出了資產類型，其中一些資產類型具有常用資產的建議格式和檔案大小。

| 資產類型 | 描述/建議 |
|--- |--- |
| 音效資料 | 輸入音訊資產格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。 可以將音訊轉碼為以下格式: MP3、AAC 和 HE-AAC。 |
| 影像 (用於調整影像大小、縮放、影像集、迴轉集) | 影像最長必須至少2000像素；一般影像大小在1500到2500像素之間，最長。 建議使用不失真的影像格式，包括 TIFF 和 PNG 檔案。 如果使用 JPEG 影像，請使用最高品質的設定。動畫GIF檔案的處理方式與其他靜態內容相同。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 應用程式中建立並儲存為「印刷就緒」的高解析度 PDF 檔案。 PDF 包括所有需要的字型、影像、遮色片以及參照的圖形化元素，採用單頁、雙頁式跨頁或多頁格式。 透過按字母數字順序為檔案命名來排列頁面順序。 將 eCatalog 的所有 PDF 檔放於一個檔案夾中，以便上載。 您可以在上載時選取裁切選項，以便從 PDF 中移除修剪區域，包括裁切標記、對齊目標或色彩導表。 多數印刷就緒的 PDF 檔案採用 CMYK 色域，因此務必要獲得用於 PDF 檔案的 CMYK ICC 色彩設定檔。 |
| 範本 | 分層影像或版面設計，可以包括文字、影像和圖層。 可以將圖層、文字字串和屬性 (如色彩和大小) 參數化，從而可以自訂變數資料。 在範本中使用時的影像要求與其他影像相同。 在 Photoshop 或其他影像編輯程式中準備圖形。 採用 TIFF 或 PNG 格式將每個圖形儲存為平面化透明檔案。 確保影像解析度適合所要求的用途。 列印影像為300 ppi。 |
| 視訊 | Dynamic Media經典版支援以OGV和MP4格式儲存的視訊檔案。 您可以在上載時，將檔案轉碼為 MP4。請參閱[支援的資產檔案格式](#supported-static-file-formats)。 |
| 字型 | 已上傳TrueType、Type1（僅限Windows®）、OpenType®字型和PhotoFonts |
| 影像 | 影像和分層影像檔案。 |
| 影像集和色票集 | 可以在檢視器中顯示的一組相關影像。 |
| ICC 設定檔 | 色彩設定檔，可以用來將上載的影像從來源色域轉換為其他色域。 |
| 暈映 | 使用「影像製作」程式製作的影像，以及相關檔案。 |
| 內容檔案 | Adobe InDesign、Illustrator 或 Photoshop 內容檔案。 |
| FXG 檔案 | 與解析度無關的圖形格式檔案，可以用來建立能夠自訂的範本，以輸出進行列印、輸出到網路、電子郵件、桌面以及裝置。 |
| SVG 檔案 | 「影像伺服」伺服器可以演算的可擴放向量圖形檔案。 |
| XML 檔案 | 定義用於修改要求路徑和查詢部分之預處理規則的檔案。 |
| 階層式樣式表檔案。 | 上載用以自訂 HTML5 檢視器的 CSS 外觀。 |
| JavaScript™檔案 | JavaScript™檔案用於檢視器工具，以保存帳戶資訊。 Adobe安全性建議僅針對具有單獨網域用於傳送的客戶帳戶使用此資產類型（以避免跨網站指令碼）。 |

>[!NOTE]
>
>當您將影像檔和PDF上傳至Dynamic Media經典檔時，系統會將這些來源檔案轉換為P-TIFF(Pyramid TIFF)檔案。 這些P-TIFF是稍後發佈至Dynamic Media影像伺服器的檔案。 Dynamic Media經典影像使用Tiff檔案格式，因為它包含各種縮放比例，可在使用Dynamic Media經典影像縮放檢視器檢視時快速縮放。

### 支援的靜態檔案格式 {#supported-static-file-formats}

Dynamic Media經典檔支援數種靜態檔案格式。 靜態內容是任何「原狀」發佈的資產，例如CSS、PDF、SVG和XML。

您可以發佈下列檔案類型:

* 動畫 GIF
* 音訊檔案
* CSS
* JavaScript™（當公司設定有其專屬網域時）
* 主視訊
* PDF（當PDF在上傳後標示為要發佈時，為避免傳送所有PDF至現有的eCatalog/PDF工作流程）
* PrX 視訊
* SVG
* XML
* ZIP

Dynamic Media經典不提供產生靜態內容預覽URL的選項。

### 檔案名稱要求 {#filename-requirements}

由於在檔案上載過程中將去除檔案名中的副檔名，因此系統不允許檔案使用相同的根名稱。在Dynamic Media經典系統中，資產檔案名稱減去副檔名會變成資產的資產ID。 因此，兩個資產不能同名。

確保貴公司的所有使用者都瞭解以下檔案命名規則: 

* 系統中不允許存在名稱完全相同的資產 ID。
* 資產ID名稱會區分大小寫。
* 最佳做法是確保資產 ID 不包含空格 (例如 black jacket.tif 和 blue jacket.jpg)。Dynamic Media傳統ASCII會在使用資產名稱來建構URL字串時，在資產名稱中編碼空白字元。 這些 ASCII 代碼不易理解，從而使 URL 更難讀取。
* 檔名中允許使用特定語言的字元，但不允許使用下列字元:

   \;/ ? :@ &amp; = + $, * &quot; &lt; > | &#39; { } %

   如果檔名中包含一或多個上述字元，上載時會將其從檔案名稱移除。

通常，資產檔案名稱可以與其項目編號、產品SKU或其他名稱相同，如下所示：

| 項目 | 檔案名稱 | 資產 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 郵編896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 檔案夾組織和結構  {#folder-organization-and-structure}

在將內容上傳至系統之前，先在Dynamic Media經典中組織並建構您的內容的檔案夾和子檔案夾。 採用這種方式提前進行規劃主要有兩個好處:

* 當您透過FTP將內容上傳至Dynamic Media經典網站時，您可以告訴系統在上傳期間複製您的資料夾結構。 這樣，您的內容就會組織在您電腦或網路上的Dynamic Media經典檔案夾和子檔案夾中。 (若要複製Dynamic Media經典中的資料夾結構，請在透過FTP上傳資產時選取「包含子檔案夾」選項。)
* 與在開始就使用經過仔細計畫的檔案夾結構相比，在檔案上載之後重新對系統內的檔案夾進行組織要困難得多。

您選擇的資料夾命名方式和結構，將內容儲存在Dynamic Media經典影像上，視組織需求而定。 以下是一些檔案夾結構範例:

**SKU架構** -資料夾會根據SKU或項目編號命名。例如，為所有以 0、20、30 開頭的編號序列分別建立單獨的檔案夾。

**以品牌為基礎** -對於擁有多個品牌系列的製造商和行銷其他公司其他品牌的零售商，請將檔案分離為以不同品牌命名的產品資料夾。

**基於項目** -根據推出／放置日期或項目名稱來組織資料夾。主要產生 eCatalog 的客戶喜歡使用這種方法。

**網站資料夾階層的鏡像** -此資料夾結構會鏡像網站的資料夾結構，例如，為產品類別命名的資料夾。

## 關於上傳檔案{#uploading-your-files}

您可以從桌面上載個別檔案，或是透過 FTP 上載檔案夾。如果要上傳超過100 MB的檔案或上傳整個檔案夾和子檔案夾，請選取「VIA FTP」標籤。****

Dynamic Media·Classic會寄電子郵件給您，確認您的上傳工作何時開始和結束，並通知您任何問題。

在大型上傳工作期間（或緊接在之後），有些新項目會顯示「影像尚未最佳化」訊息。 出現此消息是因為檔案尚未完全處理並添加到Dynamic Media經典中。 您可以稍後將這些檔案最佳化。請參閱[最佳化檔案](application-setup.md#optimize_files)。

### 使用「從案頭」頁籤{#upload-files-using-sps-desktop-application}上載檔案

Dynamic Media經典案頭應用程式可讓您透過拖曳來上傳檔案和資料夾。

1. 在「Dynamic Media經典台式機」應用程式的全局導航欄上，按一下&#x200B;**[!UICONTROL Upload]**。
1. 在「上傳」頁面上，按一下「從Desktop ]**」標籤。**[!UICONTROL 
1. 在「上載」頁的左側，在&#x200B;**[!UICONTROL 選擇要上載的檔案]**&#x200B;區域中，按一下&#x200B;**[!UICONTROL 瀏覽]**&#x200B;以選擇要上載的檔案或資料夾，然後按一下&#x200B;**[!UICONTROL 開啟]**。
1. 在「上載」頁的右側，在&#x200B;**選擇資料夾目標**&#x200B;區域中，導航到要添加已上載檔案或資料夾的目標資料夾。
1. （可選）在「上傳」頁面底部附近的&#x200B;**[!UICONTROL 「作業名稱]**」欄位中，指定上傳作業的新名稱。 或者，您只需使用Dynamic Media經典提供的預設系統產生名稱即可。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （可選）如果您要自動發佈您上傳的資產，請在「上傳」頁面底部附近選取「上傳後發佈」。
****&#x200B;當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」(Job Options)對話框中也提供了相同的選項。
1. （可選）在「上傳」頁面底部附近，如果您希望上傳的檔案以相同的名稱取代現有檔案，請選取「覆寫任何資料夾中相同的基本資產名稱」，不論副檔名&#x200B;]**。**[!UICONTROL 「作業選項」(Job Options)對話框中也提供了相同的選項。
此選項的名稱可能不同，具體取決於**應用程式設定>一般設定>上傳至應用程式>覆寫影像**&#x200B;中的設定。
1. 在「上傳」頁面的右下角附近，按一下「工作選項」，然後指定您想要的選項。****

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話框中，按一下「**[!UICONTROL 儲存]**」。
1. 在「上傳」頁面的右下角，按一下「提交上傳」。
****&#x200B;若要查看上載進度，按一下全域導覽列中的「**[!UICONTROL 工作]**」。您可以繼續在Dynamic Media經典中工作，並隨時返回「作業」頁面以查看進行中的作業。 若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

### 使用VIA FTP標籤{#upload-files-using-via-ftp}上傳檔案

1. 登入您特定地區專屬的Dynamic Media經典FTP網站。 使用管理員寄給您的 FTP 使用者名稱與密碼。
1. 在「Dynamic Media經典」的全域導覽列上，按一下「上傳」****。
1. 在「上傳」頁面上，按一下「VIA FTP ]**」標籤。**[!UICONTROL 
1. 在「上傳」頁面的左側，在&#x200B;**[!UICONTROL 選擇「FTP資料夾以進行上傳」區域中，選擇要從中上傳檔案的FTP資料夾。]**
1. 在「上傳」頁面的右側，在&#x200B;**[!UICONTROL 選擇「AdobeDynamic Media資料夾目標」區域，選擇「Dynamic Media經典」中的目標資料夾。]**
1. （可選）在「上傳」頁面底部附近的&#x200B;**[!UICONTROL 「作業名稱]**」欄位中，指定上傳作業的新名稱。 或者，您只需使用Dynamic Media經典提供的預設系統產生名稱即可。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （選擇性）如果您要自動發佈您上傳的資產，請在「上傳」頁面底部附近選取「上傳後發佈」。
****&#x200B;當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」(Job Options)對話框中也提供了相同的選項。
1. （可選）在「上傳」頁面底部附近，如果您希望上傳的檔案以相同的名稱取代現有檔案，請選取「覆寫任何資料夾中相同的基本資產名稱」，不論副檔名&#x200B;]**。**[!UICONTROL 「作業選項」(Job Options)對話框中也提供了相同的選項。
此選項的名稱可能不同，具體取決於「設定」>「應用程式設定」>「常規設定」>「上傳到應用程式」]**>「覆蓋影像」>「覆蓋影像」>中的設定。**************[!UICONTROL ****
1. 可選；僅當您按一下&#x200B;**[!UICONTROL VIA FTP]**&#x200B;頁籤時可用。 如果您想要自動從已上載的ZIP或TAR檔案解壓縮所有檔案，請在「上載」頁面底部附近選取「上載時解壓縮Zip或Tar檔案」。 ****「作業選項」(Job Options)對話框中也提供了相同的選項。
1. 在「上傳」頁面的右下角附近，按一下「工作選項」，然後指定您想要的選項。****

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話框中，按一下「**[!UICONTROL 儲存]**」。
1. 在「上傳」頁面的右下角，按一下「提交上傳」。****

   若要查看上載進度，請按一下全域導覽列中的「**[!UICONTROL 工作]**」。「工作」頁面隨即出現，並顯示上載的進度。您可以繼續在Dynamic Media經典中工作，並隨時返回「作業」頁面以查看進行中的作業。

若要取消進行中的上載工作，請按一下「持續時間」旁邊的「**[!UICONTROL 取消]**」。

## 「上載作業選項」對話框{#upload-options}

上傳檔案時，您可以在「上傳工作選項」對話方塊中選擇下列選項：

* **JOB** -按一下 **** JOB以選擇影響整個上載作業的選項。

   您也可以使用「一般設定」中的「預設上傳選項」對話方塊，為上傳工作選擇&#x200B;*default*&#x200B;選項。 ****&#x200B;按一下「**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 預設上傳選項]**」，然後設定您想要的預設選項。

   * **When**  —— 此選項僅在您選取「 **[!UICONTROL VIA]** FTP」標籤時才可用。
      * **一次性** -指定執行一次的上傳工作。選項包括：
         * **現在** -在您按一下「儲存上傳工作選項」對話方塊後，立即執行上傳工作，然後按一下「上 **** 傳 **** 」頁面上的「送出上傳」。
         * **排程稍後** -選取您要執行上傳工作的年、月、日和時間（以15分鐘為增量單位）。
      * **循環** -指定每日、每週或每月執行的上傳工作。或者，自訂上傳工作以符合您自己的規格。
         * **每日** -設定您希望工作每天執行的時間。如果希望作業僅在星期一到星期五運行，請選擇&#x200B;**[!UICONTROL 僅工作日]**。
         * **Weekly**  —— 選擇您希望工作執行的特定一週中的某天和時間。
         * **每月** -選擇要執行工作的特定月份或一週中的某天，包括開始時間。
         * **自訂** -自訂上傳或發佈工作時間間隔至您自己的規格。請參閱[建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **上傳後發佈** -如果您選取「 **[!UICONTROL FROM]** DESKTOP」標籤或「 **[!UICONTROL VIA]** FTP」標籤，則可用。選取此選項即可自動發佈您上載的資產。當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「上載」頁面上也有此選項。

   * **在任何資料夾中覆寫相同的基本資產名稱(不論副檔名為何** )-如果您選取「 **[!UICONTROL FROM]** DESKTOP」標籤或「 **[!UICONTROL VIA]** FTP」標籤，即可使用。如果您要以上載的檔案來取代現有同名檔案，請選取此選項。「上載」頁面上也有此選項。 此選項的名稱可能不同，具體取決於「設定」>「應用程式設定」>「常規設定」>「上傳到應用程式」]**>「覆蓋影像」>「覆蓋影像」>中的設定。**************[!UICONTROL ****

   * **上傳時解壓縮Zip或Tar檔案** -如果您選取「 **[!UICONTROL FROM]** DESKTOP」標籤或「 **[!UICONTROL VIA]** FTP」標籤，則可用。如果您想要自動從已上載的ZIP或TAR檔案解壓縮所有檔案，請選取此選項。 「作業選項」(Job Options)對話框中也提供了相同的選項。

   * **包含子檔案夾** -僅在您選取「VIA  **** FTP」索引標籤時可用。如果您要一併上載檔案夾及其子檔案夾，請選取此選項。您上傳的檔案夾及其子檔案夾名稱會自動在Dynamic Media經典中輸入。

   * **處理中繼資料檔案** -僅在您選取「VIA  **** FTP」標籤時可用。如果要上載 Tab 字元分隔檔案或 XML 檔案以將中繼資料增加到多個資產中，可以選取該選項。請參閱[匯入中繼資料 (透過 FTP)](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁切OPTIONS** -若要自動裁切影像的空白像素，請開啟 **** Cropmenu，按一下「手動」 ****，然後在「頂端」、「右側」、「底部」和「左側」文字欄位中輸入像素測量值，以便從兩側裁切。您也可以按一下「裁切」功能表上的「修剪」，然後選擇下列選項：****

   * **根據修剪** -選擇是根據顏色還是透明度裁切：
      * **顏色** -選擇顏色選項。接著選取「邊角」選單，然後選擇含有最能代表您要裁切之空白區域色彩的影像邊角。依據色彩修剪: 指定為 0 時，則僅當像素與您在影像邊角中所選取色彩完全相符時才會裁切像素。數值越接近 1，允許的色彩差異就越大。
      * **透明度** -選擇「透明 **** 度」選項。根據透明度進行修剪：指定0，僅在像素為透明時才裁切像素；接近1的數字使得透明度更高。
      * **公差** -拖動滑塊以指定從0到1的公差。

* **色彩描述檔OPTIONS** -當您建立用於Dynamic Media傳統動態傳送的最佳化檔案時，請選擇色彩轉換：

   * **預設色彩保留** -當影像包含色域資訊時，就會保留原始影像色彩；沒有顏色轉換。幾乎所有影像目前都已內嵌適當的色彩設定檔。不過，如果 CMYK 來源影像沒有內嵌色彩設定檔，其色彩就會轉換為 sRGB (標準三原色) 色域。sRGB 是在網頁上顯示影像時建議使用的色域。
   * **保留原始色域** -保留原始色域，在擷取至Dynamic Media經典影像時不進行任何色彩轉換。對於沒有內嵌色彩描述檔的影像，處理影像要求的任何必要色彩轉換都會使用「發佈」設定中設定的預設色彩描述檔來完成。 這些顏色描述檔不一定會與使用此選項建立的檔案中的顏色對齊。 因此，最好使用「預設色彩保存」選項。
   * **「自訂自」>「至** 」-開啟功能表，讓您選擇「轉換 **[!UICONTROL 自]** 訂」 **[!UICONTROL 和「轉]** 換至顏色」空格。這個進階選項會覆蓋來源檔案內嵌的任何色彩資訊。只有在您要送出的所有影像包含不正確或遺失色彩描述檔資料時，才選取此選項。

* **影像編輯OPTIONS** -您可以保留影像 &lt;> 中的剪裁遮色片，並選擇色彩描述檔。請參閱[上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)。

* **PostScript®OPTIONS** -您可以點陣化PostScript®檔案、裁切檔案、維持透明背景、選擇解析度，以及選擇色域。請參閱[使用 PostScript 和 Illustrator 檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **PhotoshopOPTIONS** -您可以從Adobe®Photoshop®檔案建立範本、維護圖層、指定圖層的命名方式、擷取文字，以及指定影像錨定至範本的方式。請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

* **PDFOPTIONS** -您可以點陣化檔案、擷取搜尋字詞和連結、自動產生eCatalog、設定解析度，以及選擇色域。請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

* **IllustratorOPTIONS** -您可以點陣化Adobe Illustrator®檔案、維持透明背景、選擇解析度，以及選擇色域。請參閱[使用 PostScript 和 Illustrator 檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEOOPTIONS** -您可以選擇「視訊預設集」來轉換視訊檔案。請參閱[使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他中繼資料** -輸入描述您要上傳之檔案的關鍵字。用逗號分隔關鍵字。使用關鍵字使搜尋資產變得更容易。請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

* **批集預設集** -如果要從已上載的檔案中建立影像集、多軸回轉集或色票集，請按一下要使用的預設集的「活動」列。可以選取多個預設集。可以在「應用程式設定」/「批次集預設集」頁面中建立預設集。請參閱[批次集預設集](application-setup.md#batch_set_presets)。

* **進階** -請參 [閱使用其他工作追蹤上傳](uploading-files.md#follow-an-upload-with-another-job)。

## 上載後執行其他工作 {#follow-an-upload-with-another-job}

當您使用FTP上傳項目時，可以排程後續工作，以在上傳完成時開始。 如果已排程其他作業開始，則您在此安排的作業會排入佇列。

新工作將向您指定的位址傳送一則通知，以觸發該位置的程式碼。該後續發佈工作所使用的名稱與上載工作相同，但在開頭加有文字 *Pub_*。

**上載後執行其他工作:**

1. 按一下「上傳&#x200B;****」，然後按一下「VIA FTP ]**」標籤。**[!UICONTROL 
1. 在「上傳」頁面的右下角，按一下「工作選項」。****
1. 在「上載作業選項」對話框中，展開&#x200B;**[!UICONTROL ADVANCED]**&#x200B;部分。
1. 從&#x200B;**[!UICONTROL Follow Upload with ather job]**&#x200B;下拉式清單中選擇下列任一項：

   * 無
   * HTTP 要求
   * 影像伺服發佈
   * 影像演算發佈
   * 視訊發佈

1. 指定 HTTP 位址。
1. 指定您是否只想在檔案上傳時執行。
1. 指出希望在每次完成該工作時執行要求，還是僅當檔案發佈後執行該要求。

   >[!NOTE]
   >
   >定期排程的工作有時不會發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產檔案夾](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

