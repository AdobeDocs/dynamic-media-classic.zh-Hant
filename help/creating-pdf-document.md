---
title: 建立 PDF 文件
seo-title: 建立 PDF 文件
description: 'null'
seo-description: 瞭解如何在Dynamic Media Classic中使用網路印刷程式建立PDF檔案。
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: 管理員
content-type: 參考
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTENDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 建立 PDF 文件 {#creating-a-pdf-document}

Web-to-Print 過程的最後一步是產生自訂的 PDF。在最終使用者使用您建立的網路應用程式建立個人化範本之後，他們便將建立最終 PDF 文件。這一最終 PDF 通常會傳送給列印服務提供商，以實現專業級的列印水準。為確保最終的 PDF 列印符合預期效果，開發人員要使用正確的工作選項檔案和設定正確的字型、印表機標記及色彩。

## 設定 PDF 預設集 {#setting-up-pdf-presets}

建立PDF工作選項檔案並上傳至Dynamic Media Classic server以指定PDF相容性層級和印表機設定。 例如，您可以選取符合 PDF/X-4 的 PDF 輸出 (建議用於 PDF 列印發佈工作流程)。您可以在創作軟體 (如 Adobe Illustrator) 或 Acrobat 中建立工作選項檔案。請務必諮詢您的印刷商，他能為您建議適合您列印工作的工作選項設定。

有關建立工作選項檔案的更多資訊以及有關在 Acrobat 中建立工作選項檔案的資訊，請參閱 Adobe Acrobat 說明。

若要在 Illustrator 中建立工作選項檔案:

1. 選擇「編輯 &gt; Adobe PDF 預設集」。
1. 在此對話框中，選取要使用的預設集。

   Dynamic Media Classic支援下列工作選項設定：

   | 工作選項 | 說明 |
   |--- |--- |
   | 一般 | <ul><li>相容性 </li><li>物件等級壓縮</li><li>內嵌縮圖</li><li>最佳化快速網頁檢視</li></ul> |
   | 影像 | <ul><li>縮減取樣</li><li>解析度</li><li>臨界值</li><li>色彩、灰階和單色壓縮</li></ul> |
   | 字型 | <ul><li>內嵌所有字型 (根據預設，內嵌字型)</li><li>內嵌 OpenType 字型</li><li>子集內嵌的字型，若使用的字元百分比低於:</li><li>永遠內嵌清單</li><li>永不內嵌清單</li></ul> |
   | 色彩 | <ul><li>色彩策略 (僅標記影像被視為標記所有內容)</li><li>文件演算色彩比對方式</li><li>4.2.5 僅支援下列工作空間。4.3 將允許您使用已上載到 IPS 的客戶提供設定檔案。</li><li>以下為解決方法之一，您可以使用公司的預設色彩設定檔，為要轉換的目標插圖指定目的地色域。</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>平面 XYZ</li><li>線性 ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8 位元</li><li>e-sYCC 8 位元</li></ul> |
   | 灰色 | <ul><li>灰階係數 1.8</li><li>灰階係數 2.2</li><li>網點增大 10%</li><li>網點增大 15%</li><li>網點增大 20%</li><li>網點增大 25%</li><li>網點增大 30%</li><li>sGray</li></ul> |
   | 保留用於校正 CMYK 色域的 CMYK 值 |  |
   | 進階 | 保留 OPI 註解始終處於開啟狀態 |
   | 標準 | 符合標準 |

   >[!NOTE]
   >
   >Dynamic Media Classic會忽略joboptions檔案中的印表機標籤設定。 而是使用Dynamic Media Classic URL命令來設定印表機標籤。

1. 按一下「匯出」，然後指定名稱和位置並按一下「儲存」。
1. 將工作選項檔案作為一項資產上載到 Scene7 Publishing System。

   在 URL 中參照該檔案，便可在您發佈的範本中使用它。例如: 

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## 準備 PDF 進行列印 {#preparing-the-pdf-for-print}

在完成 PDF 列印之前，請確定您遵循本節中的準則。

**影像**

請確定您的發佈工作中的所有影像都已上傳到您的Dynamic Media Classic Server並發佈。

**Fonts**

請確定您的發佈工作中的所有字型都已上傳至Dynamic Media Classic Server並發佈。 如果您打算允許最終使用者變更字型，請確定您具有代管這些字型的合法權限。

**影像解析度 (每英寸像素)**

點陣圖影像的解析度由Dynamic Media Classic伺服器以產生的可列印PDF格式保留。 Dynamic Media Classic會視需要調整影像解析度。 為獲得最佳效果，請在網頁上預覽時使用預設解析度值 (通常為 72 dpi)。請在「預設列印解析度」區段中的「發佈設定/影像伺服器」視窗中設定您公司的所有影像預設解析度。較高的解析度 (如 300 dpi) 可能會導致處理時間更長，僅適用於列印就緒的 PDF。使用 imageRes= URL 中的命令，以手動置換 PDF 工作的預設解析度。

**色彩管理**

您的文件和影像可以使用灰階、CMYK、已命名特別色、RGB 或 Lab 色彩模型。每一項都可透過採用 ICC 色彩設定檔來進行校色或取消校色。為獲得最佳效果，請將該設定檔內嵌至產生的列印就緒 PDF 中。Dynamic Media Classic伺服器預設會執行此動作。 請確定所有必要的色彩描述檔都已上傳至Dynamic Media Classic平台。 最好，請確定您設計應用程式中設定的色彩管理選項，與Dynamic Media Classic伺服器中設定的選項相符：

* **設計應用程式色彩管理設定:** 在您的創作應用程式 (如 Adobe Illustrator) 的「色彩設定」中，請在「工作空間」區段中指定 RGB 和 CMYK 色彩設定檔。

* **** Dynamic Media Classic色彩管理設定：通常，設計應用程式中的色彩管理設定應符合Dynamic Media Classic伺服器中的預設色彩設定檔。 您可以在「發佈設定/影像伺服器」視窗中找到這些設定。

## 顯示印表機標記 {#displaying-printer-marks}

在以下任一情形中，您可能需要建立 PDF:

* 已完成的文件
* 中間文件 (如膠片或印版)，可能會傳送給印表機進行製作

中間文件可能包含其他製作內容，如出血邊距、印表機標記等等。該內容通常顯示在已完成的頁面邊界外。

支援 Acrobat 的「增加印表機標記」畫面中所有可用的標記。印表機標記的控制參數為「`printerMark`」。The syntax is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

準備文件進行列印製作時，需要添加一些印表機標記以說明列印服務在產生樣稿時對齊分色膠片、為獲取正確校正資料和油墨密度而測量膠片、修剪膠片大小等等。印表機標記指示文件框 (如修剪框和出血框) 的邊界。與製作相關的內容可能包括:

* **介質**&#x200B;盒打印頁面的物理介質邊界。 可以安全捨棄介質框之外的內容，而不會影響檔案的內容。

* **出血**&#x200B;方塊在生產環境中輸出時，頁面內容被裁切到的區域。 出血框可能包括滿足剪切、折疊和修剪設備的實體限制所需的區域。預設值為頁面的裁切框。

* **修剪框**&#x200B;修剪完成頁面後的預定尺寸。 修剪框可能小於介質框，以便使用與製作相關的內容，如列印指示、剪切標記和色彩導表。預設值為頁面的裁切框。

* **圖稿**&#x200B;方塊頁面的有意義內容（包括潛在空白字元）的範圍，如頁面製作者所預期。 預設值為頁面的裁切框。

您可以使用下面表格所示的修飾元來複製 Adobe Illustrator、InDesign 和 Acrobat 中的印表機標記:

| 修飾元/值 | 說明 |
|--- |--- |
| bleedMargin=top,left,bottom,right | 在 Acrobat 的「設定頁面框」選項中指定。選取「出血框」，然後使用「頁面邊距控制」選項指定邊距。<br><br>值代表從插圖 (介質框) 的原始邊緣向內到上邊緣、左邊緣、下邊緣和右邊緣的距離。值(0-1000)以點為單位。<br><br>新高度=原始高度-（上+下）<br><br>新寬度=原始寬度-（左+右） |
| mediaMargin=top,left,bottom,right | 在 Acrobat 的「設定頁面框」選項中指定。在「變更頁面大小」選項下修改自訂頁面大小。<br><br>值代表從插圖 (介質框) 的原始邊緣向外到上邊緣、左邊緣、下邊緣和右邊緣的距離。值(0-1000)以點為單位。<br><br>新高度=top+bottom+原始高<br><br>度新寬度=top+bottom+原始<br><br>寬度新高度和新寬度值決定所產生PDF的新頁面大小。<br><br>定義新的介質框之後，所有修剪邊距和出血邊距計算都需要將新的介質框視為插圖的邊緣。 |
| trimMargin=top,left,bottom,right | 在 Acrobat 的「設定頁面框」選項中指定。選取「修剪框」，然後使用「頁面邊距控制」選項指定邊距。<br><br>值代表從插圖 (介質框) 的原始邊緣向內到上邊緣、左邊緣、下邊緣和右邊緣的距離。值(0-1000)以點為單位。<br><br>新高度=原始高度-（上+下）<br><br>新寬度=原始寬度-（左+右） |
| printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | 值如下：<br><br>修剪標籤= 0,1（預設值為0）<br><br>出血標籤= 0,1（預設值為0）<br><br>註冊標籤= 0,1（預設值為0）<br><br>色條= 0,1（預設值為0）<br><br>page information = 0,1（預設值為0）<br><br>style = Default, InDesignJ1, InDesignJ2, IllustratorillustratorJ, QuarkXPress（預設為Default）<br><br>line= 0.125-0.2，兩個值（預設為0.25）embed layer<br><br><br><br>1,1個新層包含所有打印機標籤（預設為1）Creating and marks and color bars apper arcrobat使用的樣式…… |

請注意以下有關印表機標記的事項:

* 指定印表機標記時，透過 URL 呼叫指定出血邊距、修剪邊距和媒體邊距。如果指定印表機標記而沒有指定這些邊距，可能會導致這些標記顯示在產生的 PDF 可見區域之外。此外，修剪標記和出血標記也會重疊。
* Specifying the same margin values for the trim margin and bleed margin results in trim marks and bleed marks overlapping when both these flags are set to 1 in `&printerMark`.
* 透過 URL 指定 fmt=swf/image 格式會導致輸出中沒有任何印表機標記或邊距，因為此功能專用於 PDF 輸出。
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. 但是，要將第 n 個元素設置為「開啟」，需要透過 URL 指定所有 (n-1) 個參數。
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* 對於多頁面 PDF，印表機標記/邊距將套用於所有頁面 (在 Acrobat 中，使用者可以為印表機標記/邊距選取頁面範圍)。
* 除非另有說明，否則在啟用印表機標記/邊距的情況下 PDF 輸出與 Acrobat X 完全相符。

如果您想透過 URL 中的 &amp;joboption 修飾元建立符合 PDF/X-4 的 PDF 檔案，您應注意 PDF ISO_15930-7-2008.pdf 中所指定與印表機標記相關的限制:

* PDF 檔案的每個頁面物件都包括一個「介質框」。符合 PDF/X-4 的檔案中每個頁面物件應該包括一個「修剪框」或一個「作品框」，但不能同時有兩個。可以透過繼承方式包括「介質框」。
* 如果存在「出血框」，則「作品框」或「修剪框」不應該超出「出血框」的邊界。如果存在「裁切框」，則「作品框」、「修剪框」或「出血框」不能超出「裁切框」的邊界。
* 「作品框」、「修剪框」、「裁切框」或「出血框」均不應超出「介質框」的邊界。
* 某些行業實務要求使用「出血框」。應該遵循相應的商業慣例。
* 與「作品框」相比，建議使用「修剪框」。
* 除補網和印表機標記附註以外的所有附註 Rect 值應該完全超出「出血框」(如果沒有「出血框」，則為「修剪框」或「作品框」) 範圍。所有印表機標記附註的 Rect 值都應該完全超出「修剪框」或「作品框」範圍。符合 PDF/X-4 的閱讀器可能會完全忽略除 PDF 補網附註之外的附註。
* 如果 Rect 的所有座標都超出了邊界框範圍或在其邊緣上，並且兩個矩形的交集為零，則應將 Rect 視為完全超出邊界框的範圍。
* 如果 ViewerPreferences 詞典包含 ViewArea、ViewClip、PrintArea 或 PrintClip 索引鍵，則其中每個索引鍵都應具有「介質框」或 (如果檔案的所有頁面物件都有「出血框」)「出血框」值。

