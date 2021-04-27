---
title: 個人設定
description: 所有使用者都可以變更Dynamic Media經典的個人設定畫面設定。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media經典
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# 個人設定 {#personal-setup}

所有使用者皆可在「個人設定」畫面上變更設定。若要開啟「個人設定」畫面，請按一下「設定 > 個人設定」。

>[!NOTE]
>
>「個人設定」螢幕列出了您在Dynamic Media經典中所擔任的用戶角色：公司管理員、管理員或使用者。

「個人設定」設定可控制瀏覽面板的預設行為、接收電子郵件的方式，以及密碼設定。變更這些設定後，請記得按一下「儲存」。

## 我的帳戶資訊

識別您的帳戶名稱、姓名、使用者名稱 (電子郵件地址)，以及指定的使用者角色。

## 桌上型電腦

* **清除影像快取** -從電腦中刪除所有AdobeDynamic Media快取的影像檔案。
* **清除資產快取** -從您的電腦中刪除所有AdobeDynamic Media快取資產檔案。

除了使用案頭應用程式清除影像和資產快取外，您也可以直接從檔案系統手動清除快取。 根據您的作業系統，導覽至下列：

* macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**要安裝AdobeDynamic MediaCreative Suite擴展：**

1. 在「Dynamic Media經典」工具列上，按一下「Creative Suite分機號」下的「設定」**[!UICONTROL 「設定」]**>>>「個人設定」]**，按一下「立即下載」`s7csxs.zxp`檔案。**[!UICONTROL ****
1. 按一下&#x200B;**[!UICONTROL 安裝]**&#x200B;和&#x200B;**[!UICONTROL 系統要求]**&#x200B;連結，以瞭解有關擴展的其他資訊。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## 瀏覽器

* **縮圖大小** -決定「瀏覽面板」中「格線」檢視中縮圖影像的預設大小。
* **預設資產庫檢視** -決定建立集的資產庫中的資產是以縮圖或名稱顯示。如果您正在處理「資產庫」中的大量資產，則可依名稱來檢視資產。例如，如果您使用許多 PDF 檔案建置大型 eCatalog，便可以依照名稱來檢視資產，使清單較為簡短。
* **預設瀏覽排序順序** -決定資產在「瀏覽面板」中預設顯示的順序。在選單上選擇排序條件，以及是否採用遞增或遞減排序。
* **預設瀏覽位置** -可讓您將瀏覽位置設定為預設位置、上次瀏覽的資料夾或您瀏覽和標識的特定位置。您也可以設定瀏覽位置，將檔案和檔案夾按遞增或遞減排序。
* **預設瀏覽視圖** -確定在首次開啟「瀏覽」面板時，網格視圖或清單視圖是預設視圖。
* **啟動顯示畫面顯示** -判斷您是否看到任何啟動顯示畫面，包括歡迎啟動顯示畫面。
* **顯示工具提示** -決定當您將指標移至按鈕、選單和導覽連結上時，是否顯示工具提示。工具提示說明螢幕上的使用者介面項目。
* **棋盤背景** -在影像後面顯示棋盤圖層，讓您輕鬆查看具有Alpha色版的影像的透明區域。
* **顯示檔案大小** -在瀏覽時顯示資產的檔案大小。
* **將UDF包含在搜尋中** -若要改善您執行之大部分中繼資料搜尋的系統效能，請取消選取（預設）。

   如果納入使用者定義的欄位有助於您執行中繼資料搜尋，您可以選取此選項而加以開啟。或者，您可以使用「進階搜尋」來進行比納入使用者定義的欄位更為直接而快速的搜尋。

   請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

   另請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。

* **基本搜尋類型** -您可以從兩個選項中選擇： **[!UICONTROL 容]** 器會搜尋完整字串中的指定值； **[!UICONTROL StartsWith]** 從字串開頭搜尋，並傳回結果的速度比「包 **[!UICONTROL 含」快]**。任一選項都會覆寫管理員在&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 應用程式一般設定]**&#x200B;中設定的預設值。
* **顯示命令反饋** -選擇以開啟伺服器的命令請求顯示；取消選擇以關閉。
* **導出時顯示對話框** -選擇該選項可在導出時顯示彈出對話框。如果您取消選取（關閉）此選項，您仍可以前往「工作」頁面來擷取匯出結果。

## 電子郵件

* **電子郵件選項** -選擇您要如何讓Dynamic Media經典網站在上傳和發佈工作完成時以電子郵件通知您。只有在出現警告或錯誤時才會收到工作完成通知。
* **電子郵件範圍** -確定您是否收到公司的所有工作電子郵件，還是只收到有關您啟動的上載和發佈工作的電子郵件。
* **電子郵件類型** -決定上傳工作和發佈工作完成時是否會通知您。

## 語言

* **首選語言** -確定要用於介面的語言。

## 密碼

* **當前密碼** -輸入您當前密碼的密碼。
* **新密碼** -輸入新的有效密碼。您的密碼必須符合下列要求：
   * 長度介於8-25個字元之間。
   * 至少包含一個小寫字母。
   * 至少包含一個大寫字母。
   * 至少包含一個數字。
   * 至少包含下列其中一個特殊字元：`# $ & - _ : { }`
* **重新鍵入密碼** -重新輸入新密碼以確認您輸入的密碼正確。
* **密碼過期** -以安全性措施判斷密碼在72天後是否過期。如果您選取「是」，則系統會要求您在 72 天後建立密碼。
