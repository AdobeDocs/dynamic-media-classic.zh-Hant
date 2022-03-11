---
title: 上載檔案
description: 瞭解如何在Adobe Dynamic Media Classic上傳檔案。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: ec1a981dd5cfa92ce4ae8e2676dd131d1509216f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 上載檔案{#uploading-files}

在將資產檔案上載到Adobe Dynamic Media Classic之前，請確保資產檔案的命名正確，並且資料夾結構已按您需要的方式設定和組織。 您可以從Adobe Dynamic Media Classic提供的FTP站點或直接從電腦或網路上載檔案。 Adobe Dynamic Media Classic提供了在您上傳檔案時優化檔案的選項。 如果安裝了Adobe Dynamic Media Classic案頭應用程式，則可以通過直接從案頭拖動檔案和資料夾來上載它們。 請參閱[應用程式一般設定](application-setup.md#general_settings)。

## 準備資產和資料夾以便上載 {#preparing-your-assets-and-folders-for-uploading}

在將資產上載到Adobe Dynamic Media Classic之前，請確保其格式和大小正確。 您還必須遵守Adobe Dynamic Media Classic的資產命名規則。 為檔案設定檔案夾組織和結構之前，請確定您可以輕鬆尋找和處理檔案。

### 支援的資產檔案格式 {#supported-asset-file-formats}

此表列出了Adobe Dynamic Media Classic支援的資產檔案格式。 有關支援的Camera Raw檔案的資訊，請參見 [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html)。

| 資產檔案格式 | 說明 |
| --- | --- |
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
| Adobe Dynamic Media Classic影像創作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | 塔爾 |
| 視訊 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上載支援包含一個核取框，供您選取是否想要解壓縮檔案。

### Dynamic Media不支援的影像格式 {#unsupported-image-formats-dynamic-media}

以下清單描述了以下柵格影像檔案格式的子類型： *不* 在Dynamic Media。

另請參閱 [檢測不支援的Dynamic Media檔案格式](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)。

* IDAT區塊大小大於100 MB的PNG檔案。
* PSB檔案。
* 不支援具有非CMYK、RGB、灰度或點陣圖的色彩空間的PSD檔案。 不支援DuoTone、Lab和索引顏色空間。
* PSD深度大於16的檔案。
* TIFF具有浮點資料的檔案。
* TIFF具有實驗室顏色空間的檔案。

### 資產類型 {#asset-types}

要使用Adobe Dynamic Media Classic程式獲得最佳結果，請確保使用推薦的檔案格式和大小。 下表格列出了資產類型，其中一些資產類型具有常用資產的建議格式和檔案大小。

| 資產類型 | 描述/建議 |
| --- | --- |
| 音效資料 | 輸入音訊資產格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。 可以將音訊轉碼為以下格式: MP3、AAC 和 HE-AAC。 |
| 影像 (用於調整影像大小、縮放、影像集、迴轉集) | 影像的長度至少要達到2000像素；典型影像大小在1500到2500像素之間，最長大小。 建議使用不失真的影像格式，包括 TIFF 和 PNG 檔案。 如果使用 JPEG 影像，請使用最高品質的設定。動畫GIF檔案與其他靜態內容一樣處理。 |
| eCatalog | 使用在Adobe Acrobat建立的高解析度PDF檔案或保存為「Press-ready」的AdobeCreative Suite應用程式。 PDF 包括所有需要的字型、影像、遮色片以及參照的圖形化元素，採用單頁、雙頁式跨頁或多頁格式。 透過按字母數字順序為檔案命名來排列頁面順序。 將 eCatalog 的所有 PDF 檔放於一個檔案夾中，以便上載。 您可以在上載時選取裁切選項，以便從 PDF 中移除修剪區域，包括裁切標記、對齊目標或色彩導表。 多數印刷就緒的 PDF 檔案採用 CMYK 色域，因此務必要獲得用於 PDF 檔案的 CMYK ICC 色彩設定檔。 |
| 範本 | 分層影像或版面設計，可以包括文字、影像和圖層。 可以將圖層、文字字串和屬性 (如色彩和大小) 參數化，從而可以自訂變數資料。 在範本中使用時的影像要求與其他影像相同。 在 Photoshop 或其他影像編輯程式中準備圖形。 採用 TIFF 或 PNG 格式將每個圖形儲存為平面化透明檔案。 確保影像解析度適合所要求的用途。 打印影像為300 ppi。 |
| 視訊 | Adobe Dynamic Media Classic支援以OGV和MP4格式保存的視頻檔案。 您可以在上載時，將檔案轉碼為 MP4。請參閱[支援的資產檔案格式](#supported-static-file-formats)。 |
| 字型 | 已上載TrueType、Type1（僅Windows®）、OpenType®字型和PhotoFonts。 |
| 影像 | 影像和分層影像檔案。 |
| 影像集和色票集 | 可以在檢視器中顯示的一組相關影像。 |
| ICC 設定檔 | 色彩設定檔，可以用來將上載的影像從來源色域轉換為其他色域。 |
| 暈映 | 使用「影像創作」程式創作的影像和相關檔案。 |
| 內容檔案 | Adobe InDesign、Illustrator 或 Photoshop 內容檔案。 |
| FXG 檔案 | 與解析度無關的圖形格式檔案，可以用來建立能夠自訂的範本，以輸出進行列印、輸出到網路、電子郵件、桌面以及裝置。 |
| SVG 檔案 | 「影像伺服」伺服器可以演算的可擴放向量圖形檔案。 |
| XML 檔案 | 定義用於修改要求路徑和查詢部分之預處理規則的檔案。 |
| 階層式樣式表檔案。 | 上載用以自訂 HTML5 檢視器的 CSS 外觀。 |
| JavaScript 檔案 | JavaScript檔案用於查看器檢測以保存帳戶資訊。 Adobe安全性建議僅對具有單獨域以供交付的客戶端帳戶使用此資產類型（以避免跨站點指令碼）。 |

>[!NOTE]
>
>將影像檔案和PDF上載到Adobe Dynamic Media Classic時，系統會將這些源檔案轉換為PTIFF(金字塔TIFF)檔案。 這些PTIFF是稍後發佈到Dynamic Media映像伺服器的檔案。 Adobe Dynamic Media Classic使用Pyramid Tiff檔案格式，因為它包含各種縮放比率，當使用Adobe Dynamic Media Classic縮放查看器查看時，這些比率允許快速縮放。

### 支援的靜態檔案格式 {#supported-static-file-formats}

Adobe Dynamic Media Classic支援多種靜態檔案格式。 靜態內容是「原樣」發佈的任何資產，如CSS、PDF、SVG和XML。

您可以發佈下列檔案類型:

* 動畫 GIF
* 音訊檔案
* CSS
* JavaScript (當公司設定了自己的網域時)
* 主視訊
* PDF(當PDF標籤為在上載後發佈時，為現有的eCatalog/PDF工作流避免傳遞所有PDF)
* PrX 視訊
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic不提供生成靜態內容預覽URL的選項。

### 檔案名稱要求 {#filename-requirements}

由於在檔案上載過程中將去除檔案名中的副檔名，因此系統不允許檔案使用相同的根名稱。在Adobe Dynamic Media Classic系統中，資產檔案名減去檔案副檔名後將成為資產的資產ID。 因此，兩個資產不能同名。

確保貴公司的所有使用者都瞭解以下檔案命名規則: 

* 系統中不允許存在名稱完全相同的資產 ID。
* 資產ID名稱區分大小寫。
* 最佳做法是確保資產 ID 不包含空格 (例如 black jacket.tif 和 blue jacket.jpg)。Adobe Dynamic Media ClassicASCII在使用資產名稱構造URL字串時，對資產名稱中的空格進行編碼。 這些 ASCII 代碼不易理解，從而使 URL 更難讀取。
* 檔名中允許使用特定語言的字元，但不允許使用下列字元:

   \;/? :@ &amp; = + $, * &quot; &lt; > | &#39; { } %

   如果檔名中包含一或多個上述字元，上載時會將其從檔案名稱移除。

通常，資產檔案名可以與其項目號、產品SKU或其他名稱相同，如下所述：

| 項目 | 檔案名稱 | 資產 ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 檔案夾組織和結構 {#folder-organization-and-structure}

在將內容上傳到系統之前，為您在Adobe Dynamic Media Classic的內容整理和構建資料夾和子資料夾。 採用這種方式提前進行規劃主要有兩個好處:

* 通過FTP將內容上載到Adobe Dynamic Media Classic時，可以告訴系統在上載期間複製資料夾結構。 這樣，您的內容與您的電腦或網路上的內容在Adobe Dynamic Media Classic的相同資料夾和子資料夾中組織。 (要在Adobe Dynamic Media Classic複製資料夾結構，請在通過FTP上載資產時選擇「包括子資料夾」選項。)
* 與在開始就使用經過仔細計畫的檔案夾結構相比，在檔案上載之後重新對系統內的檔案夾進行組織要困難得多。

您選擇在Adobe Dynamic Media Classic上儲存內容的資料夾命名方法和結構取決於您組織的需求。 以下是一些檔案夾結構範例:

**基於SKU**  — 根據SKU或物料編號命名資料夾。 例如，為所有以 0、20、30 開頭的編號序列分別建立單獨的檔案夾。

**基於品牌**  — 對於具有多個品牌系列的製造商和銷售其他公司其他品牌的零售商，將檔案分離到以不同品牌命名的產品資料夾中。

**基於項目**  — 資料夾按部署/刪除日期或項目名稱進行組織。 主要產生 eCatalog 的客戶喜歡使用這種方法。

**網站資料夾層次結構的鏡像**  — 此資料夾結構鏡像網站的資料夾結構，例如，為產品類別命名的資料夾。

## 關於上載檔案 {#uploading-your-files}

您可以從桌面上載個別檔案，或是透過 FTP 上載檔案夾。如果要上載超過100 MB的檔案或上載整個資料夾和子資料夾，請選擇 **通過FTP** 頁籤。

Adobe Dynamic Media Classic會向您發送一封電子郵件，確認上載作業何時開始和結束，並通知您任何問題。

在大型上載作業期間（或緊接著），某些新項目可能會顯示「影像尚未優化」消息。 出現此消息是因為檔案尚未完全處理並添加到Adobe Dynamic Media Classic。 您可以稍後將這些檔案最佳化。請參閱 [優化檔案](application-setup.md#optimize_files)。

### 使用「從案頭」頁籤上載檔案 {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic案頭應用程式允許您通過拖動來上載檔案和資料夾。

1. 在Adobe Dynamic Media Classic案頭應用程式的全局導航欄上，選擇 **[!UICONTROL 上載]**。
1. 在「上載」(Upload)頁面上，選擇 **[!UICONTROL 從案頭]** 頁籤。
1. 在上載頁面的左側， **[!UICONTROL 選擇要上載的檔案]** ，選擇 **[!UICONTROL 瀏覽]** 選擇要上載的檔案或資料夾，然後選擇 **[!UICONTROL 開啟]**。
1. 在上載頁面的右側， **選擇資料夾目標** 區域，導航到要添加上載的檔案或資料夾的目標資料夾。
1. （可選）在「上載」頁底部的「作業名稱」文本欄位中，輸入上載作業的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統生成的名稱。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （可選）在「上載」頁面底部附近，選擇 **[!UICONTROL 上載後發佈]** 的子菜單。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」(Job Options)對話框中也提供了此選項。
1. （可選）在「上載」頁面底部附近，選擇 **[!UICONTROL 在任意資料夾中覆蓋相同的基本資產名稱，而不考慮副檔名]** ，也請參見Wiki頁。 「作業選項」(Job Options)對話框中也提供了此選項。
此選項的名稱可能不同，具體取決於 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]** > **[!UICONTROL 上載到應用程式]** > **[!UICONTROL 覆蓋影像]**。
1. 在「上載」頁的右下角附近，選擇 **[!UICONTROL 作業選項]**，然後指定所需選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載作業選項」對話框中，選擇 **[!UICONTROL 保存]**。
1. 在上載頁面的右下角，選擇 **[!UICONTROL 提交上載]**。
要查看上載進度，請選擇 **[!UICONTROL 作業]** 的上界。 您可以繼續在Adobe Dynamic Media Classic工作，並隨時返回「作業」頁面以複查正在進行的作業。 若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

### 使用VIA FTP頁籤上載檔案 {#upload-files-using-via-ftp}

1. 登錄到特定區域的Adobe Dynamic Media ClassicFTP站點。 使用管理員寄給您的 FTP 使用者名稱與密碼。
1. 在Adobe Dynamic Media Classic的「全局導航」欄上，選擇 **[!UICONTROL 上載]**。
1. 在「上載」(Upload)頁面上，選擇 **[!UICONTROL 通過FTP]** 頁籤。
1. 在上載頁面的左側， **[!UICONTROL 選擇要上載的FTP資料夾]** 的子菜單。
1. 在上載頁面的右側， **[!UICONTROL 選擇AdobeDynamic Media資料夾目標]** 的子菜單。
1. （可選）在「上載」頁底部的「作業名稱」文本欄位中，輸入上載作業的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統生成的名稱。 工作和其他的上載及發佈工作會記錄於「工作」頁面中，您可以從中檢查工作的狀態。請參閱[檢查工作檔案](checking-job-files.md#checking_job_files)。
1. （可選）在「上載」頁面底部附近，選擇 **[!UICONTROL 上載後發佈]** 的子菜單。
當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「作業選項」(Job Options)對話框中也提供了此選項。
1. （可選）在「上載」頁面底部附近，選擇 **[!UICONTROL 在任意資料夾中覆蓋相同的基本資產名稱，而不考慮副檔名]** ，也請參見Wiki頁。 「作業選項」(Job Options)對話框中也提供了此選項。
此選項的名稱可能不同，具體取決於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]** > **[!UICONTROL 上載到應用程式]** > **[!UICONTROL 覆蓋影像]**。
1. 可選；僅在您按一下 **[!UICONTROL 通過FTP]** 頁籤。 在「上載」頁面底部附近，選擇 **[!UICONTROL 上傳時解壓縮ZIP或Tar檔案]** ，也請參見Wiki頁。 「作業選項」(Job Options)對話框中也提供了此選項。
1. 在「上載」頁的右下角附近，選擇 **[!UICONTROL 作業選項]**，然後指定所需選項。

   參閱[上載選項](uploading-files.md#upload_options)。

1. 在「上載作業選項」對話框中，選擇 **[!UICONTROL 保存]**。
1. 在上載頁面的右下角，選擇 **[!UICONTROL 提交上載]**。

   要查看上載的進度，請在全局導航欄上，選擇 **[!UICONTROL 作業]**。 「工作」頁面隨即出現，並顯示上載的進度。您可以繼續在Adobe Dynamic Media Classic工作，並隨時返回「作業」頁面以複查正在進行的作業。

若要取消進行中的上載工作，請選取「持續時間」旁邊的「**[!UICONTROL 取消]**」按鈕。

## 「上載作業選項」對話框 {#upload-options}

上載檔案時，可以從「上載作業選項」對話框中的以下選項中進行選擇：

* **作業**  — 選擇 **[!UICONTROL 作業]** 選擇影響整個上載作業的選項。

   您也可以選擇 *預設* 用於使用 **[!UICONTROL 預設上載選項]** 對話框。 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]** > **[!UICONTROL 預設上載選項]**，然後設定所需的預設選項。

   * **[!UICONTROL 當]**  — 此選項僅在您選擇了 **[!UICONTROL 通過FTP]** 頁籤。
      * **[!UICONTROL 一次性]**  — 指定運行一次的上載作業。 選項包括：
         * **[!UICONTROL 現在]**  — 選擇後立即運行上載作業 **[!UICONTROL 保存]** 在「上載作業選項」對話框中，選擇 **[!UICONTROL 提交上載]** 上載頁面。
         * **[!UICONTROL 計畫以後]**  — 選擇要運行上載作業的年、月、日和時間（以15分鐘為增量）。
      * **[!UICONTROL 循環]**  — 指定每天、每週或每月運行的上載作業。 或者，根據您自己的規範自定義上載作業。
         * **[!UICONTROL 每日]**  — 設定希望作業每天運行的時間。 如果希望作業僅在星期一到星期五運行，請選擇 **[!UICONTROL 僅工作日]**。
         * **[!UICONTROL 每週]**  — 選擇要運行作業的一週中的特定日期和時間。
         * **[!UICONTROL 每月]**  — 選擇要運行作業的月份或星期的特定日期，包括開始時間。
         * **[!UICONTROL 自定義]**  — 根據您自己的規範自定義上載或發佈作業時間間隔。 請參閱 [建立自定義上載或發佈作業時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **[!UICONTROL 上載後發佈]**  — 如果選擇了 **[!UICONTROL 從案頭]** 頁籤 **[!UICONTROL 通過FTP]** 頁籤。 選取此選項即可自動發佈您上載的資產。當您發佈檔案時，檔案就會傳送至即時伺服器。然後即可在外部網站和應用程式中使用這些檔案的 URL。「上載」頁面上也有此選項。

   * **[!UICONTROL 在任意資料夾中覆蓋相同的基本資產名稱，而不考慮副檔名]**  — 如果選擇了 **[!UICONTROL 從案頭]** 頁籤 **[!UICONTROL 通過FTP]** 頁籤。 如果您要以上載的檔案來取代現有同名檔案，請選取此選項。「上載」頁面上也有此選項。 此選項的名稱可能不同，具體取決於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]** > **[!UICONTROL 上載到應用程式]** > **[!UICONTROL 覆蓋影像]**。

   * **[!UICONTROL 上傳時解壓縮ZIP或Tar檔案]**  — 如果選擇了 **[!UICONTROL 從案頭]** 頁籤 **[!UICONTROL 通過FTP]** 頁籤。
如果要自動從上載的ZIP或TAR檔案中提取所有檔案，請選擇此選項。 「作業選項」(Job Options)對話框中也提供了此選項。

   * **[!UICONTROL 包括子資料夾]**  — 僅當您選擇了 **[!UICONTROL 通過FTP]** 頁籤。
如果您要一併上載檔案夾及其子檔案夾，請選取此選項。您上傳的資料夾及其子資料夾的名稱將自動輸入到Adobe Dynamic Media Classic。

   * **[!UICONTROL 處理元資料檔案]**  — 僅當您選擇了 **[!UICONTROL 通過FTP]** 頁籤。 如果要上載 Tab 字元分隔檔案或 XML 檔案以將中繼資料增加到多個資產中，可以選取該選項。請參閱[匯入中繼資料 (透過 FTP)](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁剪選項**  — 要自動從影像中裁剪空格像素，請開啟 **[!UICONTROL 裁剪]** 菜單，選擇 **[!UICONTROL 手動]**，並在「頂部」、「右側」、「底部」和「左側」文本欄位中輸入像素測量值以從側面裁剪。 也可以選擇 **[!UICONTROL 修剪]** 在「裁剪」菜單上，選擇以下選項：

   * **[!UICONTROL 基於]**  — 選擇是根據顏色還是透明度裁剪：
      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 接著選取「邊角」選單，然後選擇含有最能代表您要裁切之空白區域色彩的影像邊角。依據色彩修剪: 指定為 0 時，則僅當像素與您在影像邊角中所選取色彩完全相符時才會裁切像素。數值越接近 1，允許的色彩差異就越大。
      * **[!UICONTROL 透明度]**  — 選擇 **[!UICONTROL 透明度]** 的雙曲餘切值。
基於透明度的修剪：指定0，僅當像素為透明時才裁剪像素；接近1的數字允許更透明。
      * **[!UICONTROL 容差]**  — 拖動滑塊以指定0到1的公差。

* **顏色配置檔案選項**  — 在建立用於Adobe Dynamic Media Classic動態傳遞的優化檔案時，選擇顏色轉換：

   * **[!UICONTROL 預設顏色保留]**  — 當影像包含顏色空間資訊時，維護源影像顏色；沒有顏色轉換。 幾乎所有影像目前都已內嵌適當的色彩設定檔。不過，如果 CMYK 來源影像沒有內嵌色彩設定檔，其色彩就會轉換為 sRGB (標準三原色) 色域。sRGB 是在網頁上顯示影像時建議使用的色域。
   * **[!UICONTROL 保留原始顏色空間]**  — 保留原始顏色，在將顏色攝取到Adobe Dynamic Media Classic時不進行任何顏色轉換。 對於沒有嵌入顏色配置檔案的影像，處理影像請求所需的任何顏色轉換都使用在「發佈」設定中配置的預設顏色配置檔案來完成。 這些顏色配置檔案並不總是與使用此選項建立的檔案中的顏色對齊。 因此，最好使用「預設色彩保存」選項。
   * **[!UICONTROL 自定義自]** > **[!UICONTROL 至]**  — 開啟菜單，以便您 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 顏色空間。 這個進階選項會覆蓋來源檔案內嵌的任何色彩資訊。僅當您提交的所有影像包含不正確或缺少顏色配置檔案資料時，才選擇此選項。

* **影像編輯選項**  — 可以保留影像中的剪貼&lt;>蒙版，並選擇顏色配置檔案。
請參閱 [上載時的影像微調選項](image-editing-options-upload.md#image-editing-options-at-upload)。

* **PostScript®選項**  — 您可以柵格化PostScript®檔案、裁剪檔案、維護透明背景、選擇解析度和選擇顏色空間。
請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **Photoshop選項**  — 您可以從Adobe®Photoshop®檔案建立模板，維護圖層，指定圖層的命名方式，提取文本，並指定如何將影像定位到模板中。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

* **PDF選項**  — 您可以柵格化檔案、提取搜索詞和連結、自動生成eCatalog、設定解析度並選擇顏色空間。
請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

* **Illustrator選項**  — 您可以柵格化Adobe Illustrator®檔案、維護透明背景、選擇解析度和選擇顏色空間。
請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEO選項**  — 通過選擇「視頻預設」，可以對視頻檔案進行代碼轉換。
請參閱 [使用視頻編碼預設](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他元資料**  — 輸入描述要上載的檔案的關鍵字。 用逗號分隔關鍵字。使用關鍵字使搜尋資產變得更容易。請參閱 [執行高級搜索](searching-assets.md#conducting_an_advanced_search)。 另請參閱 [上載關鍵字](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) 培訓視頻。

* **批集預設**  — 如果要從上載的檔案建立影像集、旋轉集或色板集，請選擇 **[!UICONTROL 活動]** 列中的值。 可以選取多個預設集。可以在「應用程式設定」/「批次集預設集」頁面中建立預設集。請參閱[批次集預設集](application-setup.md#batch_set_presets)。

* **高級**  — 請參閱 [使用其他作業執行上載](uploading-files.md#follow-an-upload-with-another-job)。

## 上載後執行其他工作 {#follow-an-upload-with-another-job}

使用FTP上載項目時，可以安排後續作業在上載完成後開始。 如果其他作業已計劃開始，則您在此安排的作業將在它們之後排隊。

新工作將向您指定的位址傳送一則通知，以觸發該位置的程式碼。該後續發佈工作所使用的名稱與上載工作相同，但在開頭加有文字 *Pub_*。

**上載後執行其他工作:**

1. 選擇 **[!UICONTROL 上載]**，然後選擇 **[!UICONTROL 通過FTP]** 頁籤。
1. 在上載頁面的右下角，選擇 **[!UICONTROL 作業選項]**。
1. 在「上載作業選項」對話框中，展開 **[!UICONTROL 高級]** 的子菜單。
1. 從中選擇以下選項之一 **[!UICONTROL 使用其他作業執行上載操作]** 下拉清單：

   * 無
   * HTTP 要求
   * 影像伺服發佈
   * 影像演算發佈
   * 視訊發佈

1. 指定 HTTP 位址。
1. 指定是否僅在上載檔案時運行。
1. 指出希望在每次完成該工作時執行要求，還是僅當檔案發佈後執行該要求。

   >[!NOTE]
   >
   >定期安排的作業有時會導致不發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產資料夾](asset-folders.md#working_with_asset_folders)
>* [處理定期上載和發佈作業](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [將上載或發佈作業用作觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

