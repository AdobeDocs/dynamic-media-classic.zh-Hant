---
title: 應用程式設定
description: 瞭解如何設定和配置Adobe Dynamic Media Classic的應用程式區域。 「應用程式」區域允許您輸入常規設定、建立影像、查看器和視頻編碼預設、定義預設查看器和元資料、發佈設定和視頻SEO設定。 也可以使用區域設定批集預設，以自動生成2D旋轉集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '11299'
ht-degree: 40%

---

# 應用程式設定{#application-setup}

可以使用「應用程式設定」頁輸入常規設定、建立影像預設、視頻編碼預設、查看器預設或定義預設查看器和元資料。 您可以設定批集預設，以便還自動生成2D旋轉集（例如）、發佈設定和視頻SEO設定。

>[!NOTE]
>
>只有Adobe Dynamic Media Classic管理員才能更改「應用程式設定」頁上的設定。

## 一般設定 {#general-settings}

要開啟「應用程式一般設定」頁，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 常規設定]**。

### 伺服器

在建立帳戶時，Adobe Dynamic Media Classic會自動為您的公司提供指定的伺服器。 這些伺服器是用來為您的網站和應用程式建立 URL 字串。這些 URL 呼叫皆專屬於您的帳戶。

另請參閱 [Test安全測試服務](testing-assets-making-them-public.md#testing_the_secure_testing_service)。

* **[!UICONTROL 已發佈伺服器名稱]**  — 此伺服器是特定於您帳戶的所有系統生成URL調用中使用的即時CDN（內容分發網路）伺服器。 除非Adobe Dynamic Media Classic支援技術人員指示您更改此伺服器名稱，否則不要更改此伺服器名稱。

* **[!UICONTROL 源伺服器名稱]**  — 此伺服器僅用於質量保證測試。 除非Adobe Dynamic Media Classic支援技術人員指示更改此伺服器名稱，否則不要更改此伺服器名稱。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test目標伺服器名]**  — 您的Test目標URL，最多包括.com。 有關獲取此URL的說明，請參閱整合 [!DNL Adobe Dynamic Media Classic] 與 [!DNL Adobe Target Standard/Premium]。

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS流伺服器名稱]**  — 指向您的URL [!DNL Adobe Dynamic Media Classic] iOS流伺服器。 此伺服器會透過 HTTP 通訊協定將串流視訊傳送至以 iOS 為基礎的裝置。

* **[!UICONTROL 漸進視頻伺服器名稱]**  — 指向您的URL [!DNL Adobe Dynamic Media Classic] 漸進式視頻伺服器。 此伺服器會透過 HTTP 通訊協定來傳送漸進式視訊。

