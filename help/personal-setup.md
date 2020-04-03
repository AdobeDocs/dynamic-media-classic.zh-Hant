---
title: 個人設定
seo-title: 個人設定
description: 'null'
seo-description: 所有使用者都可以變更Dynamic Media Classic的「個人設定」畫面上的設定。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 個人設定 {#personal-setup}

所有使用者皆可在「個人設定」畫面上變更設定。若要開啟「個人設定」畫面，請按一下「設定 > 個人設定」。

>[!NOTE]
>
>「個人設定」畫面會列出您在 Scene7 Publishing System 中的使用者角色: 公司管理員、管理員或使用者。

「個人設定」設定可控制瀏覽面板的預設行為、接收電子郵件的方式，以及密碼設定。變更這些設定後，請記得按一下「儲存」。

## 我的帳戶資訊

識別您的帳戶名稱、姓名、使用者名稱 (電子郵件地址)，以及指定的使用者角色。

### 桌面版本

按一下「立即安裝」即可在本機硬碟上安裝 Scene7 Publishing System 桌面版本。或者按一下「立即重新安裝」以再次安裝桌面版本。

### 網路印刷的 Illustrator 外掛程式

在執行 Windows 7 或 8 的電腦上，您必須具有管理員權限並在 Windows 中登入為管理員，才能安裝網路印刷的 Adobe Illustrator 外掛程式。安裝外掛程式之後，即可在 Adobe Illustrator 中使用。

下列 Adobe Illustrator 版本支援外掛程式:

* Adobe Creative Cloud 2014 中的 Adobe Illustrator 18。
* Adobe Creative Cloud 中的 Adobe Illustrator 17。
* Adobe Creative Suite 6 中的 Adobe Illustrator 16。

支援的 Adobe Illustrator 平台包含下列:

* Apple Mac OS X 10.7 或以上版本。
* Windows 8、32 位元和 64 位元。
* Windows 7、32 位元和 64 位元。
* Windows XP、32 位元和 64 位元 (僅適用 Adobe Creative Suite 6 中的 Adobe Illustrator 16)。

另請參閱[範本發佈](quick-start-template-publishing.md)。

## 在您的硬碟上安裝外掛程式

1. 在 Scene7 Publishing System 中的「個人設定」頁面中，於「網路印刷的 Illustrator 外掛程式」下，按一下「**立即下載**」，以下載「**Illustrator Plug-in for Web-to-Print.zip**」檔案。
1. 解壓縮 ZIP 檔案至暫存檔案夾。

   在解壓縮檔案的根目錄中內含了讀我檔案，具有外掛程式的其他相關資訊。

1. 根據您所安裝的作業系統，執行下列任一項作業:

### Windows

| 如果您執行 | 請執行此動作 |
|--- |--- |
| Adobe Creative Cloud 2014 中的 Adobe Illustrator 18 | <ul><li>從解壓縮的檔案夾根目錄，按一下「CC-2014」。</li><li>根據您使用的 Adobe Illustrator 產品版本，按一下「win32」或「win64」。</li><li>按一下「資產庫 > flame」，然後將「`aflame.dll`」複製到 Adobe Illustrator 的執行檔檔案夾。例如，`C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`。 </li></ul><br/>**注意&#x200B;**:此示例路徑用於64位位置；32位元位置可能會落在「Program Files」(x86)之下。<br/><ul><li>返回相同的資產庫檔案夾，按一下「flamingo」，然後將 `aflamingo.dll` 複製到您在先前步驟中使用的相同 Adobe Illustrator 可執行檔檔案夾。 </li><li>返回您在步驟 2 中選取的 win32 或 win64 檔案夾，然後將「`AdobeS7FXGFileFormat.aip`」複製到 Adobe Illustrator 的外掛程式檔案夾。例如，`C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`。 </li></ul> <br/>**注意&#x200B;**:此示例路徑用於64位位置；32位元位置可能會落在「Program Files」(x86)之下。 |
| Adobe Creative Cloud 中的 Adobe Illustrator 17 | <ul><li>從解壓縮的檔案夾根目錄，按一下「CC」。 </li><li>根據您使用的 Adobe Illustrator 產品版本，按一下「win32」或「win64」。</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator&#39;s plug-ins folder. 例如，`C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`。</li></ul><br/>**注意&#x200B;**:此示例路徑用於64位位置；32位元位置可能會落在「Program Files」(x86)之下。 |
| Adobe Creative Suite 6 中的 Adobe Illustrator 16 | <ul><li>從解壓縮的檔案夾根目錄，按一下「6.0」。 </li><li>根據您使用的 Adobe Illustrator 產品版本，按一下「win32」或「win64」。 </li><li>將 AdobeS7FXGFileFormat.aip 複製到 Adobe Illustrator 的外掛程式檔案夾。例如，`C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`。</li></ul><br/>**注意&#x200B;**:此示例路徑用於64位位置；32位元位置可能會落在「Program Files」(x86)之下。 |

### Mac

| 如果您執行 | 請執行此動作 |
|--- |--- |
| Adobe Creative Cloud 2014 中的 Adobe Illustrator 18 | <ul><li>從解壓縮的檔案夾根目錄，按一下「CC-2014 > mac64」。</li><li>按一下「資產庫 > flame」，然後將「`aflame.framework`」檔案夾複製到 Adobe Illustrator 套件內容檔案夾。例如, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. （若要開啟Adobe Illustrator的套件內容檔案夾，請在Adobe Illustrator CC 2014圖示上按一下滑鼠右鍵，然後按一下「從內容選單顯示套件內容」）。</li><li>回到相同的資產庫檔案夾，按一下「`flamingo`」，然後將 `aflamingo.framework` 檔案夾複製到您在先前步驟中使用的相同 Adobe Illustrator 套件內容檔案夾。</li><li>回到您在步驟 1 中選取的「mac64」檔案夾，然後將「`AdobeS7FXGFileFormat.aip`」檔案夾複製到 Adobe Illustrator 的外掛程式檔案夾。例如，`/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`。</li></ul><br/> |
| Adobe Creative Cloud 中的 Adobe Illustrator 17 | <ul><li>從解壓縮資料夾的根目錄，按一下「CC > mac64」</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. 例如，`/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`。</li></ul><br/> |
| Adobe Creative Suite 6 中的 Adobe Illustrator 16 | <ul><li>從解壓縮資料夾的根目錄，按一下6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. 例如，`/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`。</li></ul> |

外掛程式現在已可在 Adobe Illustrator 中使用。

### 瀏覽器

* **縮圖尺寸**
   * 在瀏覽面板中，決定格點檢視內縮圖影像的預設大小。
* **預設資產庫檢視**
   * 決定建置集資產庫中的資產要以縮圖或名稱來顯示。如果您正在處理「資產庫」中的大量資產，則可依名稱來檢視資產。例如，如果您使用許多 PDF 檔案建置大型 eCatalog，便可以依照名稱來檢視資產，使清單較為簡短。
* **預設瀏覽排序順序**
   * 決定瀏覽面板中資產預設顯示的順序。在選單上選擇排序條件，以及是否採用遞增或遞減排序。
* **預設瀏覽位置**
   * 可讓您將瀏覽位置設定為預設、上次瀏覽的檔案夾，或您所導覽和識別的特定位置。您也可以設定瀏覽位置，將檔案和檔案夾按遞增或遞減排序。
* **預設瀏覽檢視**
   * 決定第一次開啟瀏覽面板時看見的預設檢視為格點檢視還是清單檢視。
* **啟動畫面顯示**
   * 決定您是否會看見任何啟動畫面，包含歡迎啟動畫面。
* **顯示工具提示**
   * 決定將指標移過按鈕、選單和導覽連結時是否顯示工具提示。工具提示會描述螢幕上的項目。
* **棋盤格背景**
   * 顯示影像後方的棋盤格圖層，可讓您輕鬆查看具有 Alpha 色版的透明影像區域。
* **顯示檔案大小**
   * 在您瀏覽時顯示資產檔案大小。
* **離開 SPS 時確認**
   * 在您結束 Scene7 Publishing System 前顯示確認視窗。
* **搜尋時包含 UDF**
   * 取消選取 (預設) 時，可讓您執行的大部分中繼資料搜尋得到較佳的系統效能。

如果納入使用者定義的欄位有助於您執行中繼資料搜尋，您可以選取此選項而加以開啟。或者，您可以使用「進階搜尋」來進行比納入使用者定義的欄位更為直接而快速的搜尋。

請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

另請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。

* **基本搜尋類型**
   * 選擇預設搜尋類型 (「包含」或「開頭為」)。
* **顯示 Media Portal 的功能**
   * 選取此選項可存取 Media Portal 的功能，例如媒體購物車。
* **顯示命令的回應效果**
   * 顯示對伺服器的命令要求。
* **匯出過程顯示對話框**
   * 執行匯出時顯示對話框。如果您取消選取此選項，您還是可以前往「工作」頁面取得匯出結果。

## 電子郵件

* **電子郵件選項**
   * 選擇您希望Dynamic Media Classic在上傳和發佈工作完成時以電子郵件通知您的方式。 只有在出現警告或錯誤時才會收到工作完成通知。
* **電子郵件範圍**
   * 決定您要接收公司的所有電子郵件，或僅接收有關您啟動之上載和發佈工作的電子郵件。
* **電子郵件類型**
   * 決定您是否會在上載工作和發佈工作完成時收到通知。
* **語言**
* **偏好語言**
   * 決定介面的語言。
* **密碼**
* **新密碼**
   * 輸入新的有效密碼。 您的密碼必須符合下列要求：
      * 長度介於8-25個字元之間
      * 至少包含一個小寫字母
      * 至少包含一個大寫字母
      * 至少包含一個數字
      * 至少包含下列其中一個特殊字元：#$&amp;-_:{}

* **重新輸入密碼**
   * 重新輸入新密碼，以確定您已正確輸入密碼。
* **密碼有效期**
   * 決定是否而讓密碼在 72 天後到期作為安全措施。如果您選取「是」，72 天後系統便會要求您建立新密碼。
