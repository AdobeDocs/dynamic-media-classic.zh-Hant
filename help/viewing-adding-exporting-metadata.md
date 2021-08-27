---
title: 檢視、增加和匯出中繼資料
description: 了解如何檢視、新增和匯出中繼資料。
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '2268'
ht-degree: 47%

---

# 檢視、增加和匯出中繼資料{#viewing-adding-and-exporting-metadata}

您可以在AdobeDynamic Media Classic中儲存您使用之檔案的特定資訊；此資訊稱為&#x200B;*metadata*。 您可以在AdobeDynamic Media Classic中使用中繼資料來組織、搜尋、篩選及排序資產。

中繼資料會連同AdobeDynamic Media Classic產生的資訊（例如檔案建立日期、發佈日期和關鍵字）一起顯示在「詳細資料檢視」中。 若要檢視中繼資料，請在「詳細資料檢視」中開啟資產，然後選取「中繼資料」面板。 您可以在詳細檢視中輸入和編輯 中繼資料。

有些中繼資料會直接內嵌在檔案中。如果檔案包含此中繼資料，AdobeDynamic Media Classic會自動連同檔案一起上傳。 您可以將中繼資料內嵌至Adobe Photoshop、InDesign、Illustrator和其他應用程式的來源資產中；AdobeDynamic Media Classic可辨識此中繼資料。 您也可以在「詳細資訊檢視」的「中繼資料」面板中，將中繼資料新增至個別檔案。 為了確保資產之間的一致性，公司管理員會建立中繼資料範本，以提供可填入的中繼資料欄位。

如需內嵌中繼資料的詳細資訊，請參閱[www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en)。

## 檢視中繼資料 {#view-metadata}

若要檢視資產的中繼資料，請在「詳細資料檢視」中開啟資產，然後點選「中繼資料」面板。 要選擇一組元資料欄位，請在「元資料視圖」菜單上選擇一個選項。 AdobeDynamic Media Classic提供下列中繼資料檢視：

* **緊密視圖**  — 基本值清單。

* **IPTC**  — 國際新聞電信理事會界定的價值。

* **XMP**  — 由可擴充中繼資料程式定義的值。

管理員可以建立中繼資料檢視。這些檢視也會顯示在「中繼資料檢視」選單上。

