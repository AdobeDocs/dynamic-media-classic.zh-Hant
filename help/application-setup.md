---
title: 應用程式設定
description: 了解如何設定Dynamic Media Classic的「應用程式」區域。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '10895'
ht-degree: 45%

---

# 應用程式設定{#application-setup}

您可以使用「應用程式設定」頁面輸入一般設定、建立影像預設集、視訊編碼預設集、檢視器預設集，或定義預設檢視器和中繼資料。 您可以設定批次集預設集，也可自動產生2D回轉集（例如）、發佈設定和視訊SEO設定。

>[!NOTE]
>
>只有Dynamic Media Classic管理員可以變更「應用程式設定」頁面上的設定。

## 一般設定 {#general-settings}

要開啟「應用程式一般設定」頁，請在全局導航欄上，轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**。

### 伺服器

建立帳戶時，Dynamic Media Classic會自動為您的公司提供指派的伺服器。 這些伺服器是用來為您的網站和應用程式建立 URL 字串。這些 URL 呼叫皆專屬於您的帳戶。

另請參閱[測試安全測試服務](testing-assets-making-them-public.md#testing_the_secure_testing_service)。

* **[!UICONTROL 已發佈伺服器名稱]**  — 此伺服器是即時內容傳送網路(CDN)伺服器，用於您帳戶專用的所有系統產生的URL呼叫。除非Dynamic Media Classic支援技術人員指示您更改此伺服器名稱，否則請勿更改此伺服器名稱。

* **[!UICONTROL 來源伺服器名稱]**  — 此伺服器僅用於品質保證測試。除非Dynamic Media Classic支援技術人員指示，否則請勿更改此伺服器名稱。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **[!UICONTROL Test&amp;Target伺服器名稱]**  — 您的Test&amp;Target URL，最多及包含.com。有關獲取此URL的說明，請參閱將[!DNL Dynamic Media Classic]與[!DNL Adobe Target Standard/Premium]整合。

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS串流伺服器名稱]**  — 您iOS串流伺 [!DNL Dynamic Media Classic] 服器的URL。此伺服器會透過 HTTP 通訊協定將串流視訊傳送至以 iOS 為基礎的裝置。

* **[!UICONTROL 漸進式視訊伺服器名稱]**  — 您的漸進式視訊伺 [!DNL Dynamic Media Classic] 服器的URL。此伺服器會透過 HTTP 通訊協定來傳送漸進式視訊。

