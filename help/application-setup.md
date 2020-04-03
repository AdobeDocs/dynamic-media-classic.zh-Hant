---
title: 應用程式設定
seo-title: 應用程式設定
description: 瞭解如何設定Dynamic Media Classic的應用程式區域。
seo-description: 瞭解如何設定Dynamic Media Classic的應用程式區域。
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: ae2d1895-a437-4463-bfac-3960c8027551
translation-type: tm+mt
source-git-commit: 8216ac64ba418987c7f5ed84c4cb957189645bd9

---


# 應用程式設定{#application-setup}

您可以使用「應用程式設定」頁面來輸入一般設定、建立影像預設集、視訊編碼預設集、檢視器預設集，或定義預設檢視器和中繼資料。 您也可以設定批次集預設集，以自動產生 2D 迴轉集 (舉例來說)、發佈設定與視訊 SEO 設定。

>[!NOTE]
>
>只有 Scene7 Publishing System 管理員可以變更「應用程式設定」頁面上的設定。

## 一般設定 {#general-settings}

若要開啟「應用程式一般設定」頁面，請在全域導覽列上按一下「**[!UICONTROL 設定 > 應用程式設定 > 一般設定]**」。

### 伺服器

在建立帳戶時，Dynamic Media Classic會自動為您的公司提供指派的伺服器。 這些伺服器是用來為您的網站和應用程式建立 URL 字串。這些 URL 呼叫皆專屬於您的帳戶。

