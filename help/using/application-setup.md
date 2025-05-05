---
title: 應用程式設定
description: 瞭解如何設定Adobe Dynamic Media Classic的應用程式區域。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10945'
ht-degree: 30%

---

# 應用程式設定{#application-setup}

您可以使用「應用程式設定」頁面來輸入「一般設定」、建立影像預設集、視訊編碼預設集、檢視器預設集，或定義預設檢視器和中繼資料。 您可以設定批次集預設集，讓批次集預設集自動產生2D迴轉集（例如）、發佈設定和視訊SEO設定。

>[!NOTE]
>
>只有Adobe Dynamic Media Classic管理員可以在應用程式設定中變更設定。

## 一般設定 {#general-settings}

若要開啟[應用程式一般設定]頁面，請在全域導覽列上，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**。

### 伺服器

建立帳戶時，Adobe Dynamic Media Classic會自動提供指派給貴公司的伺服器。 這些伺服器可用來建構您網站和應用程式的URL字串。 這些 URL 呼叫皆專屬於您的帳戶。

另請參閱[測試Secure Testing服務](testing-assets-making-them-public.md#testing_the_secure_testing_service)。

* **[!UICONTROL 已發佈的伺服器名稱]**：此伺服器是所有系統產生、特定於您帳戶的URL呼叫中所使用的即時CDN （內容傳遞網路）伺服器。 只有在Adobe Dynamic Media Classic支援技術人員指示您變更此伺服器名稱時，才能進行變更。

* **[!UICONTROL 原始伺服器名稱]**：此伺服器僅用於品質保證測試。 只有在Adobe Dynamic Media Classic支援技術人員指示您變更此伺服器名稱時，才能進行變更。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target伺服器名稱]**： Test&amp;Target URL，包括`.com`。 如需取得此URL的說明，請參閱整合[!DNL Adobe Dynamic Media Classic]與[!DNL Adobe Target Standard/Premium]。

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS串流伺服器名稱]**： [!DNL Adobe Dynamic Media Classic] iOS串流伺服器的URL。 此伺服器會使用HTTP通訊協定，將串流視訊傳送至iOS裝置。

* **[!UICONTROL 漸進式視訊伺服器名稱]**： [!DNL Adobe Dynamic Media Classic]漸進式視訊伺服器的URL。 此伺服器使用HTTP通訊協定來傳送漸進式視訊。