* **[!UICONTROL 顯示未發佈資產的URL]**  — 如果您想在預覽任 [!DNL Dynamic Media Classic] 何資產時顯示URL（無論是否已發佈），請選取此選項。如果資產尚未發佈，URL 將無法運作。不過，您可以使用 URL 來進行規劃或組織。

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN失效範本]**  — 指定用於使CDN（內容傳遞網路）快取失效的範本。

   例如，假設您輸入參考`<ID>`的影像URL（包括影像預設集或修飾元），而非如下列範例所示的特定影像ID:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   如果範本僅包含`<ID>`，則Dynamic Media Classic會填入`https://<server>/is/image`，其中`<server>`為一般設定中定義的發佈伺服器名稱。

   設定「CDN無效範本」，選取名為Backpack_B的影像，然後前往&#x200B;**[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]**，會在「CDN無效」介面中產生下列產生的URL:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   在URL清單方塊中，選取&#x200B;**[!UICONTROL 繼續]**&#x200B;以清除該特定影像URL呼叫的快取。 您也可以輸入URL或將其貼到URL清單方塊，以新增URL;您不需要預先設定範本。

   在您選取CDN失效範本，並提出使CDN無效的請求後，使用者介面中會出現指標。 它可讓您估計清除快取所需的時間。

   同樣地，如果您在前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 使CDN]**&#x200B;時在Dynamic Media Classic中選取了多個影像，則儲存的範本URL會參照每個影像。 因此，您可以定義CDN無效範本，以參考網站上參考的每個URL（例如產品詳細資料和搜尋結果）。 然後，當您從快取中選取一或影像以進行失效時，URL會自動填入介面。

   請參閱[內容快取](dmc-platform-overview.md#content_caching)。

   請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 瀏覽

* **[!UICONTROL 顯示專案]**  — 決定是否提供專案作為組織Dynamic Media Classic資產的工具。請參閱利用專案組織您的工作。

* **[!UICONTROL 顯示範例eVideo內容]**  — 開啟或關閉eVideo範例內容的顯示。

* **[!UICONTROL 顯示產生的內容]**  — 在資料夾中，顯示從資產產生的內容。例如，當PDF檔案在上傳時柵格化時，Dynamic Media Classic會以原始PDF為每個頁面建立一個影像。 如果選取了「顯示產生的內容」，則原始 PDF 上載時所產生的每個影像，都會與 PDF 一起出現在該 PDF 的上載檔案夾中。

* **[!UICONTROL 顯示編碼的視訊]**  — 預設為取消選取（關閉）。

   若要在Dynamic Media Classic中快速搜尋和瀏覽視訊，而不需導覽相同視訊的許多已編碼衍生影片，請保留取消選取此選項（預設）。 只會顯示「主視訊」縮圖（您上傳並用來建立衍生影片的來源視訊），以及「上層」適用性視訊集縮圖（包含已編碼視訊集的「下層」衍生影片）。

   不過，您仍然可以從主視訊或最適化視訊集存取個別編碼的視訊。若要執行此項操作，請按兩下視訊縮圖影像，以開啟「詳細檢視」。然後，在右側面板中選取「**[!UICONTROL 編碼視訊]**」，以便存取所有「子」視訊。

   您也可以前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]**，直接從適用性視訊集建立更編碼的「子」視訊。 Dynamic Media Classic會自動找到最適化視訊集的「父」主視訊，並將其作為轉碼的來源視訊。 不過，在您儲存新的個別編碼的視訊後，搜尋或瀏覽時並不會看到這些視訊。然而這些視訊仍可從「詳細檢視」的「編碼的視訊」標籤予以存取。

   請參閱[上傳和轉碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

   若要繼續能夠在搜尋和瀏覽時存取所有編碼視訊的衍生物，請選取「**[!UICONTROL 顯示編碼的視訊]**」。

   「建置」選單上的某些動作只能用於個別視訊，或選擇性地用於個別視訊。此功能迫使您必須顯示所有可以選取之編碼視訊的衍生物，而不受您設定「**[!UICONTROL 顯示編碼的視訊]**」的方式影響。超越&#x200B;**[!UICONTROL 顯示編碼視訊]**&#x200B;設定的「建置」動作包括&#x200B;**[!UICONTROL 適用性視訊集]**&#x200B;和&#x200B;**[!UICONTROL eCatalog]**。

   >[!NOTE]
   >
   >如果您沒有使用Dynamic Media Classic上傳和編碼您的視訊資產，Dynamic Media Classic會顯示您所有個別編碼的視訊，即使已取消選取此選項亦然。

* **[!UICONTROL 顯示刷新子資料夾按鈕]**  — 開啟或關閉子資料夾的顯示刷新按鈕。

### Dynamic Media傳統FTP帳戶

* **[!UICONTROL 伺服器]**  — 列出您的FTP帳戶伺服器。

* **[!UICONTROL 使用者名稱]**  — 列出您的FTP帳戶使用者名稱。

### 上載至應用程式

* **[!UICONTROL 覆寫影像]**  - Dynamic Media Classic不允許兩個檔案具有相同的名稱。每個項目的Dynamic Media Classic ID（影像名稱減去副檔名）必須是唯一的。 因為此規則，所以「上載」對話框擁有「覆寫」選項。此選項的確實效果取決於指定的「覆寫影像」選項。這些選項會指定取代影像的上載方式: 取代原始影像或成為重複影像。重複影像將會以「-1」重新命名 (例如，chair.tif 會重新命名為 chair-1.tif)。這些選項會影響上載至非原始檔案夾的影像，或擁有非原始副檔名 (例如 JPG、TIF 或 PNG) 的影像。(請參閱使用覆寫影像選項。)

   * **[!UICONTROL 在目前資料夾中覆寫，使用相同的基本影像名稱/擴充功能]**  — 此選項是最嚴格的取代規則。它會要求您將取代影像上載至與原始影像相同的檔案夾，且取代影像必須與原始檔案擁有相同的副檔名。如果未符合這些要求，便會建立重複項目。

   * **[!UICONTROL 在目前資料夾中覆寫相同的基本資產名稱（無論副檔名為何）]**  — 需要您將取代影像上傳至與原始檔案相同的資料夾，但副檔名可能與原始檔案不同。例如，chair.tif 會取代 chair.jpg。

   * **[!UICONTROL 在任何資料夾中覆寫相同的基本資產名稱/副檔名]**  — 需要替換影像的副檔名與原始影像相同（例如chair.jpg必須替換chair.jpg，而非chair.tif）。然而，您可以將取代影像上載至與原始影像不同的檔案夾。上載的影像將會位於新檔案夾中；無法再於原始位置中找到該檔案

   * **[!UICONTROL 在任何資料夾中覆寫相同的基本資產名稱(不論副檔名為何]** ) — 此選項是包含最多的取代規則。您可以將取代影像上載至非原始檔案夾、上載擁有不同副檔名的檔案，以及取代原始檔案。如果原始檔案位於不同檔案夾，則取代影像會位於其上載的新目標檔案夾中。

* **[!UICONTROL 保留發佈]**  — 指定上傳至Dynamic Media Classic的取代影像是否保留其要取代之影像的「準備發佈」設定，或是在上傳時指定此設定。

* **[!UICONTROL 預設顏色配置檔]**  — 指定添加CMYK影像時，作為預設顏色配置檔案選項的一部分應用的顏色配置檔案。

* **[!UICONTROL 預設上傳選項]**  — 開啟「上傳作業選項」對話方塊，您可在其中指定預設的上傳選項。如需有關這些選項的詳細資訊，請參閱上載選項。

### 應用程式的影像地圖編輯器

* **[!UICONTROL 預設影像對應HREF]**  — 定義用於影像對應中HREF欄的預設URL。此URL是您在建立影像地圖時看到的預設URL。

* **[!UICONTROL 預設影像對應範本]**  — 定義影像對應中HREF範本的預設JavaScript。您可以在此設定自訂程式碼，以便在選取影像地圖時執行。

### 應用程式的其他設定

* **[!UICONTROL 垃圾桶可以清除警告]**  — 垃圾桶中的資產會在七天內自動移除。如果您要在永久刪除「垃圾桶」之資產的前四天傳送通知至公司管理員，請選取「在自動刪除垃圾桶項目前傳送電子郵件」。請參閱管理垃圾桶檔案夾。

## 使用覆寫影像選項 {#using-the-overwrite-images-option}

Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個項目的Dynamic Media Classic ID（影像名稱減去副檔名）必須是唯一的。 因為此規則，所以「上載」對話框包含「覆寫影像」選項。此選項的確切效果取決於每間公司的Dynamic Media Classic內部設定。

如果您先前上傳的影像，然後變更原始檔案（或取代它們），選取的「覆寫」選項會指定Dynamic Media Classic取代影像的方式。 影像的任何相關資訊都不會變更，但新的影像會取代舊影像。如果資料夾中還包含尚未在Dynamic Media Classic中的影像，則會新增這些影像。

如果您上載的影像已經變更 (影像經過修改)，但影像的參照保持不變，則使用此選項。上載和擷取 Adobe® PDF 檔案時，覆寫功能也很有幫助。要微調Dynamic Media Classic *rips*&#x200B;影像的方式，請調整「上載」對話框中的ICC顏色配置檔案選項，並使用「覆蓋」功能重新上載。

從生產伺服器存取影像的Dynamic Media Classic ID衍生自影像檔案名稱。 檔案名稱中必須使用大寫和小寫字元，這在取代現有檔案和用於存取影像的Dynamic Media Classic ID時都很重要。 在上傳至Dynamic Media Classic之前，請確定檔案名稱中的大寫和小寫字元使用正確，以避免Dynamic Media Classic ID只會因相同影像而有所不同。

如果取消選取此選項，所有與現存影像擁有相同檔案名稱的影像都會視為重複項目，而不會增加。

## 影像預設集 {#image-presets}

「影像預設集」畫面是用來建立和編輯影像預設集。影像預設集可讓Dynamic Media Classic以動態方式傳送來自相同主影像的不同大小的影像。 每個影像預設集都代表了一個用來顯示影像之大小調整與格式命令的預先定義集合。建立影像預設集時，您會選取影像傳送的大小。 您也可以選擇格式化命令，以便在傳送影像以供查看時優化影像的外觀。

管理員可以建立匯出資產用的預設集。用戶在導出映像時可以選擇預設集，該預設集還會按照管理員指定的規範重新格式化映像。

若要開啟「影像預設集」畫面，請在全域導覽列上前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**。

請參閱[智慧影像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic)。

### 建立和編輯影像預設集 {#creating-and-editing-image-presets}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 影像預設集]**。
1. 建立預設集或從現有預設集開始：

   * **建立影像預設集**  — 選取「 **[!UICONTROL 新增]**」。
   * **從現有預設集建立影像預設集**  — 選取最像您要建立的影像預設集，然後選取「編 **[!UICONTROL 輯」]**。

1. 在「新增（或編輯）預設集」頁面上，輸入預設集的名稱。
1. 設定您想要的預設集選項。

   請參閱[影像預設集選項](application-setup.md#image_preset_options)。

1. 選擇「**[!UICONTROL 保存]**」，或者，如果從現有預設集開始，請選擇「**[!UICONTROL 另存為]**」。
1. 若要使用您自己的影像預覽預設集，請選取&#x200B;**[!UICONTROL 瀏覽]**，然後選取影像。 要使用預設影像預覽，請選擇&#x200B;**[!UICONTROL 重置]**。

您可以在「影像預設集」畫面上選取影像預設集名稱，然後選取&#x200B;**[!UICONTROL Edit]**，以編輯影像預設集。 若要刪除影像預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL Delete]**。

### 影像預設集選項 {#image-preset-options}

「增加預設集」和「編輯預設集」畫面提供下列選項，以建立和編輯影像預設集:

* **[!UICONTROL 預設集名稱]**  — 輸入描述性名稱，不含任何空白字元。要幫助用戶標識此影像預設集，請在名稱中包括影像大小規範。

* **[!UICONTROL 寬度和高度]**  — 以像素輸入影像傳送的大小。

* **[!UICONTROL 格式]**  — 從功能表選取格式。選擇GIF、JPEG、PDF或TIFF格式會顯示更多選項：

   * GIF 色彩量化選項

      * **[!UICONTROL 類型]**  — 選取「適用性」（預設值）、「Web」或「Macintosh」。如果選擇「Alpha ]**的GIF」，則「Macintosh」選項不可用。**[!UICONTROL 

      * **[!UICONTROL 抖動]**  — 選取「漫射」或「關閉」。

      * **[!UICONTROL 顏色數]**  — 拖曳滑桿以進入2-255。

      * **[!UICONTROL 顏色清單]**  — 輸入逗號分隔的清單。例如，對於白、灰和黑，請輸入 `000000,888888,ffffff`.
   * JPEG 選項

      * **[!UICONTROL 品質]**  — 控制JPEG壓縮級別。這個設定會同時影響檔案大小與影像品質。JPEG質量比例為1-100。

      * **[!UICONTROL 啟用JPG色度下採樣]**  — 由於眼睛對高頻顏色資訊的敏感度比高頻亮度低，因此JPEG影像將影像資訊劃分為亮度和顏色分量。壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣可將資料量減少三分之一或二分之一，而且幾乎不會影響肉眼能感知的品質。縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。
   * PDF 和 TIFF 選項

      * **[!UICONTROL 壓縮]**  — 選取壓縮演算法。



* **[!UICONTROL 顏色]**  — 選取顏色空間。

* **[!UICONTROL 銳利化]**  — 選取「啟用簡單銳利化」選項，在所有縮放發生後，將基本銳利化濾鏡套用至影像。銳利化可以幫助補償以不同大小顯示影像時所造成的模糊現象。

   有關銳利化、重新取樣模式和非銳利化遮色片的詳細資訊，請參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。

* **[!UICONTROL 重新取樣模式]**  — 選取重新取樣模式選項。下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL B — 線性]**  — 最快的重採樣方法；一些鋸齒偽影是可以注意到的。

* **[!UICONTROL 雙立方]**  — 增加影像伺服器上的CPU使用量，但產生更清晰的影像，並產生較少明顯的鋸齒偽影。

* **[!UICONTROL Sharp2]**  — 可產生比雙立方體選項更銳利的結果，但影像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 使用更高和更低的解析度（如果可用）;僅當出現鋸齒時才建議使用。這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

* **[!UICONTROL 非銳利化遮色片]**  — 選擇下列選項以微調銳利化：

* **[!UICONTROL 量]**  — 控制套用至邊緣像素的對比度量。預設是 1.0。對於高解析度的影像，您最多可以將它增加至 5.0。將「數量」視為濾鏡飽和度的度量。

* **[!UICONTROL 半徑]**  — 決定影響銳利化的邊緣像素周圍的像素數。對於高解析度的影像，請輸入 1 到 2 的數字。低數值只會銳利化邊緣的像素；高數值會銳利化較寬的像素範圍。正確的值取決於影像大小。

* **[!UICONTROL 臨界值]**  — 決定套用遮色片銳利化濾鏡時要忽略的對比度範圍。換句話說，這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。為了避免產生雜訊，請使用介於 .02 與 0.2 之間的值來實驗。預設值 6 會對影像中的所有像素進行銳利化。

* **[!UICONTROL 顏色空間]**  — 確定影像是使用建立影像的空間，通常為RGB（原始）還是亮度空間（強度）。

* **** 顏色選擇以下選項：

* **[!UICONTROL 輸出顏色配置]**  — 選擇「 **[!UICONTROL 使]** 用預設」，或Dynamic Media Classic上提供的ICC顏色配置檔案之一。

   請另參閱 [ICC 設定檔](icc-profiles.md#icc_profiles)。

* **[!UICONTROL 呈現目的]**  — 如果您要覆寫顏色描述檔的預設呈現目的，請選取選項。當其中一個預設ICC配置檔案是顏色轉換的目標顏色空間時，使用此選項。 或者，輸出設備（打印機或監視器）具有此配置檔案的特徵，並且指定的渲染目的對此配置檔案有效。

* **[!UICONTROL 內嵌設定檔]**  — 選取此選項，如果您在Adobe® Photoshop®中開啟此影像，系統就會使用此設定檔。

* **[!UICONTROL 打印解析度]**  — 選擇用於打印此影像的解析度；預設為72像素。

* **[!UICONTROL URL修飾元]**  — 如果您偏好指定定義影像預設集的URL修飾元，而非設定，請在此輸入修飾元。

* **[!UICONTROL 範例影像URL]**  — 列出Dynamic Media影像伺服器用來傳送影像的「原始」URL字串，以及您新增或編輯的影像預設集。此 URL 字串會將您在「增加預設集」或「編輯預設集」畫面中選取的所有格式設定加以編碼。

### 編輯、移除或停用影像預設集 {#editing-removing-or-deactivating-an-image-preset}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 影像預設集]**。
1. 在「影像預設集」畫面中，選取表格中的預設集，然後執行以下一項操作:

   * 選擇「**[!UICONTROL 編輯]**」，然後在「編輯預設集」對話框中指定新選項。
   * 選擇&#x200B;**[!UICONTROL Delete]**&#x200B;以從清單中刪除預設。
   * 如果您要從MediaPortal使用者的整個Dynamic Media Classic使用者介面中移除預設集名稱旁的&#x200B;**[!UICONTROL Active]**&#x200B;核取方塊。

## 啟用或停用最適化視訊預設集 {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic提供最適化視訊編碼預設集。 此為主要預設集清單，其中將 16:9 最適化視訊預設集與 4:3 最適化視訊預設集合併到一個群組中。這些預先定義的預設集反映了最常見的編碼設定，並已針對目標行動裝置、平板電腦和桌上型電腦的播放進行最佳化。

預設只會啟動 (啟用或「開啟」)「最適化視訊」編碼預設集。您可以視需要加以停用。非作用中的最適化視訊預設集，並不會以可選取的選項顯示在「上載工作選項」對話框的「eVideo」區段中。

請參閱[上傳和編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**啟用或停用最適化視訊預設集:**

1. 在Dynamic Media Classic的右上角附近，前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**。
1. 在「最適化視訊預設集」頁面上，取消選取預設集名稱旁邊的核取方框，以從「上載工作選項」對話框的「eVideo 選項」清單中移除預設集。
1. 選擇&#x200B;**[!UICONTROL 關閉]**。

## 編碼視訊檔案的視訊預設集 {#video-presets-for-encoding-video-files}

若要選取編碼預設集，請在「上傳」頁面的右下角，選取&#x200B;**[!UICONTROL 工作選項]**。 在「上傳作業選項」對話方塊中，展開「eVideo選項」並選取您想要的視訊編碼預設集。

>[!NOTE]
>
>除了「最適化視訊」（預設為啟用）外，您無法在「上傳工作選項」對話方塊中看到所有其他最適化視訊或單一視訊編碼預設集。 Dynamic Media Classic管理員會決定「上傳工作選項」對話方塊中會顯示哪些視訊編碼預設集。

* 從下列最適化視訊編碼或單一編碼預設集中選取：

   * **[!UICONTROL 16:9適用性影片]**  — 建立16:9長寬比影片，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   * **[!UICONTROL 4:3適用性影片]**  — 建立4:3外觀比例影片，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   * **[!UICONTROL 最適化視訊]**  — 單一編碼預設集，適用於任何外觀比例，以建立視訊以供傳送至行動裝置、平板電腦和桌上型電腦。使用此預設集編碼而上載的來源視訊，會設定成固定的高度。不過，寬度會自動調整為保留視訊的外觀比例。

      具有「自動縮放」的彈性預設也會在您建立自己的自訂視訊編碼預設集時可供使用。

      請參閱[新增或編輯視訊編碼預設集](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)。

   * **[!UICONTROL 適用性視訊編碼（16:9或4:3）]**  — 建立16:9和4:3長寬比視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)。所有元件皆以最符合檢視器連線速度的解析度和位元速率最佳化。

      請參閱[最適化視訊編碼 (16:9 或 4:3) 視訊預設集](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   * **[!UICONTROL 單一編碼預設集]**

      >[!NOTE]
      >
      >若要將視訊傳送至iPad，您可以選取行動裝置編碼預設集或平板電腦編碼預設集。 平板電腦預設集專為 iPad 而設計，通常具有更高的解析度和品質，以充分利用更大的畫面和頻寬連線。傳送使用平板電腦預設集編碼的視訊檔案時，必須在您的行動裝置網站或應用程式上加入裝置偵測程式碼。此程式碼會根據播放裝置的不同，在 iPhone 或 iPad 視訊體驗間切換。更簡單的工作流程是選擇行動裝置預設集將視訊檔案傳送到 iPad。原因在於您可以將同一視訊檔案用於 iPhone 和 iPad。但是，將品質標準化為解析度更低的 iPhone 體驗。

      * 在「編碼預設集」群組下方的「排序編碼預設集」下拉式清單中，選取要依據名稱或解析度大小來排序預設集時的「名稱」或「大小」。
      * 根據您計畫播放視訊的解析度大小和頻寬，選取編碼預設集。
      * 您可以選取「最適化視訊編碼」，以及一或多個每個視訊的編碼預設集。 例如，您可以在一個上載工作中針對桌面和行動裝置編碼檔案。

在您選擇&#x200B;**[!UICONTROL 開始上載]**&#x200B;後，將上載原始主視頻檔案並從主檔案生成編碼檔案。

### 關於編碼預設集選項 {#about-encoding-preset-options}

編碼預設集選項的參數如下:

* **[!UICONTROL 目標連接速度]**  — 目標最終用戶的Internet連接速度。

* **[!UICONTROL 編碼檔案尾碼]**  — 附加至編碼視訊檔案以用於識別目的的尾碼。

* **[!UICONTROL 視訊位元速率（資料速率）]**  — 編碼為構成一秒視訊播放的資料量（以千位/秒為單位）。

* **[!UICONTROL 像素寬度/高]** 度 — 螢幕影像的寬度尺寸（像素）;螢幕影像的高度維度（像素）。

* **[!UICONTROL 每秒幀數(fps)]**  — 每秒視頻的幀數，或靜止影像的數量。在美國和日本，大部分視訊以 29.97 fps 拍攝；在歐洲和亞洲 (不包括日本)，大部分視訊以 25 fps 拍攝。電影以 24 fps 拍攝。

* **[!UICONTROL 音訊位元速率]**  — 編碼為構成一秒音訊播放的資料量（千位/秒）。

下表說明在選取視訊預設集及用來指定編碼檔案的命名慣例時建議的最佳實踐。

### 最適化視訊 (預設) {#adaptive-video-default}

編碼預設集，可與任何外觀比例搭配使用，以讓您為傳遞至行動裝置、平板電腦和桌上型電腦建立視訊。使用此預設集 (預設且最佳實踐) 編碼而上載的來源視訊會設為固定的高度，寬度則是會自動縮放，以保留視訊的外觀比例。

**最適化視訊 (預設)**

|  | 編碼預設集名稱/工具提示文字 | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 自動 x 360，800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 與來源同 | 64 | 適用行動裝置 (iPhone、iPad、Android™) |
| 2 | 自動 x 480，1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 與來源同 | 96 | 適用平板電腦 (iPad、Android™) |
| 3 | 自動 x 720，2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | 與來源同 | 128 | 案頭 |

### 最適化視訊編碼 (16:9 或 4:3) 視訊預設集 {#adaptive-video-encoding-or-video-presets}

這些最適化視訊編碼預設集，結合了一系列會根據您所上載之視訊的外觀比例自動為您選取的個別編碼預設集。例如，如果您上載 4:3 視訊，則系統會自動使用在「**最適化視訊編碼 (16:9 或 4:3)**」選項的主預設集清單中找到的五個 4:3 預設集進行編碼。

有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**最適化視訊編碼 (16:9 或 4:3) 預設集**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | 中等解析度、3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 800 | 384x288 | 與來源同 | 64 | 中等解析度、3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等解析度、WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | 與來源同 | 80 | 中等解析度、WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | 與來源同 | 96 | 高解析度、WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 與來源同 | 96 | 高解析度、WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | 與來源同 | 128 | 高畫質 |

### 桌上型電腦視訊編碼預設集 {#desktop-video-encoding-presets}

桌上型電腦之 MP4 與 OGV 的視訊編碼預設集。

如需有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**H264 主影像 3.2 - 音訊 AAC、MP4 副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9、480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9、640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9、800x450 (1200 Kbps) | 1.5 Mbps | _800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9、1280x720 (2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000年 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4:3、320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4:3、480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4:3、640x480 (1200 Kbps) | 1.5 Mbps | _640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4:3、1280x960 (2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000年 | 1280x960 | 與來源同 | 128 | 高畫質 |

**OGG Theora Vorbis - OGV 副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9、480x270 (400 Kbps)、OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9、640x360 (800 Kbps)、OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9、800x450 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9、1280x720 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000年 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4:3、320x240 (400 Kbps)、OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4:3、480x360 (800 Kbps)、OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4:3、640x480 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4:3、1280x960 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000年 | 1280x960 | 與來源同 | 128 | 高畫質 |

### 行動裝置視訊編碼預設集 {#mobile-video-encoding-presets}

與來源 fps 相同。iPhone、iPad和Android™行動裝置的視訊編碼預設集。

如需有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**H264 基線 2.1 - 音訊 AAC、MP4 副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊位元速率 (Kbps) | 像素寬度/高度 | Fps | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 3 | 16:9、512x288、行動裝置 (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | 16:9、512x288、行動裝置 (600 Kbps) | 700 | _Mobile_512x288_600K | 800 | 512x288 | 與來源同 | 64 | 中等解析度、3G |
| 3 | 16:9、512x288、行動裝置 (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 4 | 16:9、512x288、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 5 | 16:9、512x288、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | 與來源同 | 96 | 高解析度、Wi-Fi |
| 6 | 4:3、384x288、行動裝置 (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 7 | 4:3、384x288、行動裝置 (600 Kbps) | 700 | _Mobile_384x288_600K | 800 | 384x288 | 與來源同 | 64 | 中等解析度、3G |
| 8 | 4:3、448x336、行動裝置 (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 9 | 4:3、448x336、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 10 | 4:3、448x336、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | 與來源同 | 96 | 高解析度、Wi-Fi |

## 檢視器預設集 {#viewer-presets}

>[!NOTE]
>
>**Flash檢視器服務終止通知**  — 自2017年1月31日起，AdobeDynamic Media Classic正式終止支援Flash檢視器平台。

*檢視器預設集*&#x200B;是決定使用者如何在電腦螢幕和行動裝置上檢視多媒體資產的設定集合。身為一名管理員，您可以建立檢視器預設集。設定可用於檢視器設定選項的陣列。例如，您可以變更檢視器顯示大小、縮放行為、色彩方案、邊框和字型。

最佳作法是使用Dynamic Media Classic HTML5視訊檢視器。 HTML5 視訊檢視器使用的預設集是健全的視訊播放器。

合併為單一播放器，可執行下列動作：

* 使用HTML5和CSS設計播放元件的功能。
* 已嵌入播放。
* 視瀏覽器功能而定，使用最適化和漸進式串流。

您可以將多媒體內容的觸及範圍擴展至桌上型電腦、平板電腦和行動使用者，並確保簡化的視訊體驗。

請參閱Adobe檢視器參考指南中的[關於HTML5檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only)。

請參閱[Dynamic Media Classic檢視器預設集相容性矩陣](application-setup.md#scene7_viewer_preset_compatibility_matrix)。

請參閱[最佳實踐: 使用 HTML5 視訊檢視器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

依據檢視器而定，您可以增加社群功能。社群功能包含「內嵌」按鈕、「電子郵件」按鈕、「連結」按鈕和「造訪網站」按鈕。這些按鈕可讓使用檢視器的使用者與他人共用檢視器，或開啟Dynamic Media Classic網站。

另請參閱[Adobe檢視器參考程式庫範例](https://landing.adobe.com/tw/na/dynamic-media/ctir-2755/live-demos.html)。

### 回應式網頁的檢視器支援 {#viewer-support-for-responsive-designed-web-pages}

不同網頁有不同的需求。有時候，您會想要的網頁提供連結，可在個別瀏覽器視窗中開啟HTML5檢視器。 在其他情況下，則需直接將HTML5檢視器內嵌在托管頁面上。 在後一種情況下，網頁可能是靜態版面。 或者，它會「回應式」，並在不同裝置上或針對不同瀏覽器視窗大小顯示不同。 為符合這些需求，隨Dynamic Media Classic提供的HTML5檢視器，可同時支援靜態網頁和回應式設計網頁。

如需如何將回應式檢視器內嵌至網頁的詳細資訊，請參閱[關於回應式影像程式庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api)、[使用回應式影像程式庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api)及[命令參考 — 命令屬性](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library)。

### 檢視器預設集類型 {#viewer-preset-types}

管理員可以建立和自訂以下類型的檢視器預設集:

* **[!UICONTROL eCatalog Viewer]**  — 模擬閱讀已打印目錄的體驗。您可以在頁面之間移動、放大和縮小頁面上的項目、使用影像地圖來查看有關頁面上項目的詳細資訊，或搜尋目錄。 如果地圖區域擁有有效的 rollover_key 屬性，您也可以加入資訊面板以顯示詳細資訊和影像對應項目。若要加入資訊面板，請在「eCatalog 檢視器預設集」視窗中指定資訊伺服器 URL。

* **[!UICONTROL 色票集查看器]**  — 以不同的顏色、材料、紋理、光潔度或結構顯示影像。使用者選取縮圖以查看影像中的變化。

* **[!UICONTROL 混合媒體集檢視器]**  — 在一個檢視器中顯示不同類型的媒體。您可以加入色票集、迴轉集、影像和視訊。您可以設定標籤以包含不同類型的內容，例如影像集標籤和視訊標籤。從混合媒體集播放的視訊會使用含有時間軸和視訊控制項 (如「停止」、「暫停」、「倒轉」和「播放」) 的標準視訊檢視器。設定混合媒體集檢視器預設集時，請指定要針對混合媒體集中不同類型資產使用的檢視器。您也可以使用格線檢視器或轉盤檢視器來檢視混合媒體集。

* **[!UICONTROL 回轉集檢視器]**  — 提供影像的多個檢視，讓使用者可以轉動物件來檢查不同的側面和角度。

* **視訊檢視器**  — 使用來源檔案的解析度維度或自訂大小來顯示視訊。Dynamic Media Classic隨附許多預先定義的檢視器預設集，以供播放視訊，如果您是管理員，則可建立自訂視訊檢視器預設集。 有十幾種不同的設定可用於配置「視訊檢視器」。您可以設定其大小、前景和背景顏色、視訊和音訊控制項、進度列、使用者介面外觀、社交功能和「說明」。

* **[!UICONTROL 縮放檢視器]**  — 提供三種縮放檢視器的選擇：

* **[!UICONTROL 縮放檢視器]**  — 讓使用者透過選取區域來放大區域。它們可以選取控制項來放大、縮小和將影像重設為預設大小。

* **[!UICONTROL 縮放檢視器：飛出]**  — 在原始影像旁邊顯示縮放區域的第二個影像。沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。主要影像大小 (「舞台寬度」和「舞台高度」) 和「縮放係數」會決定彈出影像大小。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

### Dynamic Media Classic檢視器預設集相容性矩陣 {#scene-viewer-preset-compatibility-matrix}

**Flash檢視器生命週期結束通知**:自2017年1月31日起，AdobeDynamic Media Classic已正式停止支援Flash檢視器平台。

下表識別目前可用的Dynamic Media Classic檢視器預設集。 此表格也指定了檢視器與桌上型電腦和行動裝置的相容性，以及用於個別檢視器的技術。

另請參閱[Adobe檢視器參考程式庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

如需有關檢視器支援的 Web 瀏覽器和作業系統版本的資訊，您可以檢閱「檢視器發行說明」。

請參閱[Adobe檢視器參考發行說明](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 縮放檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 色票集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 檢視器 |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv（包含對社交媒體和目錄搜尋的支援）。 | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包括支援社交媒體和目錄搜尋）。 | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 迴轉檢視器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 檢視器**

Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。

* 您可以在以下位置找到支援此視頻格式的BlackBerry®設備：[BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)上支援的視頻格式
* 您也可以在以下位置找到支援此視頻格式的Windows®設備：[Windows® Phone](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)上支援的視訊格式

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 | BlackBerry®智慧手機 | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包括對隱藏式字幕的支援。） 請參閱[最佳實務：使用通用HTML5視訊檢視器。](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包括對隱藏式字幕和社交媒體的支援）。 | HTML5 | X | X | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒體集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支援的行動檢視器手勢矩陣 {#supported-mobile-viewers-gestures-matrix}

下表識別iOS、Android™ 2.x和Android™ 3.x裝置上支援的行動檢視器手勢。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 關於「檢視器預設集」畫面 {#about-the-viewer-preset-screen}

在「檢視器預設集」畫面建立和管理檢視器預設集。要開啟此螢幕，請轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。

「檢視器預設集」畫面提供了執行下列工作的工具:

* **新增預設集**  — 在「新增檢 **** 視器預設集」對話方塊中選取「新增」並進行選擇。

       請參閱[添加和編輯查看器預設集](application-setup.md#adding_and_editing_viewer_presets)。
   
* **編輯預設**  — 選取預設集，然後選取「編 **[!UICONTROL 輯」]**。

       請參閱[添加和編輯查看器預設集](application-setup.md#adding_and_editing_viewer_presets)。
   
* **刪除預設**  — 選取預設集，然後選取「刪 **[!UICONTROL 除」]**。

* **匯出預設集**  — 選取HTML5檢視器預設集，然後選取「匯 **** 出」以下載檢視器外觀，以便您能將其用作建立和新增其他檢視器預設集的基礎。

       請參閱[匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。
   
* **篩選檢視器預設集清單**  — 使用下列工具來篩選清單：

       *開啟**Active/Inactive**下拉式清單，並選取選項以顯示使用中的預設集、非使用中的預設集或所有預設集。
       *開啟**Viewer**下拉式清單，並選取選項以只檢視特定類型的檢視器。選擇**[!UICONTROL 所有查看器]**以查看所有查看器。
   
* **排序預設集**  — 選取欄標題(**[!UICONTROL 「作用中」]**、 **[!UICONTROL 「類型」]**、 **[!UICONTROL 「預設集」]**&#x200B;或 **[!UICONTROL 「平台」]**)，以排序欄上的清單。第二次選取欄標題，以遞減（或遞增）順序排序清單。

* **啟用和停用預設集**  — 選取預設集，然後選取其「使用中」選項以啟用或停用預設集。

       請參閱[啟用或停用檢視器預設集](application-setup.md#activating_or_diskivate_viewer_presets)。
   
>[!NOTE]
>
>選取「檢視器預設集」頁面右側的「**[!UICONTROL 預覽]**」 ，以便您在選取的檢視器預設集中查看資產的外觀。 若要查看不同的資產，請在「查看器預設集」頁中選擇&#x200B;**[!UICONTROL Browse]**，然後在「選擇資產預覽」對話框中選擇不同的資產。

### 新增和編輯檢視器預設集 {#adding-and-editing-viewer-presets}

除了在使用者介面中使用&#x200B;**[!UICONTROL Add]**&#x200B;來新增檢視器預設集外，您也可以使用&#x200B;**[!UICONTROL Export]**&#x200B;來新增檢視器預設集。 您只需匯出現有的HTML5檢視器預設集，然後使用該預設集作為新預設集的基礎。

請參閱[匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。

**增加和編輯檢視器預設集:**

1. 在Dynamic Media Classic的右上角附近，前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。

   您可以篩選預設集的清單。例如，若只要查看視訊檢視器的預設集，請從表格正上方工具列上的「檢視器」下拉式選單中選取「視訊檢視器」。

1. 在「查看器預設集」頁面中，在「查看器預設集」螢幕上添加或編輯「查看器預設集」。

   * **新增**  — 在工具列上選取「 **[!UICONTROL 新增]**」。在「新增檢視器預設集」對話方塊中，選取平台，然後選取多媒體資產類型。

          完成檢視器預設集的建立時，請選取**[!UICONTROL 「另存新檔」]**。
      
   * **從現有的檢視器預設集開始新增**  — 在表格中，選取「視訊檢視器預設集」，然後選取「編輯 **** 」工具列。

          重新設定視訊檢視器後，請選取**[!UICONTROL 「另存新檔」]**，在「預設集名稱」文字欄位中使用不同名稱儲存預設集。
      
   * **編輯**  — 選取現有的檢視器預設集，然後選取編 **[!UICONTROL 輯]**。

1. 在「設定檢視器」畫面的「預設集名稱」欄位中，輸入或編輯預設集名稱。
1. 設定其它想要的選項。

   >[!NOTE]
   >
   >選擇&#x200B;**[!UICONTROL 與源相同]**&#x200B;以自動將視頻查看器的大小調整為編碼視頻本身的解析度大小。 如果選擇此選項，則不能輸入舞台寬度和舞台高度。 相反，這些選項來自視訊本身。如果選擇「**[!UICONTROL 與源相同]**」，請設定「邊距大小」選項以反映視頻播放區域外的外觀尺寸。 該邊距大小是視訊控制項的像素高度和寬度。您可以使用下列影像來協助您決定要使用的邊界大小。*

   ![視訊檢視器的邊界設定](assets/vs_video_viewer_configure_margin.png)

1. 進行以下一項操作:

   * 如果您從現有預設集開始新增檢視器預設集，請選取「**[!UICONTROL 另存新檔」。]**
   * 如果您新增或編輯了檢視器預設集，請選取「**[!UICONTROL 儲存]**」。

### 匯出HTML5檢視器預設集 {#exporting-an-html-viewer-preset}

您可以匯出現有的HTML5檢視器預設集，以作為建立HTML5檢視器預設集的基礎。 匯出選項十分有用，因為您不需從頭建立檢視器， 但可以匯出與您要的外觀和行為接近的預設集，然後將其用作進行設計調整的起點。

Dynamic Media Classic中所有預設的現成檢視器預設集CSS檔案，都使用指向`Scene7SharedAssets`上資產的相對影像伺服路徑。 例如，以下是檢視器預設集CSS檔案中影像資產的相對路徑，位於

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

不過，如果您在自己的網站上托管檢視器CSS檔案，則必須透過在自己的環境中使用影像伺服器的明確路徑來解析這些相對影像路徑。 例如，如果要將上面的相對路徑更新為顯式路徑，則可能如下所示，其中`https://s7d1.scene7.com`是指向映像伺服器的直接路徑：`https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**要導出HTML5查看器預設集：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 檢視器預設集]**。
1. 在「查看器預設集」工具欄的左側第二個下拉清單中，選擇&#x200B;**[!UICONTROL HTML5]**。
1. 在左邊第三個下拉式清單中，選取&#x200B;**[!UICONTROL 所有檢視器]**。
1. 選取您要作為新HTML5檢視器預設集基礎的檢視器預設集。
1. 在工具欄中，選擇&#x200B;**[!UICONTROL Export]**。
1. 在「導出所選資產」對話框中，選擇&#x200B;**[!UICONTROL 提交導出]**。

   匯出後，您會取得CSS檔案。 下載並解壓縮檔案。

1. 在 CSS 編輯器中開啟 CSS 檔案，進行變更後儲存檔案。
1. 上傳CSS檔案至Dynamic Media Classic。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 將CSS檔案發佈至Dynamic Media影像伺服器。

   請參閱[發佈檔案](publishing-files.md#publishing_files)。

1. 照常增加檢視器預設集。選取您上傳的檢視器CSS檔案。

   請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

### 啟用或停用檢視器預設集 {#activating-or-deactivating-viewer-presets}

若要建立顯示資產的URL，使用者會在「預覽」對話方塊中開啟「預設集」下拉式清單，選取「檢視器預設集」，然後選取「**[!UICONTROL 複製URL]**」（請參閱「[複製檢視器預設集的URL](application-setup.md#copying_the_url_of_a_viewer_preset)」）。 預設集清單提供了管理員在「檢視器預設集」畫面所增加和管理的檢視器預設集。例如，使用者預覽 eCatalog 時，所有作用中的 eCatalog 檢視器預設集都會顯示在「預覽」對話框中的「預設集」下拉式清單中。

除非您在「檢視器預設集」畫面上停用檢視器預設集，否則「預覽」對話框中的「預設集」下拉式清單可能會過於擁擠。

**若要啟用或停用檢視器預設集，請執行下列動作：**

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 檢視器預設集]**。
1. 在「查看器預設集」頁上，選擇或取消選擇&#x200B;**[!UICONTROL 活動]**&#x200B;選項以激活或停用查看器預設集。

### 複製檢視器預設集的URL {#copying-the-url-of-a-viewer-preset}

發佈資產後，您就可以複製 URL，以「檢視器預設集」的設定來顯示資產。

URL 便會複製到剪貼簿。您可以視需要在網頁、行動裝置或應用程式的 HTML 代碼中加以使用。

**複製「檢視器預設集」的 URL:**

1. 在「瀏覽面板」中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」和「內嵌程式碼」面板中，選取您要檢視器右側的「複製URL ]**」 。**[!UICONTROL 
   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**。

   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL 複製URL]**。

   * 選擇&#x200B;**[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。
   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL 複製URL]**。

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**、**[!UICONTROL 清單視圖]**&#x200B;或&#x200B;**[!UICONTROL 詳細視圖]**。 在相同工具列上，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。
   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL 複製URL]**。

### 複製檢視器預設集的內嵌程式碼 {#copying-the-embed-code-of-a-viewer-preset}

您可使用「內嵌程式碼」功能查看所選「檢視器預設集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。

「內嵌代碼」對話方塊中不允許編 輯代碼 。

**複製檢視器預設集的內嵌程式碼:**

1. 在「資產瀏覽」面板中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」面板中，選取「**[!UICONTROL 內嵌程式碼]**」。
   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**。

   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

   * 選擇&#x200B;**[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。
   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**、**[!UICONTROL 清單視圖]**&#x200B;或&#x200B;**[!UICONTROL 詳細視圖]**。 在相同工具列上，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。
   在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

1. 在「內嵌代碼」對話方塊中，選取「**[!UICONTROL 複製到剪貼簿]**」。
1. 選擇&#x200B;**[!UICONTROL 關閉]**。

## 配置預設查看器 {#configuring-default-viewers}

使用「Dynamic Media Classic預覽」時，您可以使用「預設檢視器」來設定與資產相關聯的預設檢視器。 您可以針對下列資產類型設定預設的預覽體驗:

* 影像
* 視訊
* 迴轉集
* 目錄
* 影像集
* 色票集
* 媒體集

**設定預設檢視器:**

1. 在「設定」下拉清單中，選擇&#x200B;**[!UICONTROL 應用程式設定]**。
1. 在「設定」窗口中，在左窗格中，轉至「應用程式設定」 **[!UICONTROL >**[!UICONTROL  Viewers ]**]**
1. 選擇「**[!UICONTROL 預設查看器]**」。
1. 在「預設檢視器」視窗中，從每個資產類型下拉式清單中選取您要與資產預覽相關聯的檢視器。
1. 在「預設查看器」窗口的右下角，選擇「保存設定」****。
1. 在「設定」窗口的右下角，選擇&#x200B;**[!UICONTROL Close]**&#x200B;以返回「資產」窗口。

## 中繼資料檢視 {#metadata-views}

*中繼資料*&#x200B;是有關資產的標準化資料。您可以使用中繼資料來簡化工作流程、組織資產和改善搜尋。Dynamic Media Classic支援IPTC（國際新聞電信理事會）標準和XMP（可擴展元資料平台）標準。 使用者在「詳細資料」檢視中檢視或輸入資產的中繼資料之前，可以開啟「中繼資料檢視」功能表。 他們可以從中選取要檢視或用於說明資產的中繼資料欄位集。

Dynamic Media Classic隨附預先定義的中繼資料檢視，管理員可建立自己的中繼資料檢視，供使用者在輸入中繼資料時選擇。

### 建立中繼資料檢視 {#creating-a-metadata-view}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料視圖]**。
1. 選擇&#x200B;**[!UICONTROL 添加]**。
1. 在「預設集名稱」文字欄位中，輸入檢視的名稱。
1. （可選）勾選&#x200B;**[!UICONTROL 設定預設]**，讓此檢視成為使用者在詳細資料檢視中開啟中繼資料面板時看到的檢視。
1. （可選）選取&#x200B;**[!UICONTROL 包含UDF]**&#x200B;以在檢視中包含使用者定義的欄位。 使用者定義的欄位會顯示在詳細檢視的「中繼資料」面板上方。
1. 選擇要用於視圖的欄位（選擇&#x200B;**[!UICONTROL 全選]**&#x200B;以選擇所有欄位）。
1. 選擇&#x200B;**[!UICONTROL 保存]**。

   選取的檢視類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料檢視 {#managing-metadata-views}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料視圖]**。
1. 請執行下列任一動作:

   * 若要預覽檢視，請加以選取。檢視中的欄位會顯示在「預覽」面板中。
   * 要編輯視圖，請選擇它，然後選擇&#x200B;**[!UICONTROL Edit]**。 然後，在「預覽」面板上選擇或取消選擇欄位名稱，然後選擇或取消選擇&#x200B;**[!UICONTROL 包含UDF]**&#x200B;選項。
   * 要刪除視圖，請選擇它，然後選擇&#x200B;**[!UICONTROL Delete]**。
   * 要將視圖設定為預設視圖，請選擇它，然後選擇&#x200B;**[!UICONTROL Make Default]**。 預設檢視為使用者在詳細檢視中開啟資產，並前往「中繼資料」面板時所看見的檢視。

## 中繼資料預設集 {#metadata-presets}

中繼資料預設集讓管理員能夠控制和調節為資產指定的中繼資料。在詳細檢視中，使用者可以在輸入資產中繼資料專用的欄位中輸入資產的相關中繼資料。例如，使用者可以輸入擁有者名稱、版權描述和地址。為確保用戶準確完整地輸入此資訊，您可以建立元資料預設集。 在詳細檢視中選擇中繼資料預設集，會將預先定義的值填入中繼資料欄位。例如，擁有者名稱、版權描述和地址皆會自動輸入。

針對各個您要讓使用者能夠在詳細檢視中自動輸入以描述資產的中繼資料值集，建立中繼資料預設集。

### 建立或編輯中繼資料預設集 {#creating-or-editing-a-metadata-preset}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料預設集]**。
1. 在「中繼資料預設集」面板中，執行下列任一項作業:

   * 要建立預設，請選擇&#x200B;**[!UICONTROL Add]**。 在「中繼資料範本名稱」文字欄位中，輸入預設集的名稱。 選擇「**[!UICONTROL 元資料視圖]**」，然後從下拉清單中選擇視圖（請參閱[元資料視圖](application-setup.md#metadata_views)）。
   * 若要編輯現有預設，請從「元資料預設集」清單中選取預設集，然後選取「**[!UICONTROL 編輯]**」。

1. 展開您要加入預設集的標題，並在您要加入預設集的不同欄位中輸入值。
1. 選擇&#x200B;**[!UICONTROL 保存]**。

   選取的預設集類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料預設集 {#managing-metadata-presets}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料預設集]**。
1. 請執行下列任一動作:

   * 若要預覽預設集，請選取您要預覽的預設集。預設集資訊 (類別和欄位) 會顯示在「預覽」畫面中。
   * 若要刪除預設集，請選取預設集，然後選取&#x200B;**[!UICONTROL Delete]**。

## 使用者定義的欄位 {#user-defined-fields}

媒體入口網站管理員或公司管理員可建立自訂、使用者定義的中繼資料欄位。自訂欄位可協助您在Dynamic Media Classic中整理資產。 您可以視需要將欄位標示為「作用中」。 啟用時，這些自訂中繼資料欄位的名稱會顯示在詳細檢視的「中繼資料」面板中。使用者可以在使用者自訂的中繼資料欄位中輸入資訊，以描述資產。使用者也可以將使用者定義的中繼資料欄位設定作為搜尋條件。

使用者定義的中繼資料欄位的有效用途之一，就是針對特定的上市發表會或銷售會，延遲資產的啟用時間。根據&#x200B;*Date*&#x200B;類型定義「啟用」欄位。 然後，使用「詳細資訊」視圖或&#x200B;**[!UICONTROL File]** > **[!UICONTROL Edit Info]**&#x200B;中的&#x200B;**[!UICONTROL Metadata]**&#x200B;面板，可以指定資產啟動時間。 Dynamic Media Classic會檢查資產的發佈狀態，以及發佈歷史記錄。 如果未在啟動時間內，則發佈狀態會顯示為「未發佈」。

>[!NOTE]
>
>若要讓使用者定義的欄位顯示在詳細檢視的「中繼資料」面板中，請包含「中繼資料檢視」之使用者定義的欄位。在「中繼資料檢視」畫面上選取「包含 UDF」(使用者定義欄位) 選項。如需詳細資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views)。

>[!NOTE]
>
>若要使用自訂的使用者定義欄位來搜尋資產，請前往「**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**」，然後選取「在搜尋&#x200B;]**中包含UDF」。**[!UICONTROL &#x200B;請參閱[個人設定](personal-setup.md#personal_setup)。

### 建立使用者定義的中繼資料欄位 {#creating-a-user-defined-metadata-field}

1. 前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL 用戶定義欄位]**。
1. 選擇&#x200B;**[!UICONTROL 添加]**
1. 在「自訂欄位」對話框中，設定您要的選項。

   * **[!UICONTROL 名稱]**  — 輸入中繼資料欄位的名稱。

   * **[!UICONTROL 類型]**  — 選取一個選項，定義使用者可在中繼資料欄位中輸入的資訊類型：

   * **[!UICONTROL 字串]**  — 文字字串。

   * **[!UICONTROL Int]**  — 整數。

   * **[!UICONTROL 浮點]**  — 浮點數。

   * **[!UICONTROL 是/否]**  — 是/否布林值。

   * **[!UICONTROL 日期]**  — 日期。接受 MM/DD/YYYY 格式。

   * **[!UICONTROL 檔案名]**  — 檔案的名稱。

   * **[!UICONTROL 顏色]**  — 顏色的名稱。

   * **[!UICONTROL Dimension]**  — 資產的寬度和高度。

   * **[!UICONTROL 未輸入]**  — 用於回溯相容性。請勿選取此選項。

   * **[!UICONTROL 預設值]**  — （可選）在欄位中輸入用戶最可能輸入的值。您輸入的值會成為您建立之欄位的預設值。

   * **[!UICONTROL 套用至]**  — （可選）如果您希望中繼資料欄位僅套用至特定資產類型，請選取資產類型。

      >[!NOTE]
      >
      >請小心選取&#x200B;**[!UICONTROL 套用至]**&#x200B;選項，因為在建立使用者定義欄位後，您無法變更&#x200B;**[!UICONTROL 套用至]**&#x200B;選項。 Dynamic Media Classic可讓您編輯使用者定義欄位的名稱、類型和預設值，但不能編輯&#x200B;**[!UICONTROL Appled To]**&#x200B;設定。*

1. 完成元資料欄位的建立時，請選擇&#x200B;**[!UICONTROL 保存]**。

### 管理使用者定義的欄位 {#manage-user-defined-fields}

「使用者定義的欄位」畫面提供了管理自訂、使用者定義之中繼資料欄位的命令。

只有 Media Portal 管理員或公司管理員才可以管理使用者定義的欄位。

要開啟此螢幕，請轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**。

* **編輯欄位**  — 選取欄位，然後選取 **[!UICONTROL 編輯]**。

* **刪除欄位**  — 選取欄位，然後選取 **[!UICONTROL 刪除]**。

* **激活欄位**  — 選擇或取消選 **** 擇欄位名稱旁的「活動」選項。如果您處於公司管理角色，則不會顯示此選項。 由於此選項與MediaPortal相關，因此您必須在「個人設定」中選取（開啟）「顯示MediaPortal功能」 ，才能查看啟用欄位。

## 最佳化檔案 {#optimize-files}

當您將檔案上傳至Dynamic Media Classic時，系統會針對儲存和發佈最佳化這些檔案。 不過，如果上載程序受到中斷，部分影像就無法最佳化。在此情況下，您會看見「尚未最佳化影像」訊息。但是，如果您是管理員，就可以最佳化這些檔案。

Dynamic Media Classic會搜尋您的檔案，並僅最佳化之前未完全最佳化的影像。

1. 轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**，然後選擇&#x200B;**[!UICONTROL Optimize Files]**。
1. 輸入優化作業的資訊，然後選擇&#x200B;**[!UICONTROL Submit]**。

   如果您使用超過一家公司，請分別對屬於不同公司的檔案執行最佳化。

## 批次集預設集 {#batch-set-presets}

使用批次集預設集，在執行工作時自動建立影像集或回轉集，以將資產上傳至Dynamic Media Classic。

公司管理員會先定義要在集合中分組的資產的命名慣例。 然後，您可以建立批集預設集以參考這些影像。 每個預設集都是具備唯一名稱的內部獨立式指示集，定義如何使用與預設集配置中已定義的命名慣例相符的影像來建構集。

所有作用中的公司批次集預設集都會列在「上載工作選項」對話框中，以便您指定要在每個上載工作階段期間套用的預設集。公司管理員會看到所有作用中和非作用中的批次集預設集。上傳檔案時，Dynamic Media Classic會自動建立一組，其中包含所有符合使用中預設集中所定義命名慣例的檔案。

### 預設命名 {#default-naming}

公司管理員會建立任何批次集預設集配置中使用的預設命名慣例。在批集預設集定義中選擇的預設命名慣例可能是貴公司為所有網站批量生成集所需的全部。 必須建立批次集預設集，才能使用您所定義的預設命名慣例。公司定義的預設命名有例外情況時，您可以透過特定內容集所需的替代、自訂命名慣例來建立同等數量的批次集預設集。

使用批次集預設集功能不需要設定預設命名慣例。 但是，Adobe最佳實務建議您使用預設命名慣例，以定義要分組到一組中的命名慣例的多個元素。 這樣有助於簡化批集建立。

1. 轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**。
1. 選擇 **[!UICONTROL 「查看表單]** 」或「 **[!UICONTROL 查看代碼」]** ，以指定要查看的方式並輸入有關每個元素的資訊。

   您可以選取&#x200B;**[!UICONTROL 檢視程式碼]**&#x200B;核取方塊，檢視建立與表單選取項目一併的規則運算式值。 如果表單檢視因故對您有所限制，則您可以輸入或變更這些值，以幫助定義命名慣例的元素。如果無法在表單檢視中剖析您的值，表單欄位就會變成非作用中。

   >[!NOTE]
   >
   >停用的表單欄位不代表規則運算式無效。沒有驗證方式可確認您的規則運算式是否正確。在「結果」行之後，您會看見針對個別元素所建置之規則運算式的結果。您可以在頁面底部看到完整的規則運算式。

1. 視需要展開個別元素，並輸入您要使用的命名慣例。
1. 視需要選取&#x200B;**[!UICONTROL Add]** ，為元素新增其他命名慣例。 或者，選擇&#x200B;**[!UICONTROL Remove]**&#x200B;以刪除元素的命名慣例。
1. 選擇「**[!UICONTROL 另存為]**」並鍵入預設集的名稱。 或者，如果您正在編輯現有預設集，請選取&#x200B;**[!UICONTROL 儲存]**。

您也可以使用不含任何可用表單欄位的「檢視器碼」。在此檢視中，您可以完全使用規則運算式建立命名慣例定義。

有兩個元素可供定義，分別為「符合」和「基本名稱」。這些欄位可讓您定義所有命名慣例元素，並識別慣例中用來命名其中所含之集的部分。公司的個別命名慣例可能會針對每個元素使用一或多行定義。 您可以針對唯一定義使用同等數量的行，並將其分組至不同的元素，例如「主影像」、「色彩元素」、「替代檢視」元素和「色票」元素。

### 建立批次集預設集 {#creating-a-batch-set-preset}

Dynamic Media Classic使用批次集預設集，將共用一些常見資訊或內容的資產整理成一組影像，以便在檢視器中顯示。 批次集預設配方會隨您在Dynamic Media Classic中排程的資產匯入工作一起自動執行。

使用「批次集預設集」即可建立、編輯和管理批次集預設集。您可以視需要建立任意數量的預設集，以涵蓋您需要的所有資產擷取工作。 有兩種形式的批集預設集定義：一個是您已設定的預設命名慣例，另一個是您即時建立的自訂命名慣例。

您可以使用表單欄位方法來定義批次集預設集，或使用程式碼方法來使用規則運算式。 如同在&#x200B;**[!UICONTROL 預設命名]**&#x200B;中，您可以在表單檢視中定義的同時選取&#x200B;**[!UICONTROL 程式碼檢視]**，並使用規則運算式來建立定義。 您也可以取消核取任一檢視，僅使用其中一種。

另請參閱[建立批集預設集以自動生成2D回轉集](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)。

**建立批次集預設集:**

1. 轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設集]** > **[!UICONTROL 批集預設集]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設清單」面板中，選擇&#x200B;**[!UICONTROL Add]**&#x200B;以激活頁面右側「詳細資訊」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取預設集類型。

   若要自動產生 2D 迴轉集，請從「批次集類型」下拉式清單中選取「**[!UICONTROL 多軸旋轉集]**」。

1. 進行以下一項操作:

   * 如果您使用先前在&#x200B;**[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設集]** > **[!UICONTROL 預設命名]**&#x200B;下設定的預設命名慣例，請展開&#x200B;**[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取&#x200B;**[!UICONTROL 預設]**。
   * 若要在設定預設集時定義命名慣例，請展開&#x200B;**[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取&#x200B;**[!UICONTROL 自訂]**。

1. 對於「序列順序」，定義在集在Dynamic Media Classic中分組後的影像順序。 根據預設，您的資產會按照字母順序排列。不過，您可以使用規則運算式以逗號分隔的清單來定義順序。
1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。也可定義在Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 在「詳細資訊」面板中選擇&#x200B;**[!UICONTROL Save]**。

### 建立批集預設集以自動生成2D回轉集 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您也可以使用批次集類型「**多軸旋轉集**」來建立可自動產生 2D 迴轉集的「配置」。影像的群組會使用列與欄規則運算式，使影像資產適當對齊於多維度陣列中的對應位置上。

另請參閱[建立批集預設集](application-setup.md#creating_a_batch_set_preset)。

多軸迴轉集的列數或欄數沒有上限或下限。

例如，假設您想要建立名稱為 *spin-2dspin* 的多軸迴轉集。您有一組迴轉集影像，內有三列，每列有 12 個影像。影像的命名如下:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

使用此資訊，可以按如下方式建立批集類型處方：

![](assets/se_batch_set_recipe.png)

對回轉集的共用資產名稱部分進行分組會新增至「比對」欄位（如醒目提示）。 包含行和列的資產名稱的變數部分將分別添加到 行 和 列欄位中 。

上傳和發佈回轉集時，您會啟用「上傳工作選項」對話方塊中「批次集預設集」下方所列的2D回轉集 **[!UICONTROL 方式名稱]** 。

**建立批次集預設集以自動產生 2D 迴轉集:**

1. 轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設集]** > **[!UICONTROL 批集預設集]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設清單」面板中，選擇&#x200B;**[!UICONTROL Add]**&#x200B;以激活頁面右側「詳細資訊」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批集類型」下拉式功能表中，選擇「資產 **[!UICONTROL 集」]**。
1. 在「子類型」下拉式清單中，選取「**[!UICONTROL 多軸轉旋轉集]**」。
1. 展開&#x200B;**[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取&#x200B;**[!UICONTROL 自訂]**。
1. 使用「 **[!UICONTROL 比對]** 」(Match **[!UICONTROL )和 (可選) 「基本名稱]** 」(Base Name)屬性，定義組成群組之影像資產的命名規則運算式。

   例如，您的常值「比對」規則運算式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展開「**[!UICONTROL 列欄位置]**」，然後為影像資產在 2D 迴轉集陣列內的所在位置定義名稱格式。

   使用括號括住檔案名稱中的列或欄位置。

   例如，對於您的列規則運算式，它可能如下所示：

   `\w+-R([0-9]+)-\w+`

   或

   `\w+-(\d+)-\w+`

   對於欄規則運算式，可能如下所示：

   `\w+-\w+-C([0-9]+)`

   或

   `\w+-\w+-C(\d+)`

   請記住，這些運算式只是範例。 您可以用任何想要的方式建立規則運算式以符合自己的需求。

   >[!NOTE]
   >
   >如果列和列規則運算式的組合無法判斷資產在多維度回轉集陣列內的位置，則不會將該資產新增至該集，且會記錄錯誤。

1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。也可定義在Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 在「詳細資訊」面板中選擇&#x200B;**[!UICONTROL Save]**。
1. 如往常般上載並發佈您的迴轉集，過程中確定您在「工作載入選項」對話框的「批次集預設集」下啟用 2D 迴轉集的名稱。

>[!MORELIKETHIS]
>
>* [預覽資產](previewing-asset.md#previewing_an_asset)
* [設定影像預設集](setting-image-presets.md#setting_up_image_presets)
* [檢視、新增和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [檢查作業檔案](checking-job-files.md#checking_job_files)

