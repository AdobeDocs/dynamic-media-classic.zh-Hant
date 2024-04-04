---
title: 檢視、新增和匯出中繼資料
description: 瞭解如何在Adobe Dynamic Media Classic中檢視、新增和匯出中繼資料。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '2226'
ht-degree: 40%

---

# 檢視、新增和匯出中繼資料{#viewing-adding-and-exporting-metadata}

您可以在Adobe Dynamic Media Classic中儲存您使用之檔案的特定資訊；此資訊稱為 *中繼資料*. 您可以在Adobe Dynamic Media Classic中使用中繼資料，以組織、搜尋、篩選和排序您的資產。

中繼資料會與Adobe Dynamic Media Classic產生的資訊一起顯示在「詳細資料檢視」中，例如檔案建立日期、發佈日期和關鍵字。 若要檢視中繼資料，請在「詳細資料檢視」中開啟資產，然後選取「中繼資料」面板。 您可以在「詳細資料檢視」中輸入及編輯中繼資料。

有些中繼資料會直接內嵌在檔案中。如果檔案包含此中繼資料，Adobe Dynamic Media Classic會自動將其與檔案一起上傳。 您可以將中繼資料內嵌至Adobe Photoshop、InDesign、Illustrator和其他應用程式的來源資產中；Adobe Dynamic Media Classic可辨識此中繼資料。 您也可以在「詳細資料檢視」的「中繼資料」面板中，將中繼資料新增至個別檔案。 為了確保資產之間的一致性，公司管理員會建立中繼資料範本，以提供可填入的中繼資料欄位。

