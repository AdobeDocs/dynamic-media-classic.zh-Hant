---
title: 查看、添加和導出元資料
description: 瞭解如何在Adobe Dynamic Media Classic查看、添加和導出元資料。
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 45%

---

# 查看、添加和導出元資料{#viewing-adding-and-exporting-metadata}

您可以儲存與您在Adobe Dynamic Media Classic使用的檔案相關的特定資訊；此資訊稱為 *元資料*。 您可以在Adobe Dynamic Media Classic使用元資料來組織、搜索、篩選和排序資產。

元資料隨Adobe Dynamic Media Classic生成的資訊（如檔案建立日期、發佈日期和關鍵字）一起顯示在「詳細資訊視圖」中。 要查看元資料，請在詳細資訊視圖中開啟資產，然後選擇元資料面板。 您可以在詳細檢視中輸入和編輯 中繼資料。

有些中繼資料會直接內嵌在檔案中。如果檔案包含此元資料，Adobe Dynamic Media Classic會自動將其與檔案一起上載。 您可以將元資料嵌入到Adobe Photoshop、InDesign、Illustrator和其他應用程式的源資產中；Adobe Dynamic Media Classic能識別這個元資料。 您還可以在「詳細資訊視圖」的「元資料」面板中將元資料添加到單個檔案。 為了確保資產之間的一致性，公司管理員會建立中繼資料範本，以提供可填入的中繼資料欄位。