另請參閱[測試安全測試服務](testing-assets-making-them-public.md#testing_the_secure_testing_service)。

**發佈伺服器名稱** ：此伺服器是即時CDN伺服器，用於您帳戶的特定所有系統產生的URL呼叫。 除非Dynamic Media Classic支援技術人員指示您更改此伺服器名稱。

**原始伺服器名稱** ：此伺服器僅用於品質保證測試。 除非Dynamic Media Classic支援技術人員指示，否則不要更改此伺服器名稱。

**AGM伺服器名稱** ：此伺服器用於Web-to-Print模板。 此伺服器會以全公司的基礎進行設定。除非Dynamic Media Classic支援技術人員指示，否則不要更改此伺服器名稱。

**Test&amp;Target伺服器名稱** ：您的Test&amp;Target URL，最多及包含。com。 如需有關取得此URL的指示，請參閱整合Dynamic Media Classic與Target Classic。

**iOS串流伺服器名稱** ：您的Dynamic Media Classic iOS串流伺服器的URL。 此伺服器會透過 HTTP 通訊協定將串流視訊傳送至以 iOS 為基礎的裝置。

**漸進式視訊伺服器名稱** :Dynamic Media Classic漸進式視訊伺服器的URL。 此伺服器會透過 HTTP 通訊協定來傳送漸進式視訊。

**顯示未發佈資產的URL** 如果您想要Dynamic Media Classic在預覽任何資產時顯示URL，請選取此選項，無論其是否已發佈。 如果資產尚未發佈，URL 將無法運作。不過，您可以使用 URL 來進行規劃或組織。

**允許AIR安裝** ：選取此選項可讓使用者將Scene7 Publishing System案頭版下載至其本機硬碟。 使用者可以從「個人設定」畫面的「桌面版本」區域安裝應用程式。

AIR 使用者必須手動解除安裝現有應用程式，並從 Scene7 Publishing System 網路版 (在「個人設定」中) 進行重新安裝。在此一次性重新安裝完成後，系統會在伺服器有新版本 Scene7 Publishing System AIR 時提示您升級。Scene7 Publishing System 已與「應用程式更新框架」整合，可簡化升級程序。

**CDN失效範本** ：指定用於使CDN（內容傳送網路）快取失效的範本。

For example, suppose you enter an image URL (including image presets or modifiers) referencing `<ID>`, instead of a specific image ID as in the following example:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

If the Template just contains `<ID>`, then SPS fills in the `https://<server>/is/image`, where `<server>` is the Publish Server Name that is defined in General Settings.

設定 CDN 失效範本、選取名為「Backpack_B」的影像，然後按一下「**檔案** > **使 CDN 失效**」，便會在「CDN 失效」介面中產生下列 URL:

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

在 URL 清單方塊中，按一下「**繼續**」以清除特定影像 URL 呼叫的快取。請注意，您也可以透過輸入或將其貼上至 URL 清單方塊中以新增 URL；您不需要事先設定範本。

選取您的 CDN 失效範本，並進行「使 CDN 失效」要求之後，在使用者介面中會彈出指示器，讓您估計清除快取所需的時間。

同樣地，如果在按一下「**檔案** > **使 CDN 失效**」時於 SPS 之中選取了多個影像，則會在儲存的範本 URL 中參照每個影像。因此，您可以定義參照您網站所參照之 URL (如產品詳細資訊、搜尋結果等等) 的 CDN 失效範本。然後，當您從快取中選取一或影像以進行失效時，URL會自動填入介面。

請參閱[內容快取](scene7-platform-overview.md#content_caching)。

請參閱[重新發佈的資產和 CDN 延遲](publishing-files.md#republished_assets_and_cdn_delays)。

**瀏覽**

**「顯示專案** 」會判斷「專案」是否可用來組織您的Dynamic Media Classic資產。 請參閱利用專案組織您的工作。

**顯示範例eVideo內容** 開啟或關閉eVideo範例內容的顯示。

**在資料夾中顯示產生的內容** ，顯示從資產產生的內容。 例如，當PDF檔案上傳時點陣化，Dynamic Media Classic會在原始PDF中為每個頁面建立一個影像。 如果選取了「顯示產生的內容」，則原始 PDF 上載時所產生的每個影像，都會與 PDF 一起出現在該 PDF 的上載檔案夾中。

**依預設顯示已取消選取的編碼視訊** （關閉）。

若要在 Scene7 Publishing System 中快速搜尋和瀏覽影片，而無需瀏覽相同影片許多已編碼的衍生影片，請維持取消選取此選項 (預設)。只有主要影片縮圖 (也就是您上傳並用來建立所有衍生影片的來源影片) 以及「上層」適應性影片集縮圖 (包含已編碼影片集的所有「下層」衍生影片) 會顯示在使用者介面中。

不過，您仍然可以從主視訊或最適化視訊集存取個別編碼的視訊。若要執行此項操作，請按兩下視訊縮圖影像，以開啟「詳細檢視」。接著在右側面板中按一下「**編碼的視訊**」，以存取所有「子項」視訊。

您也可以使用「**檔案 > 重新處理**」，直接從最適化視訊集來建立更多編碼的「子項」視訊。Scene7 Publishing System 會自動尋找最適化視訊集的「父項」主視訊，並使用該主視訊作為轉碼的來源視訊。不過，在您儲存新的個別編碼的視訊後，搜尋或瀏覽時並不會看到這些視訊。然而這些視訊仍可從「詳細檢視」的「編碼的視訊」標籤予以存取。

請參閱[上載和轉碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

若要繼續能夠在搜尋和瀏覽時存取所有編碼視訊的衍生物，請選取「**顯示編碼的視訊**」。

「建置」選單上的某些動作只能用於個別視訊，或選擇性地用於個別視訊。此功能迫使您必須顯示所有可以選取之編碼視訊的衍生物，而不受您設定「**顯示編碼的視訊**」的方式影響。The Build actions that over-ride the **Show Encoded Videos** setting include **Adaptive Video Sets**, and **eCatalogs**.

>[注意]
>
>如果您未使用Scene7 Publishing System來上傳和編碼您的視訊資產，Dynamic Media Classic會顯示您的所有個別編碼視訊，即使取消選取此選項亦然。

**顯示刷新子資料夾按鈕** 開啟或關閉子資料夾刷新按鈕的顯示。

**Dynamic Media Classic FTP帳戶**

**伺服器** 」列出您的FTP帳戶伺服器。

**使用者名稱** ：列出您的FTP帳戶使用者名稱。

**上載至應用程式**

**覆寫影像** Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個項目的 Scene7 Publishing System ID (不含副檔名的影像名稱) 皆必須為唯一。因為此規則，所以「上載」對話框擁有「覆寫」選項。此選項的確實效果取決於指定的「覆寫影像」選項。這些選項會指定取代影像的上載方式: 取代原始影像或成為重複影像。重複影像將會以「-1」重新命名 (例如，chair.tif 會重新命名為 chair-1.tif)。這些選項會影響上載至非原始檔案夾的影像，或擁有非原始副檔名 (例如 JPG、TIF 或 PNG) 的影像。(請參閱使用覆寫影像選項。)

**目前的檔案夾內若有基本影像名稱/副檔名相同者，將予以覆寫**

此選項為最嚴格的取代規則。它會要求您將取代影像上載至與原始影像相同的檔案夾，且取代影像必須與原始檔案擁有相同的副檔名。如果未符合這些要求，便會建立重複項目。

**目前檔案夾內若有基本資產名稱相同者 (無論副檔名為何)，將予以覆寫**

要求您將取代影像上載至與原始影像相同的檔案夾，但副檔名可以與原始檔案不同。例如，chair.tif 會取代 chair.jpg。

**任何檔案夾內若有基本資產名稱/副檔名相同者，將予以覆寫**

要求取代影像必須與原始影像擁有相同副檔名 (例如，chair.jpg 必須取代 chair.jpg 而非 chair.tif)。然而，您可以將取代影像上載至與原始影像不同的檔案夾。上載的影像將會位於新檔案夾中；無法再於原始位置中找到該檔案

**在任何檔案夾中以相同的基本資產名稱 (無論副檔名為何) 覆寫**

此選項為最廣泛的取代規則。您可以將取代影像上載至非原始檔案夾、上載擁有不同副檔名的檔案，以及取代原始檔案。如果原始檔案位於不同檔案夾，則取代影像會位於其上載的新目標檔案夾中。

**保留發佈** ：指定上傳至Dynamic Media Classic的取代影像是否保留所取代影像的「準備發佈」設定，或是在上傳時指定設定。

**預設色彩描述檔** ：指定在新增CMYK影像時，套用為「預設色彩描述檔選項」一部分的色彩描述檔。

**預設上傳選項** ：開啟「上傳工作選項」對話方塊，您可在其中指定預設的上傳選項。 如需有關這些選項的詳細資訊，請參閱上載選項。

**應用程式的影像地圖編輯器**

**預設影像對應HREF** 定義影像對應href欄使用的預設URL。 此 URL 是您建立新影像地圖時會看見的預設 URL。

**預設影像對應範本** ：定義影像對應href範本的預設Javascript。 您可以在這裡設定每次按一下影像地圖時所執行的自訂代碼。

**應用程式的其他設定**

**垃圾筒可清除警告** ，垃圾筒中的資產會在七天內自動移除。 如果您要在永久刪除「垃圾桶」之資產的前四天傳送通知至公司管理員，請選取「在自動刪除垃圾桶項目前傳送電子郵件」。請參閱管理垃圾桶檔案夾。

## 使用「覆寫影像」選項 {#using-the-overwrite-images-option}

Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個項目的 Scene7 Publishing System ID (不含副檔名的影像名稱) 皆必須為唯一。因為此規則，所以「上載」對話框包含「覆寫影像」選項。此選項的確實效果取決於各公司的 Scene7 Publishing System 內部設定的設定。

如果您先前上傳的影像，然後變更原始檔案（或取代檔案），則選取的「覆寫」選項會指定Dynamic Media Classic如何取代影像。 影像的任何相關資訊都不會變更，但新的影像會取代舊影像。如果資料夾中也包含Dynamic Media Classic中尚未包含的影像，則會新增這些影像。

如果您上載的影像已經變更 (影像經過修改)，但影像的參照保持不變，則使用此選項。上載和擷取 Adobe® PDF 檔案時，覆寫功能也很有幫助。To fine-tune how Dynamic Media Classic *rips* the image, adjust the ICC color profile options in the Upload dialog box and re-upload using the Overwrite feature.

用於從生產伺服器存取影像的Dynamic Media Classic ID是從影像檔名衍生而來。 在檔案名稱中使用大寫和小寫字元很重要，不論是在取代現有檔案時，還是用於存取影像的Dynamic Media Classic ID。 請確定在上傳至Dynamic Media Classic之前，檔案名稱中的大寫和小寫字元使用正確，以避免只針對相同影像大小寫不同的Dynamic Media Classic ID。

如果取消選取此選項，所有與現存影像擁有相同檔案名稱的影像都會視為重複項目，而不會增加。

## 影像預設集 {#image-presets}

「影像預設集」畫面是用來建立和編輯影像預設集。影像預設集可讓Dynamic Media Classic以不同大小動態傳送相同主影像的影像。 每個影像預設集都代表了一個用來顯示影像之大小調整與格式命令的預先定義集合。建立影像預設集時，請選擇影像傳送大小。同時也請選擇格式命令，以便在影像傳送供檢視時將影像外觀最佳化。

管理員可以建立匯出資產用的預設集。使用者可以選擇匯出影像時要用的預設集，該預設集同時可將影像重新格式化為管理員指定的規格。

To open the Image Preset screen, on the Global Navigation bar, click **Setup** > **Image Presets**.

請參閱 [智慧型影像](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)。

### 建立和編輯「影像預設集」{#creating-and-editing-image-presets}

1. 按一下「**設定** > **影像預設集**」。
1. 建立新預設集，或從現有預設集開始建立:
   * **建立影像預設集** -按一下「 **新增**」。
   * **從現有預設集建立影像預設集** -選取最像您要建立的影像預設集，然後按一下「編輯」。

1. 在「增加預設集」或「編輯預設集」畫面中，輸入預設集名稱。
1. 設定您想要的預設集選項。

   請參閱[影像預設集選項](application-setup.md#image_preset_options)。

1. Click **Save**, or if you started from an existing preset, click **Save As**.
1. To preview the preset with your own image, click **Browse** and then select an image. To preview with the default image, click **Reset**.

您可以在「影像預設集」畫面中選取影像預設集名稱，並按一下「編輯」，即可編輯影像預設集。若要刪除影像預設集，請加以選取，然後按一下「刪除」。

### 影像預設集選項 {#image-preset-options}

「增加預設集」和「編輯預設集」畫面提供下列選項，以建立和編輯影像預設集:

**預設名稱** ：輸入不含空格的描述性名稱。 在名稱中包括影像大小規格以，即可幫助使用者識別此影像預設集。

**寬度和高度** ：輸入影像傳送大小的像素。

**格式** ：從菜單中選擇格式。 如果選擇 GIF、JPEG、PDF 或 TIFF 格式，則會顯示其它選項:

* GIF 色彩量化選項

   **類型**

   選擇「適應性」(預設)、「Web」或「Macintosh」。如果您選擇「使用 Alpha 色版的 GIF」將無法使用「Macintosh®」選項。

   **混色**

   選擇「擴散」或「關閉」。

   **色彩數目**

   拖曳滑桿以進入2-255。

   **色彩清單**

   輸入逗號分隔清單。例如，對於白、灰和黑，請輸入 000000,888888,ffffff。

* JPEG 選項

   **品質**

   控制 JPEG 壓縮層級。這個設定會同時影響檔案大小與影像品質。JPEG品質等級為1-100。

   **啟用 JPG 色度縮減取樣**

   因為肉眼對於高頻率色彩資訊較不敏感 (相對於高頻率明度)，所以 JPEG 影像會將影像資訊區分為明度與色彩組件。壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣可將資料量減少三分之一或二分之一，而且幾乎不會影響肉眼能感知的品質。縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。

* PDF 和 TIFF 選項

   **壓縮**

   選擇壓縮演算法。

**色域** ：選擇色域。

**銳利化** ：選取「啟用簡單銳利化」選項，在所有縮放發生後，將基本銳利化濾鏡套用至影像。 銳利化可以幫助補償以不同大小顯示影像時所造成的模糊現象。

如需更多有關銳利化、重新取樣模式和遮色片銳利化調整的資訊，請參閱[銳利化影像](sharpening-image.md#sharpening_an_image)。

**重新取樣模式** ：選擇重新取樣模式選項。 下列選項會在縮減取樣影像時予以銳利化:

**B-Linear** ：最快的重採樣方法；有些鋸齒不自然現象很明顯。

**Bi-Cubic** Reaves Image Server的CPU使用量增加，但產生更銳利的影像，並且鋸齒不自然現象較少。

**Sharp2** 比「雙三次方」選項產生的結果稍微銳利，但影像伺服器的CPU成本更高。

**Tri-Linear** Uses both higher resolutions and lower resolutions, if available;僅當鋸齒是問題時建議使用。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

**銳利化遮色片** ：選擇下列選項以微調銳利化：

**量** ：控制套用至邊緣像素的對比度。 預設是 1.0。對於高解析度的影像，您最多可以將它增加至 5.0。將「數量」視為濾鏡飽和度的度量。

**半徑** ：決定影響銳利化的邊緣像素周圍的像素數。 對於高解析度的影像，請輸入 1 到 2 的數字。低數值只會銳利化邊緣的像素；高數值會銳利化較寬的像素範圍。正確的值取決於影像大小。

**臨界值** ：決定套用非銳利遮色片濾鏡時要忽略的對比範圍。 換句話說，這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。為了避免產生雜訊，請使用介於 .02 與 0.2 之間的值來實驗。預設值 6 會對影像中的所有像素進行銳利化。

**色域** ：判斷影像使用的是建立影像的空間，通常是RGB（原始）或明度空間（強度）。

**顏色** ：選擇下列選項：

**輸出色彩描述檔** ：選取「使用預設值」，或Scene7 Publishing System上提供的其中一個ICC色彩描述檔。

請另參閱 [ICC 設定檔](icc-profiles.md#icc_profiles)。

**渲染方式** (Rendering Intent)如果要覆蓋顏色配置檔案的預設渲染方式，請選擇一個選項。 符合以下所有條件時使用此選項: 其中一個預設 ICC 設定檔是色彩轉換的目標色域、此設定檔中特別含有輸出裝置 (印表機或螢幕)，且指定的演算色彩比對方式在此設定檔中有效。

**內嵌描述檔** ：選取這個選項，如果您在Adobe® Photoshop®中開啟此影像，它就會使用這個描述檔。

**列印解析度** ：選擇列印此影像的解析度；預設值為72像素。

**URL修飾詞** ：如果您偏好指定定義影像預設集的URL修飾詞，而非設定，請在此處輸入修飾詞。

**範例影像URL** ：列出動態媒體影像伺服器用來傳送包含您新增或編輯之影像預設集之影像的「原始」URL字串。 此 URL 字串會將您在「增加預設集」或「編輯預設集」畫面中選取的所有格式設定加以編碼。

### 編輯、移除或停用影像預設集 {#editing-removing-or-deactivating-an-image-preset}

1. 按一下「**設定** > **影像預設集**」。
1. 在「影像預設集」畫面中，選取表格中的預設集，然後執行以下一項操作:

   * Click **Edit** and then specify new options in the Edit Preset dialog box.
   * Click **Delete** to remove the preset from the list.
   * 取消選取預設集名稱旁邊的「作用中」核取方框，將其從 MediaPortal 使用者的整個 Scene7 Publishing System 使用者介面中移除。

## 啟用或停用最適化視訊預設集 {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic提供最適化視訊編碼預設集。 此為主要預設集清單，其中將 16:9 最適化視訊預設集與 4:3 最適化視訊預設集合併到一個群組中。這些預先定義的預設集反映了最常見的編碼設定，並已針對目標行動裝置、平板電腦和桌上型電腦的播放進行最佳化。

預設只會啟動 (啟用或「開啟」)「最適化視訊」編碼預設集。您可以視需要加以停用。非作用中的最適化視訊預設集，並不會以可選取的選項顯示在「上載工作選項」對話框的「eVideo」區段中。

請參閱[上載與編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**啟用或停用最適化視訊預設集**

1. 在靠近 Scene7 Publishing System 右上角的地方，按一下「**設定** > **應用程式設定** > **視訊預設集** > **最適化視訊預設集**」。
1. 在「最適化視訊預設集」頁面上，取消選取預設集名稱旁邊的核取方框，以從「上載工作選項」對話框的「eVideo 選項」清單中移除預設集。
1. 按一下「**關閉**」。

## 編碼視訊檔案的視訊預設集 {#video-presets-for-encoding-video-files}

若要選擇編碼預設集，在「上載」頁面的右下角，按一下「工作選項」。在「上載工作選項」對話框中，展開「eVideo 選項」，選擇您想要的視訊編碼預設集。

>[!NOTE]
>
>除了預設啟用的「最適化視訊」以外，您可能無法在「上載工作選項」對話框中查看所有其他的最適化視訊或單一視訊編碼預設集。Dynamic Media Classic管理員會決定在「上傳工作選項」對話方塊中顯示哪些視訊編碼預設集。

* 從下列最適化視訊編碼或單一編碼預設集中選擇一項:

   **16:9 最適化視訊**

   建立16:9外觀比例視訊，以發佈至桌上型電腦、行動裝置(iPhone、iPad、Android)和平板電腦(iPad、Android)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   **4:3 最適化視訊**

   建立4:3外觀比例視訊，以發佈至桌上型電腦、行動裝置(iPhone、iPad、Android)和平板電腦(iPad、Android)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   **適應性影片**

   單一編碼預設集，可與任何外觀比例搭配使用，以為傳遞至行動裝置、平板電腦和桌上型電腦建立視訊。使用此預設集編碼而上載的來源視訊，會設定成固定的高度。不過，寬度會自動調整為保留視訊的外觀比例。

   具有「自動縮放」的彈性預設也會在您建立自己的自訂視訊編碼預設集時可供使用。

   請參閱[增加或編輯視訊編碼預設集](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)。

   **最適化視訊編碼 (16:9 或 4:3)**

   建立16:9和4:3外觀比例的視訊，以發佈至桌上型電腦、行動裝置(iPhone、iPad、Android)和平板電腦(iPad、Android)，並以最符合檢視器連線速度的解析度和位元速率最佳化。

   請參閱[最適化視訊編碼 (16:9 或 4:3) 視訊預設集](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   **單一編碼預設集**

   >[註]
   >
   >若要將視訊傳送到 iPad，您可以選擇「行動裝置」編碼預設集或「平板電腦」編碼預設集。平板電腦預設集專為 iPad 而設計，通常具有更高的解析度和品質，以充分利用更大的畫面和頻寬連線。傳送使用平板電腦預設集編碼的視訊檔案時，必須在您的行動裝置網站或應用程式上加入裝置偵測程式碼。此程式碼會根據播放裝置的不同，在 iPhone 或 iPad 視訊體驗間切換。更簡單的工作流程是選擇行動裝置預設集將視訊檔案傳送到 iPad。原因在於您可以將同一視訊檔案用於 iPhone 和 iPad。但是，將品質標準化為解析度更低的 iPhone 體驗。

   * 在「編碼預設集」群組下方的「排序編碼預設集」下拉式清單中，選取要依據名稱或解析度大小來排序預設集時的「名稱」或「大小」。
   * 根據您計畫播放視訊的解析度大小和頻寬，選擇編碼預設集。
   * 您可以為每個視訊選取「最適化視訊編碼」及一個或多個編碼預設集。例如，您可以在一個上載工作中針對桌面和行動裝置編碼檔案。

在您按一下「**開始上載**」之後，會上載原始主視訊檔案，並從主檔案產生編碼檔案。

### 關於編碼預設集選項 {#about-encoding-preset-options}

編碼預設集選項的參數如下:

**目標連線速度** ：目標使用者的網際網路連線速度。

**編碼檔案字尾** ：附加至編碼視訊檔案以用於識別目的的字尾。

**視訊位元速率（資料速率）** ：編碼成視訊播放一秒（千位／秒）的資料量。

**像素寬度／高度** ：螢幕影像的寬度尺寸，以像素為單位；螢幕影像的高度尺寸（以像素為單位）。

**每秒影格數(fps)** ：視訊每秒的影格數，或靜止影像數。 在美國和日本，大部分視訊以 29.97 fps 拍攝；在歐洲和亞洲 (不包括日本)，大部分視訊以 25 fps 拍攝。電影以 24 fps 拍攝。

**音訊位元速率** ：編碼成每秒音訊播放一秒的資料量（千位／秒）。

下表說明在選取視訊預設集及用來指定編碼檔案的命名慣例時建議的最佳實踐。

### 最適化視訊 (預設) {#adaptive-video-default}

編碼預設集，可與任何外觀比例搭配使用，以讓您為傳遞至行動裝置、平板電腦和桌上型電腦建立視訊。使用此預設集 (預設且最佳實踐) 編碼而上載的來源視訊會設為固定的高度，寬度則是會自動縮放，以保留視訊的外觀比例。

**最適化視訊 (預設)**

|  | 編碼預設集名稱/工具提示文字 | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 自動 x 360，800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 與來源同 | 64 | 適用行動裝置 (iPhone、iPad、Android) |
| 2 | 自動 x 480，1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 與來源同 | 96 | 適用平板電腦 (iPad、Android) |
| 3 | 自動 x 720，2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | 與來源同 | 128 | 適用於案頭 |

### 最適化視訊編碼 (16:9 或 4:3) 視訊預設集 {#adaptive-video-encoding-or-video-presets}

這些最適化視訊編碼預設集，結合了一系列會根據您所上載之視訊的外觀比例自動為您選取的個別編碼預設集。例如，如果您上載 4:3 視訊，則系統會自動使用在「**最適化視訊編碼 (16:9 或 4:3)**」選項的主預設集清單中找到的五個 4:3 預設集進行編碼。

有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

**最適化視訊編碼 (16:9 或 4:3) 預設集**

|  | 編碼預設集名稱/工具提示文字 | 目標連線速度 (Kbps) | 編碼檔案字尾 | 視訊資料速率 (Kbps) | 寬度/高度 (像素) | Fps | 音訊位元速率 (kbps) | 建議 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、512x288、行動裝置 (iPhone、iPad、Android)、(400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 與來源同 | 64 | 低解析度、3G |
| 2 | 4:3、384x288px、行動裝置 (iPhone、iPad、Android)、(400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 與來源同 | 64 | 低解析度、3G |
| 3 | 16:9、512x288、行動裝置 (iPhone、iPad、Android)、(600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 與來源同 | 64 | 中等解析度、3G |
| 4 | 4:3、384x288、行動裝置 (iPhone、iPad、Android)、(600 Kbps) | 700 | _Mobile_384x288_600 | 600 | 384x288 | 與來源同 | 64 | 中等解析度、3G |
| 5 | 16:9、640x360、平板電腦 (iPad、Android)、(800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640x360 | 與來源同 | 80 | 中等解析度、WiFi |
| 6 | 4:3、640x480、平板電腦 (iPad、Android)、(800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640x480 | 與來源同 | 80 | 中等解析度、WiFi |
| 7 | 16:9、768x432、平板電腦 (iPad、Android)、(1200 Kbps) | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768x432 | 與來源同 | 96 | 高解析度、WiFi |
| 8 | 4:3、768x576、平板電腦 (iPad、Android)、(1200 Kbps) | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 與來源同 | 96 | 高解析度、WiFi |
| 9 | 16:9, 1280x720，桌上型電腦，(2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 與來源同 | 128 | 高畫質、寬螢幕 |
| 10 | 4:3, 1280x960，桌上型電腦，(2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | 與來源同 | 128 | 高畫質 |

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

與來源 fps 相同。iPhone、iPad 與 Android 行動裝置的視訊編碼預設集。

有關編碼選項參數的資訊，請參閱[關於編碼預設集選項](application-setup.md#about_encoding_preset_options)。

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
>**Flash檢視器停售通知** -自2017年1月31日起，Adobe Scene7 Publishing System正式終止對Flash檢視器平台的支援。 如需此重要變更的詳細資訊，請參閱下列常見問答網站： [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html)。

*檢視器預設集*&#x200B;是決定使用者如何在電腦螢幕和行動裝置上檢視多媒體資產的設定集合。身為一名管理員，您可以建立檢視器預設集。設定可用於檢視器設定選項的陣列。例如，您可以變更檢視器顯示大小、縮放行為、色彩方案、邊框和字型。

最佳實務是使用Dynamic Media Classic HTML5視訊檢視器。 HTML5 視訊檢視器使用的預設集是健全的視訊播放器。此單一播放程式集諸多功能於一身，能夠使用 HTML5 與 CSS 來設計播放組件，能夠實現內嵌播放，還能夠根據瀏覽器的功能來使用最適化串流與漸進式串流，可協助您將多媒體內容同時提供給桌上型電腦、平板電腦和行動裝置使用者，並確保順暢的視訊體驗。

請參 [閱Adobe檢視器參考指南](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) 中的關於HTML5檢視器。

請參 [閱Dynamic Media Classic檢視器預設集相容性矩陣](application-setup.md#scene7_viewer_preset_compatibility_matrix)。

請參閱[最佳實踐: 使用 HTML5 視訊檢視器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

依據檢視器而定，您可以增加社群功能。社群功能包含「內嵌」按鈕、「電子郵件」按鈕、「連結」按鈕和「造訪網站」按鈕。這些按鈕可讓使用檢視器的使用者與其他人共用檢視器，或開啟Dynamic Media Classic網站。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

### 回應式網頁的檢視器支援 {#viewer-support-for-responsive-designed-web-pages}

不同網頁有不同的需求。有時候您希望網頁提供的連結可在個別的瀏覽器視窗中開啟 HTML5 檢視器。有時候，則必須將 HTML5 檢視器直接嵌入主控頁面中。以後者來說，網頁可能有靜態版面。或者，可能會依據不同的裝置或不同的瀏覽器視窗大小進行「回應」並顯示不同的內容。為滿足這些需求，Dynamic Media Classic隨附的HTML5檢視器支援靜態網頁和互動式設計網頁。

See [Responsive Static Image library](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)in the *Adobe Image Serving API Help* for more information on how to embed responsive viewers onto your web pages.

### 檢視器預設集類型 {#viewer-preset-types}

管理員可以建立和自訂以下類型的檢視器預設集:

**eCatalog Viewer** （eCatalog檢視器）模擬閱讀列印目錄的體驗。 您可以在頁面之間移動、放大和縮小頁面上的項目、使用影像地圖來查看頁面上項目的更多資訊，或搜尋目錄。 如果地圖區域擁有有效的 rollover_key 屬性，您也可以加入資訊面板以顯示詳細資訊和影像對應項目。若要加入資訊面板，請在「eCatalog 檢視器預設集」視窗中指定資訊伺服器 URL。

**色票集檢視器** ：以不同的顏色、材質、紋理、光潔度或結構顯示影像。 使用者按一下縮圖，即可查看到影像的變化。

**混合媒體集檢視器** ：在單一檢視器中顯示不同類型的媒體。 您可以加入色票集、迴轉集、影像和視訊。您可以設定標籤以包含不同類型的內容，例如影像集標籤和視訊標籤。從混合媒體集播放的視訊會使用含有時間軸和視訊控制項 (如「停止」、「暫停」、「倒轉」和「播放」) 的標準視訊檢視器。設定混合媒體集檢視器預設集時，請指定要針對混合媒體集中不同類型資產使用的檢視器。您也可以使用格線檢視器或轉盤檢視器來檢視混合媒體集。

**回轉集檢視器** —提供影像的多個檢視，讓使用者可以旋轉物件來檢查不同的側面和角度。

**視訊檢視器** ：使用來源檔案的解析度尺寸或自訂大小來顯示視訊。 Dynamic Media Classic隨附許多預先定義的檢視器預設集，以播放視訊，如果您是管理員，則可建立自訂的視訊檢視器預設集。 有十幾種不同的設定可用於配置「視訊檢視器」。您可以設定其大小、前景和背景顏色、視訊和音訊控制項、進度列、使用者介面外觀、社交功能和「說明」。

**縮放檢視器** ：提供三種縮放檢視器類型的選擇：

**縮放檢視器** ：讓使用者按一下區域即可放大檢視。 使用者可以按一下控制項來放大、縮小，以及將影像重設為預設大小。

**縮放檢視器：飛出** ：在原始影像旁顯示縮放區域的第二個影像。 沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。主要影像大小 (「舞台寬度」和「舞台高度」) 和「縮放係數」會決定彈出影像大小。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

### Dynamic Media Classic檢視器預設集相容性矩陣 {#scene-viewer-preset-compatibility-matrix}

**Flash檢視器生命週期結束注意事項**:自2017年1月31日起，Adobe Scene7 Publishing System正式終止對Flash檢視器平台的支援。

如需此重要變更的詳細資訊，請參閱下列常見問答網站： [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html)。

下表列出目前可用的Dynamic Media Classic Viewer預設集。 此表格也指定了檢視器與桌上型電腦和行動裝置的相容性，以及用於個別檢視器的技術。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

如需有關檢視器支援的 Web 瀏覽器和作業系統版本的資訊，您可以檢閱「檢視器發行說明」。

請參閱 [Adobe檢視器參考發行說明](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 縮放檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 色票集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 檢視器 |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv（包含對社交媒體和目錄搜尋的支援）。 | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包含對社交媒體和目錄搜尋的支援）。 | HTML5 | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 迴轉檢視器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 檢視器**

Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。

* 您可以在以下位置找到支援此視訊格式的Blackberry裝置：Blackberry [上支援的視訊格式](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* 您也可以在下列位置找到支援此視訊格式的Windows裝置：Windows Phone[上支援的視訊格式](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 | BlackBerry 智慧型手機 | Windows 電話 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包含隱藏字幕的支援）。See [Best practice: Using the Universal HTML5 Video viewer.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包含對隱藏字幕和社交媒體的支援）。 | HTML5 | X | X | X | X | X | X | X |

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒體集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支援的行動檢視器手勢矩陣 {#supported-mobile-viewers-gestures-matrix}

下表說明 iOS、Android 2.x 與 Android 3.x 裝置所支援的行動檢視器手勢。

|  | 檢視器技術 | 桌上型電腦 | Apple iPhone | Apple iPad | Android 智慧型手機 | Android 平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 影像集檢視器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 關於「檢視器預設集」畫面 {#about-the-viewer-preset-screen}

在「檢視器預設集」畫面建立和管理檢視器預設集。若要開啟此畫面，請按一下「**設定** > **檢視器預設集**」。

「檢視器預設集」畫面提供了執行下列工作的工具:

**新增預設集** 「按一下新增」，並在「新增檢視器預設集」對話方塊中做出選擇。

請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

**編輯預設** ：選取預設，然後按一下「編 **輯」**。

請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

**刪除預設** ：選取預設，然後按一下「刪 **除」**。

**匯出預設** ：選取HTML5檢視器預設，然後按一下「匯出」以下載檢視器面板，讓您將它當做建立和新增檢視器預設的基礎。

請參 [閱匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。

**篩選檢視器預設集清單** ：使用這些工具來篩選清單：

* 開啟「**作用中/非作用中**」下拉式清單並選擇一個選項，以顯示作用中的預設集、非作用中的預設集或所有預設集。
* 開啟「**檢視器**」下拉式清單並選擇一個選項，以僅查看特定種類的檢視器。選擇「**所有檢視器**」以查看所有檢視器。

**排序預設** ：按一下欄標題（「作用中」、「文字」、「預設集」或「平台」），以排序欄上的清單。 再按一下欄標題即可依遞減 (或遞增) 順序排列清單。

**啟用和停用預設** ：選取預設集，然後按一下其「作用中」選項以啟用或停用它。

請參閱[啟用或停用檢視器預設集](application-setup.md#activating_or_deactivating_viewer_presets)。

>[!NOTE]
>
>按一下「檢視器預設集」畫面右側的「預覽」即可檢視資產在您選取的檢視器預設集中外觀如何。若要查看不同資產，您可以按一下「檢視器預設集」畫面中的「瀏覽」，並在「選取資產預覽」對話框中選取不同資產。

### 增加和編輯檢視器預設集 {#adding-and-editing-viewer-presets}

除了在使用者介面中使用「增加」來增加檢視器預設集之外，您也可以使用「匯出」來增加檢視器預設集。您只需匯出現有的HTML5檢視器預設集，然後將該預設集當做新預設集的基礎。

請參 [閱匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。

**增加和編輯檢視器預設集**

1. 在靠近 Scene7 Publishing System 右上角的地方，按一下「**設定** > **檢視器預設集**」。

   您可以篩選預設集的清單。例如，若只要查看視訊檢視器的預設集，請從表格正上方工具列上的「檢視器」下拉式選單中選取「視訊檢視器」。

1. 在「檢視器預設集」畫面中，增加或編輯「檢視器預設集」畫面上的檢視器預設集。

   **新增** ，按一下工具列上的新增。 在「增加檢視器預設集」對話框中，選擇平台後，然後選擇多媒體資產類型。

   完成建立檢視器預設集後，請按一下「**另存新檔**」。

   **從現有的檢視器預設集開始新增** 。在表格中，選取視訊檢視器預設集，然後按一下工具列上的編輯。

   重新設定「視訊檢視器」後，在「預設集名稱」文字欄位中按一下「**另存新檔**」，以不同的名稱儲存預設集。

   **編輯** ：選取現有的檢視器預設集，然後按一下「編 **輯」**。

1. 在「設定檢視器」畫面的「預設集名稱」欄位中，輸入或編輯預設集名稱。
1. 設定其它想要的選項。

   >[註]
   >
   >選擇「與來源同」，將「視訊檢視器」自動調整為編碼視訊自身的解析度大小。如果選擇該選項，則不能輸入「舞台寬度」和「舞台高度」。相反，這些選項來自視訊本身。如果您選擇「與來源同」，請設定「邊距大小」選項以反映視訊播放區域外部的外觀尺寸。該邊距大小是視訊控制項的像素高度和寬度。您可以使用以下圖示來協助您決定要使用的邊距大小。*

   ![](assets/vs_video_viewer_configure_margin.png)

1. 進行以下一項操作:

   * 如果從現有預設集開始增加「檢視器預設集」，請按一下「**另存新檔**」。
   * 如果是增加或編輯「檢視器預設集」，請按一下「**儲存**」。

### 匯出HTML5檢視器預設集 {#exporting-an-html-viewer-preset}

您可以匯出現有的HTML5檢視器預設集，做為建立新HTML5檢視器預設集的基礎。 匯出選項十分有用，因為您不需從頭建立檢視器， 但可以匯出與您要的外觀和行為接近的預設集，然後將其用作進行設計調整的起點。

請注意，SPS中所有預設的現成檢視器預設CSS檔案都使用指向位於資產的相對影像伺服路徑 `Scene7SharedAssets`。 例如，以下是檢視器預設CSS檔案中影像資產的相對路徑，位於 `Scene7SharedAsset`:不 `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`過，如果您在自己的網站上代管檢視器CSS檔案，則必須透過在自己的環境中使用影像伺服器的明確路徑來解析這些相對影像路徑。 為了便於說明，如果要將上面的相對路徑更新為顯式路徑，則其外觀可能如下，其中 `https://s7d1.scene7.com` 是映像伺服器的直接路徑： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**若要匯出HTML5檢視器預設集**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 按一下「**設定**」>「**檢視器預設集**」。
1. On the Viewer Presets toolbar, in the second drop-down list from the left, select **HTML5**.
1. 在左邊第三個下拉式清單中，選取&#x200B;**所有檢視器**。
1. 選取您要當做新HTML5檢視器預設集基礎的檢視器預設集。
1. 在工具列中按一下「**匯出**」。
1. 在「匯出選取的資產」對話框中按一下「**提交匯出**」。

   匯出後，您會取得CSS檔案。 下載並解壓縮檔案。

1. 在 CSS 編輯器中開啟 CSS 檔案，進行變更後儲存檔案。
1. 將CSS檔案上傳至Scene7 Publishing System。

   請參閱[上載檔案](uploading-files.md#uploading_files)。

1. 將CSS檔案發佈至動態媒體影像伺服器。

   請參閱[發佈檔案](publishing-files.md#publishing_files)。

1. 照常增加檢視器預設集。選取您上傳的檢視器CSS檔案。

   請參閱[增加和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。

### 啟用或停用檢視器預設集 {#activating-or-deactivating-viewer-presets}

若要建立 URL 來顯示資產，使用者可以開啟「預覽」對話框中的「預設集」下拉式清單、選取「檢視器預設集」，然後按一下「複製 URL」(請參閱[複製檢視器預設集的 URL](application-setup.md#copying_the_url_of_a_viewer_preset))。預設集清單提供了管理員在「檢視器預設集」畫面所增加和管理的檢視器預設集。例如，使用者預覽 eCatalog 時，所有作用中的 eCatalog 檢視器預設集都會顯示在「預覽」對話框中的「預設集」下拉式清單中。

除非您在「檢視器預設集」畫面上停用檢視器預設集，否則「預覽」對話框中的「預設集」下拉式清單可能會過於擁擠。

**啟用或停用「檢視器預設集」**

1. Choose **Setup** > **Viewer Presets** to open the Viewer Presets screen.
1. 選取或取消選取「作用中」選項，即可啟用或停用檢視器預設集。

### 複製檢視器預設集的 URL {#copying-the-url-of-a-viewer-preset}

發佈資產後，您就可以複製 URL，以「檢視器預設集」的設定來顯示資產。

URL 便會複製到剪貼簿。您可以視需要在網頁、行動裝置或應用程式的 HTML 代碼中加以使用。

**複製檢視器預設集的 URL**

1. 在「瀏覽面板」中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側「URL」和「內嵌程式碼」面板中，按一下您要的檢視器右側的「**複製 URL**」。
   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方按一下「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。

   * 按一下「**清單檢視**」。在「資產瀏覽」面板中，選取單一資產，然後按一下縮圖影像右側的「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。

   * 按一下「**格點檢視**」、「**清單檢視**」或「**詳細檢視**」。在同一個工具列上，按一下「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**複製 URL**」。

### 複製檢視器預設集的內嵌程式碼 {#copying-the-embed-code-of-a-viewer-preset}

您可使用「內嵌程式碼」功能查看所選「檢視器預設集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。

「內嵌代碼」對話方塊中不允許編 輯代碼 。

**複製檢視器預設集的內嵌程式碼**

1. 在「資產瀏覽」面板中選取資產。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的 URL 面板中，按一下「**內嵌程式碼**」。
   * 按一下「**格點檢視**」。在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方按一下「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。

   * 按一下「**清單檢視**」。在「資產瀏覽」面板中，選取單一資產，然後按一下縮圖影像右側的「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。

   * 按一下「**格點檢視**」、「**清單檢視**」或「**詳細檢視**」。在同一個工具列上，按一下「**預覽** > **檢視器清單**」。
   在「檢視器清單」頁面，按一下表格中「動作」欄下方的「**內嵌程式碼**」。

1. 在「內嵌程式碼」對話框中，按一下「**複製至剪貼簿**」。
1. 按一下「**關閉**」。

## 設定預設檢視器 {#configuring-default-viewers}

您可以使用「預設檢視器」來設定當您使用 Scene7 Publishing System 中的「預覽」功能時，要與其相關聯的預設檢視器。您可以針對下列資產類型設定預設的預覽體驗:

* 影像
* 視訊
* 迴轉集
* 目錄
* 影像集
* 色票集
* 媒體集

**設定預設檢視器**

1. In the Setup drop-down list, click **Application Setup**.
1. In the Setup window, in the left pane, expand **Application Setup** > **Viewers**
1. Click **Default Viewers**.
1. 在「預設檢視器」視窗中，從每個資產類型下拉式清單中選取您要與資產預覽相關聯的檢視器。
1. In the lower-right corner of the Default Viewers window, click **Save Settings**.
1. In the lower-right corner of the Setup window, click **Close** to return to the Asset window.

## 中繼資料檢視 {#metadata-views}

*中繼資料*&#x200B;是有關資產的標準化資料。您可以使用中繼資料來簡化工作流程、組織資產和改善搜尋。Dynamic Media Classic支援IPTC（國際新聞通訊委員會）標準和XMP（可擴充的中繼資料平台）標準。 使用者在詳細檢視中檢視或輸入有關資產的中繼資料前，可以開啟「中繼資料檢視」選單，並選擇要檢視或用來描述資產的中繼資料欄位集。

Dynamic Media Classic隨附預先定義的中繼資料檢視，管理員可建立自己的中繼資料檢視，讓使用者在輸入中繼資料時選擇。

### 建立中繼資料檢視 {#creating-a-metadata-view}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Views**.
1. 按一下「**增加**」。
1. 在「預設集名稱」文字欄位中，輸入檢視的名稱。
1. (Optional) Check **Make Default** to make this view the one that users see when they open the Metadata panel in Detail View.
1. (Optional) Select **Include UDF** to include user-defined fields in the view. 使用者定義的欄位會顯示在詳細檢視的「中繼資料」面板上方。
1. Select the fields you want for the view (click **Select All** to select all the fields).
1. 按一下&#x200B;**「儲存」**。

   選取的檢視類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料檢視 {#managing-metadata-views}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Views**.
1. 請執行下列任一動作:

   * 若要預覽檢視，請加以選取。檢視中的欄位會顯示在「預覽」面板中。
   * To edit a view, select it and then click **Edit**. Then select or deselect field names on the Preview panel, and select or deselect the **Include UDF** option.
   * To delete a view, select it and then click **Delete**.
   * To make a view the default, select it and then click **Make Default**. 預設檢視為使用者在詳細檢視中開啟資產，並前往「中繼資料」面板時所看見的檢視。

## 中繼資料預設集 {#metadata-presets}

中繼資料預設集讓管理員能夠控制和調節為資產指定的中繼資料。在詳細檢視中，使用者可以在輸入資產中繼資料專用的欄位中輸入資產的相關中繼資料。例如，使用者可以輸入擁有者名稱、版權描述和地址。若要確保使用者準確且完整地輸入此資訊，您可以建立中繼資料預設集。在詳細檢視中選擇中繼資料預設集，會將預先定義的值填入中繼資料欄位。例如，擁有者名稱、版權描述和地址皆會自動輸入。

針對各個您要讓使用者能夠在詳細檢視中自動輸入以描述資產的中繼資料值集，建立中繼資料預設集。

### 建立或編輯中繼資料預設集 {#creating-or-editing-a-metadata-preset}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Presets** .
1. 在「中繼資料預設集」面板中，執行下列任一項作業:

   * To create a preset, click **Add**. 在「中繼資料範本名稱」文字欄位中，輸入預設集的名稱，然後按一下「中繼資料檢視 **」，然後從下拉式清單中選擇檢視(請參閱** 中繼資料檢視 [](application-setup.md#metadata_views))。
   * To edit an existing preset, select the preset from the Metadata Presets list and then click **Edit**.

1. 展開您要加入預設集的標題，並在您要加入預設集的不同欄位中輸入值。
1. 按一下&#x200B;**「儲存」**。

   選取的預設集類別和欄位會顯示在「預覽」面板中。

### 管理中繼資料預設集 {#managing-metadata-presets}

1. Click **Setup** > **Application Setup** > **Metadata** > **Metadata Presets**.
1. 請執行下列任一動作:

   * 若要預覽預設集，請選取您要預覽的預設集。預設集資訊 (類別和欄位) 會顯示在「預覽」畫面中。
   * To delete a preset, select the preset, and then click **Delete**.

## 使用者定義的欄位 {#user-defined-fields}

媒體入口網站管理員或公司管理員可建立自訂、使用者定義的中繼資料欄位。自訂欄位可協助您在Scene7 Publishing System中組織資產。 您可以視需要將欄位標示為「作用中」。 啟用時，這些自訂中繼資料欄位的名稱會顯示在詳細檢視的「中繼資料」面板中。使用者可以在使用者自訂的中繼資料欄位中輸入資訊，以描述資產。使用者也可以將使用者定義的中繼資料欄位設定作為搜尋條件。

使用者定義的中繼資料欄位的有效用途之一，就是針對特定的上市發表會或銷售會，延遲資產的啟用時間。您會根據「日期」類型定義「啟動」 *欄位*。 Then, using the **Metadata** panel in **Detail** view or **File** > **Edit Info**, you can specify when the asset is activated. Scene7 Publishing System 會檢查資產的發佈狀態與發佈操作記錄。如果未在啟動時間內，則發佈狀態會顯示為「未發佈」。

>[!NOTE]
>
>若要讓使用者定義的欄位顯示在詳細檢視的「中繼資料」面板中，請包含「中繼資料檢視」之使用者定義的欄位。在「中繼資料檢視」畫面上選取「包含 UDF」(使用者定義欄位) 選項。如需詳細資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views)。

>[!NOTE]
>
>若要使用自訂、使用者定義的欄位搜尋資產，請按一下「**設定**」>「**個人設定**」，然後選取「**搜尋時包含 UDF**」。請參閱[個人設定](personal-setup.md#personal_setup)。

### 建立使用者定義的中繼資料欄位 {#creating-a-user-defined-metadata-field}

1. 按一下「**設定** > **應用程式設定** > **中繼資料** > **使用者定義的欄位**」。
1. 按一下「**增加**」
1. 在「自訂欄位」對話框中，設定您要的選項。

   **名稱** ：輸入中繼資料欄位的名稱。

   **類型** ：選擇一個選項，它定義用戶可以在元資料欄位中輸入的資訊類型：

   **字串** ：文字字串。

   **整數** 。

   **浮點數** ：浮點數。

   **是／否** A是／否布爾值。

   **日期** A日期。 接受 MM/DD/YYYY 格式。

   **檔案名** ：檔案的名稱。

   **顏色** ：顏色的名稱。

   **Dimension** 資產的寬度和高度。

   **無類型** ，以向後相容。 請勿選取此選項。

   **預設值** （可選）輸入用戶最可能在欄位中輸入的值。 您輸入的值會成為您建立之欄位的預設值。

   **套用至** （可選）如果希望元資料欄位僅應用於特定資產類型，請選擇資產類型。

   ***Note**: Choose an **Applies To** option carefully because you cannot change the **Applies To** option after you create a user-defined field. Dynamic Media Classic lets you edit the name, type, and default value of a user-defined field, but not the **Applies To** setting. *

1. 完成建立中繼資料欄位後，請按一下「**儲存**」。

### 管理使用者定義的欄位 {#manage-user-defined-fields}

「使用者定義的欄位」畫面提供了管理自訂、使用者定義之中繼資料欄位的命令。

只有 Media Portal 管理員或公司管理員才可以管理使用者定義的欄位。

若要開啟此畫面，請按一下「**設定** > **應用程式設定** > **中繼資料** > **使用者定義的欄位**」。

**編輯欄位** ：選取欄位，然後按一下「編 **輯」**。

**刪除欄位** ：選取欄位，然後按一下「刪 **除」**。

**啟用欄位** ：按一下以選取或取消選取欄位名稱旁的「作用中」選項。 如果您的角色是公司管理員，這個選項可能不會顯示。由於此選項與MediaPortal相關，因此您必須在個人設定中選取（開啟）「顯示MediaPortal功能」，以檢視啟動欄位。

## 最佳化檔案 {#optimize-files}

將檔案上載至 Scene7 Publishing System 後，系統便會將其最佳化以供儲存和發佈。不過，如果上載程序受到中斷，部分影像就無法最佳化。在此情況下，您會看見「尚未最佳化影像」訊息。但是，如果您是管理員，就可以最佳化這些檔案。

Scene7 Publishing System 會搜尋檔案，並僅最佳化先前尚未完整最佳化的影像。

1. 選擇「 **設定** >應用 **程式設定**」，然後選取「最&#x200B;**佳化檔案」**。
1. Enter information for the optimization job and click **Submit**.

   如果您使用超過一家公司，請分別對屬於不同公司的檔案執行最佳化。

## 批次集預設集 {#batch-set-presets}

將資產上載至 Scene7 Publishing System 的工作仍在執行時，使用批次集預設集即可自動建立影像集或迴轉集。

公司管理員必須先為要分組至同一個集的資產定義命名慣例。接著，您可以建立批次集預設集來參考這些影像。每個預設集都是具備唯一名稱的內部獨立式指示集，定義如何使用與預設集配置中已定義的命名慣例相符的影像來建構集。

所有作用中的公司批次集預設集都會列在「上載工作選項」對話框中，以便您指定要在每個上載工作階段期間套用的預設集。公司管理員會看到所有作用中和非作用中的批次集預設集。當您上傳檔案時，Dynamic Media Classic會自動建立一組檔案，其中所有檔案都符合作用中預設集中定義的命名慣例。

### 預設命名 {#default-naming}

公司管理員會建立任何批次集預設集配置中使用的預設命名慣例。在批次集預設集定義中選取的預設命名慣例，可能便是您的公司為所有網站批次產生集時所需的一切。必須建立批次集預設集，才能使用您所定義的預設命名慣例。公司定義的預設命名有例外情況時，您可以透過特定內容集所需的替代、自訂命名慣例來建立同等數量的批次集預設集。

雖然不需設定預設命名慣例即可使用批次集預設集功能，但最佳實務是，建議您使用預設命名慣例，盡量充分定義要分組至某個集的命名慣例元素，以簡化批次集的建立作業。

1. 按一下「**設定** > **應用程式設定** > **批次集預設集** > **預設命名**」。
1. 選擇 **「查看表單** 」或「 **查看代碼」** ，以指定要查看的方式並輸入有關每個元素的資訊。

   您可以選取「檢視器碼」核取方框，來檢視表格選擇項目旁的規則運算式值建置。如果表單檢視因故對您有所限制，則您可以輸入或變更這些值，以幫助定義命名慣例的元素。如果您的值無法在表單檢視中剖析，則表單欄位的狀態會變成非作用中。

   >[!NOTE]
   停用的表單欄位不代表規則運算式無效。沒有驗證方式可確認您的規則運算式是否正確。在「結果」行之後，您會看見針對個別元素所建置之規則運算式的結果。您可以在頁面底部看到完整的規則運算式。

1. 視需要展開個別元素，並輸入您要使用的命名慣例。
1. 視需要按一下「**增加**」即可新增其他元素的命名慣例。或按一下「**移除**」，即可刪除元素命名慣例。
1. 按一下「**另存新檔**」並輸入預設集名稱。或者如果您正在編輯現有預設集，請按一下「**儲存**」。

您也可以使用不含任何可用表單欄位的「檢視器碼」。在此檢視中，您可以完全使用規則運算式來建立命名慣例定義。

有兩個元素可供定義，分別為「符合」和「基本名稱」。這些欄位可讓您定義所有命名慣例元素，並識別慣例中用來命名其中所含之集的部分。公司的個別命名慣例可能會針對個別元素採用一或多行的定義。您可以針對唯一定義使用同等數量的行，並將其分組至不同的元素，例如「主影像」、「色彩元素」、「替代檢視」元素和「色票」元素。

### 建立批次集預設集 {#creating-a-batch-set-preset}

Dynamic Media Classic使用批次集預設集，將共用某些常見資訊或內容的資產組織成一組影像，以便在檢視器中顯示。 批次集預設方式會隨您在Dynamic Media Classic中排程的資產匯入工作一起自動執行。

使用「批次集預設集」即可建立、編輯和管理批次集預設集。您可以視需要建立同等數量的批次集預設集，以涵蓋您需要得所有資產擷取工作。批次集預設集定義共有兩個形式: 一種用於您可能已經設定的預設命名慣例，另一種則用於您動態建立的自訂命名慣例。

您可以使用表單欄位方式來定義批次集預設集，也可以使用代碼方式來允許使用規則運算式。如同「預設命名」一樣，在「檢視表單」中定義的同時，您也可以選擇「檢視器碼」，並使用規則運算式來建置定義。您也可以取消核取任一檢視，僅使用其中一種。

另請參閱[建立批次集預設集以自動產生 2D 迴轉集](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)。

**建立批次集預設集**

1. 按一下「**設定** > **應用程式設定** > **批次集預設集** > **批次集預設集**」。「**檢視表單**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設集清單」面板中按一下「**增加**」，以啟用畫面右側「詳細資料」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批次集類型」下拉式功能表中，選取預設集類型。

   若要自動產生 2D 迴轉集，請從「批次集類型」下拉式清單中選取「**多軸旋轉集**」。

1. 進行以下一項操作:

   * 如果您要使用先前在「應用程式設定 > 批次集預設集 > 預設命名」下設定的預設命名慣例，請展開「**資產命名慣例**」，然後在「檔案命名」下拉式清單中按一下「**預設**」。
   * 若要在設定預設集時定義命名慣例，請展開「**資產命名慣例**」，然後在「檔案命名」下拉式清單中按一下「**自訂**」。

1. 在「序列」順序中，在Dynamic Media Classic中將影像集分組後，定義影像的順序。 根據預設，您的資產會按照字母順序排列。不過，您可以使用規則運算式以逗號分隔的清單來定義順序。
1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。也可定義在Dynamic Media Classic檔案夾結構中建立影像集的位置。

   如果您定義了大量影像集，則您可能會想要將這些影像集與本身含有資產的檔案夾加以區隔。許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 在「詳細資料」面板中按一下「**儲存**」。

### 建立批次集預設集以自動產生 2D 迴轉集 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您也可以使用批次集類型「**多軸旋轉集**」來建立可自動產生 2D 迴轉集的「配置」。影像的群組會使用列與欄規則運算式，使影像資產適當對齊於多維度陣列中的對應位置上。

另請參閱[建立批次集預設集](application-setup.md#creating_a_batch_set_preset)。

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

根據這些資訊，可以建立的「批次集類型」配置如下:

![](assets/se_batch_set_recipe.png)

對spinset的共用資產名稱部分進行分組將添加到「匹 **配** 」欄位 (如突出顯示)。包含行和列的資產名稱的變數部分將分別添加到 **行** 和 **列欄位中** 。

上傳和發佈回轉集時，您會啟用「上傳工作選項」對話方塊中「批次集預設集」下方所列的2D回轉集 **方式名稱****** 。

**建立批次集預設集以自動產生 2D 迴轉集**

1. 選擇「**設定**」>「**應用程式設定**」>「**批次集預設集**」>「**批次集預設集**」。 「**檢視表單**」(設定於「詳細資料」頁面的右上角) 是預設檢視。
1. 在「預設集清單」面板中按一下「**增加**」，以啟用畫面右側「詳細資料」面板中的定義欄位。
1. 在「詳細資料」面板的「預設集名稱」欄位中，輸入預設集的名稱。
1. 在「批集類型」下拉式功能表中，選擇「資產 **集」**。
1. 在「子類型」下拉式清單中，選取「**多軸轉旋轉集**」。
1. 展開「**資產命名慣例**」，然後在「檔案命名」下拉式清單中按一下「**自訂**」。
1. 使用「 **比對** 」(Match **)和 (可選) 「基本名稱** 」(Base Name)屬性，定義組成群組之影像資產的命名規則運算式。

   例如，您實際的「符合」規則運算式可能看起來如下:

   `(\w+)-\w+-\w+`

1. 展開「**列欄位置**」，然後為影像資產在 2D 迴轉集陣列內的所在位置定義名稱格式。

   使用括號括住檔案名稱中的列或欄位置。

   例如，對於您的列規則運算式，可能看起來如下:

   `\w+-R([0-9]+)-\w+`

   或

   `\w+-(\d+)-\w+`

   對於您的欄規則運算式，可能看起來如下:

   `\w+-\w+-C([0-9]+)`

   或

   `\w+-\w+-C(\d+)`

   請記住，這些只是範例。您可以用任何想要的方式建立規則運算式以符合自己的需求。

   >[!NOTE]
   如果列與欄規則運算式的組合無法決定資產在多維度迴轉集陣列內的位置，則不會將該資產增加至集內，並且會記錄錯誤。

1. 針對「設定命名和建立慣例」，請為您在「資產命名慣例」中定義的基本名稱指定字尾或字首。也可定義在Dynamic Media Classic檔案夾結構中建立影像集的位置。

   如果您定義了大量影像集，則您可能會想要將這些影像集與本身含有資產的檔案夾加以區隔。許多客戶會建立影像集檔案夾，並將應用程式重新導向，以將批次集所產生的集置放於此處。

1. 在「詳細資料」面板中按一下「**儲存**」。
1. 如往常般上載並發佈您的迴轉集，過程中確定您在「工作載入選項」對話框的「批次集預設集」下啟用 2D 迴轉集的名稱。

>[!MORELIKETHIS]
* [預覽資產](previewing-asset.md#previewing_an_asset)
* [設定影像預設集](setting-image-presets.md#setting_up_image_presets)
* [檢視、增加和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Checking job files](checking-job-files.md#checking_job_files)

