---
title: 發佈設定
description: 發佈設定可讓您決定預設如何從Adobe Dynamic Media Classic伺服器將資產傳送到網站或應用程式。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T20:08:29.260Z'
TQID: 'https://experienceleague.adobe.com/-fupHROLSD2veWgnchj2uhPQCKhLqtMasdqOVUNri6g'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 202f477d78272c66d0ac490e3a5041839b3e4f4d
workflow-type: tm+mt
source-wordcount: 2368
ht-degree: 23%

---

# 發佈設定 {#publish-setup}

Adobe Dynamic Media Classic伺服器預設會將資產傳送至網站或應用程式，具體取決於發佈設定頁面設定。 如果未指定設定，Adobe Dynamic Media Classic伺服器會根據發佈設定頁面上的預設設定傳送資產。 例如，傳送不包含解析度屬性的影像的要求會以「影像伺服器」頁面上的「預設物件解析度」設定產生影像。

管理員可以在「影像伺服器」、「影像轉譯器」和「暈映」頁面上變更預設設定，以建立從伺服器傳送資產的預設設定。

若要開啟發佈設定的頁面，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]**。

>[!NOTE]
>
>「發佈設定」頁面可供有經驗的網站開發人員和程式設計專業人士使用。 Adobe Dynamic Media Classic假設在這些頁面上變更設定的使用者熟悉Adobe Dynamic Media Classic、HTTP通訊協定標準和慣例，以及基本影像處理技術。

## 影像伺服器 {#image-server}

「影像伺服器」頁面會建立從「影像伺服器」傳送影像的預設設定。 設定值可用於這五個類別（請參閱「影像伺服器」頁面本身，以取得設定的詳細說明）。

請僅在Adobe Dynamic Media Classic支援團隊成員的協助下變更這些設定。

* **[!UICONTROL 目錄管理]**：這些設定會決定Adobe Dynamic Media Classic和目錄互動的方式。 與大部分的Web伺服器不同，Dynamic Media影像伺服器URL呼叫會導向到資訊清單或目錄檔案，而不是實際的影像檔案。 目錄檔案（不要與eCatalog混淆）包含發佈至影像伺服器的所有內容清單。 它也會包含每個影像的路徑。 如果您有 Digimarc ID，請在「Digimarc 使用者資訊」區段輸入您的使用者資訊。

* **[!UICONTROL 要求屬性]**：這些設定對可從伺服器傳送的影像施加限制。 例如，*最大值* **[!UICONTROL 回覆影像大小限制]**&#x200B;為&#x200B;**[!UICONTROL 寬度]** 5000和&#x200B;**[!UICONTROL 高度]** 5000。

* **[!UICONTROL 預設要求屬性]**：這些設定與影像的預設外觀有關。

* **[!UICONTROL 一般縮圖屬性]**：這些設定與縮圖影像的預設外觀和對齊方式有關。

* **[!UICONTROL 目錄欄位的預設值]**：這些設定與影像的解析度和預設縮圖型別有關。

* **[!UICONTROL 色彩管理屬性]**：這些設定會決定要使用哪些ICC色彩設定檔。

* **[!UICONTROL 相容性屬性]**：此設定可讓文字圖層中的前導段落和尾隨段落在3.6版中被視為回溯相容性。