有關嵌入式元資料的詳細資訊，請參見 [可擴展元資料平台](https://www.adobe.com/products/xmp.html)。

## 檢視中繼資料 {#view-metadata}

要查看資產的元資料，請在詳細資訊視圖中開啟資產，然後點擊元資料面板。 要選擇一組元資料欄位，請在「元資料視圖」菜單上選擇一個選項。 Adobe Dynamic Media Classic提供以下元資料視圖：

* **壓縮視圖**  — 基本值清單。

* **IPTC**  — 國際新聞電信理事會所界定的價值。

* **XMP**  — 可擴展元資料程式定義的值。

管理員可以建立中繼資料檢視。這些檢視也會顯示在「中繼資料檢視」選單上。

請參閱 [元資料視圖](application-setup.md#metadata_views) 的子菜單。

## 手動輸入資產的中繼資料 {#manually-enter-metadata-for-an-asset}

1. 在「詳細資訊視圖」中開啟資產。
1. 開啟「中繼資料」面板，然後進行下列其中一項或兩項操作:

   * 選擇「中繼資料檢視」，即可決定面板要顯示那些中繼資料欄位。
   * 選擇預設值，然後選擇 **[!UICONTROL 應用]** 用預設值填充元資料欄位。 公司管理員會建立這些預設值。

1. 在「中繼資料」面板中輸入值。

>[!NOTE]
>
>要同時編輯多個資產的元資料，請選擇這些資產並轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**。 您在「編輯資訊」視窗針對中繼資料進行的編輯，會套用至您選取的所有資產。

## 增加或編輯關鍵字 {#add-or-edit-keywords}

除了元資料外，還可以使用關鍵字幫助搜索和管理資產。

如果在此會話期間已將關鍵字添加到其他檔案，或者已從清單中刪除了關鍵字，則這些關鍵字將顯示在「關鍵字建議」表中。

1. 在詳細檢視中開啟檔案。
1. 選擇 **[!UICONTROL 關鍵字]**。
1. 若要增加關鍵字，請執行下列任一動作:

   * 在文本框中鍵入關鍵字並選擇 **[!UICONTROL 添加]**。
   * 在 **[!UICONTROL 關鍵字建議]** 的子菜單。

1. 要刪除關鍵字，請選擇該關鍵字並選擇 **[!UICONTROL 刪除]**。 此時關鍵字即會移至「關鍵字建議」表格。

>[!NOTE]
>
>在將關鍵字上載到Adobe Dynamic Media Classic時，可以將關鍵字添加到檔案。 在「上載作業選項」對話框中，選擇 **[!UICONTROL 其他元資料]** 並輸入關鍵字。
>參閱[上載選項](uploading-files.md#upload_options)。

## 匯入中繼資料 {#import-metadata}

您可以從 Tab 字元分隔檔案或 XML 檔案匯入多項不同資產的中繼資料，而不是逐一針對資產手動輸入中繼資料。比起在個別資產中輸入中繼資料，在 Tab 字元分隔或 XML 檔案中輸入中繼資料並匯入檔案會更加省時。在 Tab 字元分隔檔案的第一列，針對想要記錄中繼資料的欄位輸入 ID 和名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。若要從 XML 檔案匯入中繼資料，請確定符合 DTD。

>[!NOTE]
>
>您可以建立用於輸入元資料的模板，以便可以將其正確導入Adobe Dynamic Media Classic。 建立範本後，您便可使用範本來輸入中繼資料。
>請參閱[建立範本以輸入要上載的中繼資料](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)。

您可以在以下位置查找有關標準化屬性的詳細資訊： [Adobe開XMP發中心](https://www.adobe.com/devnet/xmp.html)。

1. 在瀏覽面板中，從 Tab 字元分隔檔案或 XML 檔案選取要增加中繼資料的影像。
1. 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 導入元資料]**。
1. 在 **[!UICONTROL 上載元資料]** 對話框，選擇 **[!UICONTROL 瀏覽]**。
1. 在「**[!UICONTROL 選取要上載的檔案]**」對話框中，選取包含中繼資料的 Tab 字元分隔檔案或 XML 檔案。
1. 輸入工作名稱。
1. 選擇 **[!UICONTROL 上載]**。

### 在導入中標識不同的元資料類型

識別要匯入的不同中繼資料類型時，請記住下列事項:

* 用戶定義欄位由在中建立的名稱標識 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 用戶定義的欄位]**。 使用「產生」檔案功能，以正確的匯入格式取得所有已定義 UDF 的清單。
* XMP 中繼資料屬性的 (property-) 名稱前必須有相關的 XMP 字首。字首和名稱會以冒號區隔。可XMP以在 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料架構]** 編輯器。 您可以在相關的 XMP 資料結構文件中找到技術名稱。屬性XMP名稱不出現在「生成檔案」功能中。
* 中繼資料結構 屬性的 (property-) 名稱前必須有相關的字首。字首和名稱會以冒號區隔。字首和屬性名稱皆是在「中繼資料結構編輯器」中定義。元資料架構屬性名稱不會顯示在生成檔案功能中。

例如：關XMP鍵字的屬XMP性是帶前置詞的架構&quot;Dublin Core&quot; `dc` 和 `subject` 是技術名XMP稱。 前置詞和技XMP術名稱組合到 `dc:subject` 完全屬性名。 以XML元資料導入格式， `dc.subject` 必須是屬性名。 在制表符分隔的導入格式中，它必須是列標題。

### 匯入關鍵字

關鍵字可以作為逗號分隔的清單導入。 如果逗號出現在任何單個值中，則必須用反斜槓(\)轉義它。 如果是常值反斜線，則使用一般的雙反斜線 (\\)。

例如，包含該值的元資料導入檔案 `Hello\, World!,back\\slash,foo` 為 `dc:subject` 設定三XMP個關鍵字： `Hello, World!,` `back\slash,` 和 `foo`。

### 匯入 XMP 和中繼資料結構中繼資料 XMP 檔案

XML 匯入只接受有效的 XML。導入或元XMP資料架構欄位時，將添加命名空間前置詞，並在此處的行為與命名空XMP間類似。 必須聲明此命名空間。 例如，在頂級標籤中。

例如: 

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### 導入XMP和元資料架構元資料制表符分隔的檔案

必須將字首新增至匯入欄位相關的欄標題。

## 匯入中繼資料 (透過 FTP) {#import-metadata-via-ftp}

通過在制表符分隔或XML檔案中輸入元資料並選擇 **[!UICONTROL 處理元資料檔案]** 上載作業選項（通過FTP頁籤）頁。

確定 Tab 字元分隔或 XML 檔案中的資料格式正確無誤。在第一列中輸入 ID 欄位，後面跟著要修改的中繼資料欄位名稱。在每個後續的列中，輸入隨後附有中繼資料值的資產 ID 名稱。系統不會修改 Tab 字元分隔或 XML 檔案中未包含的欄位。

在全局導航欄上，選擇 **[!UICONTROL 上載]**。 要導入元資料，請在「上載」頁上，選擇 **[!UICONTROL 通過FTP]** ，然後選擇 **[!UICONTROL 作業選項]**。 在「上載作業選項」對話框中，選擇 **[!UICONTROL 作業]**，然後選擇 **[!UICONTROL 處理元資料檔案]** 的子菜單。

## 使用中繼資料批次重新命名 ID {#batch-rename-ids-using-metadata}

使用從制表符分隔的檔案或XML檔案導入的元資料，可以更名Adobe Dynamic Media ClassicID。 匯入的中繼資料只會套用於中繼資料檔案本身所指定的影像， 在「瀏覽面板」上是否選擇影像並不重要。

要更名影像的Adobe Dynamic Media ClassicID，請添加一列 *內維希德* 添加到制表符分隔的檔案，或添加名為 `new_vc_objectname` 到XML資料。

例如: 

|  | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

元資料作業的作業日誌顯示哪些ID已成功更名，哪些ID未成功更名。

## 建立範本以輸入要上載的中繼資料 {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic提供了建立用於記錄元資料的模板的命令。 使用模板可確保以正確的格式輸入元資料，以便能夠將其正確上載到Adobe Dynamic Media Classic。 要建立用於記錄和將元資料導入Adobe Dynamic Media Classic的模板，請執行以下步驟：

1. 為模板選擇包含您想要的元資料欄位的影像資產。
1. 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 導入元資料]**。
1. 對於 **[!UICONTROL 資產屬性類型]**&#x200B;選中 **[!UICONTROL 影像]**。
1. 從 **[!UICONTROL 生成檔案]** 下拉清單，選擇 **[!UICONTROL 制表符分隔的模板]**。 **[!UICONTROL 資產的XML元資料]**&#x200B;或 **[!UICONTROL XML DTD]**。
1. 選擇 **[!UICONTROL 生成]**。
1. 在顯示的對話框中複製資料。使用此資料來建構範本。