如需建立中繼資料檢視的相關資訊，請參閱[中繼資料檢視](application-setup.md#metadata_views) 。

## 手動輸入資產的中繼資料 {#manually-enter-metadata-for-an-asset}

1. 在「詳細資訊檢視」中開啟資產。
1. 開啟「中繼資料」面板，然後進行下列其中一項或兩項操作:

   * 選擇「中繼資料檢視」，即可決定面板要顯示那些中繼資料欄位。
   * 選擇預設值，然後按一下&#x200B;**[!UICONTROL Apply]**&#x200B;以用預設值填入元資料欄位。 公司管理員會建立這些預設值。

1. 在「中繼資料」面板中輸入值。

>[!NOTE]
>
>若要一次編輯多個資產的中繼資料，請選取資產並按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**」。 您在「編輯資訊」視窗針對中繼資料進行的編輯，會套用至您選取的所有資產。

## 增加或編輯關鍵字 {#add-or-edit-keywords}

除了中繼資料，您也可以使用關鍵字來協助搜尋及管理資產。

如果在此工作階段期間將關鍵字新增至其他檔案，或者您已從清單中移除關鍵字，關鍵字建議表格中就會顯示關鍵字。

1. 在詳細檢視中開啟檔案。
1. 按一下「**[!UICONTROL 關鍵字]**」。
1. 若要增加關鍵字，請執行下列任一動作:

   * 在文本框中鍵入關鍵字，然後按一下&#x200B;**[!UICONTROL Add]**。
   * 按一下&#x200B;**[!UICONTROL 關鍵字建議]**&#x200B;表格中的關鍵字。

1. 若要移除關鍵字，請選取該關鍵字，然後按一下「**[!UICONTROL 移除]**」。 此時關鍵字即會移至「關鍵字建議」表格。

>[!NOTE]
>
>您可以在將關鍵字上傳至Dynamic Media Classic時，將關鍵字新增至檔案。 在「上載作業選項」對話框中，選擇&#x200B;**[!UICONTROL 其他元資料]**並輸入關鍵字。
>參閱[上載選項](uploading-files.md#upload_options)。

## 匯入中繼資料 {#import-metadata}

您可以從 Tab 字元分隔檔案或 XML 檔案匯入多項不同資產的中繼資料，而不是逐一針對資產手動輸入中繼資料。比起在個別資產中輸入中繼資料，在 Tab 字元分隔或 XML 檔案中輸入中繼資料並匯入檔案會更加省時。在 Tab 字元分隔檔案的第一列，針對想要記錄中繼資料的欄位輸入 ID 和名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。若要從 XML 檔案匯入中繼資料，請確定符合 DTD。

>[!NOTE]
>
>您可以建立輸入中繼資料的範本，以便正確匯入至AdobeDynamic Media Classic。 建立範本後，您便可使用範本來輸入中繼資料。
>請參閱[建立範本以輸入要上載的中繼資料](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)。

您可以在[AdobeXMP開發人員中心](https://www.adobe.com/devnet/xmp.html)找到有關標準化屬性的詳細資訊。

1. 在瀏覽面板中，從 Tab 字元分隔檔案或 XML 檔案選取要增加中繼資料的影像。
1. 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**」。
1. 在「**[!UICONTROL 上載中繼資料]**」對話框中，按一下「**[!UICONTROL 瀏覽]**」。
1. 在「**[!UICONTROL 選取要上載的檔案]**」對話框中，選取包含中繼資料的 Tab 字元分隔檔案或 XML 檔案。
1. 輸入工作名稱。
1. 按一下&#x200B;**[!UICONTROL 上載]**。

### 識別匯入中不同的中繼資料類型

識別要匯入的不同中繼資料類型時，請記住下列事項:

* 用戶定義欄位由其名稱標識，如在&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined欄位]**&#x200B;中建立。 使用「產生」檔案功能，以正確的匯入格式取得所有已定義 UDF 的清單。
* XMP 中繼資料屬性的 (property-) 名稱前必須有相關的 XMP 字首。字首和名稱會以冒號區隔。XMP前置詞可在&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]**&#x200B;編輯器中找到。 您可以在相關的 XMP 資料結構文件中找到技術名稱。XMP屬性名稱不會出現在「產生檔案」功能中。
* 中繼資料結構 屬性的 (property-) 名稱前必須有相關的字首。字首和名稱會以冒號區隔。字首和屬性名稱皆是在「中繼資料結構編輯器」中定義。中繼資料結構屬性名稱不會顯示在產生檔案功能中。

例如：關鍵字的XMP屬性為XMP結構「Dublin Core」，其首碼為`dc`，而`subject`為技術XMP名稱。 前置詞和技術XMP名稱會結合到`dc:subject`完整屬性名稱中。 在XML元資料導入格式中，`dc.subject`必須是屬性名稱。 在以Tab分隔的匯入格式中，它必須是欄標題。

### 匯入關鍵字

關鍵字可匯入為逗號分隔清單。 如果逗號出現在任何個別值中，則必須以反斜線(\)來逸出。 如果是常值反斜線，則使用一般的雙反斜線 (\\)。

例如，`dc:subject`包含「Hello\, World!,back\\slash,foo」值的中繼資料匯入檔案會在資產上設定三個XMP關鍵字：「你好，世界！」、「反斜線」和「foo」。

### 匯入 XMP 和中繼資料結構中繼資料 XMP 檔案

XML 匯入只接受有效的 XML。匯入XMP或中繼資料結構欄位時，會新增命名空間首碼，其行為類似於XMP命名空間。 必須聲明此命名空間。 例如，在頂層標籤中。

例如：

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### 匯入XMP和中繼資料結構中繼資料Tab分隔檔案

必須將字首新增至匯入欄位相關的欄標題。

## 匯入中繼資料 (透過 FTP) {#import-metadata-via-ftp}

您可以在以制表符分隔或XML檔案中輸入中繼資料，並在「上傳工作選項」（透過FTP索引標籤）頁面上選取&#x200B;**[!UICONTROL 「處理中繼資料檔案」]**，以匯入多個檔案的中繼資料。

確定 Tab 字元分隔或 XML 檔案中的資料格式正確無誤。在第一列中輸入 ID 欄位，後面跟著要修改的中繼資料欄位名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。

在「全域導覽列」上，按一下「**[!UICONTROL 上載]**」。若要匯入中繼資料，請在「上傳」頁面上按一下「透過FTP ]**」標籤，然後按一下「**[!UICONTROL &#x200B;工作選項&#x200B;]**」。**[!UICONTROL &#x200B;在「上載作業選項」對話框中，按一下&#x200B;**[!UICONTROL 作業]**，然後選擇&#x200B;**[!UICONTROL 處理元資料檔案]**&#x200B;複選框。

## 使用中繼資料批次重新命名 ID {#batch-rename-ids-using-metadata}

使用從以定位點分隔的檔案或XML檔案匯入的中繼資料，您可以重新命名AdobeDynamic Media Classic ID。 匯入的中繼資料只會套用於中繼資料檔案本身所指定的影像， 是否在「瀏覽」面板上選取影像並不重要。

若要重新命名影像的AdobeDynamic Media Classic ID，請將標示為&#x200B;*newipsid*&#x200B;的欄新增至以Tab分隔的檔案，或將名為`new_vc_objectname`的欄位新增至XML資料。

例如：

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

中繼資料作業的作業記錄會顯示哪些ID已成功重新命名，哪些ID未重新命名。

## 建立範本以輸入要上載的中繼資料 {#create-a-template-for-entering-metadata-to-upload}

AdobeDynamic Media Classic提供建立範本以記錄中繼資料的命令。 使用範本可確保以正確的格式輸入中繼資料，以便能夠正確上傳至AdobeDynamic Media Classic。 若要建立範本以用於記錄和匯入中繼資料以AdobeDynamic Media Classic，請遵循下列步驟：

1. 選取具有範本所要用的中繼資料欄位的影像資產。
1. 按一下「**[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**」。
1. 對於&#x200B;**[!UICONTROL 資產屬性類型]**，選擇&#x200B;**[!UICONTROL 影像]**。
1. 從&#x200B;**[!UICONTROL 生成檔案]**&#x200B;下拉清單中，選擇&#x200B;**[!UICONTROL Tab分隔模板]**、**[!UICONTROL 資產的XML元資料]**&#x200B;或&#x200B;**[!UICONTROL XML DTD]**。
1. 按一下「**[!UICONTROL 產生]**」。
1. 在顯示的對話框中複製資料。使用此資料來建構範本。

## 處理中繼資料結構  {#working-with-metadata-schemas}

公司管理員可以檢視所有可用資料結構的清單。在全局導航欄上，按一下「**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料架構]**」。

起初，會隱藏全域標準結構清單(例如XMP)。 但可以使用清單底部的核取方塊加以顯示。

公司管理員可以建立自訂架構，或編輯現有的自訂架構。

您可以使用「中繼資料結構編輯器」執行下列動作:

| 動作 | 說明 |
|--- |--- |
| 新增 | 將屬性新增至架構。 強制回應對話方塊會收集資訊：ID、標籤、結構和資料類型。 |
| 新增選擇值 | 新增選擇至屬性，其結構為「開放選擇」或「限定選擇」。所有選擇值皆擁有相同的類型。選取屬性本身以啟用按鈕。 |
| 編輯 | 編輯屬性或選擇值的標籤。您只能更改標籤、ID，但類型資訊不可變。 |
| 往上移/往下移 | 資料結構中的順序會反映在 UI 中。若要變更順序，請選取屬性或選擇值，並以按鈕加以移動。目前不支援拖放功能。 |
| 刪除 | 從資料結構刪除屬性或選擇值。它不會刪除XMP區塊或資料庫中的值。 中繼資料檢視不再提供該屬性，且該屬性已從資產詳細資料檢視中移除。 如果屬性已發佈到元資料伺服器，請執行強制發佈，從公開的中繼資料伺服器中移除資料。 |

系統會自動為首碼為`s7udf`的用戶定義欄位生成自定義架構。 這是現有的用戶定義欄位，它們在自己的「設定」部分中進行編輯。

>[!NOTE]
>
>資料結構的變更絕不會變更資產中繼資料。不過，這些變數不會顯示於所有AdobeDynamic Media Classic和中繼資料伺服器功能，且在變更後無法存取。 同樣地，如果資產的中繼資料存在，則建立相符的結構可讓中繼資料在Dynamic Media Classic和中繼資料伺服器中使用。

中繼資料結構編輯器提供圖形式方式，可在AdobeDynamic Media Classic中新增或編輯自訂公司結構。 資料結構是由一個字首、一個命名空間，以及一份屬性清單所定義。

* **名稱**  — 結構的UI — 名稱。用來在「中繼資料檢視」和「進階搜尋」中識別屬性。類似於 XMP 區段，如「基本」、「IPTC」和「PDF」。

* **前置詞**  — 結構的技術唯一識別碼。限於字母a-z和A-Z。前置詞不會顯示在AdobeDynamic Media Classic UI，但會在資產的中繼資料儲存在XMP區塊和資料庫時使用。 字首的用途為，在中繼資料伺服器上的中繼資料搜尋查詢中識別唯一的中繼資料欄位，或是進行匯入。

* **命名空間**  — 結構的技術唯一識別碼，通常為表單中的 `https://your.company.com/name/version/`URL。如需範例，請參閱標準資料結構清單。AdobeDynamic Media Classic UI中不會顯示命名空間，但用於將中繼資料儲存在XMP區塊中。

* **說明**  — 結構的自由格式說明。

>[!NOTE]
>
>無法編輯字首和命名空間。若要變更這些屬性，您必須刪除並重新建立資料結構。

屬性描述了可以使用此資料結構儲存於 XMP 區塊的中繼資料。屬性的組成包含:

| 屬性 | 說明 |
|--- |--- |
| ID | 此屬性的技術識別名稱。ID不會顯示在AdobeDynamic Media Classic UI，但會在資產的中繼資料儲存在XMP區塊和資料庫時使用。 ID 會用來在中繼資料伺服器上建立搜尋查詢。ID 有下列限制: <ul><li>不可包含空格</li><li>不可包含「.」、「:」、「$」</li><li>第一個字元不可為數字</li><li>最佳實務為使用 a-z 或 A-Z 作為第一個字元</li></ul> <br>建立之後，便無法再變更 ID。 |
| 標籤 | 此特性的 UI 名稱。 |
| 結構 | 決定特性類型和資料類型。結構可為下列項目:<ul><li>簡單類型: 單一資料類型值</li><li>順序: 相同資料類型值的清單</li><li>開放選擇: 從預先定義值清單選取項目，或輸入自由文字。資料類型僅可為「字串」或「整數」</li><li>限定選擇: 從預先定義值清單 (彈出式或組合式) 選取項目</li></ul> |
| 資料類型 | 從下列可用類型中選取: <ul><li>字串</li><li>整數</li><li>浮點</li><li>是/否 (布林)</li><li>日期</li></ul> |

特性結構為「開放選擇」或「限定選擇」時，您必須提供至少一個選擇值。開放選擇可以變更。限定選擇無法變更。所有選擇值都擁有該特性的資料類型。

| 屬性 | 說明 |
|--- |--- |
| ID | 此值的技術識別名稱。ID不會顯示在AdobeDynamic Media Classic UI，但當資產的中繼資料儲存在XMP區塊和資料庫時，就會使用。 ID 會用於中繼資料伺服器上的搜尋查詢。ID 不可包含任何空格。建立之後，便無法再變更 ID。 |
| 標籤 | 此值的 UI 名稱。 |

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)

