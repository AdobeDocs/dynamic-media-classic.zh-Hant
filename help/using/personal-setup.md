---
title: 個人設定
description: 所有使用者均可在Adobe Dynamic Media Classic的「個人設定」畫面中變更設定。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# 個人設定 {#personal-setup}

所有使用者皆可在「個人設定」畫面上變更設定。若要開啟「個人設定」畫面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

>[!NOTE]
>
>「個人設定」畫面會列出您在Adobe Dynamic Media Classic中的使用者角色：公司管理員、管理員或使用者。

「個人設定」設定可控制「瀏覽」面板的預設行為、接收電子郵件的方式以及密碼設定。 記得選取 **[!UICONTROL 儲存]** 變更這些設定之後。

## 我的帳戶資訊

識別您的帳戶名稱、姓名、使用者名稱 (電子郵件地址)，以及指定的使用者角色。

## 桌上型電腦

* **清除影像快取**：從電腦中移除所有Adobe Dynamic Media快取影像檔案。
* **清除資產快取**：從您的電腦移除所有Adobe Dynamic Media快取資產檔案。

除了使用案頭應用程式清除影像和資產快取以外，您也可以直接從檔案系統手動清除快取。 根據您的作業系統，瀏覽至下列專案：

* macOS： `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®： `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**若要安裝Adobe Dynamic MediaCreative Suite擴充功能：**

1. 在Adobe Dynamic Media Classic的工具列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，在Creative Suite擴充功能下，選取 **[!UICONTROL 立即下載]** 若要下載 `s7csxs.zxp` 檔案。
1. 選取 **[!UICONTROL 安裝]** 和 **[!UICONTROL 系統需求]** 連結，以取得擴充功能的其他資訊。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## 瀏覽器

* **[!UICONTROL 縮圖大小]**：決定「瀏覽」面板中格線檢視的縮圖影像預設大小。
* **[!UICONTROL 預設資產庫檢視]**：決定組建集的資產庫中的資產是以縮圖還是名稱顯示。 如果您正在處理「資產庫」中的大量資產，則可依名稱來檢視資產。例如，如果您使用許多 PDF 檔案建置大型 eCatalog，便可以依照名稱來檢視資產，使清單較為簡短。
* **[!UICONTROL 預設瀏覽排序順序]**：決定資產在瀏覽面板中的預設顯示順序。 在選單上選擇排序條件，以及是否採用遞增或遞減排序。
* **[!UICONTROL 預設瀏覽位置]**：可讓您將瀏覽位置設為預設值、瀏覽的最後一個資料夾，或設為您導覽以識別的特定位置。 您也可以設定瀏覽位置，將檔案和檔案夾按遞增或遞減排序。
* **[!UICONTROL 預設瀏覽檢視]**：決定「格點檢視」或「清單檢視」是您第一次開啟「瀏覽」面板時看到的預設檢視。
* **[!UICONTROL 啟動畫面顯示]**：決定您是否看到任何啟動畫面，包括歡迎啟動畫面。
* **[!UICONTROL 顯示工具提示]**：決定當您將指標移到按鈕、選單和導覽連結上時是否顯示工具提示。 工具提示說明熒幕上的使用者介面專案。
* **[!UICONTROL 棋盤格背景]**：在影像後面顯示棋盤格圖層，讓您輕鬆檢視具有Alpha色版的影像的透明區域。
* **[!UICONTROL 顯示檔案大小]**：瀏覽時顯示資產的檔案大小。
* **[!UICONTROL 在搜尋中包含UDF]**：若要改善您執行的大部分中繼資料搜尋的系統效能，請取消選取（預設）。

  如果納入使用者定義的欄位有助於您執行中繼資料搜尋，您可以選取此選項而加以開啟。相較於包含使用者定義的欄位，使用進階搜尋可提供更直接且更快速的搜尋體驗。

  請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

  另請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。

* **[!UICONTROL 基本搜尋型別]**：您可從兩個選項中選取： **[!UICONTROL 包含]** 搜尋指定值的完整字串； **[!UICONTROL 開頭為]** 從字串的開頭開始搜尋並傳回結果的速度比 **[!UICONTROL 包含]**. 任一選項都會覆寫在中設定的預設值 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 應用程式一般設定]** 由管理員執行。
* **[!UICONTROL 顯示命令回饋]**：選取此選項可開啟對伺服器顯示命令要求的功能；取消選取此選項可關閉。
* **[!UICONTROL 匯出期間顯示對話方塊]**：選取此項可在匯出期間顯示快顯對話方塊。 如果取消選取（關閉）此選項，您仍可以移至「工作」頁面來擷取匯出結果。

## 電子郵件

* **[!UICONTROL 電子郵件選項]**：選擇您希望Adobe Dynamic Media Classic在上傳和發佈作業完成時，透過電子郵件通知您的方式。 只有在出現警告或錯誤時才會收到工作完成通知。
* **[!UICONTROL 電子郵件範圍]**：決定您是收到公司的所有工作電子郵件，還是只收到您啟動的上傳和發佈工作相關電子郵件。
* **[!UICONTROL 電子郵件型別]**：決定是否會在上傳作業和發佈作業完成時通知您。

## 語言

* **[!UICONTROL 偏好語言]**：決定您要用於介面的語言。

## 密碼

* **[!UICONTROL 目前密碼]**：輸入您目前密碼的密碼。
* **[!UICONTROL 新密碼]**：輸入新的有效密碼。 您的密碼必須符合下列要求：
   * 長度必須介於8到25個字元之間。
   * 至少包含一個小寫字母。
   * 至少包含一個大寫字母。
   * 至少包含一個數字。
   * 至少包含下列其中一個特殊字元： `# $ &: _ : { }`
* **[!UICONTROL 重新輸入密碼]**：重新輸入新密碼以確認您輸入正確。
* **[!UICONTROL 密碼過期]**：決定您的密碼在72天後是否作為安全性措施到期。 如果您選取「是」，系統會要求您在72天後建立密碼。