## 處理中繼資料結構  {#working-with-metadata-schemas}

公司管理員可以檢視所有可用資料結構的清單。在全局導航欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 元資料]** > **[!UICONTROL 元資料架構]**。

最初，全局標準架構（如）的清單XMP將隱藏。 但可以使用清單底部的核取方塊加以顯示。

公司管理員可以建立自定義架構或編輯現有的自定義架構。

您可以使用「中繼資料結構編輯器」執行下列動作:

| 動作 | 說明 |
| --- | --- |
| 新增 | 將屬性添加到架構。 模式對話框將收集以下資訊：ID、標籤、結構和資料類型。 |
| 新增選擇值 | 新增選擇至屬性，其結構為「開放選擇」或「限定選擇」。所有選擇值皆擁有相同的類型。選擇屬性本身以啟用按鈕。 |
| 編輯 | 編輯屬性或選擇值的標籤。您只能更改標籤、ID，但類型資訊不可變。 |
| 往上移/往下移 | 資料結構中的順序會反映在 UI 中。若要變更順序，請選取屬性或選擇值，並以按鈕加以移動。當前不支援拖放。 |
| 刪除 | 從資料結構刪除屬性或選擇值。它不會從塊或數XMP據庫中刪除值。 該屬性不再可用於元資料視圖，並將從資產詳細資訊視圖中刪除。 如果屬性已發佈到元資料伺服器，請執行強制發佈以從面向公共的元資料伺服器中刪除資料。 |

