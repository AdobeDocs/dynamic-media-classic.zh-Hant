---
title: 發佈設定
seo-title: 發佈設定
description: 'null'
seo-description: 「發佈設定」畫面設定會決定預設從Dynamic Media Classic伺服器傳送資產至網站或應用程式的方式。
uuid: 196f25c-abf5-4c5 d-8f6 f-bc70007 a0301
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
discoiquuid: cba59093-28b6-4490-b838-d942 b72 ad1 ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 發佈設定 {#publish-setup}

「發佈設定」畫面設定會決定預設從Dynamic Media Classic伺服器傳送資產至網站或應用程式的方式。如果未指定任何設定，Dynamic Media Classic伺服器會根據「發佈設定」畫面上的預設設定來傳送資產。例如，不包含解析度屬性的傳遞影像要求，會在「影像伺服器」畫面中產生含有「預設物件解析度」設定的影像。

管理員可以在「影像伺服器」、「影像演算」和「暈映」畫面中變更預設設定，以建立預設設定並用來從伺服器傳送資產。

若要開啟「發佈資產」畫面，請按一下「設定 &gt; 應用程式設定 &gt; 發佈設定」。

>[!NOTE]
>
>「發佈設定」畫面可供資深的網站開發人員與程式設計師使用。Dynamic Media Classic假設使用者在這些畫面上變更設定時，熟悉Scene Publishing System、HTTP通訊協定標準和慣例，以及基本的影像技術。

## 影像伺服器 {#image-server}

「影像伺服器」畫面會建立預設設定，以從影像伺服器傳送影像。有下列五種設定可供使用 (請參閱「影像伺服器」畫面以取得詳細的設定描述)。

僅在Dynamic Media Classic支援人員的協助下變更這些設定。

**目錄管理** 這些設定可決定Scene Publishing System和目錄的互動方式。和多數Web伺服器不同的是，動態媒體影像伺服器URL呼叫會移至manifest-or catalog-file，而非影像檔案適當的位置。目錄檔案 (請勿與 eCatalog 混淆) 包含了所有發佈至影像伺服器的內容清單，以及各個影像的路徑。如果您有 Digimarc ID，請在「Digimarc 使用者資訊」區段輸入您的使用者資訊。

**請求屬性** 這些設定會限制可從伺服器傳送的影像。

**預設請求屬性** 這些設定與影像的預設外觀有關。

**常見縮圖屬性** 這些設定與預設外觀和縮圖影象對齊有關。

**目錄欄位預設** 值這些設定會與解析度和預設縮圖類型有關。

**色彩管理屬性** 這些設定決定使用哪些ICC色彩設定檔。

**相容性屬性** 此設定可讓文字圖層中的前導和尾隨段落被視為其在版本3.6中的向下相容性。

**本地化支援** 這些設定可讓您管理多個地區設定屬性。也可以讓您指定地區地圖字串，以便您定義要在「檢視器」的各種工具提示中支援的語言。

例如，如果您是在不同國家/地區銷售的跨國品牌，則請確認每個國家/地區皆擁有自己的特定地區「檢視器」。若要完成此功能設定，您須指定地區地圖字串。然後為您要的語言增加翻譯文字字串，以編輯「檢視器」預設集中的工具提示文字。

>[!NOTE]
> 若要設定本地化支援選項，請聯絡Adobe Dynamic Media Classic技術支援，或傳送電子郵件至requesting要求設定說明。

如需關於設定「**本地化支援**」的詳細資訊，請參閱[進行資產本地化設定時的注意事項](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 進行資產本地化設定時的注意事項 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果您想要在Scene Publishing System(例如Locale Map欄位)中設定本地化支援選項，請聯絡Adobe Dynamic Media Classic技術支援。或者，請將電子郵件傳送到 s7support@adobe.com 請求設定協助。

Scene7 Publishing System (SPS) 常見的用途之一，就是管理電子商務網站上的產品圖像。國際企業常面臨類似產品的資產在不同國家間有外觀差異的問題。這些差異通常出現在整體媒體中的微小部分上。針對每個國家來複製所有資產，然後僅就差異的部分進行覆寫來處理此類差異，不僅工程浩大，也與單一主資產的精神相違背。資產的此類差異可能無所不在，從因不同國家而有不同配音的視訊，到產品所用電源線這種微小但重要的差異都包括在內。Dynamic Media Classic使用基本查閱機制。您可以定義影像伺服器查閱資產字尾的順序，以從必要的地區開始。

**資產本地化的方式**

IS (影像伺服) 請求的地區可透過下列 IS/IR (影像演算) 命令來識別:

`locale=`

此命令可接受不區分大小寫的地區 ID (locId) 字串。地區 ID 通常是 2 到 6 個由字母與“_”字元組成的字串。

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. 不支援一個請求有多個地區 (例如每個圖層各有不同的地區)。但要允許在內嵌的請求中進行明確覆寫，這倒是可行。

`locale=` 如果未指定 `attribute::DefaultLocale` ，則會傳遞至翻譯引擎。Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* 共用多個地區的內容。
* 使用通用 ID 存取地區特定內容。
* 在命名慣例與地區特定內容的管理上更具彈性，例如地區字首與字尾的比較，或是個別目錄中的地區特定內容。
* 支援直接存取地區特定版本。
* 彙總物件 (例如影像集) 可包含對可能隨地區而不同之內容的通用參考。
* 支援所有以目錄管理而可能需要本地化的內容，包括影像、影像集、暈映、材質與檢視器設定記錄。
* 將 IPS 資料庫與 IS 資訊清單機制的變更降至最低。
* 在實作 RFC IS-63 時，將會增加靜態內容 (例如視訊與外觀) 的支援。
* 預設地區是可設定的。

**應用程式案例**

| 應用程式 | 案例 |
|--- |--- |
| 檢視器本地化 | 在實作靜態內容目錄後，本地化會完全以 locale= 參數控制；此參數會附加至所有對 IS 提出的請求。設定記錄、外觀、啟動畫面等項目可能會有地區特定變體。IS 會提供正確的內容，檢視器無須知道哪些內容已本地化以及內容的 ID。 |
| 影像與視訊 | 跨國公司常會混用通用內容與地區特定內容。在此機制下，對影像或視訊的參考會是通用的，而 IS 會在有可用的地區特定內容時加以提供。 |
| 影像集與媒體集 | 某些地區設定的整個影像集都不同—例如eCatalog完全不同—將一般的一般ID轉換為由檢視器處理的地區設定影象集。一般設定中的個別ID可能參照本地化的內容。例如，一項設備大部分的相片可能跨所有語言都相同，唯獨控制台的相片是例外。IS 會自動翻譯 ID，因此無須產生地區特定影像集。 |

**實作資產本地化**

Scene7 Publishing 與「影像伺服」有個介面可將影像與靜態內容本地化。

若未本地化，影像伺服器的 URL 將看起來如下:

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** &gt; **Application Setup** &gt; **Publish Setup** &gt; **Image Server** &gt; **Localization Support** group.

「地區地圖」欄位會包含以管線符號 (|) 分隔的項目清單。

每個項目都包含一份以逗號分隔的值清單。The first value is the search value that is passed by the `locale=` parameter. 其餘值則為後續持續嘗試直到比對出現有影像為止的字尾/取代值。

應套用字尾值還是取代值，取決於「**設定**」&gt;「**應用程式設定**」&gt;「**發佈設定**」&gt;「**影像伺服器**」&gt;「**本地化支援**」群組中的「全域地區」設定。

>[!NOTE]
>
>就目前而言，「全域地區」只能透過 API 進行設定，而無法在 Scene7 Publishing System 介面內設定。

**字尾範例**

| URL | localeMap ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 請注意，其中並未定義 GlobalLocale。地區參數 de_DE 會與 localeMap 中的第一個項目進行比對。第一個對應值 _DE 會增加為資產的字尾 (image_DE)，接著會嘗試在影像伺服器上尋找此項目。如果在伺服器上找到此項目，則會加以傳回。如果找不到，則會以第二個值“”作為字尾，而傳回影像本身。 |

**取代範例**

| URL | GlobalLocale 與 localeMap ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在上述取代範例中，GlobalLocale 設為 main。地區參數 de_DE 會與 localeMap 中的第一個項目進行比對。在找到 GlobalLocale 子字串後，此子字串被取代為 localeMap 中的第一個對應值 de: image-de-01。如果在影像伺服器上找到此項目，則會加以傳回。如果找不到，則會取代第二個值，而產生 image-main-01。 |

如果 URL 中未定義地區，影像伺服器會使用 DefaultLocale，如果已定義，則會將該地區套用至 URL。

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. 請務必設定此值，以便在地區不明時套用預設地區。

**關於 defaultImage**

影像伺服器會針對所請求的地區逐一嘗試各個選項。如果找不到相符項目，則會將地區選項套用至 defaultImage，並傳回相符的版本。因此，每個地區都應有未本地化的影像所適用的選項，或者，本地化的 defaultImage 版本必須設定成可在 Scene7 Publishing System 中使用。

**尋找 localeMap 的案例** 

假設您要支援下列地區:

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. 在所有範例中，通用輸入影像 ID 皆為 `myImg`。

*尋找 localeMap 的標準行為*

地區 ID 會對應至其對應的字尾。如果在目錄中找不到地區特定 ID，則會以通用 ID 嘗試。記下對應至通用 ID 的空 locSuffix 值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| 地區設定= | 要搜尋的輸出 ID |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他 | - |

*在地區不明時尋找 localeMap*

您可以將不明的地區對應至特定 ID 或通用 ID。在此處的範例中，您可以將不明的地區對應至英文 ID，或在沒有英文 ID 存在時對應至通用 ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| 地區設定= | 要搜尋的輸出 ID |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他 | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，您可以直接對應至通用 ID，如下所示:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*使用多層式查閱尋找 localeMap*

我們常會需要將地區 (例如歐洲、中東與北美洲) 分組，以滿足地區性標準 (例如外觀)。您可以使用多層式查閱達到此效用。

例如，假設您要支援使用西方與中東地區的集合。這兩個集合都以通用影像集合為基礎，增加或修改了一些影像。Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. 不明地區只會對應至通用集合，且無權存取地區特定影像。以下是地圖將看起來的樣子:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| 地區設定= | 要搜尋的輸出 ID |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他 | mylmg |

*搜尋特定 ID 來尋找 localeMap*

有些影像命名慣例可能不支援通用影像 ID。請求中的通用 ID 必須對應至目錄中的特定 ID。但在某些情況下，確切的 ID 可能仍屬未知。

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| 地區設定= | 要搜尋的輸出 ID |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他 | myImg_1, myImg_2, myImg_3 |

**實作本地化支援時的重要注意事項**

* 本地化限用於以 ID 為基礎的資產呼叫，而無法用於以路徑為基礎的資產呼叫。因此，在呼叫具有地區設定的視訊時，必須以 company/assetID 的形式呼叫，而不是以視訊的完整路徑。這表示您無法將 rtmp 用於本地化，因為該方法僅適用於以路徑為基礎的視訊呼叫。
* 如果 localeMap 作用中，您就無法使用包含單一視訊的混合媒體集，否則對該媒體集之內容的呼叫將會失敗。若要解決此問題，您可以將單一視訊增加至最適化視訊集。接著，將最適化視訊集增加至混合媒體集。
* 有些請求並不會本地化，例如最適化視訊集之內容的請求。因此，如果您想將最適化視訊集用於本地化，則應將最適化視訊集放入混合媒體集內。Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## 影像演算 {#image-renderer}

「影像演算」畫面會建立預設設定，以從影像演算伺服器傳送影像集。有下列五種設定可供使用 (請參閱「影像伺服器」畫面以取得詳細的設定描述):

**目錄管理** 這些設定會決定Scene Publishing System和目錄檔案互動的方式。Dynamic Media Classic Render Server URL會呼叫目錄，此目錄會輪流呼叫從伺服器傳送影像。僅在Dynamic Media Classic支援人員的協助下變更這些設定。

**作業屬性** 這些設定會建立錯誤參數、相對影象URL的URL，以及是否允許物件重疊。

**預設材質屬性** 這些設定會建立影像的預設解析度和銳利化設定。

**回應影像屬性** 這些設定與影像的預設外觀有關。

**色彩管理屬性** 這些設定與影像的預設色彩設定有關。

## 暈映 {#vignette}

「暈映」畫面提供了建立預設暈映外觀 (如需詳細的選項描述，請參閱該畫面) 的設定。