* **[!UICONTROL 本地化支援]**：這些設定可讓您管理多個地區設定屬性。 它們也可讓您指定地區設定對應字串。 這可讓您定義要支援的語言。 註解可套用至檢視器中的各種工具提示。

  例如，如果您是在不同國家/地區銷售的跨國品牌，則請確認每個國家/地區皆擁有自己的特定地區「檢視器」。 若要完成此功能設定，您須指定地區地圖字串。 然後，在檢視器的預設集中編輯工具提示文字。 只要為您想要的語言新增翻譯文字字串。

  >[!NOTE]
  > 若要設定本地化支援選項，[請使用Admin Console建立支援案例](https://helpx.adobe.com/business/enterprise.html)。 在您的支援案例中，要求設定說明。

  如需關於設定「**[!UICONTROL 本地化支援]**」的詳細資訊，請參閱[進行資產本地化設定時的注意事項](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 進行資產本地化設定時的注意事項 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果您想在Adobe Dynamic Media Classic中設定本地化支援選項，例如「地區設定地圖」欄位，[請使用Admin Console建立支援案例](https://helpx.adobe.com/business/enterprise.html)。 在您的支援案例中，要求設定說明。

使用Adobe Dynamic Media Classic的常見方式是管理電子商務網站上的產品影像。 跨國企業面臨的挑戰是，相似產品的資產因地區而異。 通常差異在於媒體的某些元件。 複製每個國家/地區的所有資產並覆寫差異來管理這些差異是一項複雜的任務，並且與單一主要資產原則不一致。 資產的差異可能包括國別、不同音軌的影片，以及產品使用的電源線細微但重要的差異。 Adobe Dynamic Media Classic使用基本搜尋機制。 您可以定義影像伺服器尋找的資產尾碼順序，從所需的地區設定開始。

#### 資產本地化方式

IS (影像伺服) 請求的地區可透過下列 IS/IR (影像演算) 命令來識別:

`locale=`

這個命令接受不區分大小寫的區域設定ID (locId)字串。 地區設定識別碼通常是2-6個字元的字串，由字母和&quot;`_`&quot;組成。

IS支援任意可列印的ASCII字串。 `locale=`命令會全域套用至整個請求，包括巢狀請求、範本和圖層。 不支援每個要求使用多個語言環境，例如每個圖層使用不同的語言環境。 但要允許在內嵌的請求中進行明確覆寫，這倒是可行。

如果未指定`locale=`，則會將`attribute::DefaultLocale`傳遞至翻譯引擎。 有限的輸入驗證已套用至`locale=`值。 允許空的`locale=`值。 因為`locale=`具有全域範圍，所以主目錄會為整個要求提供`attribute::DefaultLocale`。

使用`locale=`和`attribute::DefaultLocale`的某些優點包括：

* 共用多個地區的內容。
* 使用通用 ID 存取地區特定內容。
* 在命名慣例與地區特定內容的管理上更具彈性，例如地區字首與字尾的比較，或是個別目錄中的地區特定內容。
* 支援地區設定特定版本的存取。
* 彙總物件（例如「影像集」）有時可以包含對可能地區設定特定內容的一般參照。
* 支援所有需要本地化的目錄管理內容，包括影像、集合、暈映、素材和組態。
* 將 IPS 資料庫與 IS 資訊清單機制的變更降至最低。
* 實作RFC IS-63時，新增對靜態內容（例如視訊和外觀）的支援。
* 預設地區是可設定的。

#### 應用程式案例

| 應用程式 | 案例 |
| --- | --- |
| 檢視器本地化 | 實作靜態內容目錄後，本地化完全以locale=引數控制，附加至向IS提出的所有要求。 設定記錄、外觀、啟動畫面等項目可能會有地區特定變體。 IS 會提供正確的內容，檢視器無須知道哪些內容已本地化以及內容的 ID。 |
| 影像和視訊 | 跨國公司常會混用通用內容與地區特定內容。 在此機制下，對影像或視訊的參考會是通用的，而 IS 會在有可用的地區特定內容時加以提供。 |
| 影像集和媒體集 | 有些地區設定的整個影像集可能不同，例如當eCatalog不同時，由檢視器處理從一般到地區設定特定影像集的轉譯。 更常見的情況是，一般集中的個別ID可以參照本地化的內容。 例如，除控制面板的像片外，裝置的大部分像片在所有語言中都可能相同。 IS會自動翻譯ID，因此不需要產生地區設定特有的影像集。 |

#### 實施資產本地化

Adobe Dynamic Media Classic和「影像伺服」擁有可本地化影像和靜態內容的介面。

若未本地化，影像伺服器的 URL 將看起來如下:

`https://server/is/image/company/image`

透過本地化，影像伺服器URL會將`locale=`引數新增至路徑，如下所示：

`https://server/is/image/company/image?locale=de_DE`

影像伺服器收到http呼叫時，會透過&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]** > **[!UICONTROL 本地化支援]**&#x200B;群組中的`localeMap`欄位來剖析`locale=`引數。

「地區地圖」欄位會包含以管線符號 (|) 分隔的項目清單。

每個項目都包含一份以逗號分隔的值清單。 第一個值是透過`locale=`引數傳遞的搜尋值。 其餘的值是字尾/取代值，之後會嘗試這些值，直到其中一個值產生現有影像為止。

應套用字尾值還是取代值，取決於「**[!UICONTROL 設定]**」>「**[!UICONTROL 應用程式設定]**」>「**[!UICONTROL 發佈設定]**」>「**[!UICONTROL 影像伺服器]**」>「**[!UICONTROL 本地化支援]**」群組中的「全域地區」設定。

>[!NOTE]
>
>全域地區設定只有在您透過API設定，而不是在Adobe Dynamic Media Classic介面中設定時才可行。

**尾碼範例：**

| URL | localeMap ID | 結果 | 附註 |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | 請注意，其中並未定義 GlobalLocale。 地區設定引數de_DE與`localeMap`中的第一個專案相符。 第一個對應值_DE會新增為資產image_DE的尾碼，並嘗試在影像伺服器上尋找該資產。 若在伺服器上找到，則會傳回。 否則，第二個值「」會作為尾碼，導致影像本身傳回。 |

**取代範例：**

| URL | `GlobalLocale`與`localeMap` ID | 結果 | 附註 |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | 在上述取代範例中，GlobalLocale設定為main。 地區設定引數de_DE與`localeMap`中的第一個專案相符。 找到GlobalLocale子字串，並以`localeMap`中的第一個對應值`de`取代： `image-de-01`。 若在影像伺服器上找到，則會傳回。 如果沒有，則會取代第二個值，產生`image-main-01`。 |

如果 URL 中未定義地區，影像伺服器會使用 DefaultLocale，如果已定義，則會將該地區套用至 URL。

如果`locale=`提供了未知或空白的地區設定引數，則會掃描`localeMap`以找出空白值「開頭為」。 為未知地區設定套用預設地區設定是很重要的事。

#### 關於defaultImage

影像伺服器會針對所請求的地區逐一嘗試各個選項。 若找不到相符專案，區域設定選項會套用至defaultImage，並傳回相符版本。 因此，每個地區設定都必須包含影像的選項，但不進行本地化，或是在Adobe Dynamic Media Classic中提供本地化的defaultImage版本。

#### 尋找localeMap的案例

假設您要支援下列地區:

`en, en_us, en_uk, de, de_at, de_de, fr`

您將這些地區設定對應到字尾`_E` （英文）、`_G` （德文）和`_F` （法文）。 在所有範例中，一般輸入影像識別碼為`myImg`。

##### 尋找localeMap的標準行為

地區 ID 會對應至其對應的字尾。 如果在目錄中找不到地區特定 ID，則會以通用 ID 嘗試。 請注意對應至通用ID的空白locSuffix值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| en， en_us， en_uk | 我的影像(_E)，我的影像 |
| de， de_de， de_at | myImg_D， myImg |
| fr | myImg_F， myImg |
| 所有其他 | : |

##### 地區設定不明時尋找localeMap

您可以將不明的地區對應至特定 ID 或通用 ID。 例如，您可以將未知的地區設定對應至英文ID，如果沒有的話，則對應至一般ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| de， de_de， de_at | myImg_D， myImg |
| fr | myImg_F， myImg |
| 所有其他 | 我的影像(_E)，我的影像 |

對未知的地區設定使用專用的locSuffix，並在沒有`_U`時強制預設影像，如以下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，您可以直接對應至通用 ID，如下所示:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### 使用多階層查詢來尋找localeMap

群組地區設定，以符合地區標準，例如皮膚暴露。 您可以使用多階層查閱來執行此操作。

例如，假設您想支援西方和中東使用的收藏集。 這兩個集合都以通用影像集合為基礎，增加或修改了一些影像。 然後針對特定地區設定進一步調整這兩個集合。 例如，`m1, m2`代表兩個中東變體，`w1, w2`和`w3`代表三個西方地區設定，除了影像共用給`w1`和`w3`以外。 不明地區只會對應至通用集合，且無權存取地區特定影像。 地圖如下：

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| w1， w3 | 我的影像 — W、我的影像 |
| w2 | myImg-W2、myImg-W、myImg |
| m1 | myImg-M1、myImg-M、myImg |
| m2 | myImg-M2、myImg-M、myImg |
| 所有其他 | mylmg |

##### 透過搜尋特定ID來尋找localeMap

有些影像命名慣例不支援一般影像ID。 請求中的通用 ID 必須對應至目錄中的特定 ID。 但在某些情況下，確切的特定ID會不明。

以第一個範例為基礎，所有語言的影像都有尾碼`_1`、`_2`或`_3`。 法國地區設定的特定影像尾碼為`_22`或`_23`。 而德文地區設定的特定影像尾碼為`_470`或`_480`。

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de， de_at， de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他 | myImg_1, myImg_2, myImg_3 |

##### 實作本地化支援時的重要考量

* 本地化限用於以 ID 為基礎的資產呼叫，而無法用於以路徑為基礎的資產呼叫。 因此，使用地區設定呼叫視訊時，必須呼叫這些視訊作為公司/資產ID，而且沒有視訊的完整路徑。 您無法將`RTMP`與本地化搭配使用，因為此方法僅適用於以路徑為基礎的視訊呼叫。
* 當localeMap作用中時，無法使用包含單一視訊的混合媒體集；否則，呼叫該集內容會失敗。 若要解決此問題，您可以將單一視訊新增至最適化視訊集。 接著，將最適化視訊集增加至混合媒體集。
* 有些請求並不會本地化，例如最適化視訊集之內容的請求。 因此，如果您打算將自我調整視訊集與本地化搭配使用，請將自我調整視訊集放置在混合媒體集中。 然後，使用`locale=`引數將集合呼叫為混合媒體檢視器。

## 影像演算 {#image-renderer}

「影像轉譯器」頁面會建立從影像轉譯伺服器傳送影像集的預設設定。 設定值可用於這五個類別（請參閱「影像伺服器」頁面本身，以取得設定的詳細說明）：

* **[!UICONTROL 目錄管理]**：這些設定決定Adobe Dynamic Media Classic和目錄檔案互動的方式。 Adobe Dynamic Media Classic轉譯器伺服器URL會呼叫目錄，然後目錄會從伺服器傳送影像。 請僅在Adobe Dynamic Media Classic支援團隊成員的協助下變更這些設定。

* **[!UICONTROL 工作階段屬性]**：這些設定會建立錯誤引數、相對影像URL的URL，以及是否允許物件重疊。

* **[!UICONTROL 預設材質屬性]**：這些設定可建立影像的預設解析度和銳利化設定。

* **[!UICONTROL 回應影像屬性]**：這些設定與影像的預設外觀有關。

* **[!UICONTROL 色彩管理屬性]**：這些設定與影像的預設色彩設定有關。

## 暈映 {#vignette}

「暈映」頁面提供建立暈映預設外觀的設定值（請參閱頁面本身以取得選項的詳細說明）。