系統自動為帶有前置詞的用戶定義欄位生成自定義模式 `s7udf`。 它是現有的用戶定義欄位，它們在自己的「設定」部分中編輯。

>[!NOTE]
>
>資料結構的變更絕不會變更資產中繼資料。但是，它們對於所有Adobe Dynamic Media Classic和元資料伺服器功能都不可見，更改後無法訪問。 同樣，如果資產的元資料存在，則建立匹配模式可使元資料在Adobe Dynamic Media Classic和元資料伺服器中可用。

元資料架構編輯器提供了在Adobe Dynamic Media Classic內添加或編輯自定義公司架構的圖形方式。 資料結構是由一個字首、一個命名空間，以及一份屬性清單所定義。

* **[!UICONTROL 名稱]**  — 架構的UI — 名稱。 用來在「中繼資料檢視」和「進階搜尋」中識別屬性。類似於 XMP 區段，如「基本」、「IPTC」和「PDF」。

* **[!UICONTROL 前置詞]**  — 架構的技術唯一標識符。 僅限於字母a-z和A-Z。前置詞在Adobe Dynamic Media ClassicUI中不可見，但在塊和資料庫中儲存資產的元資料時XMP使用該前置詞。 字首的用途為，在中繼資料伺服器上的中繼資料搜尋查詢中識別唯一的中繼資料欄位，或是進行匯入。

* **[!UICONTROL 命名空間]**  — 架構的技術唯一標識符，通常為表單中的URL `https://your.company.com/name/version/`。 如需範例，請參閱標準資料結構清單。命名空間在Adobe Dynamic Media ClassicUI中不可見，但用於在塊中儲存元XMP資料。

* **[!UICONTROL 說明]**  — 架構的自由格式說明。

>[!NOTE]
>
>無法編輯字首和命名空間。若要變更這些屬性，您必須刪除並重新建立資料結構。

屬性描述了可以使用此資料結構儲存於 XMP 區塊的中繼資料。屬性的組成包含:

| 屬性 | 說明 |
| --- | --- |
| ID | 此屬性的技術識別名稱。該ID在Adobe Dynamic Media ClassicUI中不可見，但在塊和資料庫中儲存資產的元資料時XMP使用它。 ID 會用來在中繼資料伺服器上建立搜尋查詢。ID 有下列限制: <ul><li>不可包含空格</li><li>不可包含「.」、「:」、「$」</li><li>第一個字元不可為數字</li><li>最佳實務為使用 a-z 或 A-Z 作為第一個字元</li></ul> <br>建立之後，便無法再變更 ID。 |
| 標籤 | 此特性的 UI 名稱。 |
| 結構 | 決定特性類型和資料類型。結構可為下列項目:<ul><li>簡單類型: 單一資料類型值</li><li>順序: 相同資料類型值的清單</li><li>開放選擇: 從預先定義值清單選取項目，或輸入自由文字。資料類型僅可為「字串」或「整數」</li><li>限定選擇: 從預先定義值清單 (彈出式或組合式) 選取項目</li></ul> |
| 資料類型 | 從下列可用類型中選取: <ul><li>字串</li><li>整數</li><li>浮點</li><li>是/否 (布林)</li><li>日期</li></ul> |

特性結構為「開放選擇」或「限定選擇」時，您必須提供至少一個選擇值。開放選擇可以變更。限定選擇無法變更。所有選擇值都擁有該特性的資料類型。

| 屬性 | 說明 |
| --- | --- |
| ID | 此值的技術識別名稱。該ID在Adobe Dynamic Media ClassicUI中不可見，但在塊和資料庫中儲存資產的元資料XMP時使用。 ID 會用於中繼資料伺服器上的搜尋查詢。ID 不可包含任何空格。建立之後，便無法再變更 ID。 |
| 標籤 | 此值的 UI 名稱。 |

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)

