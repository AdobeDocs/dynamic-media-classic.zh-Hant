---
title: 發佈設定
description: 發佈設定設定可讓您決定預設如何將資產從Adobe Dynamic Media Classic伺服器傳遞至網站或應用程式。
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

「發佈設定」頁面設定會決定預設情況下如何將資產從Adobe Dynamic Media Classic伺服器傳遞至網站或應用程式。 如果未指定任何設定，Adobe Dynamic Media Classic伺服器會根據「發佈設定」頁面上的預設設定來傳送資產。 例如，傳送不包含解析度屬性的影像的請求會產生影像，影像伺服器頁面上具有「預設物件解析度」設定。

管理員可以變更影像伺服器、影像轉譯器和暈映頁面上的預設設定，以建立從伺服器傳送資產的預設設定。

若要開啟「發佈設定」頁面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]**.

>[!NOTE]
>
>「發佈設定」頁面可供經驗豐富的網站開發人員和程式設計人員使用。 Adobe Dynamic Media Classic假設在這些頁面上變更設定的使用者熟悉Adobe Dynamic Media Classic、HTTP通訊協定標準和慣例，以及基本影像技術。

## 影像伺服器 {#image-server}

「影像伺服器」頁建立從影像伺服器傳送影像的預設設定。 這五個類別中都有設定可用（如需設定的詳細說明，請參閱影像伺服器頁面本身）。

請僅在Adobe Dynamic Media Classic支援人員協助下變更這些設定。

* **[!UICONTROL 目錄管理]**  — 這些設定決定Adobe Dynamic Media Classic和目錄的互動方式。 與大多數Web伺服器不同，Dynamic Media影像伺服器URL呼叫會轉至資訊清單或目錄檔案，而非影像檔案適當。 目錄檔案 (請勿與 eCatalog 混淆) 包含了所有發佈至影像伺服器的內容清單，以及各個影像的路徑。如果您有 Digimarc ID，請在「Digimarc 使用者資訊」區段輸入您的使用者資訊。

* **[!UICONTROL 請求屬性]**  — 這些設定對可從伺服器傳送的影像施加限制。 例如， *最大值* **[!UICONTROL 回覆影像大小限制]** is **[!UICONTROL 寬度]** 5000和 **[!UICONTROL 高度]** 5000。

* **[!UICONTROL 預設請求屬性]**  — 這些設定與影像的預設外觀相關。

* **[!UICONTROL 常見縮圖屬性]**  — 這些設定與縮圖影像的預設外觀和對齊方式有關。

* **[!UICONTROL 目錄欄位的預設值]**  — 這些設定與影像的解析度和預設縮圖類型相關。

* **[!UICONTROL 色彩管理屬性]**  — 這些設定確定使用的ICC顏色配置檔案。

* **[!UICONTROL 相容性屬性]**  — 此設定允許將文本層中的前導段落和尾隨段落與3.6版中的段落一樣處理，以實現向後相容性。