如需內嵌中繼資料的詳細資訊，請參閱 [可延伸的中繼資料平台](https://www.adobe.com/products/xmp.html).

## 檢視中繼資料 {#view-metadata}

若要檢視資產的中繼資料，請在「詳細資料檢視」中開啟資產，然後點選「中繼資料」面板。 若要選取一組中繼資料欄位，請選擇「中繼資料檢視」功能表上的選項。 Adobe Dynamic Media Classic提供下列中繼資料檢視：

* **精簡檢視**  — 基本值清單。

* **IPTC**  — 國際新聞通訊委員會定義的價值。

* **XMP**  — 可延伸中繼資料程式所定義的值。

管理員可以建立中繼資料檢視。這些檢視也會出現在中繼資料檢視功能表中。

另請參閱 [中繼資料檢視](application-setup.md#metadata_views) 以取得有關建立中繼資料檢視的資訊。

## 手動輸入資產的中繼資料 {#manually-enter-metadata-for-an-asset}

1. 在「詳細資料檢視」中開啟資產。
1. 開啟「中繼資料」面板，然後進行下列其中一項或兩項操作:

   * 選擇「中繼資料檢視」，即可決定面板要顯示那些中繼資料欄位。
   * 選擇預設值，然後選取 **[!UICONTROL 套用]** 以使用預設值填入中繼資料欄位。 公司管理員會建立這些預設值。

1. 在「中繼資料」面板中輸入值。

>[!NOTE]
>
>若要一次編輯多個資產的中繼資料，請選取資產並前往 **[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**. 您在「編輯資訊」視窗中對中繼資料所做的編輯會套用至您選取的所有資產。

## 增加或編輯關鍵字 {#add-or-edit-keywords}

除了中繼資料之外，您還可以使用關鍵字來協助搜尋和管理您的資產。

如果您在此工作階段期間將關鍵字新增至其他檔案，或者如果您已從清單中移除關鍵字，這些關鍵字會顯示在「關鍵字建議」表格中。

1. 在詳細檢視中開啟檔案。
1. 選取 **[!UICONTROL 關鍵字]**.
1. 若要增加關鍵字，請執行下列任一動作:

   * 在文字方塊中輸入關鍵字，然後選取 **[!UICONTROL 新增]**.
   * 選取中的關鍵字 **[!UICONTROL 關鍵字建議]** 表格。

1. 若要移除關鍵字，請選取該關鍵字並選取 **[!UICONTROL 移除]**. 此時關鍵字即會移至「關鍵字建議」表格。

>[!NOTE]
>
>您可以將關鍵字上傳至Adobe Dynamic Media Classic時新增至檔案。 在「上載工作選項」對話方塊中，選擇 **[!UICONTROL 更多中繼資料]** 並輸入關鍵字。
>參閱[上載選項](uploading-files.md#upload_options)。

## 匯入中繼資料 {#import-metadata}

您可以從 Tab 字元分隔檔案或 XML 檔案匯入多項不同資產的中繼資料，而不是逐一針對資產手動輸入中繼資料。比起在個別資產中輸入中繼資料，在 Tab 字元分隔或 XML 檔案中輸入中繼資料並匯入檔案會更加省時。在 Tab 字元分隔檔案的第一列，針對想要記錄中繼資料的欄位輸入 ID 和名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。若要從 XML 檔案匯入中繼資料，請確定符合 DTD。

>[!NOTE]
>
>您可以建立用於輸入中繼資料的範本，以便正確地將其匯入至Adobe Dynamic Media Classic。 建立範本後，您可以用它來輸入中繼資料。
>請參閱[建立範本以輸入要上載的中繼資料](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)。

如需標準化屬性的詳細資訊，請參閱 [Adobe XMP開發人員中心](https://www.adobe.com/devnet/xmp.html).

1. 在瀏覽面板中，從 Tab 字元分隔檔案或 XML 檔案選取要增加中繼資料的影像。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**.
1. 在 **[!UICONTROL 上傳中繼資料]** 對話方塊，選取 **[!UICONTROL 瀏覽]**.
1. 在「**[!UICONTROL 選取要上載的檔案]**」對話框中，選取包含中繼資料的 Tab 字元分隔檔案或 XML 檔案。
1. 輸入工作名稱。
1. 選取 **[!UICONTROL 上傳]**.

### 識別匯入中的不同中繼資料型別

識別要匯入的不同中繼資料類型時，請記住下列事項:

* 使用者定義的欄位是以在中建立的名稱來識別 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義的欄位]**. 使用 `Generate file` 功能以取得正確匯入格式之所有已定義UDF的清單。
* XMP 中繼資料屬性的 (property-) 名稱前必須有相關的 XMP 字首。字首和名稱會以冒號區隔。XMP首碼可在下列位置找到： **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料結構]** 編輯者。 您可以在相關的 XMP 資料結構文件中找到技術名稱。XMP屬性名稱未出現在 `Generate file` 功能。
* 中繼資料結構 屬性的 (property-) 名稱前必須有相關的字首。字首和名稱會以冒號區隔。字首和屬性名稱皆是在「中繼資料結構編輯器」中定義。中繼資料結構描述屬性名稱不會出現在 `Generate file` 功能。

例如：關鍵字的XMP屬性是首碼為XMP結構描述「Dublin Core」 `dc` 和 `subject` 是技術XMP名稱。 前置詞和技術XMP名稱會合併至 `dc:subject` 完整屬性名稱。 在XML中繼資料匯入格式中， `dc.subject` 必須為屬性名稱。 在以Tab字元分隔的匯入格式中，它必須是欄標題。

### 匯入關鍵字

關鍵字可以匯入為逗號分隔清單。 如果任何個別值中出現逗號，則必須使用反斜線(\)逸出逗號。 如果是常值反斜線，則使用一般的雙反斜線 (\\)。

例如，包含值的中繼資料匯入檔案 `Hello\, World!,back\\slash,foo` 的 `dc:subject` 在資產上設定三個XMP關鍵字： `Hello, World!,` `back\slash,` 和 `foo`.

### 匯入 XMP 和中繼資料結構中繼資料 XMP 檔案

XML 匯入只接受有效的 XML。匯入XMP或中繼資料結構欄位時，會新增名稱空間前置詞，其行為類似於XMP-namespace。 必須宣告此名稱空間。 例如，在頂層標籤中。

例如: 

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### 匯入XMP和中繼資料結構描述資料（以Tab分隔）檔案

必須將字首新增至匯入欄位相關的欄標題。

## 匯入中繼資料 (透過 FTP) {#import-metadata-via-ftp}

您可以在以Tab字元分隔的或XML檔案中輸入中繼資料，然後選取 **[!UICONTROL 處理中繼資料檔案]** 上傳工作選項（透過FTP標籤）頁面。

確定 Tab 字元分隔或 XML 檔案中的資料格式正確無誤。在第一列中輸入 ID 欄位，後面跟著要修改的中繼資料欄位名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。

在全域導覽列上，選取 **[!UICONTROL 上傳]**. 若要匯入中繼資料，請在「上傳」頁面上選取 **[!UICONTROL 透過FTP]** 索引標籤，然後選取 **[!UICONTROL 工作選項]**. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 工作]**，然後選取 **[!UICONTROL 處理中繼資料檔案]** 核取方塊。

## 使用中繼資料批次重新命名 ID {#batch-rename-ids-using-metadata}

您可以使用從定位字元分隔檔案或XML檔案匯入的中繼資料，重新命名Adobe Dynamic Media Classic ID。 匯入的中繼資料只會套用於中繼資料檔案本身所指定的影像， 無論是否在「瀏覽」面板上選取影像。

若要重新命名影像的Adobe Dynamic Media Classic ID，請新增標籤為的欄 *newipsid* 至定位字元分隔的檔案，或新增欄位 `new_vc_objectname` 到XML資料。

例如: 

| | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

中繼資料工作的工作記錄會顯示哪些ID已成功重新命名，哪些未重新命名。

## 建立範本以輸入要上載的中繼資料 {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic提供用來建立記錄中繼資料範本的命令。 使用範本可確保中繼資料以正確的格式輸入，以便正確地上傳至Adobe Dynamic Media Classic。 若要建立範本以用於記錄中繼資料並將其匯入至Adobe Dynamic Media Classic，請遵循下列步驟：

1. 選取包含您要用於範本的中繼資料欄位的影像資產。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**.
1. 對於 **[!UICONTROL 資產屬性型別]**，選取 **[!UICONTROL 影像]**.
1. 從 **[!UICONTROL `Generate File`]** 下拉式清單，選擇 **[!UICONTROL Tab字元分隔範本]**， **[!UICONTROL 資產的XML中繼資料]**，或 **[!UICONTROL XML DTD]**.
1. 選取 **[!UICONTROL 產生]**.
1. 在顯示的對話框中複製資料。使用此資料來建構範本。

## 處理中繼資料結構  {#working-with-metadata-schemas}

公司管理員可以檢視所有可用資料結構的清單。在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料結構]**.

最初，會隱藏XMP等全域標準結構描述的清單。 但可以使用清單底部的核取方塊加以顯示。

公司管理員可以建立自訂結構描述，或編輯現有的自訂結構描述。

您可以使用「中繼資料結構編輯器」執行下列動作:

| 動作 | 說明 |
| --- | --- |
| 新增 | 將屬性新增至結構描述。 強制回應對話方塊會收集資訊：ID、標籤、結構和資料型別。 |
| 新增選擇值 | 新增選擇至屬性，其結構為「開放選擇」或「限定選擇」。所有選擇值皆擁有相同的類型。選取屬性本身以啟用按鈕。 |
| 編輯 | 編輯屬性或選擇值的標籤。您只能更改標籤、ID，但類型資訊不可變。 |
| 上移/下移 | 資料結構中的順序會反映在 UI 中。若要變更順序，請選取屬性或選擇值，並以按鈕加以移動。目前不支援拖放。 |
| 刪除 | 從資料結構刪除屬性或選擇值。它不會刪除XMP區塊或資料庫中的值。 屬性不再適用於中繼資料檢視，且已從資產詳細資料檢視中移除。 如果屬性已發佈至中繼資料伺服器，請執行強制發佈，從公開的中繼資料伺服器移除資料。 |

系統會自動為具有前置詞的使用者定義欄位產生自訂結構 `s7udf`. 此結構描述由在設定區段中編輯的現有使用者定義欄位組成。

>[!NOTE]
>
>資料結構的變更絕不會變更資產中繼資料。不過，並非所有Adobe Dynamic Media Classic和中繼資料伺服器功能都能看見這些專案，且無法在變更後加以存取。 同樣地，如果資產的中繼資料存在，建立相符的結構描述會使中繼資料可用於Adobe Dynamic Media Classic和中繼資料伺服器。

中繼資料結構編輯器提供在Adobe Dynamic Media Classic中新增或編輯自訂公司結構的圖形方式。 資料結構是由一個字首、一個命名空間，以及一份屬性清單所定義。

* **[!UICONTROL 名稱]**  — 結構的UI-Name。 用來在「中繼資料檢視」和「進階搜尋」中識別屬性。類似於 XMP 區段，如「基本」、「IPTC」和「PDF」。

* **[!UICONTROL 前置詞]**  — 結構描述的技術唯一識別碼。 限定於字母a-z和A-Z。前置詞在Adobe Dynamic Media Classic UI中不可見，但用於資產的中繼資料儲存在XMP區塊和資料庫時。 前置詞用於唯一識別中繼資料伺服器或匯入之中繼資料搜尋查詢中的中繼資料欄位。

* **[!UICONTROL 名稱空間]**  — 結構描述的技術唯一識別碼，通常為表單中的URL `https://your.company.com/name/version/`. 如需範例，請參閱標準資料結構清單。名稱空間不會顯示在Adobe Dynamic Media Classic UI中，但會用來將中繼資料儲存在XMP區塊中。

* **[!UICONTROL 說明]**  — 結構的自由形式說明。

>[!NOTE]
>
>無法編輯字首和命名空間。若要變更這些屬性，您必須刪除並重新建立資料結構。

屬性描述了可以使用此資料結構儲存於 XMP 區塊的中繼資料。屬性的組成包含:

| 屬性 | 說明 |
| --- | --- |
| ID | 此屬性的技術識別名稱。ID不會顯示在Adobe Dynamic Media Classic UI中，但用於資產的中繼資料儲存在XMP區塊和資料庫時。 ID可用來在中繼資料伺服器上建立搜尋查詢。 ID有一些限制，例如： `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>ID一旦建立便無法變更。 |
| 標籤 | 此特性的 UI 名稱。 |
| 結構 | 決定特性類型和資料類型。結構可為下列項目:<ul><li>簡單類型: 單一資料類型值</li><li>順序: 相同資料類型值的清單</li><li>開放選擇: 從預先定義值清單選取項目，或輸入自由文字。資料類型僅可為「字串」或「整數」</li><li>限定選擇: 從預先定義值清單 (彈出式或組合式) 選取項目</li></ul> |
| 資料類型 | 從下列可用類型中選取: <ul><li>字串</li><li>整數</li><li>浮點</li><li>是/否 (布林)</li><li>日期</li></ul> |

特性結構為「開放選擇」或「限定選擇」時，您必須提供至少一個選擇值。開放選擇可以變更。限定選擇無法變更。所有選擇值都擁有該特性的資料類型。

| 屬性 | 說明 |
| --- | --- |
| ID | 此值的技術識別名稱。ID不會顯示在Adobe Dynamic Media Classic UI中，但用於資產的中繼資料儲存在XMP區塊和資料庫時。 ID 會用於中繼資料伺服器上的搜尋查詢。ID 不可包含任何空格。建立之後，便無法再變更 ID。 |
| 標籤 | 此值的 UI 名稱。 |

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)
