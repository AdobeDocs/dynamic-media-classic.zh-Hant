---
title: 個人設定
description: 所有使用者都可以變更Dynamic Media Classic「個人設定」畫面上的設定。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# 個人設定 {#personal-setup}

所有使用者皆可在「個人設定」畫面上變更設定。若要開啟「個人設定」畫面，請按一下「設定 > 個人設定」。

>[!NOTE]
>
>「個人設定」畫面會列出您在Dynamic Media Classic中的使用者角色：公司管理員、管理員或使用者。

「個人設定」設定可控制瀏覽面板的預設行為、接收電子郵件的方式，以及密碼設定。變更這些設定後，請記得按一下「儲存」。

## 我的帳戶資訊

識別您的帳戶名稱、姓名、使用者名稱 (電子郵件地址)，以及指定的使用者角色。

## 桌上型電腦

* **清除影像快取**  — 從您的電腦中移除所有AdobeDynamic Media快取的影像檔案。
* **清除資產快取**  — 移除電腦中快取資產檔案的所有AdobeDynamic Media。

除了使用案頭應用程式清除影像和資產快取外，您也可以直接從檔案系統手動清除快取。 根據您的作業系統，導覽至下列項目：

* macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**若要安裝AdobeDynamic MediaCreative Suite擴充功能：**

1. 在Dynamic Media Classic中，在工具列上，按一下&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**，在「Creative Suite副檔名」下，按一下&#x200B;**[!UICONTROL Download Now]**&#x200B;以下載`s7csxs.zxp`檔案。
1. 按一下&#x200B;**[!UICONTROL Installation]**&#x200B;和&#x200B;**[!UICONTROL System Requirements]**&#x200B;連結，以了解有關該擴展的其他資訊。

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

* **縮圖大小**  — 決定「瀏覽」面板中「網格」視圖中縮圖影像的預設大小。
* **預設資產庫檢視**  — 決定組建集的資產庫中的資產是否顯示為縮圖或依名稱。如果您正在處理「資產庫」中的大量資產，則可依名稱來檢視資產。例如，如果您使用許多 PDF 檔案建置大型 eCatalog，便可以依照名稱來檢視資產，使清單較為簡短。
* **預設的瀏覽排序順序**  — 決定資產在「瀏覽」面板中預設顯示的順序。在選單上選擇排序條件，以及是否採用遞增或遞減排序。
* **預設瀏覽位置**  — 可讓您將瀏覽位置設定為預設、上次瀏覽的資料夾，或設定為您導覽至並識別的特定位置。您也可以設定瀏覽位置，將檔案和檔案夾按遞增或遞減排序。
* **預設瀏覽視圖**  — 確定首次開啟「瀏覽」面板時看到的預設視圖是網格視圖還是清單視圖。
* **閃屏顯示**  — 確定您是否看到任何閃屏，包括歡迎閃屏。
* **顯示工具提示**  — 確定將指針移到按鈕、菜單和導航連結上時是否顯示工具提示。工具提示說明螢幕上的使用者介面項目。
* **棋盤背景**  — 在影像後面顯示棋盤圖層，讓您輕鬆查看具有Alpha通道的影像的透明區域。
* **顯示檔案大小**  — 在瀏覽時顯示資產的檔案大小。
* **在搜尋中包含UDF**  — 若要改善您執行之大部分中繼資料搜尋的系統效能，請取消選取（預設）。

   如果納入使用者定義的欄位有助於您執行中繼資料搜尋，您可以選取此選項而加以開啟。或者，您可以使用「進階搜尋」來進行比納入使用者定義的欄位更為直接而快速的搜尋。

   請參閱[實施進階搜尋](searching-assets.md#conducting_an_advanced_search)。

   另請參閱[使用者定義的欄位](application-setup.md#user_defined_fields)。

* **基本搜尋類型**  — 您可以從兩個選項中選取： **** 容器會搜尋指定值的完整字串； **** StartsWithsearches從字串的開頭開始搜尋，並傳回結果的速度比「包 **[!UICONTROL 含」]**&#x200B;快。其中一個選項將覆蓋管理員在&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]**&#x200B;中設定的預設值。
* **顯示命令反饋**  — 選擇此選項可開啟對伺服器的命令請求的顯示；取消選擇以關閉。
* **導出時顯示對話框**  — 選擇該選項可在導出時顯示彈出對話框。如果取消選擇（關閉）此選項，您仍可以轉至「作業」頁以檢索導出結果。

## 電子郵件

* **電子郵件選項**  — 選擇您希望Dynamic Media Classic在上傳和發佈作業完成時，透過電子郵件通知您的方式。只有在出現警告或錯誤時才會收到工作完成通知。
* **電子郵件範圍**  — 決定您是否收到公司的所有工作電子郵件，或是只收到您起始的上傳和發佈工作的電子郵件。
* **電子郵件類型**  — 決定上傳作業和發佈作業完成時是否收到通知。

## 語言

* **偏好語言**  — 決定您要用於介面的語言。

## 密碼

* **當前密碼**  — 輸入您當前密碼的密碼。
* **新密碼**  — 輸入新的有效密碼。您的密碼必須符合下列要求：
   * 長度介於8到25個字元之間。
   * 至少包含一個小寫字母。
   * 至少包含一個大寫字母。
   * 至少包含一個數字。
   * 至少包含下列其中一個特殊字元：`# $ & - _ : { }`
* **重新鍵入密碼**  — 重新輸入新密碼以確認輸入正確。
* **密碼過期**  — 以安全措施的形式，決定您的密碼在72天後過期。如果您選取「是」，則系統會要求您在 72 天後建立密碼。