* **[!UICONTROL 顯示未發佈資產的URL]**：如果您希望[!DNL Adobe Dynamic Media Classic]在您預覽任何已發佈或未發佈的資產時顯示URL，請選取此選項。 如果資產尚未發佈，URL 將無法運作。不過，您可以使用 URL 來進行規劃或組織。

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN失效範本]**：指定用於使CDN （內容傳遞網路）快取失效的範本。

  例如，假設您輸入參照`<ID>`的影像URL （包括影像預設集或修飾元），而不是如以下範例所示輸入特定的影像ID：

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  如果範本只包含`<ID>`，則Adobe Dynamic Media Classic會填入`https://<server>/is/image`，其中`<server>`是在「一般設定」中定義的發佈伺服器名稱。

  設定CDN無效範本，選取名為Backpack_B的影像，然後前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 無效CDN]**&#x200B;會在CDN無效介面中產生下列已產生的URL：

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  在URL清單方塊中，選取&#x200B;**[!UICONTROL 繼續]**&#x200B;以清除該特定影像URL呼叫的快取。 您也可以輸入URL或將其貼到URL清單方塊中來新增URL；您不需要事先設定範本。

  選取CDN失效範本並提出CDN失效請求後，使用者介面中會彈出一個指示器。 它可讓您估計清除快取所需的時間。

  當您按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 使CDN失效]**」時，如果在Dynamic Media Classic中選取了多個影像，則儲存的範本URL會參照每個影像。 因此，您可以定義CDN無效範本，以參考網站上參考的每個URL （例如產品詳細資料和搜尋結果）。 然後，當您從快取中選取一或影像以進行失效時，URL會自動填入介面。

  請參閱[內容快取](dmc-platform-overview.md#content_caching)。

  請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 瀏覽

* **[!UICONTROL 顯示專案]**：判斷是否有專案可用來組織您的Adobe Dynamic Media Classic資產。 請參閱[組織您的專案工作](/help/using/organizing-projects.md)。

* **[!UICONTROL 顯示範例eVideo內容]**：開啟或關閉eVideo範例內容的顯示。

* **[!UICONTROL 顯示產生的內容]**：在資料夾中，它顯示從資產產生的內容。 例如，當PDF檔案在上傳時點陣化時，Adobe Dynamic Media Classic會為原始PDF中的每個頁面建立一個影像。 如果選取了「顯示產生的內容」 ，則上傳原始PDF時產生的每個影像都會顯示。 它會與PDF一起出現在將PDF上傳到的資料夾中。

* **[!UICONTROL 顯示編碼的視訊]**：預設為取消選取（關閉）。

  您可以在Adobe Dynamic Media Classic中快速搜尋和瀏覽影片，而無需瀏覽相同影片的大量已編碼衍生影片。 保留取消選取此選項（預設）。 只會顯示主要視訊縮圖（您上傳並用來建立衍生影片的來源視訊）和「上層」最適化視訊集縮圖（包含已編碼視訊集的「下層」衍生影片）。

  不過，您仍然可以從主要視訊或最適化視訊集中存取個別編碼視訊。 若要執行此項操作，請按兩下視訊縮圖影像，以開啟「詳細檢視」。然後在右側面板中選取&#x200B;**[!UICONTROL 編碼的視訊]**，讓您能夠存取所有「子」視訊。

  您也可以前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]**，直接從最適化視訊集建立更多編碼的「子」視訊。 Adobe Dynamic Media Classic會自動找到最適化視訊集的「父」主視訊，並將其作為轉碼的源視訊。 不過，在您儲存新的個別編碼的視訊後，搜尋或瀏覽時並不會看到這些視訊。然而這些視訊仍可從「詳細檢視」的「編碼的視訊」標籤予以存取。

  請參閱[上傳及轉碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

  若要繼續能夠在搜尋和瀏覽時存取所有編碼視訊的衍生物，請選取「**[!UICONTROL 顯示編碼的視訊]**」。

  「建置」選單上的某些動作只能用於個別視訊，或選擇性地用於個別視訊。此功能迫使您必須顯示所有可以選取之編碼視訊的衍生物，而不受您設定「**[!UICONTROL 顯示編碼的視訊]**」的方式影響。覆寫&#x200B;**[!UICONTROL Show Encoded Video]**&#x200B;設定的組建動作包含&#x200B;**[!UICONTROL 最適化視訊集]**&#x200B;和&#x200B;**[!UICONTROL eCatalogs]**。

  >[!NOTE]
  >
  >如果您未使用Adobe Dynamic Media Classic上傳及編碼視訊資產，即使取消選取此選項，Adobe Dynamic Media Classic也會顯示所有個別編碼的視訊。

* **[!UICONTROL 顯示[重新整理子資料夾]按鈕]**：開啟或關閉子資料夾[重新整理]按鈕的顯示。

### Adobe Dynamic Media Classic FTP帳戶

* **[!UICONTROL 伺服器]**：列出您的FTP帳戶伺服器。

* **[!UICONTROL 使用者名稱]**：列出您的FTP帳戶使用者名稱。

### 上載至應用程式

另請參閱上傳工作的[選項](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS)訓練影片。

* **[!UICONTROL 覆寫影像]**： Adobe Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個專案的Adobe Dynamic Media Classic ID （影像名稱減去副檔名）必須是唯一的。 因為此規則，所以「上載」對話框擁有「覆寫」選項。此選項的確實效果取決於指定的「覆寫影像」選項。這些選項會指定取代影像的上載方式: 取代原始影像或成為重複影像。重複的影像會以「–1」重新命名（例如chair.tif會重新命名為chair-1.tif）。 這些選項會影響上載至非原始檔案夾的影像，或擁有非原始副檔名 (例如 JPG、TIF 或 PNG) 的影像。請參閱[使用覆寫影像選項](#using-the-overwrite-images-option)。

   * **[!UICONTROL 在目前檔案夾中有相同的基本影像名稱或副檔名時覆寫]**：此選項是最嚴格的取代規則。 它會要求您將取代影像上載至與原始影像相同的檔案夾，且取代影像必須與原始檔案擁有相同的副檔名。如果未符合這些要求，便會建立重複項目。

   * **[!UICONTROL 在目前資料夾中覆寫相同的基本資產名稱（無論副檔名為何）]**：需要您將取代影像上傳到與原始影像相同的資料夾，但副檔名可能與原始影像不同。 例如，chair.tif 會取代 chair.jpg。

   * **[!UICONTROL 在任何資料夾、相同的基本資產名稱或副檔名中覆寫]**：取代影像的副檔名必須與原始影像相同。 例如，chair.jpg必須取代chair.jpg，而非chair.tif)。 然而，您可以將取代影像上載至與原始影像不同的檔案夾。上載的影像將會位於新檔案夾中；無法再於原始位置中找到該檔案

   * **[!UICONTROL 在任何資料夾中覆寫相同的基本資產名稱（無論副檔名為何）]**：此選項是最具包容性的取代規則。 您可以將取代影像上載至非原始檔案夾、上載擁有不同副檔名的檔案，以及取代原始檔案。如果原始檔案位於不同檔案夾，則取代影像會位於其上載的新目標檔案夾中。

* **[!UICONTROL 保留Publish]**：指定上傳至Adobe Dynamic Media Classic的取代影像是否保留其取代影像的「準備就緒Publish」設定。 或者，在上傳時指定設定。

* **[!UICONTROL 預設色彩設定檔]**：指定新增CMYK影像時套用為預設色彩設定檔選項一部分的色彩設定檔。

* **[!UICONTROL 預設上載選項]**：開啟[上載工作選項]對話方塊，您可以在此指定預設上載選項。 如需有關這些選項的詳細資訊，請參閱[上載選項](/help/using/uploading-files.md#upload_options)。

### 影像地圖編輯器（至應用程式）

* **[!UICONTROL 預設影像對應HREF]**：定義影像對應中HREF欄使用的預設URL。 此URL是您在建立影像地圖時看到的預設URL。

* **[!UICONTROL 預設影像對應範本]**：為影像對應中的HREF範本定義預設JavaScript。 您可以在此處設定自訂程式碼，以便在選取「影像地圖」時執行。

### 其他設定（至應用程式）

* **[!UICONTROL 垃圾桶清理警告]**：垃圾桶中的Assets會在七天內自動移除。 選取「自動刪除垃圾桶專案之前先傳送電子郵件」，以便在垃圾桶中的資產距離永久刪除日期四天後通知公司管理員。 請參閱[管理垃圾桶](/help/using/trash-folder.md)。

## 使用「覆寫影像」選項 {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個專案的Adobe Dynamic Media Classic ID （影像名稱減去副檔名）必須是唯一的。 因為此規則，所以「上載」對話框包含「覆寫影像」選項。此選項的確切效果取決於每個公司的「Adobe Dynamic Media Classic內部設定」設定。

如果您先前已上傳影像，然後變更原始檔案（或取代原始檔案），則所選的「覆寫」選項會指定Adobe Dynamic Media Classic取代影像的方式。 影像的任何相關資訊都不會變更，但新的影像會取代舊影像。如果資料夾中同時包含Adobe Dynamic Media Classic中尚未包含的影像，則會新增這些影像。

如果上傳的影像以某種方式變更（影像已變更），但影像的參照保持不變，請使用此選項。 上傳和擷取Adobe®PDF時，覆寫也相當實用。 您可以微調Adobe Dynamic Media Classic *擷取*&#x200B;影像的方式。 您也可以在「上傳」對話方塊中調整ICC色彩設定檔選項，並使用覆寫功能重新上傳。

用來從生產伺服器存取影像的Adobe Dynamic Media Classic ID衍生自影像檔案名稱。 在檔案名稱中使用大寫和小寫字元是很重要的，這無論是在取代現有檔案還是用於存取影像的Adobe Dynamic Media Classic ID中。 在上傳至Adobe Dynamic Media Classic之前，使用包含大寫和小寫字元的檔案名稱是正確之舉，可避免Adobe Dynamic Media Classic ID只有針對相同影像才會有差異。

如果取消選取此選項，所有與現存影像擁有相同檔案名稱的影像都會視為重複項目，而不會增加。

## 影像預設集 {#image-presets}

「影像預設集」畫面是用來建立和編輯影像預設集。影像預設集可讓Adobe Dynamic Media Classic以動態方式，從相同的主要影像傳送不同大小的影像。 每個影像預設集都代表了一個用來顯示影像之大小調整與格式命令的預先定義集合。建立影像預設集時，您可以選取影像傳送的大小。 您也可以選取格式化指令，以便在傳送影像供檢視時最佳化影像外觀。

管理員可以建立匯出資產用的預設集。使用者可以在匯出影像時選擇預設集，這樣也會將影像重新格式化為管理員指定的規格。

若要開啟「影像預設集」畫面，請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**。

請參閱[智慧型影像處理](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq)。

### 建立和編輯影像預設集 {#creating-and-editing-image-presets}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**。
1. 建立預設集或從現有預設集開始：

   * **建立影像預設集**：選取&#x200B;**[!UICONTROL 新增]**。
   * **從現有的預設集建立影像預設集**：選取最像您要建立的影像預設集，然後選取&#x200B;**[!UICONTROL 編輯]**。

1. 在「新增（或編輯）預設集」頁面上，輸入預設集名稱。
1. 設定您想要的預設集選項。

   請參閱[影像預設集選項](application-setup.md#image_preset_options)。

1. 選取「**[!UICONTROL 儲存]**」，或者，如果您是從現有的預設集開始，請選取「**[!UICONTROL 另存新檔]**」。
1. 若要使用您自己的影像預覽預設集，請選取&#x200B;**[!UICONTROL 瀏覽]**，然後選取影像。 若要以預設影像預覽，請選取&#x200B;**[!UICONTROL 重設]**。

您可以編輯影像預設集，方法是在「影像預設集」畫面上選取其名稱，然後選取&#x200B;**[!UICONTROL 編輯]**。 若要刪除影像預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL 刪除]**。

### 影像預設集選項 {#image-preset-options}

「增加預設集」和「編輯預設集」畫面提供下列選項，以建立和編輯影像預設集:

* **[!UICONTROL 預設集名稱]**：請輸入不含空格的描述性名稱。 為協助使用者識別此影像預設集，請在名稱中包含影像大小規格。

* **[!UICONTROL 寬度和高度]**：輸入遞送影像的畫素大小。

* **[!UICONTROL 格式]**：從功能表選取格式。 選擇GIF、JPEG、PDF或TIFF格式會提供更多選項：

   * GIF 色彩量化選項

      * **[!UICONTROL 型別]**：選取最適化（預設）、Web或Mac。 如果您選取&#x200B;**[!UICONTROL Alpha為]**&#x200B;的GIF，則Mac選項無法使用。

      * **[!UICONTROL 遞色]**：選取「擴散」或「關閉」。

      * **[!UICONTROL 色彩數目]**：拖曳滑桿以輸入2-255。

      * **[!UICONTROL 色彩清單]**：請輸入逗號分隔的清單。 例如，對於白色、灰色和黑色，請輸入`000000,888888,ffffff`。

   * JPEG 選項

      * **[!UICONTROL 品質]**：控制JPEG壓縮等級。 這個設定會同時影響檔案大小與影像品質。JPEG 品質範圍為 1 – 100。

      * **[!UICONTROL 啟用JPG色度縮減取樣]**：因為眼睛對高頻色彩資訊的敏感性低於高頻明度，所以JPEG影像會將影像資訊分成明度和色彩元件。 壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣將資料量減少一半或三分之一，幾乎不影響感知品質。 縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。

   * PDF 和 TIFF 選項

      * **[!UICONTROL 壓縮]**：選取壓縮演演算法。

* **[!UICONTROL 色域]**：選取色域。

* **[!UICONTROL 銳利化]**：選取「啟用簡單銳利化」選項，可在所有縮放完成後將基本銳利化濾鏡套用至影像。 銳利化可以幫助補償以不同大小顯示影像時所造成的模糊現象。

  如需銳利化、重新取樣模式和遮色片銳利化的詳細資訊，請參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。 另請觀看[銳利化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS)訓練影片。

* **[!UICONTROL 重新取樣模式]**：選取重新取樣模式選項。 下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL B線性]**：最快速的重新取樣方法；會產生某些明顯的鋸齒狀不自然感。

* **[!UICONTROL 雙立方式]**：增加影像伺服器的CPU使用量，但會產生較清晰的影像，且鋸齒狀不自然感比較不明顯。

* **[!UICONTROL `Sharp 2`]**：產生的結果可能會比「雙立方式」選項稍微銳利，但影像伺服器的CPU成本更高。

* **[!UICONTROL 三線性式]**：同時使用較高和較低解析度（如果有的話）；建議只在出現鋸齒問題時才使用。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

* **[!UICONTROL 不銳利化遮色片]**：選擇下列選項以微調銳利化：

* **[!UICONTROL 數量]**：控制套用至邊緣畫素的對比數量。 預設是 1.0。對於高解析度的影像，您最多可以將它增加至 5.0。將「數量」視為濾鏡飽和度的度量。

* **[!UICONTROL 半徑]**：決定邊緣畫素周圍影響銳利化的畫素數量。 對於高解析度的影像，請輸入 1 到 2 的數字。低數值只會銳利化邊緣的像素；高數值會銳利化較寬的像素範圍。正確的值取決於影像大小。

* **[!UICONTROL 臨界值]**：決定套用遮色片銳利化調整濾鏡時要忽略的對比範圍。 也就是說，它可以協助解決銳化畫素與周圍區域必須有多大的差異，才會被視為邊緣畫素並加以銳化。 為避免產生雜訊，請使用介於`.02`到`0.2`之間的值來實驗。 預設值6會銳利化影像中的所有畫素。

* **[!UICONTROL 色域]**：決定影像是使用建立影像的空間，通常是RGB（原始）還是亮度空間（強度）。

* **[!UICONTROL 色彩]**&#x200B;選擇下列選項：

* **[!UICONTROL 輸出色彩設定檔]**：選取&#x200B;**[!UICONTROL 使用預設值]**&#x200B;或Adobe Dynamic Media Classic上可用的其中一個ICC色彩設定檔。

  請另參閱 [ICC 設定檔](icc-profiles.md#icc_profiles)。

* **[!UICONTROL 色彩演算比對方式]**：如果要覆寫色彩設定檔的預設色彩演算比對方式，請選取選項。 當其中一個預設ICC設定檔是色彩轉換的目標色域時，請使用此選項。 或者，此描述檔會描述輸出裝置（印表機或熒幕），而且指定的演算色彩比對方式對此描述檔有效。

* **[!UICONTROL 內嵌設定檔]**：選取此選項，以便當您在Adobe® Photoshop®中開啟此影像時，它會使用此設定檔。

* **[!UICONTROL 列印解析度]**：選取列印此影像的解析度；預設為72畫素。

* **[!UICONTROL URL修飾元]**：如果您偏好指定定義影像預設集的URL修飾元，而非設定，請在此輸入修飾元。

* **[!UICONTROL 範例影像URL]**：列出Dynamic Media影像伺服器用來傳送含有您新增或編輯之影像預設集之影像的「原始」URL字串。 此URL字串會編碼您在「新增預設集」或「編輯預設集」畫面中選取的所有格式設定。

### 編輯、移除或停用影像預設集 {#editing-removing-or-deactivating-an-image-preset}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**。
1. 在「影像預設集」畫面中，選取表格中的預設集，然後執行以下一項操作:

   * 選取&#x200B;**[!UICONTROL 編輯]**，然後在[編輯預設集]對話方塊中指定新選項。
   * 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以從清單中移除預設集。
   * 如果您要從MediaPortal使用者的整個Adobe Dynamic Media Classic使用者介面中移除預設集名稱，請取消選取預設集名稱旁的&#x200B;**[!UICONTROL 作用中]**&#x200B;核取方塊。

## 啟用或停用最適化視訊預設集 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic提供最適化視訊編碼預設集。 這是將16:9最適化視訊預設集和4:3最適化視訊預設集合併為一個群組的主要預設集清單。 這些預先定義的預設集反映了最常見的編碼設定，並已針對目標行動裝置、平板電腦和桌上型電腦的播放進行最佳化。

依預設，僅會啟用「最適化視訊」編碼預設集（啟用或「開啟」）。 您可以視需要加以停用。非作用中的最適化視訊預設集，並不會以可選取的選項顯示在「上載工作選項」對話框的「eVideo」區段中。

請參閱[上傳及編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

另請參閱[視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)訓練視訊。

**若要啟用或停用最適化視訊預設集：**

1. 在Adobe Dynamic Media Classic的右上角附近，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 最適化視訊預設集]**。
1. 在「最適化視訊預設集」頁面上，取消選取預設集名稱旁邊的核取方框，以從「上載工作選項」對話框的「eVideo 選項」清單中移除預設集。
1. 選取&#x200B;**[!UICONTROL 關閉]**。

## 編碼視訊檔案的視訊預設集 {#video-presets-for-encoding-video-files}

若要選取編碼預設集，請在[上傳]頁面的右下角選取&#x200B;**[!UICONTROL 工作選項]**。 在「上載工作選項」對話方塊中，展開「eVideo選項」並選取您想要的「視訊編碼預設集」。

>[!NOTE]
>
>除了預設啟用的「最適化視訊」之外，您無法在上傳工作選項對話方塊中看到所有其他最適化視訊或單一視訊編碼預設集。 Adobe Dynamic Media Classic管理員會決定哪些視訊編碼預設集會顯示在「上傳工作選項」對話方塊中。

* 從下列最適化視訊編碼或單一編碼預設集中選取：

   * **[!UICONTROL 16:9最適化視訊]**：建立16:9畫面寬高比視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   * **[!UICONTROL 4:3最適化視訊]**：建立4:3外觀比例視訊，以遞送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，以最符合檢視者連線速度的解析度和位元速率最佳化。

   * **[!UICONTROL 最適化視訊]**：單一編碼預設集，可與任何外觀比例搭配使用，建立視訊以傳送至行動裝置、平板電腦和案頭。 使用此預設集編碼而上載的來源視訊，會設定成固定的高度。不過，寬度會自動調整比例，以保留視訊的外觀比例。

     當您建立自己的自訂視訊編碼預設集時，也可預設使用「自動縮放」的彈性。

     請參閱[新增或編輯視訊編碼預設集](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)。

   * **[!UICONTROL 最適化視訊編碼（16:9或4:3）]**：建立16:9和4:3外觀比例視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)。 以最符合檢視器連線速度的解析度和位元速率最佳化。

     請參閱[最適化視訊編碼 (16:9 或 4:3) 視訊預設集](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   * **[!UICONTROL 單一編碼預設集]**

     >[!NOTE]
     >
     >若要將視訊傳送至iPad，您可以選取行動編碼預設集或平板電腦編碼預設集。 平板電腦預設集專為 iPad 而設計，通常具有更高的解析度和品質，以充分利用更大的畫面和頻寬連線。傳送使用平板電腦預設集編碼的視訊檔案時，必須在您的行動裝置網站或應用程式上加入裝置偵測程式碼。此程式碼會根據播放裝置的不同，在 iPhone 或 iPad 視訊體驗間切換。更簡單的工作流程是選擇行動裝置預設集將視訊檔案傳送到 iPad。原因在於您可以將同一視訊檔案用於 iPhone 和 iPad。但是，將品質標準化為解析度更低的 iPhone 體驗。

      * 在「編碼預設集」群組的「排序編碼預設集」下拉式清單中，選取「名稱」或「大小」，依名稱或解析度大小排序預設集。
      * 根據您計畫播放視訊的解析度大小和頻寬，選取編碼預設集。
      * 您可以選取「自我調整視訊編碼」，以及每個視訊的一或多個編碼預設集。 例如，您可以在一個上載工作中針對桌面和行動裝置編碼檔案。

選取&#x200B;**[!UICONTROL 開始上傳]**&#x200B;後，就會上傳原始主要視訊檔案，並從主要檔案產生編碼檔案。

### 關於編碼預設集選項 {#about-encoding-preset-options}

編碼預設集選項的參數如下:

* **[!UICONTROL 目標連線速度]**：目標一般使用者的網際網路連線速度。

* **[!UICONTROL 編碼檔案字尾]**：附加至編碼視訊檔案的字尾，用於識別。

* **[!UICONTROL 視訊位元速率（資料速率）]**：經過編碼以構成一秒的視訊播放的資料量（以每秒千位元為單位）。

* **[!UICONTROL 畫素寬度/高度]**：熒幕影像的寬度維度（以畫素為單位）；熒幕影像的高度維度（以畫素為單位）。

* **[!UICONTROL 每秒影格數(fps)]**：視訊的每秒影格數（或靜止影像）。 在美國和日本，大部分視訊以 29.97 fps 拍攝；在歐洲和亞洲 (不包括日本)，大部分視訊以 25 fps 拍攝。電影的拍攝速度為24 fps。

* **[!UICONTROL 音訊位元速率]**：經過編碼以構成音訊播放一秒的資料量（以每秒千位元為單位）。

下表說明在選取視訊預設集及用來指定編碼檔案的命名慣例時建議的最佳實踐。

### 最適化視訊 (預設) {#adaptive-video-default}

編碼預設集，可與任何外觀比例搭配使用，以讓您為傳遞至行動裝置、平板電腦和桌上型電腦建立視訊。使用此預設集編碼的上傳來源視訊（預設和最佳實務）會設為固定高度，而寬度會自動調整以保留視訊的外觀比例。

**最適化視訊（預設）**

|  | 編碼預設集名稱/工具提示文字 | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | FPS | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 自動× 360， 800 Kbps | _行動_自動×360p_800K | 800 | Auto×360 | 與來源同 | 64 | 適用於行動裝置(iPhone、iPad、Android™) |
| 2 | 自動× 480， 1400 Kbps | _平板電腦_自動×480p_1400K | 1400 | Auto×480 | 與來源同 | 96 | 適用於平板電腦(iPad、Android™) |
| 3 | 自動× 720， 2600 Kbps | _案頭_自動×720p_2600K | 2600 | Auto×720 | 與來源同 | 128 | 適用於案頭 |

### 自我調整視訊編碼（16:9或4:3）預設集 {#adaptive-video-encoding-or-video-presets}

這些最適化視訊編碼預設集會結合一系列個別編碼預設集，這些預設集是根據您上傳的視訊外觀比例自動為您選取。 例如，如果您上傳4:3視訊，則會使用&#x200B;**最適化視訊編碼（16:9或4:3）**&#x200B;選項中主要預設集清單內找到的所有五個4:3預設集，自動對其進行編碼。

有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**最適化視訊編碼（16:9或4:3）預設集**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | FPS | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | Medium解析度，3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | 與來源同 | 64 | Medium解析度，3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | 與來源同 | 80 | Medium解析度，WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | 與來源同 | 80 | Medium解析度，WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | 與來源同 | 96 | 高解析度、WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 與來源同 | 96 | 高解析度、WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | 與來源同 | 128 | 高畫質 |

### 桌上型電腦視訊編碼預設集 {#desktop-video-encoding-presets}

桌上型電腦之 MP4 與 OGV 的視訊編碼預設集。

如需有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**H264主要3.2：音訊AAC、MP4副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | FPS | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9、640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9、800x450 (1200 Kbps) | 1.5 Mbps | _800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9、1280x720 (2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4:3、320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4:3、480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4:3、640x480 (1200 Kbps) | 1.5 Mbps | _640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4:3、1280x960 (2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000 | 1280x960 | 與來源同 | 128 | 高畫質 |

**OGG Theora Vorbis： OGV副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | FPS | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps)、OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9， 640x360 (800 Kbps)，OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9， 800x450 (1200 Kbps)，OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9， 1280x720 (2000 Kbps)，OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4：3,320x240 (400 Kbps)，OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4：3,480x360 (800 Kbps)，OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4：3,640x480 (1200 Kbps)，OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4：3,1280x960 (2000 Kbps)，OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | 與來源同 | 128 | 高畫質 |

### 行動裝置視訊編碼預設集 {#mobile-video-encoding-presets}

與來源 fps 相同。iPhone、iPad和Android™行動裝置的視訊編碼預設集。

如需有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**H264基準2.1：音訊AAC，MP4副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊位元速率 (Kbps) | 像素寬度/高度 | FPS | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、512x288、行動裝置 (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | 16:9、512x288、行動裝置 (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | Medium解析度，3G |
| 3 | 16:9、512x288、行動裝置 (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 4 | 16:9、512x288、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 5 | 16:9、512x288、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | 與來源同 | 96 | 高解析度、Wi-Fi |
| 6 | 4:3、384x288、行動裝置 (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 7 | 4:3、384x288、行動裝置 (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | 與來源同 | 64 | Medium解析度，3G |
| 8 | 4:3、448x336、行動裝置 (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 9 | 4:3、448x336、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 10 | 4:3、448x336、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | 與來源同 | 96 | 高解析度、Wi-Fi |

## 檢視器預設集 {#viewer-presets}

>[!NOTE]
>
>**Flash檢視器生命週期結束通知**：自2017年1月31日起，Adobe Dynamic Media Classic正式終止支援Flash檢視器平台。

*檢視器預設集*&#x200B;是決定使用者如何在電腦螢幕和行動裝置上檢視多媒體資產的設定集合。身為一名管理員，您可以建立檢視器預設集。設定可用於檢視器設定選項的陣列。例如，您可以變更檢視器顯示大小、縮放行為、色彩方案、邊框和字型。

最佳實務是使用Adobe Dynamic Media Classic HTML5視訊檢視器。 HTML5視訊檢視器中使用的預設集是強大的視訊播放器。

將下列專案結合至單一播放器：

* 能夠使用HTML5和CSS設計播放元件。
* 具有內嵌式播放。
* 根據瀏覽器的功能使用最適化和漸進式串流。

您可以將多媒體內容的觸角伸展至桌上型電腦、平板電腦和行動使用者，並確保提供簡化的視訊體驗。

請參閱HTML檢視器參考指南中的[關於Adobe5檢視器](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)。

請參閱[Adobe Dynamic Media Classic檢視器預設集相容性對照表](application-setup.md#scene7_viewer_preset_compatibility_matrix)。

請參閱[最佳實踐: 使用 HTML5 視訊檢視器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

依據檢視器而定，您可以增加社群功能。社群功能包含「內嵌」按鈕、「電子郵件」按鈕、「連結」按鈕和「造訪網站」按鈕。這些按鈕可讓使用檢視器的人與其他人共用檢視器，或開啟Adobe Dynamic Media Classic網站。

另請參閱[Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

### 檢視器支援回應式設計的網頁 {#viewer-support-for-responsive-designed-web-pages}

不同的網頁有不同的需求。 有時候，您會想要一個提供連結的網頁，該連結會在個別的瀏覽器視窗中開啟HTML5檢視器。 在其他情況下，必須直接將HTML5檢視器內嵌在託管頁面上。 在後一種情況下，網頁可能會有靜態配置。 或是「回應式」功能，且在不同裝置或不同瀏覽器視窗大小中顯示的方式有所不同。 為因應這些需求，Adobe Dynamic Media Classic隨附的HTML5檢視器同時支援靜態網頁和回應式設計的網頁。

有關如何將回應式檢視器內嵌到網頁上的詳細資訊，請參閱[關於回應式影像庫](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api)、[使用回應式影像庫](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api)和[命令參考：命令屬性](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library)。

### 檢視器預設集類型 {#viewer-preset-types}

管理員可以建立和自訂以下類型的檢視器預設集:

* **[!UICONTROL eCatalog檢視器]**：模擬讀取列印目錄的體驗。 您可以在不同頁面間移動、放大和縮小頁面上的專案、使用影像地圖來檢視頁面上專案的詳細資訊，或搜尋目錄。 如果對應區域具有有效的rollover_key屬性，您也可以包含「資訊」面板來顯示詳細資訊和影像對應專案。 若要包含「資訊」面板，請在「eCatalog檢視器預設集」視窗的「資訊」面板「設定」面板中指定「資訊伺服器URL」。

* **[!UICONTROL 色票集檢視器]**：以不同的色彩、材質、紋理、表面處理或織物顯示影像。 使用者可選取縮圖以檢視影像中的變化。

* **[!UICONTROL 混合媒體集檢視器]**：在一個檢視器中顯示不同型別的媒體。 您可以加入色票集、迴轉集、影像和視訊。您可以設定標籤以包含不同型別的內容，例如影像集的標籤和視訊的標籤。 從混合媒體集播放的視訊會使用標準視訊檢視器，該檢視器具有時間軸和視訊控制項，例如「停止」、「暫停」、「倒帶」和「播放」。 當您設定混合媒體集檢視器預設集時，請指定您要用於混合媒體集中不同資產型別的檢視器。 您也可以使用格線檢視器或轉盤檢視器來檢視混合媒體集。

* **[!UICONTROL 迴轉集檢視器]**：提供影像的多個檢視，讓使用者可以轉動物件來檢查不同的側邊和角度。

* **視訊檢視器**：使用來源檔案的解析度維度或自訂大小來顯示視訊。 Adobe Dynamic Media Classic隨附許多預先定義的視訊檢視器預設集，以供您播放視訊，如果您是管理員，可以建立自訂視訊檢視器預設集。 設定Video Viewer有12種以上的不同設定。 您可以設定其：

   * 大小
   * 前景和背景顏色
   * 視訊與音訊控制項
   * 進度列
   * 使用者介面外觀
   * 社交功能
   * 和說明

* **[!UICONTROL 縮放檢視器]**：提供三種縮放檢視器型別的選擇：

* **[!UICONTROL 縮放檢視器]**：可讓使用者透過選取來縮放區域。 他們可以選取控制項來放大、縮小影像，以及將影像重設為預設大小。

* **[!UICONTROL 縮放檢視器：彈出]**：在原始影像旁邊顯示縮放區域的第二個影像。 沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。主要影像大小 (「舞台寬度」和「舞台高度」) 和「縮放係數」會決定彈出影像大小。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

### Adobe Dynamic Media Classic檢視器預設集相容性矩陣 {#scene-viewer-preset-compatibility-matrix}

**Flash檢視器生命週期結束通知**：自2017年1月31日起，Adobe Dynamic Media Classic正式終止支援Flash檢視器平台。

下表列出目前可用的Adobe Dynamic Media Classic檢視器預設集。 此表格也指定檢視器與桌上型電腦和行動裝置的相容性，以及每個指定檢視器所使用的技術。

另請參閱[Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

如需有關檢視器支援的網頁瀏覽器和作業系統版本的資訊，您可以檢閱「檢視器發行說明」。

請參閱[Adobe檢視器參考發行說明](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources)。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 縮放檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 色票集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog檢視器 |  |  |  |  |  |  |
| Universal_Catalog5_eCatalog_Adv(包含對社交HTML和目錄搜尋的支援)。 | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog （包含對社群媒體和目錄搜尋的支援。） | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 迴轉檢視器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 檢視器**

Adobe Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。

* 您可以在下列位置找到支援此視訊格式的BlackBerry®裝置： [BlackBerry®](https://developers.blackberry.com/us/en)支援的視訊格式
* 您也可以在下列位置找到支援此視訊格式的Windows®裝置： [Windows® Phone上支援的視訊格式](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 | BlackBerry®智慧型手機 | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包含對隱藏式字幕的支援）。 請參閱[最佳實務：使用通用HTML5視訊檢視器。](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包含對隱藏式字幕和社群媒體的支援。） | HTML5 | X | X | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒體集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支援的行動檢視器手勢矩陣 {#supported-mobile-viewers-gestures-matrix}

下表列出iOS、Android™ 2.x和Android™ 3.x裝置支援的行動檢視器手勢。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 關於檢視器預設集畫面 {#about-the-viewer-preset-screen}

在「檢視器預設集」畫面建立和管理檢視器預設集。若要開啟此熒幕，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。

「檢視器預設集」畫面提供了執行下列工作的工具:

* **新增預設集**：選取「**[!UICONTROL 新增]**」，並在「新增檢視器預設集」對話方塊中進行選擇。

      請參閱[新增及編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。
  
* **編輯預設集**：選取預設集，然後選取&#x200B;**[!UICONTROL 編輯]**。

      請參閱[新增及編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。
  
* **刪除預設集**：選取預設集，然後選取&#x200B;**[!UICONTROL 刪除]**。

* **匯出預設集**：選取HTML5檢視器預設集。 然後按一下[匯出]&#x200B;**&#x200B;**&#x200B;下載檢視器外觀元素，以將其作為建立及新增其他檢視器預設集的基礎。

      請參閱[匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。
  
* **篩選檢視器預設集清單**：使用這些工具來篩選清單：

      *開啟&#x200B;**作用中/非作用中**&#x200B;下拉式清單，並選取顯示作用中預設集、非作用中預設集或所有預設集的選項。
     *開啟&#x200B;**檢視器**&#x200B;下拉式清單，並選取選項以僅檢視特定型別的檢視器。 選取&#x200B;**[!UICONTROL 所有檢視者]**&#x200B;以檢視所有檢視者。
  
* **排序預設集**：選取欄標題（**[!UICONTROL Active]**、**[!UICONTROL Type]**、**[!UICONTROL Preset]**&#x200B;或&#x200B;**[!UICONTROL Platform]**）來排序欄上的清單。 第二次選取欄標題，依遞減（或遞增）順序排序清單。

* **啟用和停用預設集**：選取預設集，然後選取其[作用中]選項，以便您可以啟用或停用預設集。

      請參閱[啟動或停用檢視器預設集](application-setup.md#activating_or_deactivating_viewer_presets)。
  
>[!NOTE]
>
>選取「檢視器預設集」頁面右側的「**[!UICONTROL 預覽]**」，您就能檢視資產在您選取的檢視器預設集中是什麼樣子。 若要檢視其他資產，請在[檢視器預設集]頁面中選取&#x200B;**[!UICONTROL 瀏覽]**，然後在[選取資產預覽]對話方塊中選取其他資產。

### 新增和編輯檢視器預設集 {#adding-and-editing-viewer-presets}

除了在使用者介面中使用&#x200B;**[!UICONTROL 新增]**&#x200B;來新增檢視器預設集之外，您也可以使用&#x200B;**[!UICONTROL 匯出]**&#x200B;來新增檢視器預設集。 您只需匯出現有的HTML5檢視器預設集，然後使用該預設集作為新預設集的基礎。

請參閱[HTML5檢視器預設集匯出](application-setup.md#exporting_an_html5_viewer_preset)。

另請觀看[檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)訓練影片。

**若要新增及編輯檢視器預設集：**

1. 在Adobe Dynamic Media Classic的右上角附近，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。

   您可以篩選預設集的清單。例如，若只要查看視訊檢視器的預設集，請從表格正上方工具列上的「檢視器」下拉式選單中選取「視訊檢視器」。

1. 在「檢視器預設集」頁面中，新增或編輯「檢視器預設集」畫面上的「檢視器預設集」 。

   * **新增**：在工具列上，選取&#x200B;**[!UICONTROL 新增]**。 在「新增檢視器預設集」對話方塊中，選取平台，然後選取多媒體資產型別。

     完成檢視器預設集建立後，    選取&#x200B;**[!UICONTROL 另存新檔]**。
     
   * **從現有的檢視器預設集開始新增**：在表格中，選取視訊檢視器預設集，然後在工具列上選取&#x200B;**[!UICONTROL 編輯]**。

         重新設定Video Viewer後，選取&#x200B;**[!UICONTROL 另存新檔]**，在「預設集名稱」文字欄位中使用其他名稱儲存預設集。
     
   * **編輯**：選取現有的檢視器預設集，然後選取&#x200B;**[!UICONTROL 編輯]**。

1. 在「配置檢視器」頁面的「預設集名稱」欄位中，輸入或編輯預設集名稱。
1. 設定其它想要的選項。

   >[!NOTE]
   >
   >選取「**[!UICONTROL 與Source相同]**」，讓您可以自動將視訊檢視器大小調整為已編碼視訊本身的解析度大小。 如果選取此選項，則無法輸入「舞台寬度」和「舞台高度」。 相反，這些選項來自視訊本身。如果您選取「**[!UICONTROL 與Source相同]**」，請設定「邊界大小」選項以反映視訊播放區域以外的外觀尺寸。 該邊距大小是視訊控制項的像素高度和寬度。您可以使用下列影像來協助您決定要使用的邊界大小。*

   ![視訊檢視器的邊界設定](assets/vs_video_viewer_configure_margin.png)

1. 進行以下一項操作:

   * 如果您從現有的預設集開始新增檢視器預設集，請選取&#x200B;**[!UICONTROL 另存新檔]**。
   * 如果您新增或編輯檢視器預設集，請選取「**[!UICONTROL 儲存]**」。

### 匯出HTML5檢視器預設集 {#exporting-an-html-viewer-preset}

您可以匯出現有的HTML5檢視器預設集，以作為建立HTML5檢視器預設集的基礎。 匯出選項十分有用，因為您不需從頭建立檢視器， 但可以匯出與您要的外觀和行為接近的預設集，然後將其用作進行設計調整的起點。

Adobe Dynamic Media Classic中所有預設、立即可用的檢視器預設集CSS檔案，都會使用指向`Scene7SharedAssets`上資產的相對影像伺服路徑。 例如，以下為上檢視器預設集CSS檔案中影像資產的相對路徑

`Scene7SharedAsset`： `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

不過，如果您將Viewer CSS檔案託管在您自己的網站上，則必須在您自己的環境中使用影像伺服器的明確路徑來解析這些相對影像路徑。 例如，如果您將上方的相對路徑更新為明確路徑，可能會如下所示，其中`https://s7d1.scene7.com`是影像伺服器的直接路徑： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**要匯出HTML5檢視器預設集：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。
1. 在「檢視器預設集」工具列左側的第二個下拉式清單中，選取&#x200B;**[!UICONTROL HTML5]**。
1. 在左邊第三個下拉式清單中，選取&#x200B;**[!UICONTROL 所有檢視器]**。
1. 選取您要用來作為新HTML5檢視器預設集基礎的檢視器預設集。
1. 在工具列中選取&#x200B;**[!UICONTROL 匯出]**。
1. 在「匯出選取的Assets」對話方塊中，選取&#x200B;**[!UICONTROL 送出匯出]**。

   匯出後，您會取得CSS檔案。 下載並解壓縮檔案。

1. 在 CSS 編輯器中開啟 CSS 檔案，進行變更後儲存檔案。
1. 將CSS檔案上傳至Adobe Dynamic Media Classic。

   請參閱[上傳檔案](uploading-files.md#uploading_files)。

1. 將CSS檔案Publish至Dynamic Media影像伺服器。

   檢視[Publish檔案](publishing-files.md#publishing_files)。

1. 照常新增檢視器預設集。 選取您上傳的檢視器CSS檔案。

   請參閱[新增及編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

### 啟用或停用檢視器預設集 {#activating-or-deactivating-viewer-presets}

若要建立用於顯示資產的URL，使用者可以在「預覽」對話方塊中開啟「預設集」下拉式清單，選取「檢視器預設集」，然後選取「**[!UICONTROL 複製URL]**」（請參閱[複製檢視器預設集的URL](application-setup.md#copying_the_url_of_a_viewer_preset)）。 預設集清單提供了管理員在「檢視器預設集」畫面所增加和管理的檢視器預設集。例如，當使用者預覽eCatalog時，所有作用中的eCatalog檢視器預設集都會顯示在「預覽」對話方塊的「預設集」下拉式清單中。

除非您在「檢視器預設集」畫面上停用檢視器預設集，否則「預覽」對話框中的「預設集」下拉式清單可能會過於擁擠。

**若要啟用或停用檢視器預設集：**

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。
1. 在[檢視器預設集]頁面上，選取或取消選取&#x200B;**[!UICONTROL 作用中]**&#x200B;選項，以啟用或停用檢視器預設集。

### 複製檢視器預設集的URL {#copying-the-url-of-a-viewer-preset}

發佈資產後，您就可以複製 URL，以「檢視器預設集」的設定來顯示資產。

URL 便會複製到剪貼簿。您可以視需要在網頁、行動裝置或應用程式的HTML程式碼中使用它。

**若要複製檢視器預設集的URL：**

1. 在「瀏覽」面板中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 複製URL]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

### 複製檢視器預設集的內嵌程式碼 {#copying-the-embed-code-of-a-viewer-preset}

您可使用「內嵌程式碼」功能查看所選「檢視器預設集」的檢視器程式碼。您也可以將程式碼複製到剪貼簿，以便貼到網頁中來部署檢視器。

不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製檢視器預設集的內嵌程式碼：**

1. 在「資產瀏覽」面板中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL面板中，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

   在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

1. 在「內嵌程式碼」對話方塊中，選取&#x200B;**[!UICONTROL 複製到剪貼簿]**。
1. 選取&#x200B;**[!UICONTROL 關閉]**。

## 設定預設檢視器 {#configure-default-viewers}

在Adobe Dynamic Media Classic中使用預覽時，您可以使用預設檢視器來設定與資產相關聯的預設檢視器。 您可以針對下列資產類型設定預設的預覽體驗:

* 影像
* 視訊
* 迴轉集
* 目錄
* 影像集
* 色票集
* 媒體集

**設定預設檢視器：**

1. 在[設定]下拉式清單中，選取&#x200B;**[!UICONTROL 應用程式設定]**。
1. 在設定視窗的左窗格中，移至&#x200B;**[!UICONTROL 應用程式設定]** > **[!UICONTROL 檢視器]**
1. 選取&#x200B;**[!UICONTROL 預設檢視器]**。
1. 在「預設檢視器」視窗中，於每個資產型別的下拉式清單中，選取您要與資產預覽相關聯的檢視器。
1. 在「預設檢視器」視窗的右下角，選取&#x200B;**[!UICONTROL 「儲存設定」]**。
1. 在「設定」視窗的右下角，選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回「資產」視窗。

## 中繼資料檢視 {#metadata-views}

*中繼資料*&#x200B;是有關資產的標準化資料。您可以使用中繼資料來簡化工作流程、組織資產和改善搜尋。Adobe Dynamic Media Classic支援IPTC （國際新聞通訊委員會）標準和XMP （可延伸中繼資料平台）標準。 使用者在「詳細資料檢視」中檢視或輸入有關資產的中繼資料之前，可以開啟「中繼資料檢視」功能表。 接著，他們就可以選取要檢視或用來描述資產的中繼資料欄位集。

Adobe Dynamic Media Classic隨附預先定義的中繼資料檢視，管理員可以建立自己的中繼資料檢視，讓使用者在輸入中繼資料時進行選擇。

### 建立中繼資料檢視 {#creating-a-metadata-view}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料檢視]**。
1. 選取&#x200B;**[!UICONTROL 新增]**。
1. 在「預設集名稱」文字欄位中，輸入檢視的名稱。
1. （選擇性）勾選&#x200B;**[!UICONTROL 設為預設值]**，讓此檢視成為使用者在詳細資料檢視中開啟中繼資料面板時看到的檢視。
1. （選擇性）選取&#x200B;**[!UICONTROL 包含UDF]**&#x200B;以在檢視中包含使用者定義的欄位。 使用者定義的欄位會顯示在詳細檢視的「中繼資料」面板上方。
1. 選取您要檢視的欄位（選取&#x200B;**[!UICONTROL 全選]**&#x200B;以選取所有欄位）。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

   選取的檢視類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料檢視 {#managing-metadata-views}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料檢視]**。
1. 請執行下列任一動作:

   * 若要預覽檢視，請加以選取。檢視中的欄位會顯示在「預覽」面板中。
   * 若要編輯檢視，請選取該檢視，然後選取&#x200B;**[!UICONTROL 編輯]**。 接著在「預覽」面板上選取或取消選取欄位名稱，然後選取或取消選取&#x200B;**[!UICONTROL 包含UDF]**&#x200B;選項。
   * 若要刪除檢視，請選取該檢視，然後選取&#x200B;**[!UICONTROL 刪除]**。
   * 若要將檢視設為預設值，請選取該檢視，然後選取&#x200B;**[!UICONTROL 設為預設值]**。 預設檢視是使用者在「詳細資料檢視」中開啟資產並前往「中繼資料」面板時看到的檢視。

## 中繼資料預設集 {#metadata-presets}

中繼資料預設集可讓管理員控制並規範指派給資產的中繼資料。 在「詳細資料檢視」中，使用者可在為此目的提供的欄位中輸入有關資產的中繼資料。 例如，使用者可以輸入擁有者名稱、版權描述和地址。為確保使用者正確且完整地輸入此資訊，您可以建立中繼資料預設集。 在「詳細資料檢視」中選擇中繼資料預設集，會以預先定義的值填入中繼資料欄位。 例如，擁有者名稱、版權描述和地址皆會自動輸入。

為您希望使用者能在詳細資料檢視中自動輸入以說明資產的每一組中繼資料值建立中繼資料預設集。

### 建立或編輯中繼資料預設集 {#creating-or-editing-a-metadata-preset}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料預設集]**。
1. 在「中繼資料預設集」面板中，執行下列任一項作業:

   * 若要建立預設集，請選取&#x200B;**[!UICONTROL 新增]**。 在「中繼資料範本名稱」文字欄位中，輸入預設集名稱。 選取&#x200B;**[!UICONTROL 中繼資料檢視]**，然後從下拉式清單中選取檢視（請參閱[中繼資料檢視](application-setup.md#metadata_views)）。
   * 若要編輯現有的預設集，請從[中繼資料預設集]清單中選取預設集，然後選取[**[!UICONTROL 編輯]**]。

1. 展開您要加入預設集的標題，然後在您要加入預設集的不同欄位中輸入值。
1. 選取&#x200B;**[!UICONTROL 儲存]**。

   選取的預設集類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料預設集 {#managing-metadata-presets}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料預設集]**。
1. 請執行下列任一動作:

   * 若要預覽預設集，請選取您要預覽的預設集。預設集資訊 (類別和欄位) 會顯示在「預覽」畫面中。
   * 若要刪除預設集，請選取預設集，然後選取&#x200B;**[!UICONTROL 刪除]**。

## 使用者定義的欄位 {#user-defined-fields}

媒體入口網站管理員或公司管理員可建立自訂、使用者定義的中繼資料欄位。自訂欄位可協助您在Adobe Dynamic Media Classic中組織資產。 您可以視需要將欄位標示為「使用中」。 啟動後，這些自訂中繼資料欄位的名稱會出現在詳細檢視的中繼資料面板中。 使用者可以在使用者自訂的中繼資料欄位中輸入資訊，以描述資產。使用者也可以將使用者定義的中繼資料欄位設定作為搜尋條件。

使用者定義的中繼資料欄位的有效用途之一，就是針對特定的上市發表會或銷售會，延遲資產的啟用時間。您根據型別&#x200B;*Date*&#x200B;定義「啟用」欄位。 然後，在詳細資料檢視中使用&#x200B;**[!UICONTROL 中繼資料]**&#x200B;面板，或使用&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**，您可以指定啟動資產的時間。 Adobe Dynamic Media Classic會檢查資產的已發佈狀態和發佈歷史記錄。 如果不在啟動時間內，發佈狀態會顯示為「未發佈」。

>[!NOTE]
>
>若要讓使用者定義的欄位顯示在「詳細資料檢視」的中繼資料面板中，請在中繼資料檢視中加入使用者定義的欄位。 在「中繼資料檢視」畫面上選取「包含 UDF」(使用者定義欄位) 選項。如需詳細資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views)。

>[!NOTE]
>
>若要使用自訂、使用者定義的欄位來搜尋資產，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，然後選取&#x200B;**[!UICONTROL 在搜尋中包含UDF]**。 請參閱[個人設定](personal-setup.md#personal_setup)。

### 建立使用者定義的中繼資料欄位 {#creating-a-user-defined-metadata-field}

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義的欄位]**。
1. 選取&#x200B;**[!UICONTROL 新增]**
1. 在「自訂欄位」對話框中，設定您要的選項。

   * **[!UICONTROL 名稱]**：輸入中繼資料欄位的名稱。

   * **[!UICONTROL 型別]**：選取一個選項，定義使用者可在中繼資料欄位中輸入的資訊型別：

   * **[!UICONTROL 字串]**：文字字串。

   * **[!UICONTROL Int]**：整數。

   * **[!UICONTROL 浮點數]**：浮點數。

   * **[!UICONTROL 是/否]**：是/否布林值。

   * **[!UICONTROL 日期]**：日期。 接受 MM/DD/YYYY 格式。

   * **[!UICONTROL 檔案名稱]**：檔案的名稱。

   * **[!UICONTROL 色彩]**：色彩的名稱。

   * **[!UICONTROL Dimension]**：資產的寬度和高度。

   * **[!UICONTROL 無型別]**：為了回溯相容性。 請勿選取此選項。

   * **[!UICONTROL 預設值]**：選擇性。 輸入使用者最有可能在欄位中輸入的值。 您輸入的值會成為您建立之欄位的預設值。

   * **[!UICONTROL 套用至]**：選擇性。 如果您希望中繼資料欄位僅套用至特定型別的資產，請選取資產型別。

     >[!NOTE]
     >
     >請謹慎選取&#x200B;**[!UICONTROL 套用至]**&#x200B;選項，因為在您建立使用者定義的欄位後，就無法變更&#x200B;**[!UICONTROL 套用至]**&#x200B;選項。 Adobe Dynamic Media Classic可讓您編輯使用者定義欄位的名稱、型別和預設值，但無法編輯&#x200B;**[!UICONTROL 套用至]**&#x200B;設定。*

1. 當您完成建立中繼資料欄位時，選取&#x200B;**[!UICONTROL 儲存]**。

### 管理使用者定義的欄位 {#manage-user-defined-fields}

「使用者定義的欄位」畫面提供了管理自訂、使用者定義之中繼資料欄位的命令。

只有 Media Portal 管理員或公司管理員才可以管理使用者定義的欄位。

若要開啟此熒幕，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義欄位]**。

* **編輯欄位**：選取欄位，然後選取&#x200B;**[!UICONTROL 編輯]**。

* **刪除欄位**：選取欄位，然後選取&#x200B;**[!UICONTROL 刪除]**。

* **啟用欄位**：選取或取消選取欄位名稱旁的&#x200B;**[!UICONTROL 啟用]**&#x200B;選項。 如果您處於公司管理角色，此選項不會顯示。 由於此選項與MediaPortal有關，因此您必須選取（開啟） 「在個人設定中顯示MediaPortal功能」才能檢視已啟用的欄位。

## 最佳化檔案 {#optimize-files}

當您上傳檔案至Adobe Dynamic Media Classic時，系統會針對儲存和發佈檔案進行最佳化。 不過，如果上載程序受到中斷，部分影像就無法最佳化。在此情況下，您會看到「影像尚未最佳化」訊息。 但是，如果您是管理員，就可以最佳化這些檔案。

Adobe Dynamic Media Classic會搜尋您的檔案，並只最佳化之前未完全最佳化的影像。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**，然後選取&#x200B;**[!UICONTROL 最佳化檔案]**。
1. 輸入最佳化工作的資訊，並選取&#x200B;**[!UICONTROL 送出]**。

   如果您使用超過一家公司，請分別對屬於不同公司的檔案執行最佳化。

## 批次集預設集 {#batch-set-presets}

使用批次集預設集，以便您可以在工作執行時將資產上傳到Adobe Dynamic Media Classic時自動建立影像集或迴轉集。

公司管理員首先會為想要分組到資產集的資產定義命名慣例。 然後您可以建立「批次集預設集」來參照這些影像。 每個預設集都是具備唯一名稱的內部獨立式指示集，定義如何使用與預設集配置中已定義的命名慣例相符的影像來建構集。

公司的所有作用中批次集預設集都會列在「上載工作選項」對話方塊中，因此您可以指定要在每個上載工作階段期間套用的預設集。 公司管理員會看到所有作用中和非作用中的批次集預設集。 上傳檔案時，Adobe Dynamic Media Classic會自動建立一個集合，其中包含與作用中預設集中定義的命名慣例相符的所有檔案。

### 預設命名 {#default-naming}

公司管理員會建立用於任何「批次集預設集」配方的預設命名慣例。 在「批次集預設集」定義中選取的預設命名慣例，可能正是貴公司為所有網站批次產生集所需的一切。 會建立批次集預設集，以使用您定義的預設命名慣例。 您可以針對特定內容集建立所需數量的批次集預設集，並搭配替代自訂命名慣例，以因應公司定義預設命名例外情況。

使用批次集預設集功能不需要設定預設命名慣例。 不過，Adobe最佳實務建議您使用預設命名慣例來定義要分組到一組中的命名慣例元素。 這麼做有助於簡化批次集的建立。

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 預設命名]**。
1. 選取「**[!UICONTROL 檢視表單]**」或「**[!UICONTROL 檢視器碼]**」即可指定您要如何檢視和輸入個別元素的相關資訊。

   您可以選取&#x200B;**[!UICONTROL 檢視程式碼]**&#x200B;核取方塊，以檢視表單選取專案旁邊的規則運算式值建置。 如果「表單檢視」因任何原因限制您，您就可以輸入或變更這些值，以協助定義命名慣例的元素。 如果無法在表單檢視中剖析您的值，則表單欄位會變為非使用中。

   >[!NOTE]
   >
   >停用的表單欄位不代表規則運算式無效。沒有驗證方式可確認您的規則運算式是否正確。您會在「結果」行後面看到針對每個元素所建置的規則運算式結果。 您可以在頁面底部看到完整的規則運算式。

1. 視需要展開個別元素，並輸入您要使用的命名慣例。
1. 必要時，選取&#x200B;**[!UICONTROL 新增]**&#x200B;為元素新增其他命名慣例。 或者，選取&#x200B;**[!UICONTROL 移除]**&#x200B;以刪除元素的命名慣例。
1. 選取「**[!UICONTROL 另存新檔]**」並輸入預設集名稱。 或者，如果您正在編輯現有的預設集，請選取&#x200B;**[!UICONTROL 儲存]**。

您也可以使用不含任何可用表單欄位的「檢視器碼」。在此檢視中，您會完全使用規則運算式來建立命名慣例定義。

有兩個元素可供定義，分別為「符合」和「基本名稱」。這些欄位是您為命名慣例定義的所有元素。 它們有助於識別用於命名包含它們的集合的慣例部分。 公司的個別命名慣例可能會對其中每個元素使用一或多行定義。 您可以針對唯一的定義使用儘可能多的線條，並將它們分組為不同的元素，例如主影像、顏色元素、替代檢視元素和色票元素。

### 建立批次集預設集 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic使用批次集預設集將共用某些一般資訊或內容的資產組織到影像集中，以便顯示在檢視器中。 「批次集預設集」配方會自動與您在Adobe Dynamic Media Classic中排程的資產匯入作業一起執行。

使用批次集預設集來建立、編輯和管理您的批次集預設集。 您可以視需要建立儘可能多的預設集，以涵蓋所需的所有資產擷取工作。 批次集預設集定義有兩種形式：一種用於您已設定的預設命名慣例，另一個用於您即時建立的自訂命名慣例。

您可以使用表單欄位方法來定義批次集預設集，或使用代碼方法來讓您使用規則運算式。 如同在&#x200B;**[!UICONTROL 預設命名]**&#x200B;中一樣，您可以在表單檢視中定義並使用規則運算式建置定義的同時，選取&#x200B;**[!UICONTROL 程式碼檢視]**。 您也可以取消核取任一檢視，僅使用其中一種。

另請參閱[建立批次集預設集以自動產生2D迴轉集](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)。

另請觀看[2D迴轉集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS)訓練影片。

**若要建立批次集預設集：**

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 批次集預設集]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設集清單」面板中，選取&#x200B;**[!UICONTROL 新增]**&#x200B;以啟動頁面右側「詳細資料」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取預設集類型。

   若要自動產生 2D 迴轉集，請從「批次集類型」下拉式清單中選取「**[!UICONTROL 多軸旋轉集]**」。

1. 進行以下一項操作:

   * 如果您使用先前在&#x200B;**[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 預設命名]**&#x200B;下設定的預設命名慣例，請展開&#x200B;**[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取&#x200B;**[!UICONTROL 預設]**。
   * 若要在設定預設集時定義命名慣例，請展開&#x200B;**[!UICONTROL Asset Naming Conventions]**，然後在[檔案命名]下拉式清單中，選取&#x200B;**[!UICONTROL 自訂]**。

1. 針對「序列順序」，請在影像集在Adobe Dynamic Media Classic中分組後，定義影像的順序。 根據預設，您的資產會按照字母順序排列。不過，您可以使用規則運算式以逗號分隔的清單來定義順序。
1. 在「設定命名與建立慣例」中，請為您在「資產命名慣例」中定義的「基本名稱」指定字尾或字首。 也會定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立「影像集」資料夾，並將應用程式重新導向，將「批次集」產生的影像集放置在此處。

1. 在[詳細資料]面板中選取[**[!UICONTROL 儲存]**]。

### 建立批次集預設集以自動產生2D迴轉集 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您可以使用批次集型別&#x200B;**多軸迴轉集**&#x200B;來建立「方式」，自動產生2D迴轉集。 影像的群組會使用列與欄規則運算式，使影像資產適當對齊於多維度陣列中的對應位置上。

另請參閱[建立批次集預設集](application-setup.md#creating_a_batch_set_preset)。

多軸「迴轉集」中沒有最小或最大列數或欄數。

例如，假設您要建立名為&#x200B;*spin-2dspin*&#x200B;的多軸迴轉集。 您有一組包含三列的迴轉集影像，每列有12個影像。 影像的命名如下:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

您可以使用此資訊來建立「批次集型態」配方，如下所示：

![批次集配方影像](assets/se_batch_set_recipe.png)

「迴轉集」之共用資產名稱部分的分組會新增至「比對」欄位（反白顯示）。 包含行和列的資產名稱的變數部分將分別新增到行和列欄位中。

上傳和發佈迴轉集時，您會啟用「上傳工作選項」對話方塊中&#x200B;**[!UICONTROL 批次集預設集]**&#x200B;下方所列的2D迴轉集方式名稱。

**若要建立批次集預設集以自動產生2D迴轉集：**

1. 移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 批次集預設集]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設集清單」面板中，選取&#x200B;**[!UICONTROL 新增]**&#x200B;以啟動頁面右側「詳細資料」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取「**[!UICONTROL 資產集]**」。
1. 在「子型別」下拉式清單中，選取&#x200B;**[!UICONTROL 多軸迴轉集]**。
1. 展開&#x200B;**[!UICONTROL 資產命名慣例]**，然後在[檔案命名]下拉式清單中，選取[自訂]&#x200B;**&#x200B;**。
1. 使用「**[!UICONTROL 符合]**」，並選擇性地使用「**[!UICONTROL 基本名稱]**」屬性，定義用來為組成群組的影像資產命名的規則運算式。

   例如，您的常值Match規則運算式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展開「**[!UICONTROL 列欄位置]**」，然後為影像資產在 2D 迴轉集陣列內的所在位置定義名稱格式。

   使用括號括住檔案名稱中的列或欄位置。

   例如，針對列的規則運算式，如下所示：

   `\w+-R([0-9]+)-\w+`

   或

   `\w+-(\d+)-\w+`

   若是欄規則運算式，可能如下所示：

   `\w+-\w+-C([0-9]+)`

   或

   `\w+-\w+-C(\d+)`

   請記住，這些運算式只是範例。 您可以用任何想要的方式建立規則運算式以符合自己的需求。

   >[!NOTE]
   >
   >如果列和欄中的規則運算式組合無法判斷資產在多維度迴轉集陣列中的位置，該資產不會新增到迴轉集內。 已記錄錯誤。

1. 在「設定命名與建立慣例」中，請為您在「資產命名慣例」中定義的「基本名稱」指定字尾或字首。 也會定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立「影像集」資料夾，並將應用程式重新導向，將「批次集」產生的影像集放置在此處。

1. 在[詳細資料]面板中選取[**[!UICONTROL 儲存]**]。
1. 照常上傳並發佈迴轉集，確保在「批次集預設集」下的「工作載入選項」對話方塊中啟動2D迴轉集的名稱。

>[!MORELIKETHIS]
>
>* [預覽資產](previewing-asset.md#previewing_an_asset)
>* [設定影像預設集](setting-image-presets.md#setting_up_image_presets)
>* [檢視、新增和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [檢查工作檔案](checking-job-files.md#checking_job_files)
