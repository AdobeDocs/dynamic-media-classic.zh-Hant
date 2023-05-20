---
title: 發佈設定
description: 「發佈設定」設定允許您確定預設情況下如何將資產從Adobe Dynamic Media Classic伺服器傳送到網站或應用程式。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2405'
ht-degree: 42%

---

# 發佈設定 {#publish-setup}

「發佈設定」頁設定確定預設情況下如何將資產從Adobe Dynamic Media Classic伺服器傳送到網站或應用程式。 如果未指定任何設定，則Adobe Dynamic Media Classic伺服器會根據「發佈設定」(Publish Setup)頁面上的預設設定來傳遞資產。 例如，請求傳送不包含解析度屬性的影像會生成具有「影像伺服器」頁上「預設對象解析度」設定的影像。

管理員可以更改「映像伺服器」、「映像呈現器」和「視頻」頁上的預設設定，以建立從伺服器傳遞資產的預設設定。

要開啟「發佈設定」頁，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]**。

>[!NOTE]
>
>「發佈設定」頁面供經驗豐富的網站開發人員和程式設計師使用。 Adobe Dynamic Media Classic假定更改這些頁面設定的用戶熟悉Adobe Dynamic Media Classic、HTTP協定標準和慣例以及基本成像技術。

## 影像伺服器 {#image-server}

「映像伺服器」頁為從映像伺服器傳送映像建立預設設定。 這五個類別中提供了設定（有關設定的詳細說明，請參閱「映像伺服器」頁本身）。

只有在Adobe Dynamic Media Classic支援人員的協助下才更改這些設定。

* **[!UICONTROL 目錄管理]**  — 這些設定決定了Adobe Dynamic Media Classic與目錄的交互方式。 與大多數Web伺服器不同，Dynamic Media映像伺服器URL調用會轉到清單或目錄檔案，而不是映像檔案。 目錄檔案 (請勿與 eCatalog 混淆) 包含了所有發佈至影像伺服器的內容清單，以及各個影像的路徑。如果您有 Digimarc ID，請在「Digimarc 使用者資訊」區段輸入您的使用者資訊。

* **[!UICONTROL 請求屬性]**  — 這些設定對可以從伺服器傳送的映像施加限制。 例如， *最大* **[!UICONTROL 答復影像大小限制]** 是 **[!UICONTROL 寬度]** 5000和 **[!UICONTROL 高度]** 5000。

* **[!UICONTROL 預設請求屬性]**  — 這些設定與影像的預設外觀有關。

* **[!UICONTROL 常用縮略圖屬性]**  — 這些設定與縮略圖影像的預設外觀和對齊方式有關。

* **[!UICONTROL 目錄欄位的預設值]**  — 這些設定與影像的解析度和預設縮略圖類型有關。

* **[!UICONTROL 顏色管理屬性]**  — 這些設定確定使用的ICC顏色配置檔案。

* **[!UICONTROL 相容性屬性]**  — 此設定允許文本圖層中的前導段和尾隨段落按照3.6版中的段落進行處理，以實現向後相容性。