* **[!UICONTROL 本地化支援]*** — 這些設定可讓您管理多個地區設定屬性。 也可以讓您指定地區地圖字串，以便您定義要在「檢視器」的各種工具提示中支援的語言。

   例如，如果您是在不同國家/地區銷售的跨國品牌，則請確認每個國家/地區皆擁有自己的特定地區「檢視器」。若要完成此功能設定，您須指定地區地圖字串。然後，您可以添加所需語言的翻譯文本字串，以編輯查看器預設集中的工具提示文本。

   >[!NOTE]
   > 要設定本地化支援選項， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，請求設定說明。

   如需關於設定「**[!UICONTROL 本地化支援]**」的詳細資訊，請參閱[進行資產本地化設定時的注意事項](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 進行資產本地化設定時的注意事項 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果要在Adobe Dynamic Media Classic中設定「本地化支援」選項，如「地區對應」欄位， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，請求設定說明。

使用Adobe Dynamic Media Classic的常見方式是管理電子商務網站上的產品影像。 國際企業常面臨類似產品的資產在不同國家間有外觀差異的問題。通常，這些差異適用於整體介質的某些部分。 通過複製每個國家的所有資產和僅對這些差異進行疊加處理來解決這些差異是一項巨大的努力，與單一的主要資產隱喻相矛盾。 資產的此類差異可能無所不在，從因不同國家而有不同配音的視訊，到產品所用電源線這種微小但重要的差異都包括在內。Adobe Dynamic Media Classic使用基本查閱機制。 您可以定義影像伺服器查閱資產字尾的順序，以從必要的地區開始。

#### 資產本地化的方式

IS (影像伺服) 請求的地區可透過下列 IS/IR (影像演算) 命令來識別:

`locale=`

此命令可接受不區分大小寫的地區 ID (locId) 字串。地區 ID 通常是 2 到 6 個由字母與“_”字元組成的字串。

IS支援任意可打印的ASCII字串。 此 `locale=` 命令具有全局範圍，這表示它將應用於整個請求，包括所有嵌套的IS和IR請求、引用的模板和影像層。 不支援一個請求有多個地區 (例如每個圖層各有不同的地區)。但要允許在內嵌的請求中進行明確覆寫，這倒是可行。

若 `locale=` 未指定， `attribute::DefaultLocale` 會傳遞至翻譯引擎。 有限的輸入驗證會套用至 `locale=` 值。 空白 `locale=` 允許值。 因為 `locale=` 有全球範圍， `attribute::DefaultLocale` 由整個請求的主要目錄提供。

使用的部分優點 `locale=` 和 `attribute::DefaultLocale` 包括下列項目：

* 共用多個地區的內容。
* 使用通用 ID 存取地區特定內容。
* 在命名慣例與地區特定內容的管理上更具彈性，例如地區字首與字尾的比較，或是個別目錄中的地區特定內容。
* 支援對特定地區版本的訪問。
* 聚合對象（如影像集）有時可以包含對可能特定於語言環境的內容的一般引用。
* 支援由需要本地化的目錄管理的所有內容，包括影像、影像集、暈映、材料和查看器配置記錄。
* 將 IPS 資料庫與 IS 資訊清單機制的變更降至最低。
* 實作RFC IS-63時，新增對靜態內容（例如視訊和外觀）的支援。
* 預設地區是可設定的。

#### 應用程式案例

| 應用程式 | 案例 |
| --- | --- |
| 檢視器本地化 | 在實作靜態內容目錄後，本地化會完全以 locale= 參數控制；此參數會附加至所有對 IS 提出的請求。設定記錄、外觀、啟動畫面等項目可能會有地區特定變體。IS 會提供正確的內容，檢視器無須知道哪些內容已本地化以及內容的 ID。 |
| 影像與影片 | 跨國公司常會混用通用內容與地區特定內容。在此機制下，對影像或視訊的參考會是通用的，而 IS 會在有可用的地區特定內容時加以提供。 |
| 影像集和媒體集 | 對於某些區域設定（例如當eCatalog不同時），整個影像集可能不同，從通用影像轉換為由查看器處理的特定於區域設定的影像集。 通常，一般集中的個別ID可以指當地語系化內容。 例如，設備的大多數照片可以用所有語言相同，但控制面板的照片除外。 IS 會自動翻譯 ID，因此無須產生地區特定影像集。 |

#### 實作資產本地化

Adobe Dynamic Media Classic和影像伺服有一個介面，可將影像和靜態內容定位。

若未本地化，影像伺服器的 URL 將看起來如下:

`https://server/is/image/company/image`

透過本地化，影像伺服器URL會新增 `locale=` 參數，如下所示：

`https://server/is/image/company/image?locale=de_DE`

影像伺服器收到http呼叫時， `locale=` 參數會透過 `localeMap` 在 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]** > **[!UICONTROL 本地化支援]** 群組。

「地區地圖」欄位會包含以管線符號 (|) 分隔的項目清單。

每個項目都包含一份以逗號分隔的值清單。第一個值是 `locale=` 參數。 其餘值是尾碼/取代值，然後會嘗試這些值，直到有一個值產生現有影像為止。

應套用字尾值還是取代值，取決於「**[!UICONTROL 設定]**」>「**[!UICONTROL 應用程式設定]**」>「**[!UICONTROL 發佈設定]**」>「**[!UICONTROL 影像伺服器]**」>「**[!UICONTROL 本地化支援]**」群組中的「全域地區」設定。

>[!NOTE]
>
>只有透過API設定時，才能使用「全域地區設定」，而不是在Adobe Dynamic Media Classic介面中。

**字尾範例:**

| URL | localeMap ID | 結果 |
| --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 請注意，其中並未定義 GlobalLocale。區域設定參數de_DE與 `localeMap`. 第一個對應值 _DE 會增加為資產的字尾 (image_DE)，接著會嘗試在影像伺服器上尋找此項目。如果在伺服器上找到此項目，則會加以傳回。如果找不到，則會以第二個值“”作為字尾，而傳回影像本身。 |

**取代範例:**

| URL | `GlobalLocale` 和 `localeMap` ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在上述取代範例中，GlobalLocale 設為 main。區域設定參數de_DE與 `localeMap`. 找到GlobalLocale子字串，並用第一個對應值替換 `de` 在 `localeMap`: `image-de-01`. 如果在影像伺服器上找到此項目，則會加以傳回。如果找不到，則會取代第二個值，而產生 `image-main-01`。 |