* **[!UICONTROL 顯示未發佈資產的URL]**  — 如果需要，請選擇此選項 [!DNL Adobe Dynamic Media Classic] 以在預覽任何資產時顯示URL，無論它是否已發佈。 如果資產尚未發佈，URL 將無法運作。不過，您可以使用 URL 來進行規劃或組織。

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN無效模板]**  — 指定用於使CDN（內容傳遞網路）快取失效的模板。

   例如，假設您輸入了引用的影像URL（包括影像預設或修飾符） `<ID>`，而不是像以下示例中所示的特定影像ID:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   如果模板僅包含 `<ID>`然後Adobe Dynamic Media Classic加入 `https://<server>/is/image`，也請參見Wiki頁。 `<server>` 是在常規設定中定義的發佈伺服器名稱。

   設定CDN無效模板，選擇名為Dackg_B的影像，然後轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 無效CDN]** 在CDN無效介面中生成以下生成的URL:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   在URL清單框中，選擇 **[!UICONTROL 繼續]** 清除該特定映像URL調用的快取。 也可以通過鍵入URL或將其貼上到URL清單框中來添加URL;您無需預先設定模板。

   選擇CDN無效模板並發出無效CDN請求後，用戶介面中會彈出一個指示器。 它會為您估計清除快取所需的時間。

   同樣，如果在Adobe Dynamic Media Classic內選擇了多個影像，則 **[!UICONTROL 檔案]** > **[!UICONTROL 無效CDN]**，每個影像都在保存的模板URL中引用。 因此，您可以定義一個CDN無效模板，該模板引用了網站上引用的每個URL（如產品詳細資訊和搜索結果）。 然後，在您從快取選取一或多個影像以使其失效時，URL 便會自動填入介面。

   請參閱[內容快取](dmc-platform-overview.md#content_caching)。

   請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

### 瀏覽

* **[!UICONTROL 顯示項目]**  — 確定項目是否可用作組織您的Adobe Dynamic Media Classic資產的一種方式。 請參閱 [組織您的項目工作](/help/organizing-projects.md)。

* **[!UICONTROL 顯示示例電子視頻內容]**  — 開啟或關閉eVideo示例內容的顯示。

* **[!UICONTROL 顯示生成的內容]**  — 在資料夾中，顯示從資產生成的內容。 例如，當PDF檔案在上載時柵格化時，Adobe Dynamic Media Classic會為原始PDF中的每個頁面建立一個影像。 如果選取了「顯示產生的內容」，則原始 PDF 上載時所產生的每個影像，都會與 PDF 一起出現在該 PDF 的上載檔案夾中。

* **[!UICONTROL 顯示編碼視頻]**  — 預設情況下取消選定（關閉）。

   要快速搜索和瀏覽Adobe Dynamic Media Classic的視頻，而無需瀏覽同一視頻的大量編碼衍生項，請取消選擇此選項（預設）。 僅顯示主視頻縮略圖（您上傳並用於建立衍生項的源視頻）和「父」自適應視頻集縮略圖（包含編碼視頻集的「子」衍生項）。

   但是，您仍然可以從主視頻或自適應視頻集訪問單個編碼視頻。 若要執行此項操作，請按兩下視訊縮圖影像，以開啟「詳細檢視」。然後選擇 **[!UICONTROL 編碼視頻]** 在右側面板中，以便您可以訪問所有「子」視頻。

   您也可以 **[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]** 直接從自適應視頻集建立更多編碼的「子」視頻。 Adobe Dynamic Media Classic會自動找到自適應視頻集的「父」主視頻，並將其用作源視頻進行轉碼。 不過，在您儲存新的個別編碼的視訊後，搜尋或瀏覽時並不會看到這些視訊。然而這些視訊仍可從「詳細檢視」的「編碼的視訊」標籤予以存取。

   請參閱 [上傳和轉碼視頻](uploading-encoding-videos.md#uploading_and_encoding_videos)。

   若要繼續能夠在搜尋和瀏覽時存取所有編碼視訊的衍生物，請選取「**[!UICONTROL 顯示編碼的視訊]**」。

   「建置」選單上的某些動作只能用於個別視訊，或選擇性地用於個別視訊。此功能迫使您必須顯示所有可以選取之編碼視訊的衍生物，而不受您設定「**[!UICONTROL 顯示編碼的視訊]**」的方式影響。過載的生成操作 **[!UICONTROL 顯示編碼視頻]** 設定包 **[!UICONTROL 自適應視頻集]**, **[!UICONTROL 電子目錄]**。

   >[!NOTE]
   >
   >如果您沒有使用Adobe Dynamic Media Classic來上傳和編碼視頻資產，Adobe Dynamic Media Classic會顯示您所有單獨編碼的視頻，即使取消選擇了此選項。

* **[!UICONTROL 「顯示刷新子資料夾」按鈕]**  — 開啟或關閉子資料夾「刷新」按鈕的顯示。

### Adobe Dynamic Media ClassicFTP帳戶

* **[!UICONTROL 伺服器]**  — 列出FTP帳戶伺服器。

* **[!UICONTROL 用戶名]**  — 列出FTP帳戶用戶名。

### 上載至應用程式

另請參閱 [預設上載作業選項](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) 培訓視頻。

* **[!UICONTROL 覆蓋影像]** -Adobe Dynamic Media Classic不允許兩個檔案具有相同的名稱。 每個項的Adobe Dynamic Media ClassicID（映像名稱減去檔案副檔名）必須唯一。 因為此規則，所以「上載」對話框擁有「覆寫」選項。此選項的確實效果取決於指定的「覆寫影像」選項。這些選項會指定取代影像的上載方式: 取代原始影像或成為重複影像。重複影像將會以「-1」重新命名 (例如，chair.tif 會重新命名為 chair-1.tif)。這些選項會影響上載至非原始檔案夾的影像，或擁有非原始副檔名 (例如 JPG、TIF 或 PNG) 的影像。請參閱 [使用「覆蓋影像」選項](#using-the-overwrite-images-option)。

   * **[!UICONTROL 在當前資料夾中覆蓋，相同的基本映像名稱/副檔名]**  — 此選項是最嚴格的替換規則。 它會要求您將取代影像上載至與原始影像相同的檔案夾，且取代影像必須與原始檔案擁有相同的副檔名。如果未符合這些要求，便會建立重複項目。

   * **[!UICONTROL 在當前資料夾中覆蓋，無論副檔名如何，均使用相同的基本資產名稱]**  — 要求將替換映像上載到與原始映像相同的資料夾，但檔案副檔名可能與原始映像不同。 例如，chair.tif 會取代 chair.jpg。

   * **[!UICONTROL 在任何資料夾中覆蓋相同的基本資產名稱/副檔名]**  — 要求替換影像與原始影像具有相同的檔案副檔名（例如，chair.jpg必須替換chair.jpg，而不是chair.tif）。 然而，您可以將取代影像上載至與原始影像不同的檔案夾。上載的影像將會位於新檔案夾中；無法再於原始位置中找到該檔案

   * **[!UICONTROL 在任意資料夾中覆蓋相同的基本資產名稱，而不考慮副檔名]**  — 此選項是最包容的替換規則。 您可以將取代影像上載至非原始檔案夾、上載擁有不同副檔名的檔案，以及取代原始檔案。如果原始檔案位於不同檔案夾，則取代影像會位於其上載的新目標檔案夾中。

* **[!UICONTROL 保留發佈]**  — 指定上載到Adobe Dynamic Media Classic的替換映像是保留其正在替換的映像的「準備發佈」設定，還是在上載時指定了該設定。

* **[!UICONTROL 預設顏色配置檔案]**  — 指定在添加CMYK影像時作為預設顏色配置檔案選項的一部分應用的顏色配置檔案。

* **[!UICONTROL 預設上載選項]**  — 開啟「上載作業選項」對話框，可在其中指定預設上載選項。 如需有關這些選項的詳細資訊，請參閱[上載選項](/help/uploading-files.md#upload_options)。

### 應用程式的影像地圖編輯器

* **[!UICONTROL 預設映像映射HREF]**  — 定義用於映射影像中HREF列的預設URL。 此URL是建立映像映射時看到的預設URL。

* **[!UICONTROL 預設映像映射模板]**  — 定義映射中HREF模板的預設JavaScript。 您可以在此處設定自定義代碼，以便在選擇映像映射時運行。

### 應用程式的其他設定

* **[!UICONTROL 垃圾可清除警告]**  — 垃圾箱中的資產在七天內自動移走。 如果您要在永久刪除「垃圾桶」之資產的前四天傳送通知至公司管理員，請選取「在自動刪除垃圾桶項目前傳送電子郵件」。請參閱 [管理垃圾資料夾](/help/trash-folder.md)。

## 使用「覆蓋影像」選項 {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic不允許兩個檔案同名。 每個項的Adobe Dynamic Media ClassicID（映像名稱減去檔案副檔名）必須唯一。 因為此規則，所以「上載」對話框包含「覆寫影像」選項。此選項的確切效果取決於每家公司的Adobe Dynamic Media Classic內部設定的設定。

如果您以前上傳了影像，然後更改了原始檔案（或替換了它們），則選擇的「覆蓋」選項指定了Adobe Dynamic Media Classic如何替換影像。 影像的任何相關資訊都不會變更，但新的影像會取代舊影像。如果資料夾中還包含不在Adobe Dynamic Media Classic的影像，則會添加這些影像。

如果已上載的影像在某種方式上發生了更改（影像已經更改），但對影像的引用保持不變，則使用此選項。 上載和擷取 Adobe® PDF 檔案時，覆寫功能也很有幫助。對Adobe Dynamic Media Classic *脊* 影像中，調整「上載」(Upload)對話框中的「ICC顏色」(ICC color)配置檔案選項，並使用「覆蓋」(Overwrite)功能重新上載。

用於從生產伺服器訪問影像的Adobe Dynamic Media ClassicID從影像檔案名派生。 在檔案名中使用大寫和小寫字元非常重要，無論是在替換現有檔案時，還是在用於訪問影像的Adobe Dynamic Media ClassicID中都是如此。 在上載到Adobe Dynamic Media Classic之前，請確保檔案名中使用大寫和小寫字元的正確性，以避免只對同一影像使用大小寫不同的Adobe Dynamic Media ClassicID。

如果取消選取此選項，所有與現存影像擁有相同檔案名稱的影像都會視為重複項目，而不會增加。

## 影像預設集 {#image-presets}

「影像預設集」畫面是用來建立和編輯影像預設集。「影像預設」使Adobe Dynamic Media Classic能夠以不同大小動態傳送來自同一主映像的影像。 每個影像預設集都代表了一個用來顯示影像之大小調整與格式命令的預先定義集合。建立「影像預設」時，將選擇影像傳送的大小。 您還可以選擇格式命令，以便在傳送影像以供查看時優化影像的外觀。

管理員可以建立匯出資產用的預設集。用戶在導出影像時可以選擇預設，這也會按照管理員指定的規範重新格式化影像。

要開啟「影像預設」螢幕，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設]**。

請參閱 [智慧映像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic)。

### 建立和編輯影像預設集 {#creating-and-editing-image-presets}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設]**。
1. 建立預設或從現有預設開始：

   * **建立影像預設**  — 選擇 **[!UICONTROL 添加]**。
   * **從現有預設建立影像預設**  — 選擇最類似於要建立的影像預設，然後選擇 **[!UICONTROL 編輯]**。

1. 在「添加（或編輯）預設」頁面上，輸入預設的名稱。
1. 設定您想要的預設集選項。

   請參閱[影像預設集選項](application-setup.md#image_preset_options)。

1. 選擇 **[!UICONTROL 保存]**，或從現有預設開始，選擇 **[!UICONTROL 另存為]**。
1. 要使用您自己的影像預覽預設，請選擇 **[!UICONTROL 瀏覽]** ，然後選擇影像。 要使用預設影像預覽，請選擇 **[!UICONTROL 重置]**。

通過在「影像預設」螢幕上選擇影像預設的名稱，然後選擇 **[!UICONTROL 編輯]**。 要刪除「影像預設」，請選擇它，然後選擇 **[!UICONTROL 刪除]**。

### 影像預設集選項 {#image-preset-options}

「增加預設集」和「編輯預設集」畫面提供下列選項，以建立和編輯影像預設集:

* **[!UICONTROL 預設名稱]**  — 輸入不帶空格的描述性名稱。 要幫助用戶識別此影像預設，請在名稱中包括影像大小規範。

* **[!UICONTROL 寬度和高度]**  — 以像素為單位輸入影像傳送的大小。

* **[!UICONTROL 格式]**  — 從菜單中選擇格式。 選擇GIF、JPEG、PDF或TIFF格式會顯示更多選項：

   * GIF 色彩量化選項

      * **[!UICONTROL 類型]**  — 選擇「自適應」（預設）、「Web」或「Macintosh」。 如果選擇 **[!UICONTROL 帶Alpha的GIF]**, Macintosh選項不可用。

      * **[!UICONTROL 抖動]**  — 選擇「擴散」或「關閉」。

      * **[!UICONTROL 顏色數]**  — 拖動滑塊以輸入2-255。

      * **[!UICONTROL 顏色清單]**  — 輸入逗號分隔的清單。 例如，對於白、灰和黑，請輸入 `000000,888888,ffffff`.
   * JPEG 選項

      * **[!UICONTROL 質量]**  — 控制JPEG壓縮級別。 這個設定會同時影響檔案大小與影像品質。JPEG質量等級為1-100。

      * **[!UICONTROL 啟用JPG色度下採樣]**  — 由於眼睛對高頻顏色資訊的敏感度低於高頻亮度，JPEG影像將影像資訊分為亮度和顏色分量。 壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣可將資料量減少三分之一或二分之一，而且幾乎不會影響肉眼能感知的品質。縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。
   * PDF 和 TIFF 選項

      * **[!UICONTROL 壓縮]**  — 選擇壓縮算法。



* **[!UICONTROL 色彩空間]**  — 選擇顏色空間。

* **[!UICONTROL 銳化]**  — 選擇「啟用簡單銳化」選項，以便在進行所有縮放後將基本銳化濾鏡應用於影像。 銳利化可以幫助補償以不同大小顯示影像時所造成的模糊現象。

   有關銳化、重新取樣模式和反銳化蒙版的詳細資訊，請參見 [銳化影像](sharpening-image.md#sharpening_an_image)。 另請參閱 [銳化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 培訓視頻。

* **[!UICONTROL 重新取樣模式]**  — 選擇重新取樣模式選項。 下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL B線性]**  — 最快的重採樣方法；有些鋸齒偽影是可以察覺的。

* **[!UICONTROL 雙立方]**  — 提高影像伺服器上的CPU使用率，但生成更清晰的影像，並減少明顯的鋸齒偽像。

* **[!UICONTROL 夏普2]**  — 比Bi-Cubic選項產生的結果略為尖銳，但映像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 使用較高和較低解析度（如果可用）;僅在出現混淆時建議。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

* **[!UICONTROL 反銳化掩碼]**  — 選擇以下選項以微調銳化：

* **[!UICONTROL 金額]**  — 控制應用於邊緣像素的對比度量。 預設是 1.0。對於高解析度的影像，您最多可以將它增加至 5.0。將「數量」視為濾鏡飽和度的度量。

* **[!UICONTROL 半徑]**  — 確定影響銳化的邊緣像素周圍的像素數。 對於高解析度的影像，請輸入 1 到 2 的數字。低數值只會銳利化邊緣的像素；高數值會銳利化較寬的像素範圍。正確的值取決於影像大小。

* **[!UICONTROL 閾值]**  — 確定應用非銳化蒙版濾鏡時要忽略的對比度範圍。 換句話說，這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。為了避免產生雜訊，請使用介於 .02 與 0.2 之間的值來實驗。預設值 6 會對影像中的所有像素進行銳利化。

* **[!UICONTROL 顏色空間]**  — 確定影像是使用建立影像的空間，通常是RGB（原始）還是亮度空間（強度）。

* **[!UICONTROL 顏色]** 選擇以下選項：

* **[!UICONTROL 輸出顏色配置檔案]**  — 選擇 **[!UICONTROL 使用預設值]** 或者Adobe Dynamic Media Classic上的ICC顏色配置檔案。

   請另參閱 [ICC 設定檔](icc-profiles.md#icc_profiles)。

* **[!UICONTROL 渲染意圖]**  — 如果要覆蓋顏色配置檔案的預設渲染方式，請選擇一個選項。 當預設ICC配置檔案之一是顏色轉換的目標顏色空間時，使用此選項。 或者，輸出設備（打印機或監視器）的特徵是此配置檔案，並且指定的渲染意圖對此配置檔案有效。

* **[!UICONTROL 嵌入配置檔案]**  — 選擇此選項，如果在Adobe®Photoshop®中開啟此映像，則它將使用此配置檔案。

* **[!UICONTROL 打印解析度]**  — 選擇打印此影像的解析度；預設為72像素。

* **[!UICONTROL URL修飾符]**  — 如果您更願意指定定義「影像預設」的URL修飾符，而不是設定，請在此處輸入修飾符。

* **[!UICONTROL 示例影像URL]**  — 列出Dynamic Media影像伺服器用於傳遞包含您添加或編輯的影像預設的影像的「原始」URL字串。 此URL字串對您在「添加預設」或「編輯預設」螢幕中選擇的所有格式設定進行編碼。

### 編輯、刪除或停用影像預設 {#editing-removing-or-deactivating-an-image-preset}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設]**。
1. 在「影像預設集」畫面中，選取表格中的預設集，然後執行以下一項操作:

   * 選擇 **[!UICONTROL 編輯]** 然後在「編輯預設」對話框中指定新選項。
   * 選擇 **[!UICONTROL 刪除]** 從清單中刪除預設。
   * 取消選擇 **[!UICONTROL 活動]** 如果要從MediaPortal用戶的整個Adobe Dynamic Media Classic用戶介面中刪除預設名稱，請選中該預設名稱旁邊的複選框。

## 激活或停用自適應視頻預設 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic提供自適應視頻編碼預設。 它是預設的主清單，它將16:9自適應視頻預設和4:3自適應視頻預設組合到一個組中。 這些預先定義的預設集反映了最常見的編碼設定，並已針對目標行動裝置、平板電腦和桌上型電腦的播放進行最佳化。

預設只會啟動 (啟用或「開啟」)「最適化視訊」編碼預設集。您可以視需要加以停用。非作用中的最適化視訊預設集，並不會以可選取的選項顯示在「上載工作選項」對話框的「eVideo」區段中。

請參閱 [上傳和編碼視頻](uploading-encoding-videos.md#uploading_and_encoding_videos)。

另請參閱 [視頻預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 培訓視頻。

**啟用或停用最適化視訊預設集:**

1. 在Adobe Dynamic Media Classic右上角，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視頻預設]** > **[!UICONTROL 自適應視頻預設]**。
1. 在「最適化視訊預設集」頁面上，取消選取預設集名稱旁邊的核取方框，以從「上載工作選項」對話框的「eVideo 選項」清單中移除預設集。
1. 選擇 **[!UICONTROL 關閉]**。

## 編碼視訊檔案的視訊預設集 {#video-presets-for-encoding-video-files}

要選擇編碼預設，請在「上載」頁的右下角選擇 **[!UICONTROL 作業選項]**。 在「上載作業選項」對話框中，展開「視頻選項」，然後選擇所需的視頻編碼預設。

>[!NOTE]
>
>除了預設啟用的「自適應視頻」外，您無法在「上載作業選項」對話框中看到所有其他自適應視頻或單個視頻編碼預設。 Adobe Dynamic Media Classic管理員確定在「上載作業選項」對話框中可以看到哪些視頻編碼預設。

* 從以下自適應視頻編碼或單個編碼預設中選擇：

   * **[!UICONTROL 16:9自適應視頻]**  — 建立16:9寬高比視頻，以交付到台式機、移動設備(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並使用與查看器連接速度最匹配的解析度和比特率進行優化。

   * **[!UICONTROL 4:3自適應視頻]**  — 建立4:3寬高比視頻，以交付到台式機、移動設備(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並使用與查看器連接速度最匹配的解析度和比特率進行優化。

   * **[!UICONTROL 自適應視頻]**  — 單個編碼預設，可與任意縱橫比配合使用，以建立視頻，以交付到移動、平板和案頭。 使用此預設集編碼而上載的來源視訊，會設定成固定的高度。不過，寬度會自動調整為保留視訊的外觀比例。

      具有「自動縮放」的彈性預設也會在您建立自己的自訂視訊編碼預設集時可供使用。

      請參閱 [添加或編輯視頻編碼預設](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)。

   * **[!UICONTROL 自適應視頻編碼（16:9或4:3）]**  — 建立16:9和4:3寬高比視頻，以交付到台式機、移動設備(iPhone、iPad、Android™)和平板電腦(iPad、Android™)。 所有這些都使用與查看器連接速度最匹配的解析度和比特率進行優化。

      請參閱[最適化視訊編碼 (16:9 或 4:3) 視訊預設集](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   * **[!UICONTROL 單一編碼預設集]**

      >[!NOTE]
      >
      >要向iPad傳送視頻，您可以選擇移動編碼預設或平板電腦編碼預設。 平板電腦預設集專為 iPad 而設計，通常具有更高的解析度和品質，以充分利用更大的畫面和頻寬連線。傳送使用平板電腦預設集編碼的視訊檔案時，必須在您的行動裝置網站或應用程式上加入裝置偵測程式碼。此程式碼會根據播放裝置的不同，在 iPhone 或 iPad 視訊體驗間切換。更簡單的工作流程是選擇行動裝置預設集將視訊檔案傳送到 iPad。原因在於您可以將同一視訊檔案用於 iPhone 和 iPad。但是，將品質標準化為解析度更低的 iPhone 體驗。

      * 在「編碼預設集」群組下方的「排序編碼預設集」下拉式清單中，選取要依據名稱或解析度大小來排序預設集時的「名稱」或「大小」。
      * 根據計畫播放視頻的解析度大小和頻寬選擇編碼預設。
      * 可以選擇「自適應視頻編碼」和每個視頻的一個或多個編碼預設。 例如，您可以在一個上載工作中針對桌面和行動裝置編碼檔案。

選擇後 **[!UICONTROL 開始上載]**，上載原始主視頻檔案，並從主檔案生成編碼檔案。

### 關於編碼預設集選項 {#about-encoding-preset-options}

編碼預設集選項的參數如下:

* **[!UICONTROL 目標連接速度]**  — 目標最終用戶的Internet連接速度。

* **[!UICONTROL 編碼檔案尾碼]**  — 附加到編碼視頻檔案以用於標識目的的尾碼。

* **[!UICONTROL 視頻比特率（資料速率）]**  — 編碼以構成視頻回放一秒的資料量（千比特/秒）。

* **[!UICONTROL 像素寬度/高度]**  — 螢幕影像的寬度尺寸（以像素為單位）;螢幕影像的高度尺寸（以像素為單位）。

* **[!UICONTROL 每秒幀數(fps)]**  — 每秒視頻的幀數或靜止影像數。 在美國和日本，大部分視訊以 29.97 fps 拍攝；在歐洲和亞洲 (不包括日本)，大部分視訊以 25 fps 拍攝。電影以 24 fps 拍攝。

* **[!UICONTROL 音頻比特率]**  — 編碼以構成每秒千比特音頻播放的每秒資料量。

下表說明在選取視訊預設集及用來指定編碼檔案的命名慣例時建議的最佳實踐。

### 最適化視訊 (預設) {#adaptive-video-default}

編碼預設集，可與任何外觀比例搭配使用，以讓您為傳遞至行動裝置、平板電腦和桌上型電腦建立視訊。使用此預設集 (預設且最佳實踐) 編碼而上載的來源視訊會設為固定的高度，寬度則是會自動縮放，以保留視訊的外觀比例。

**最適化視訊 (預設)**

|  | 編碼預設集名稱/工具提示文字 | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 自動 x 360，800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 與來源同 | 64 | 適用行動裝置 (iPhone、iPad、Android™) |
| 2 | 自動 x 480，1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 與來源同 | 96 | 適用平板電腦 (iPad、Android™) |
| 3 | 自動 x 720，2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | 與來源同 | 128 | 對於案頭 |

### 最適化視訊編碼 (16:9 或 4:3) 視訊預設集 {#adaptive-video-encoding-or-video-presets}

這些最適化視訊編碼預設集，結合了一系列會根據您所上載之視訊的外觀比例自動為您選取的個別編碼預設集。例如，如果上載4:3視頻，則會使用在主預設清單中找到的所有五個4:3預設自動編碼 **自適應視頻編碼（16:9或4:3）** 的雙曲餘切值。

有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**最適化視訊編碼 (16:9 或 4:3) 預設集**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | 中等解析度、3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | 與來源同 | 64 | 中等解析度、3G |
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
| 1 | 16:9、480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9、640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9、800x450 (1200 Kbps) | 1.5 Mbps | _800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9、1280x720 (2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4:3、320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4:3、480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4:3、640x480 (1200 Kbps) | 1.5 Mbps | _640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4:3、1280x960 (2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000 | 1280x960 | 與來源同 | 128 | 高畫質 |

**OGG Theora Vorbis - OGV 副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps)、OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 與來源同 | 64 | 低階寬螢幕解析度 |
| 2 | 16:9、640x360 (800 Kbps)、OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等寬螢幕解析度 |
| 3 | 16:9、800x450 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 與來源同 | 96 | 中高解析度 |
| 4 | 16:9、1280x720 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 5 | 4:3、320x240 (400 Kbps)、OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 與來源同 | 64 | 低解析度 |
| 6 | 4:3、480x360 (800 Kbps)、OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 與來源同 | 80 | 中等解析度 |
| 7 | 4:3、640x480 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 與來源同 | 96 | 中高解析度 |
| 8 | 4:3、1280x960 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | 與來源同 | 128 | 高畫質 |

### 行動裝置視訊編碼預設集 {#mobile-video-encoding-presets}

與來源 fps 相同。iPhone、iPad和Android™移動設備的視頻編碼預設。

如需有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**H264 基線 2.1 - 音訊 AAC、MP4 副檔名**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊位元速率 (Kbps) | 像素寬度/高度 | Fps | 音訊位元速率 (Kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、512x288、行動裝置 (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | 16:9、512x288、行動裝置 (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | 中等解析度、3G |
| 3 | 16:9、512x288、行動裝置 (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 4 | 16:9、512x288、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 5 | 16:9、512x288、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | 與來源同 | 96 | 高解析度、Wi-Fi |
| 6 | 4:3、384x288、行動裝置 (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 7 | 4:3、384x288、行動裝置 (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | 與來源同 | 64 | 中等解析度、3G |
| 8 | 4:3、448x336、行動裝置 (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | 與來源同 | 80 | 中等解析度、Wi-Fi |
| 9 | 4:3、448x336、行動裝置 (1000 Kbps) | 1.2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | 與來源同 | 80 | 高解析度、Wi-Fi |
| 10 | 4:3、448x336、行動裝置 (1200 Kbps) | 1.5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | 與來源同 | 96 | 高解析度、Wi-Fi |

## 檢視器預設集 {#viewer-presets}

>[!NOTE]
>
>**Flash查看者生命結束通知**  — 自2017年1月31日起，Adobe Dynamic Media Classic正式終止對Flash觀看平台的支援。

*檢視器預設集*&#x200B;是決定使用者如何在電腦螢幕和行動裝置上檢視多媒體資產的設定集合。身為一名管理員，您可以建立檢視器預設集。設定可用於檢視器設定選項的陣列。例如，您可以變更檢視器顯示大小、縮放行為、色彩方案、邊框和字型。

最好使用Adobe Dynamic Media ClassicHTML5視頻觀看器。 HTML5 視訊檢視器使用的預設集是健全的視訊播放器。

通過組合成單個玩家，可以執行以下操作：

* 使用HTML5和CSS設計回放元件的能力。
* 嵌入式播放。
* 根據瀏覽器的功能使用自適應和漸進式流。

您可以將富媒體內容擴展到案頭、平板電腦和移動用戶，並確保獲得簡化的視頻體驗。

請參閱 [關於HTML5查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) 的下界。

請參閱 [Adobe Dynamic Media Classic查看器預設相容性矩陣](application-setup.md#scene7_viewer_preset_compatibility_matrix)。

請參閱[最佳實踐: 使用 HTML5 視訊檢視器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

依據檢視器而定，您可以增加社群功能。社群功能包含「內嵌」按鈕、「電子郵件」按鈕、「連結」按鈕和「造訪網站」按鈕。這些按鈕使使用瀏覽器的用戶可以與其他人共用瀏覽器或開啟Adobe Dynamic Media Classic網站。

另請參閱 [Adobe查看器參考庫示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

### 對響應性設計的網頁的查看器支援 {#viewer-support-for-responsive-designed-web-pages}

不同網頁有不同的需求。有時，您需要一個網頁，該網頁提供在單獨的瀏覽器窗口中開啟HTML5查看器的連結。 在其它情況下，需要將HTML5查看器直接嵌入到托管頁面。 在後一種情況下，網頁可能具有靜態佈局。 或者，它「響應」，在不同設備上或不同瀏覽器窗口大小時顯示不同。 為了滿足這些需求，隨Adobe Dynamic Media Classic提供的HTML5瀏覽器支援靜態網頁和響應性設計的網頁。

有關如何將響應式查看器嵌入到網頁的詳細資訊，請參閱 [關於響應映像庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api)。 [使用響應映像庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api), [命令引用 — 命令屬性](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library)。

### 檢視器預設集類型 {#viewer-preset-types}

管理員可以建立和自訂以下類型的檢視器預設集:

* **[!UICONTROL eCatalog查看器]**  — 模擬閱讀打印目錄的體驗。 您可以在頁面之間移動、放大和縮小頁面上的項目、使用影像映射查看有關頁面上項目的詳細資訊或搜索目錄。 如果地圖區域擁有有效的 rollover_key 屬性，您也可以加入資訊面板以顯示詳細資訊和影像對應項目。若要加入資訊面板，請在「eCatalog 檢視器預設集」視窗中指定資訊伺服器 URL。

* **[!UICONTROL 色板集查看器]**  — 以不同的顏色、材料、紋理、光潔度或織物顯示影像。 用戶選擇縮略圖以查看影像中的變體。

* **[!UICONTROL 混合媒體集查看器]**  — 在一個查看器中顯示不同類型的媒體。 您可以加入色票集、迴轉集、影像和視訊。您可以設定標籤以包含不同類型的內容，例如影像集標籤和視訊標籤。從混合媒體集播放的視訊會使用含有時間軸和視訊控制項 (如「停止」、「暫停」、「倒轉」和「播放」) 的標準視訊檢視器。設定混合媒體集檢視器預設集時，請指定要針對混合媒體集中不同類型資產使用的檢視器。您也可以使用格線檢視器或轉盤檢視器來檢視混合媒體集。

* **[!UICONTROL 旋轉集查看器]**  — 提供影像的多個視圖，以便用戶能夠轉動對象檢查不同的側面和角度。

* **視頻查看器**  — 使用源檔案的解析度尺寸或自定義大小顯示視頻。 Adobe Dynamic Media Classic提供了許多用於播放視頻的預定義查看器預設，如果您是管理員，則可以建立自定義視頻查看器預設。 配置視頻查看器時有12種以上不同的設定。 您可以設定其大小、前景和背景顏色、視訊和音訊控制項、進度列、使用者介面外觀、社交功能和「說明」。

* **[!UICONTROL 縮放查看器]**  — 提供三種縮放查看器：

* **[!UICONTROL 縮放查看器]**  — 允許用戶通過選擇區域來放大區域。 它們可以選擇控制項以放大、縮小和將影像重置為其預設大小。

* **[!UICONTROL 縮放查看器：飛出]**  — 在原始影像旁顯示縮放區域的第二個影像。 沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。主要影像大小 (「舞台寬度」和「舞台高度」) 和「縮放係數」會決定彈出影像大小。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

### Adobe Dynamic Media Classic查看器預設相容性矩陣 {#scene-viewer-preset-compatibility-matrix}

**Flash查看者生命結束通知**:自2017年1月31日起，Adobe Dynamic Media Classic正式終止對Flash觀看平台的支援。

下表標識了當前可用的Adobe Dynamic Media Classic查看器預設。 此表格也指定了檢視器與桌上型電腦和行動裝置的相容性，以及用於個別檢視器的技術。

另請參閱 [Adobe查看器參考庫示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

如需有關檢視器支援的 Web 瀏覽器和作業系統版本的資訊，您可以檢閱「檢視器發行說明」。

請參閱 [Adobe查看器參考發行說明](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)。

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
| Universal_HTML5_eCatalog_Adv（包括對社交媒體和目錄搜索的支援。） | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包括對社交媒體和目錄搜索的支援。） | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 迴轉檢視器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 檢視器**

Adobe Dynamic Media Classic支援MP4 H.264視頻的移動視頻播放。

* 您可以在以下位置找到支援此視頻格式的BlackBerry®設備： [BlackBerry®上支援的視頻格式](https://developers.blackberry.com/us/en)
* 您還可以在以下位置找到支援此視頻格式的Windows®設備： [Windows® Phone上支援的視頻格式](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 | BlackBerry®智慧手機 | Windows®電話 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包括對隱藏字幕的支援。） 請參閱 [最佳做法：使用通用HTML5視頻查看器。](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包括對隱藏字幕和社交媒體的支援。） | HTML5 | X | X | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒體集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支援的行動檢視器手勢矩陣 {#supported-mobile-viewers-gestures-matrix}

下表列出了iOS、Android™ 2.x和Android™ 3.x設備支援的移動查看器手勢。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android™智慧手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 關於檢視器預設集畫面 {#about-the-viewer-preset-screen}

在「檢視器預設集」畫面建立和管理檢視器預設集。要開啟此螢幕，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。

「檢視器預設集」畫面提供了執行下列工作的工具:

* **添加預設**  — 選擇 **[!UICONTROL 添加]** 並在「添加查看器預設」對話框中進行選擇。

       請參閱[添加和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)。
   
* **編輯預設**  — 選擇預設，然後選擇 **[!UICONTROL 編輯]**。

       請參閱[添加和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)。
   
* **刪除預設**  — 選擇預設，然後選擇 **[!UICONTROL 刪除]**。

* **導出預設**  — 選擇HTML5查看器預設，然後選擇 **[!UICONTROL 導出]** 下載查看器外觀，以便您可以將其用作建立和添加另一個查看器預設的基礎。

       請參見[導出HTML5查看器預設](application-setup.md#exporting_an_html5_viewer_preset)。
   
* **篩選查看器預設清單**  — 使用這些工具篩選清單：

       *開啟**「活動/非活動」**下拉清單，並選擇一個選項以顯示活動預設、非活動預設或所有預設。
       *開啟**查看器**下拉清單並選擇一個選項，以僅查看某種類型的查看器。 選擇**[!UICONTROL 所有查看器]**查看所有查看者。
   
* **對預設排序**  — 選擇列標題(**[!UICONTROL 活動]**。 **[!UICONTROL 類型]**。 **[!UICONTROL 預設]**&#x200B;或 **[!UICONTROL 平台]**)中的設定。 再次選擇列標題以按降序（或升序）順序對清單進行排序。

* **激活和停用預設**  — 選擇預設，然後選擇其「活動」選項以激活或停用它。

       請參閱[激活或停用查看器預設](application-setup.md#activing_or_decivating_viewer_presets)。
   
>[!NOTE]
>
>選擇 **[!UICONTROL 預覽]** 在「查看器預設」頁面的右側，以便您可以在選定的「查看器預設」中查看資產的外觀。 要查看其他資產，請選擇 **[!UICONTROL 瀏覽]** 在「查看器預設」頁中，並在「選擇資產預覽」對話框中選擇其他資產。

### 添加和編輯查看器預設 {#adding-and-editing-viewer-presets}

除使用 **[!UICONTROL 添加]** 在用戶介面中，您還可以 **[!UICONTROL 導出]** 的子菜單。 您只需導出現有的HTML5查看器預設，然後將其用作新預設的基礎。

請參閱 [導出HTML5查看器預設](application-setup.md#exporting_an_html5_viewer_preset)。

另請參閱 [查看器預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 培訓視頻。

**增加和編輯檢視器預設集:**

1. 在Adobe Dynamic Media Classic右上角，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。

   您可以篩選預設集的清單。例如，若只要查看視訊檢視器的預設集，請從表格正上方工具列上的「檢視器」下拉式選單中選取「視訊檢視器」。

1. 在「查看器預設」頁中，在「查看器預設」螢幕上添加或編輯「查看器預設」。

   * **添加**  — 在工具欄上，選擇 **[!UICONTROL 添加]**。 在「添加查看器預設」對話框中，選擇平台，然後選擇富媒體資產類型。

          選擇**[!UICONTROL 另存為]**建立完「查看器預設」後。
      
   * **通過從現有查看器預設開始添加**  — 在表中，選擇視頻查看器預設，然後選擇 **[!UICONTROL 編輯]** 的上界。

          重新配置視頻查看器後，選擇**[!UICONTROL 另存為]**使用「預設名稱」文本欄位中的其他名稱保存預設。
      
   * **編輯**  — 選擇現有的查看器預設，然後選擇 **[!UICONTROL 編輯]**。

1. 在「配置查看器」螢幕的「預設名稱」欄位中，輸入或編輯預設名稱。
1. 設定其它想要的選項。

   >[!NOTE]
   >
   >選擇 **[!UICONTROL 與源相同]** 自動將視頻查看器的大小調整到編碼視頻本身的解析度大小。 如果選擇此選項，則不能輸入舞台寬度和舞台高度。 相反，這些選項來自視訊本身。如果選擇 **[!UICONTROL 與源相同]**，設定「邊距大小」選項以反映視頻回放區域外的外觀尺寸。 該邊距大小是視訊控制項的像素高度和寬度。您可以使用以下影像幫助您確定要使用的邊距大小。*

   ![視頻查看器的邊距配置](assets/vs_video_viewer_configure_margin.png)

1. 進行以下一項操作:

   * 選擇 **[!UICONTROL 另存為]** 從現有預設開始添加查看器預設。
   * 選擇 **[!UICONTROL 保存]** 的子菜單。

### 導出HTML5查看器預設 {#exporting-an-html-viewer-preset}

可以導出現有HTML5查看器預設，以用作建立HTML5查看器預設的基礎。 匯出選項十分有用，因為您不需從頭建立檢視器， 但可以匯出與您要的外觀和行為接近的預設集，然後將其用作進行設計調整的起點。

所有預設的開箱查看器預設的Adobe Dynamic Media ClassicCSS檔案都使用指向上的資產的相對影像服務路徑 `Scene7SharedAssets`。 例如，以下是查看器預設的CSS檔案中影像資源的相對路徑

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

但是，如果您在自己的站點上托管Viewer CSS檔案，則必須使用在自己環境中指向Image Server的顯式路徑來解析這些相對映像路徑。 例如，如果要將上面的相對路徑更新為顯式路徑，則可能如下所示，其中 `https://s7d1.scene7.com` 是指向映像伺服器的直接路徑： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**導出HTML5查看器預設：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。
1. 在「查看器預設」工具欄上，在左側第二個下拉清單中，選擇 **[!UICONTROL HTML5]**。
1. 在左邊第三個下拉式清單中，選取&#x200B;**[!UICONTROL 所有檢視器]**。
1. 選擇要用作新HTML5查看器預設基礎的查看器預設。
1. 在工具欄中，選擇 **[!UICONTROL 導出]**。
1. 在「導出選定資產」對話框中，選擇 **[!UICONTROL 提交導出]**。

   導出後，將獲取CSS檔案。 下載並解壓縮檔案。

1. 在 CSS 編輯器中開啟 CSS 檔案，進行變更後儲存檔案。
1. 將CSS檔案上載到Adobe Dynamic Media Classic。

   請參閱 [上載檔案](uploading-files.md#uploading_files)。

1. 將CSS檔案發佈到Dynamic Media映像伺服器。

   請參閱 [發佈檔案](publishing-files.md#publishing_files)。

1. 照常增加檢視器預設集。選擇您上載的查看器CSS檔案。

   請參閱 [添加和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)。

### 激活或停用查看器預設 {#activating-or-deactivating-viewer-presets}

要建立用於顯示資產的URL，用戶將開啟「預覽」對話框中的「預設」下拉清單，選擇「查看器預設」，然後選擇 **[!UICONTROL 複製URL]** （請參見） [複製查看器預設的URL](application-setup.md#copying_the_url_of_a_viewer_preset))。 預設集清單提供了管理員在「檢視器預設集」畫面所增加和管理的檢視器預設集。例如，使用者預覽 eCatalog 時，所有作用中的 eCatalog 檢視器預設集都會顯示在「預覽」對話框中的「預設集」下拉式清單中。

除非您在「檢視器預設集」畫面上停用檢視器預設集，否則「預覽」對話框中的「預設集」下拉式清單可能會過於擁擠。

**若要啟用或停用檢視器預設集，請執行下列動作：**

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。
1. 在「查看器預設」頁面上，選擇或取消選擇 **[!UICONTROL 活動]** 選項以激活或停用查看器預設。

### 複製查看器預設的URL {#copying-the-url-of-a-viewer-preset}

發佈資產後，您就可以複製 URL，以「檢視器預設集」的設定來顯示資產。

URL 便會複製到剪貼簿。您可以視需要在網頁、行動裝置或應用程式的 HTML 代碼中加以使用。

**複製「檢視器預設集」的 URL:**

1. 在「瀏覽面板」中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和嵌入代碼」面板中，選擇 **[!UICONTROL 複製URL]** 按鈕。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

### 複製查看器預設的嵌入代碼 {#copying-the-embed-code-of-a-viewer-preset}

您可使用「內嵌程式碼」功能查看所選「檢視器預設集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。

不可在「內嵌程式碼」對話框中編輯程式碼。

**複製檢視器預設集的內嵌程式碼:**

1. 在「資產瀏覽」面板中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL面板中，選擇 **[!UICONTROL 嵌入代碼]**。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。
   在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

1. 在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。
1. 選擇 **[!UICONTROL 關閉]**。

## 配置預設查看器 {#configuring-default-viewers}

使用「預覽」(Preview)在Adobe Dynamic Media Classic時，可以使用「預設查看器」(Default Viewers)來配置與資產關聯的預設查看器。 您可以針對下列資產類型設定預設的預覽體驗:

* 影像
* 視訊
* 迴轉集
* 目錄
* 影像集
* 色票集
* 媒體集

**設定預設檢視器:**

1. 在「設定」下拉清單中，選擇 **[!UICONTROL 應用程式設定]**。
1. 在「Setup（設定）」窗口的左窗格中，轉到 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 查看者]**
1. 選擇 **[!UICONTROL 預設查看器]**。
1. 在「預設檢視器」視窗中，從每個資產類型下拉式清單中選取您要與資產預覽相關聯的檢視器。
1. 在「預設查看器」窗口的右下角，選擇 **[!UICONTROL 保存設定]**。
1. 在「設定」窗口的右下角，選擇 **[!UICONTROL 關閉]** 返回「資產」窗口。

## 中繼資料檢視 {#metadata-views}

*中繼資料*&#x200B;是有關資產的標準化資料。您可以使用中繼資料來簡化工作流程、組織資產和改善搜尋。Adobe Dynamic Media Classic支援國際新聞電信委員會(IPTC)標準和XMP（可擴展元資料平台）標準。 在用戶查看或在詳細資訊視圖中輸入有關資產的元資料之前，他們可以開啟元資料視圖菜單。 從中，他們可以選擇要查看或用於描述資產的元資料欄位集。

Adobe Dynamic Media Classic提供了預定義的元資料視圖，管理員可以建立自己的元資料視圖，供用戶在輸入元資料時進行選擇。

### 建立中繼資料檢視 {#creating-a-metadata-view}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料視圖]**。
1. 選擇 **[!UICONTROL 添加]**。
1. 在「預設名稱」文本欄位中，輸入視圖的名稱。
1. （可選）檢查 **[!UICONTROL 設為預設值]** 使此視圖成為用戶在「詳細資訊視圖」中開啟「元資料」面板時看到的視圖。
1. （可選）選擇 **[!UICONTROL 包括UDF]** 在視圖中包括用戶定義的欄位。 使用者定義的欄位會顯示在詳細檢視的「中繼資料」面板上方。
1. 選擇要查看的欄位(選擇 **[!UICONTROL 全選]** 的子菜單。
1. 選擇 **[!UICONTROL 保存]**。

   選取的檢視類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料檢視 {#managing-metadata-views}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料視圖]**。
1. 請執行下列任一動作:

   * 若要預覽檢視，請加以選取。檢視中的欄位會顯示在「預覽」面板中。
   * 要編輯視圖，請選擇它，然後選擇 **[!UICONTROL 編輯]**。 然後在「預覽」面板上選擇或取消選擇欄位名稱，然後選擇或取消選擇 **[!UICONTROL 包括UDF]** 的雙曲餘切值。
   * 要刪除視圖，請選擇它，然後選擇 **[!UICONTROL 刪除]**。
   * 要使視圖成為預設視圖，請選擇它，然後選擇 **[!UICONTROL 設為預設值]**。 預設視圖是用戶在「詳細資訊視圖」中開啟資產並轉至「元資料」面板時看到的視圖。

## 中繼資料預設集 {#metadata-presets}

中繼資料預設集讓管理員能夠控制和調節為資產指定的中繼資料。在「詳細資訊視圖」中，用戶可以在為此目的提供的欄位中輸入有關資產的元資料。 例如，使用者可以輸入擁有者名稱、版權描述和地址。為確保用戶準確、完整地輸入此資訊，您可以建立元資料預設。 在詳細資訊視圖中選擇元資料預設將使用預定義的值填充元資料欄位。 例如，擁有者名稱、版權描述和地址皆會自動輸入。

為希望用戶能夠在詳細資訊視圖中自動輸入以描述資產的每組元資料值建立元資料預設。

### 建立或編輯中繼資料預設集 {#creating-or-editing-a-metadata-preset}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料預設]**。
1. 在「中繼資料預設集」面板中，執行下列任一項作業:

   * 要建立預設，請選擇 **[!UICONTROL 添加]**。 在「元資料模板名稱」文本欄位中，鍵入預設的名稱。 選擇 **[!UICONTROL 元資料視圖]**，然後從下拉清單中選擇一個視圖(請參閱 [元資料視圖](application-setup.md#metadata_views))。
   * 要編輯現有預設，請從「元資料預設」清單中選擇預設，然後選擇 **[!UICONTROL 編輯]**。

1. 展開要包括在預設中的標題，然後在要包括在預設中的不同欄位中輸入值。
1. 選擇 **[!UICONTROL 保存]**。

   選取的預設集類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料預設集 {#managing-metadata-presets}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料預設]**。
1. 請執行下列任一動作:

   * 若要預覽預設集，請選取您要預覽的預設集。預設集資訊 (類別和欄位) 會顯示在「預覽」畫面中。
   * 要刪除預設，請選擇預設，然後選擇 **[!UICONTROL 刪除]**。

## 使用者定義的欄位 {#user-defined-fields}

媒體入口網站管理員或公司管理員可建立自訂、使用者定義的中繼資料欄位。自定義欄位可幫助您組織Adobe Dynamic Media Classic的資產。 您可以根據需要將欄位標籤為「活動」。 激活後，這些自定義元資料欄位的名稱將顯示在「詳細資訊視圖」的「元資料」面板中。 使用者可以在使用者自訂的中繼資料欄位中輸入資訊，以描述資產。使用者也可以將使用者定義的中繼資料欄位設定作為搜尋條件。

使用者定義的中繼資料欄位的有效用途之一，就是針對特定的上市發表會或銷售會，延遲資產的啟用時間。根據類型定義「激活」欄位 *日期*。 然後，使用 **[!UICONTROL 元資料]** 「詳細資訊」視圖或 **[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**，您可以指定激活資產的時間。 Adobe Dynamic Media Classic檢查資產的發佈狀態和發佈歷史記錄。 如果不在激活時間內，則發佈狀態顯示為「未發佈」。

>[!NOTE]
>
>要使用戶定義的欄位顯示在「詳細資訊視圖」的「元資料」面板中，請在「元資料視圖」中包括用戶定義的欄位。 在「中繼資料檢視」畫面上選取「包含 UDF」(使用者定義欄位) 選項。如需詳細資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views)。

>[!NOTE]
>
>要使用自定義自定義欄位搜索資產，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，然後選擇 **[!UICONTROL 在搜索中包括UDF]**。 請參閱[個人設定](personal-setup.md#personal_setup)。

### 建立用戶定義的元資料欄位 {#creating-a-user-defined-metadata-field}

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 用戶定義的欄位]**。
1. 選擇 **[!UICONTROL 添加]**
1. 在「自訂欄位」對話框中，設定您要的選項。

   * **[!UICONTROL 名稱]**  — 輸入元資料欄位的名稱。

   * **[!UICONTROL 類型]**  — 選擇一個選項，該選項定義用戶可以在元資料欄位中輸入的資訊類型：

   * **[!UICONTROL 字串]**  — 文本字串。

   * **[!UICONTROL 整型]**  — 整數。

   * **[!UICONTROL 浮動]**  — 浮點數。

   * **[!UICONTROL 是/否]**  — 是/否布爾值。

   * **[!UICONTROL 日期]**  — 日期。 接受 MM/DD/YYYY 格式。

   * **[!UICONTROL 檔案名]**  — 檔案的名稱。

   * **[!UICONTROL 顏色]**  — 顏色的名稱。

   * **[!UICONTROL Dimension]**  — 資產的寬度和高度。

   * **[!UICONTROL 無類型]**  — 用於向後相容。 請勿選取此選項。

   * **[!UICONTROL 預設值]**  — （可選）在欄位中輸入用戶最可能輸入的值。 您輸入的值會成為您建立之欄位的預設值。

   * **[!UICONTROL 應用於]**  — （可選）如果希望元資料欄位僅應用於特定類型的資產，請選擇資產類型。

      >[!NOTE]
      >
      >選擇 **[!UICONTROL 應用於]** 選項，因為您無法更改 **[!UICONTROL 應用於]** 選項。 Adobe Dynamic Media Classic允許您編輯用戶定義的欄位的名稱、類型和預設值，但不能編輯 **[!UICONTROL 應用於]** 的子菜單。*

1. 選擇 **[!UICONTROL 保存]** 建立完元資料欄位。

### 管理使用者定義的欄位 {#manage-user-defined-fields}

「使用者定義的欄位」畫面提供了管理自訂、使用者定義之中繼資料欄位的命令。

只有 Media Portal 管理員或公司管理員才可以管理使用者定義的欄位。

要開啟此螢幕，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 用戶定義的欄位]**。

* **編輯欄位**  — 選擇欄位，然後選擇 **[!UICONTROL 編輯]**。

* **刪除欄位**  — 選擇欄位，然後選擇 **[!UICONTROL 刪除]**。

* **激活欄位**  — 選擇或取消選擇 **[!UICONTROL 活動]** 的子菜單。 如果您是公司管理角色，則不顯示此選項。 由於此選項與MediaPortal相關，因此必須選擇（開啟）「個人設定」中的「顯示MediaPortal功能」以查看激活欄位。

## 最佳化檔案 {#optimize-files}

將檔案上載到Adobe Dynamic Media Classic時，系統會優化這些檔案以儲存和發佈。 不過，如果上載程序受到中斷，部分影像就無法最佳化。在此情況下，您會看見「尚未最佳化影像」訊息。但是，如果您是管理員，就可以最佳化這些檔案。

Adobe Dynamic Media Classic搜索您的檔案，並僅優化以前未完全優化的映像。

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**，然後選擇 **[!UICONTROL 優化檔案]**。
1. 輸入優化作業的資訊並選擇 **[!UICONTROL 提交]**。

   如果您使用超過一家公司，請分別對屬於不同公司的檔案執行最佳化。

## 批次集預設集 {#batch-set-presets}

使用批處理集預設在作業運行時將資產上載到Adobe Dynamic Media Classic時自動建立影像集或旋轉集。

公司管理員首先為要在集合中分組的資產定義命名約定。 然後，可建立批集預設以引用這些影像。 每個預設集都是具備唯一名稱的內部獨立式指示集，定義如何使用與預設集配置中已定義的命名慣例相符的影像來建構集。

所有作用中的公司批次集預設集都會列在「上載工作選項」對話框中，以便您指定要在每個上載工作階段期間套用的預設集。公司管理員會看到所有作用中和非作用中的批次集預設集。上載檔案時，Adobe Dynamic Media Classic會自動建立一個集，其中包含所有與活動預設中定義的命名約定相匹配的檔案。

### 預設命名 {#default-naming}

公司管理員會建立任何批次集預設集配置中使用的預設命名慣例。在批處理集預設定義中選擇的預設命名約定可能是貴公司為所有網站批處理生成集所需的全部。 必須建立批次集預設集，才能使用您所定義的預設命名慣例。公司定義的預設命名有例外情況時，您可以透過特定內容集所需的替代、自訂命名慣例來建立同等數量的批次集預設集。

使用批集預設功能不需要設定預設命名約定。 但是，Adobe最佳實踐建議您使用預設的命名約定來定義要在集合中分組的命名約定的任意多個元素。 這樣做有助於簡化批集建立。

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設]** > **[!UICONTROL 預設命名]**。
1. 選取「**[!UICONTROL 檢視表單]**」或「**[!UICONTROL 檢視器碼]**」即可指定您要如何檢視和輸入個別元素的相關資訊。

   可以選擇 **[!UICONTROL 查看代碼]** 框中，選擇「 CSV文本」。 如果表單檢視因故對您有所限制，則您可以輸入或變更這些值，以幫助定義命名慣例的元素。如果無法在表單視圖中分析您的值，則表單欄位將變為非活動狀態。

   >[!NOTE]
   >
   >停用的表單欄位不代表規則運算式無效。沒有驗證方式可確認您的規則運算式是否正確。在「結果」行之後，您會看見針對個別元素所建置之規則運算式的結果。您可以在頁面底部看到完整的規則運算式。

1. 視需要展開個別元素，並輸入您要使用的命名慣例。
1. 根據需要，選擇 **[!UICONTROL 添加]** 為元素添加其他命名約定。 或，選擇 **[!UICONTROL 刪除]** 刪除元素的命名約定。
1. 選擇 **[!UICONTROL 另存為]** 鍵入預設的名稱。 或，選擇 **[!UICONTROL 保存]** 編輯現有預設。

您也可以使用不含任何可用表單欄位的「檢視器碼」。在此視圖中，您完全使用規則運算式建立命名約定定義。

有兩個元素可供定義，分別為「符合」和「基本名稱」。這些欄位可讓您定義所有命名慣例元素，並識別慣例中用來命名其中所含之集的部分。公司的單個命名約定可以為每個元素使用一條或多條定義線。 您可以針對唯一定義使用同等數量的行，並將其分組至不同的元素，例如「主影像」、「色彩元素」、「替代檢視」元素和「色票」元素。

### 建立批次集預設集 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic使用批集預設來將共用某些公共資訊或內容的資產組織成一組影像，供觀看者顯示。 批集預設配方會自動與您在Adobe Dynamic Media Classic計畫的資產導入作業一起運行。

使用「批次集預設集」即可建立、編輯和管理批次集預設集。您可以根據需要建立盡可能多的預設，以涵蓋所需的所有資產攝取作業。 有兩種形式的批集預設定義：一個用於您設定的預設命名約定，另一個用於您即時建立的自定義命名約定。

您可以使用表單域方法定義批集預設或使用規則運算式的代碼方法。 與 **[!UICONTROL 預設命名]**&#x200B;頁籤 **[!UICONTROL 代碼視圖]** 同時，您正在「表單視圖」中定義並使用規則運算式來構建定義。 您也可以取消核取任一檢視，僅使用其中一種。

另請參閱 [為自動生成2D旋轉集建立批集預設](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)。

另請參閱 [2D自旋集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) 培訓視頻。

**建立批次集預設集:**

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設]** > **[!UICONTROL 批集預設]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設清單」面板中，選擇 **[!UICONTROL 添加]** 以激活頁面右側「詳細資訊」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取預設集類型。

   若要自動產生 2D 迴轉集，請從「批次集類型」下拉式清單中選取「**[!UICONTROL 多軸旋轉集]**」。

1. 進行以下一項操作:

   * 如果您使用的是先前在以下位置設定的預設命名約定 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設]** > **[!UICONTROL 預設命名]**&#x200B;展開 **[!UICONTROL 資產命名約定]**，然後在「檔案命名」下拉清單中，選擇 **[!UICONTROL 預設]**。
   * 要在設定預設時定義命名約定，請展開 **[!UICONTROL 資產命名約定]**，然後在「檔案命名」下拉清單中，選擇 **[!UICONTROL 自定義]**。

1. 對於序列順序，在集在Adobe Dynamic Media Classic分組後定義影像的順序。 根據預設，您的資產會按照字母順序排列。不過，您可以使用規則運算式以逗號分隔的清單來定義順序。
1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。還定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果定義了大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 選擇 **[!UICONTROL 保存]** 的子菜單。

### 為自動生成2D旋轉集建立批集預設 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您也可以使用批次集類型「**多軸旋轉集**」來建立可自動產生 2D 迴轉集的「配置」。影像的群組會使用列與欄規則運算式，使影像資產適當對齊於多維度陣列中的對應位置上。

另請參閱 [建立批集預設](application-setup.md#creating_a_batch_set_preset)。

在多軸旋轉集中，不存在必須具有的最小或最大行數或列數。

例如，假設要建立名為 *自旋2dspin*。 您有一組迴轉集影像，內有三列，每列有 12 個影像。影像的命名如下:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

使用此資訊，您可以按如下方式建立批集類型處方：

![批集處方影像](assets/se_batch_set_recipe.png)

對旋轉集的共用資產名稱部分進行分組將添加到「匹配」欄位（如突出顯示）。 含列與欄的資產名稱的變數部分會分別增加到「列」和「欄」欄位。

上載並發佈「迴轉集」後，您就可以在「上載工作選項」對話框中啟用「**[!UICONTROL 批次集預設集]**」之下 2D 迴轉集配置的名稱。

**建立批次集預設集以自動產生 2D 迴轉集:**

1. 轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批集預設]** > **[!UICONTROL 批集預設]**。 「**[!UICONTROL 檢視表單]**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設清單」面板中，選擇 **[!UICONTROL 添加]** 以激活頁面右側「詳細資訊」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取「**[!UICONTROL 資產集]**」。
1. 在「子類型」下拉式清單中，選取「**[!UICONTROL 多軸轉旋轉集]**」。
1. 展開 **[!UICONTROL 資產命名約定]**，然後在「檔案命名」下拉清單中，選擇 **[!UICONTROL 自定義]**。
1. 使用「**[!UICONTROL 符合]**」，並選擇性地使用「**[!UICONTROL 基本名稱]**」屬性，定義用來為組成群組的影像資產命名的規則運算式。

   例如，您的文字「匹配」規則運算式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展開「**[!UICONTROL 列欄位置]**」，然後為影像資產在 2D 迴轉集陣列內的所在位置定義名稱格式。

   使用括號括住檔案名稱中的列或欄位置。

   例如，對於行規則運算式，它可能如下所示：

   `\w+-R([0-9]+)-\w+`

   或

   `\w+-(\d+)-\w+`

   對於列規則運算式，它可能如下所示：

   `\w+-\w+-C([0-9]+)`

   或

   `\w+-\w+-C(\d+)`

   請記住，這些表達式只是示例。 您可以用任何想要的方式建立規則運算式以符合自己的需求。

   >[!NOTE]
   >
   >如果行和列中規則運算式的組合無法確定資產在多維旋轉集陣列中的位置，則不會將該資產添加到該集中，並記錄錯誤。

1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。還定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果定義了大量影像集，請將這些集與包含資產本身的資料夾分開。 許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 選擇 **[!UICONTROL 保存]** 的子菜單。
1. 如往常般上載並發佈您的迴轉集，過程中確定您在「工作載入選項」對話框的「批次集預設集」下啟用 2D 迴轉集的名稱。

>[!MORELIKETHIS]
>
>* [預覽資產](previewing-asset.md#previewing_an_asset)
>* [設定影像預設](setting-image-presets.md#setting_up_image_presets)
>* [查看、添加和導出元資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [檢查作業檔案](checking-job-files.md#checking_job_files)