* **[!UICONTROL 本地化支援]*** — 這些設定允許您管理多個區域設定屬性。 也可以讓您指定地區地圖字串，以便您定義要在「檢視器」的各種工具提示中支援的語言。

   例如，如果您是在不同國家/地區銷售的跨國品牌，則請確認每個國家/地區皆擁有自己的特定地區「檢視器」。若要完成此功能設定，您須指定地區地圖字串。然後，通過為所需語言添加已翻譯的文本字串，在查看器的預設中編輯工具提示文本。

   >[!NOTE]
   > 要設定本地化支援選項， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，請求安裝幫助。

   如需關於設定「**[!UICONTROL 本地化支援]**」的詳細資訊，請參閱[進行資產本地化設定時的注意事項](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 進行資產本地化設定時的注意事項 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果要在Adobe Dynamic Media Classic設定本地化支援選項，如「區域設定映射」欄位， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，請求安裝幫助。

使用Adobe Dynamic Media Classic的一種常見方法是管理電子商務網站上的產品影像。 國際企業常面臨類似產品的資產在不同國家間有外觀差異的問題。通常，這些差異只適用於整個介質的一小部分。 通過複製每個國家的所有資產並誇大差異來解決這些差異是一項巨大的努力，與單一的主要資產比喻相矛盾。 資產的此類差異可能無所不在，從因不同國家而有不同配音的視訊，到產品所用電源線這種微小但重要的差異都包括在內。Adobe Dynamic Media Classic使用基本的查找機制。 您可以定義影像伺服器查閱資產字尾的順序，以從必要的地區開始。

#### 資產本地化的方式

IS (影像伺服) 請求的地區可透過下列 IS/IR (影像演算) 命令來識別:

`locale=`

此命令可接受不區分大小寫的地區 ID (locId) 字串。地區 ID 通常是 2 到 6 個由字母與“_”字元組成的字串。

IS支援可打印的任意ASCII字串。 的 `locale=` 命令具有全局範圍，這意味著它應用於整個請求，包括所有嵌套的IS和IR請求、引用的模板和影像層。 不支援一個請求有多個地區 (例如每個圖層各有不同的地區)。但要允許在內嵌的請求中進行明確覆寫，這倒是可行。

如果 `locale=` 未指定， `attribute::DefaultLocale` 被傳遞到翻譯引擎。 有限輸入驗證應用於 `locale=` 值。 空 `locale=` 允許使用值。 因為 `locale=` 有全球範圍， `attribute::DefaultLocale` 由整個請求的主目錄提供。

使用 `locale=` 和 `attribute::DefaultLocale` 包括：

* 共用多個地區的內容。
* 使用通用 ID 存取地區特定內容。
* 在命名慣例與地區特定內容的管理上更具彈性，例如地區字首與字尾的比較，或是個別目錄中的地區特定內容。
* 支援訪問特定於區域設定的版本。
* 聚合對象（如影像集）有時可能包含對可能特定於區域設定的內容的泛型引用。
* 支援由需要本地化的目錄管理的所有內容，包括影像、影像集、小圖、材料和查看器配置記錄。
* 將 IPS 資料庫與 IS 資訊清單機制的變更降至最低。
* 在實施RFC IS-63時，將添加對靜態內容（如視頻和外觀）的支援。
* 預設地區是可設定的。

#### 應用程式案例

| 應用程式 | 案例 |
| --- | --- |
| 查看器本地化 | 在實作靜態內容目錄後，本地化會完全以 locale= 參數控制；此參數會附加至所有對 IS 提出的請求。設定記錄、外觀、啟動畫面等項目可能會有地區特定變體。IS 會提供正確的內容，檢視器無須知道哪些內容已本地化以及內容的 ID。 |
| 影像和視頻 | 跨國公司常會混用通用內容與地區特定內容。在此機制下，對影像或視訊的參考會是通用的，而 IS 會在有可用的地區特定內容時加以提供。 |
| 映像集和媒體集 | 對於某些語言環境（例如，當eCatalog不同時），整個影像集可以不同，而查看器將處理從泛型到特定於語言環境的影像集的轉換。 通常，泛型集中的單個ID可以引用本地化內容。 例如，除控制面板的照片外，設備的大多數照片都可以用所有語言顯示。 IS 會自動翻譯 ID，因此無須產生地區特定影像集。 |

#### 實施資產本地化

Adobe Dynamic Media Classic和影像服務具有允許影像和靜態內容本地化的介面。

若未本地化，影像伺服器的 URL 將看起來如下:

`https://server/is/image/company/image`

通過本地化，影像伺服器URL將 `locale=` 路徑的參數，如下所示：

`https://server/is/image/company/image?locale=de_DE`

在接收到映像伺服器的http調用時， `locale=` 通過 `localeMap` 在 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 映像伺服器]** > **[!UICONTROL 本地化支援]** 組。

「地區地圖」欄位會包含以管線符號 (|) 分隔的項目清單。

每個項目都包含一份以逗號分隔的值清單。第一個值是由 `locale=` 的下界。 其餘值是尾碼/替換值，然後嘗試這些值，直到一個值產生現有影像。

應套用字尾值還是取代值，取決於「**[!UICONTROL 設定]**」>「**[!UICONTROL 應用程式設定]**」>「**[!UICONTROL 發佈設定]**」>「**[!UICONTROL 影像伺服器]**」>「**[!UICONTROL 本地化支援]**」群組中的「全域地區」設定。

>[!NOTE]
>
>只有通過API(而不是在Adobe Dynamic Media Classic介面內)設定全局區域設定時，才可能設定全局區域設定。

**字尾範例:**

| URL | localeMap ID | 結果 |
| --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 請注意，其中並未定義 GlobalLocale。區域設定參數de_DE與 `localeMap`。 第一個對應值 _DE 會增加為資產的字尾 (image_DE)，接著會嘗試在影像伺服器上尋找此項目。如果在伺服器上找到此項目，則會加以傳回。如果找不到，則會以第二個值“”作為字尾，而傳回影像本身。 |

**取代範例:**

| URL | `GlobalLocale` 和 `localeMap` ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在上述取代範例中，GlobalLocale 設為 main。區域設定參數de_DE與 `localeMap`。 找到GlobalLocale子字串，並用第一個相應值替換 `de` 的 `localeMap`: `image-de-01`。 如果在影像伺服器上找到此項目，則會加以傳回。如果找不到，則會取代第二個值，而產生 `image-main-01`。 |

如果 URL 中未定義地區，影像伺服器會使用 DefaultLocale，如果已定義，則會將該地區套用至 URL。