如果 URL 中未定義地區，影像伺服器會使用 DefaultLocale，如果已定義，則會將該地區套用至 URL。

如果為未知或空的地區設定參數提供 `locale=`，則 `localeMap` 會掃描空白值「開頭為」。 請務必為未知地區套用預設地區設定。

#### 關於defaultImage

影像伺服器會針對所請求的地區逐一嘗試各個選項。如果未找到匹配項，則語言環境選項將應用於defaultImage，並返回匹配版本。 因此，每個語言環境必須包含一個不本地化的影像選項，或是使用本地化的defaultImage版本。Adobe Dynamic Media Classic

#### 尋找 localeMap 的案例 

假設您要支援下列地區:

`en, en_us, en_uk, de, de_at, de_de, fr`

將這些區域設定映射到尾碼 `_E`, `_G`，和 `_F`，分別用於英文、德文和法文。 在所有範例中，通用輸入影像 ID 皆為 `myImg`。

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

您可以將不明的地區對應至特定 ID 或通用 ID。例如，您可以將未知的地區設定對應至英文ID，或者如果不存在，則對應至一般ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他 | myImg_E,myImg |

您也可以只針對未知的地區設定，使用專用的locSuffix（例如U），若否則強制使用預設影像 `_U` 存在，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，您可以直接對應至通用 ID，如下所示:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### 使用多層查找查找查找localeMap

我們常會需要將地區 (例如歐洲、中東與北美洲) 分組，以滿足地區性標準 (例如外觀)。您可以使用多層式查閱達到此效用。

例如，假設您要支援使用西方與中東地區的集合。這兩個集合都以通用影像集合為基礎，增加或修改了一些影像。然後會針對特定地區設定(例如 `m1, m2` 兩種中東變體， `w1, w2,` 和 `w3` 只是共用影像 `w1` 和 `w3`. 不明地區只會對應至通用集合，且無權存取地區特定影像。以下是地圖將看起來的樣子:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他 | mylmg |

##### 通過搜索特定ID查找localeMap

有些影像命名慣例不支援一般影像ID。 請求中的通用 ID 必須對應至目錄中的特定 ID。不過，在某些情況下，系統不會知道確切的特定ID。

以第一個範例為基礎，所有語言的影像都可能有尾碼 `_1`, `_2`，或 `_3`. 法國地區設定的特定影像可能具有尾碼 `_22` 或 `_23` 尾碼。 而德國地區特有的影像可能具有尾碼 `_470` 或 `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| 地區設定= | 要搜尋的輸出 ID |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他 | myImg_1, myImg_2, myImg_3 |

##### 實作本地化支援時的重要注意事項

* 本地化限用於以 ID 為基礎的資產呼叫，而無法用於以路徑為基礎的資產呼叫。因此，在呼叫具有地區設定的視訊時，必須以 company/assetID 的形式呼叫，而不是以視訊的完整路徑。您無法透過本地化使用rtmp，因為該方法僅用於路徑型視訊呼叫。
* 如果 localeMap 作用中，您就無法使用包含單一視訊的混合媒體集，否則對該媒體集之內容的呼叫將會失敗。若要解決此問題，您可以將單一視訊新增至最適化視訊集。 接著，將最適化視訊集增加至混合媒體集。
* 有些請求並不會本地化，例如最適化視訊集之內容的請求。因此，如果您想要將適用性視訊集與本地化搭配使用，請將適用性視訊集置於混合媒體集內。 然後，使用將該集呼叫至混合媒體檢視器 `locale=` 參數。

## 影像演算 {#image-renderer}

「影像轉譯器」頁面建立從影像轉譯伺服器傳送影像集的預設設定。 這五個類別中都有設定可用（如需設定的詳細說明，請參閱影像伺服器頁面本身）:

* **[!UICONTROL 目錄管理]**  — 這些設定可決定Adobe Dynamic Media Classic和目錄檔案的互動方式。 Adobe Dynamic Media Classic會對目錄進行轉譯伺服器URL呼叫，而目錄會進行呼叫，以從伺服器傳送影像。 請僅在Adobe Dynamic Media Classic支援人員協助下變更這些設定。

* **[!UICONTROL 工作階段屬性]**  — 這些設定會建立錯誤參數、相對影像URL的URL，以及是否允許物件重疊。

* **[!UICONTROL 預設材料屬性]**  — 這些設定建立影像的預設解析度和銳利化設定。

* **[!UICONTROL 回應影像屬性]**  — 這些設定與影像的預設外觀相關。

* **[!UICONTROL 色彩管理屬性]**  — 這些設定屬於影像的預設顏色設定。

## 暈映 {#vignette}

「暈映」頁面提供建立暈映預設外觀的設定（如需選項的詳細說明，請參閱頁面本身）。