如果提供了未知或空的區域設定參數 `locale=`，則 `localeMap` 將掃描空值「開頭為」。 對未知語言環境應用預設語言環境非常重要。

#### 關於defaultImage

影像伺服器會針對所請求的地區逐一嘗試各個選項。如果找不到匹配項，則區域設定選項將應用於defaultImage，並返回匹配版本。 因此，每個語言環境都必須包含一個不本地化的影像選項，或本地化的defaultImage版本在Adobe Dynamic Media Classic可用。

#### 尋找 localeMap 的案例 

假設您要支援下列地區:

`en, en_us, en_uk, de, de_at, de_de, fr`

將這些區域設定映射到尾碼 `_E`。 `_G`, `_F`，分別用於英語、德語和法語。 在所有範例中，通用輸入影像 ID 皆為 `myImg`。

##### 尋找 localeMap 的標準行為

地區 ID 會對應至其對應的字尾。如果在目錄中找不到地區特定 ID，則會以通用 ID 嘗試。記下對應至通用 ID 的空 locSuffix 值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他 | - |

##### 在地區不明時尋找 localeMap

您可以將不明的地區對應至特定 ID 或通用 ID。例如，可以將未知語言環境映射到英語ID，或者如果不存在，則映射到泛型ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他 | myImg_E,myImg |

您也可以只為未知區域設定使用專用locSuffix（如U），如果沒有，則強制使用預設映像 `_U` 存在，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，您可以直接對應至通用 ID，如下所示:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### 使用多層查找查找localeMap

我們常會需要將地區 (例如歐洲、中東與北美洲) 分組，以滿足地區性標準 (例如外觀)。您可以使用多層式查閱達到此效用。

例如，假設您要支援使用西方與中東地區的集合。這兩個集合都以通用影像集合為基礎，增加或修改了一些影像。然後，將針對特定區域(如 `m1, m2` 兩種中東變種 `w1, w2,` 和 `w3` 三個西方區域設定，但是 `w1` 和 `w3`。 不明地區只會對應至通用集合，且無權存取地區特定影像。以下是地圖將看起來的樣子:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他 | mylmg |

##### 通過搜索特定ID查找localeMap

某些映像命名約定不支援一般映像ID。 請求中的通用 ID 必須對應至目錄中的特定 ID。但是，有些實例不知道確切的特定ID。

使用第一個示例作為基礎，所有語言的影像都可能具有尾碼 `_1`。 `_2`或 `_3`。 特定於法國語言環境的影像可能具有尾碼 `_22` 或 `_23` 尾碼。 特定於德國語言環境的影像可以有尾碼 `_470` 或 `_480`。

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他 | myImg_1, myImg_2, myImg_3 |

##### 實作本地化支援時的重要注意事項

* 本地化限用於以 ID 為基礎的資產呼叫，而無法用於以路徑為基礎的資產呼叫。因此，在呼叫具有地區設定的視訊時，必須以 company/assetID 的形式呼叫，而不是以視訊的完整路徑。無法將rtmp與本地化一起使用，因為此方法僅用於基於路徑的視頻呼叫。
* 如果 localeMap 作用中，您就無法使用包含單一視訊的混合媒體集，否則對該媒體集之內容的呼叫將會失敗。要解決此問題，可以將單個視頻添加到自適應視頻集。 接著，將最適化視訊集增加至混合媒體集。
* 有些請求並不會本地化，例如最適化視訊集之內容的請求。因此，如果要將自適應視頻集與本地化一起使用，請將自適應視頻集置於混合媒體集中。 然後，使用 `locale=` 的下界。

## 影像演算 {#image-renderer}

「影像呈現器」頁為從影像呈現伺服器傳遞影像集建立預設設定。 這五個類別中提供了設定（有關設定的詳細說明，請參閱「映像伺服器」頁本身）:

* **[!UICONTROL 目錄管理]**  — 這些設定決定了Adobe Dynamic Media Classic與目錄檔案的交互方式。 Adobe Dynamic Media Classic呈現伺服器URL調用到目錄，而目錄又調用從伺服器傳送映像。 只有在Adobe Dynamic Media Classic支援人員的協助下才更改這些設定。

* **[!UICONTROL 會話屬性]**  — 這些設定建立錯誤參數、相對影像URL的URL以及是否允許對象重疊。

* **[!UICONTROL 預設物料屬性]**  — 這些設定為影像建立預設解析度和銳化設定。

* **[!UICONTROL 響應影像屬性]**  — 這些設定與影像的預設外觀有關。

* **[!UICONTROL 顏色管理屬性]**  — 這些設定與影像的預設顏色設定相關。

## 暈映 {#vignette}

「Vignette」(Vignette)頁面提供了設定，用於建立小圖的預設外觀（有關選項的詳細說明，請參閱頁面本身）。
