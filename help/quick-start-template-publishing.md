---
title: 「快速入門：範本發佈」
seo-title: 「快速入門：範本發佈」
description: 'null'
seo-description: 簡介和快速入門範本發佈，協助您快速上手使用。
uuid: 101b6211-2421-4565-8635-944315a5c512
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/category/範本發佈
discoiquuid: 03671fc1-ce3 b-4fe-ad1 f-53c99 abcaberde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web-to-Print可讓您建立具專業水準的平面內容，讓客戶、客戶和員工輕鬆自訂及個人化。您可以在整個發佈程序中保有公司內容和品牌身分。終端使用者可以自訂列印內容 — 但僅限您允許其自訂的部分內容。個人化文具、名片、海報、賀卡、標籤、支票、禮品、服裝、日曆、剪貼簿和相簿等，都是您可以提供的自訂列印產品範例。公司可以在標記中保有通用品牌身分，他們可以自訂標記，用於不同地區、經銷權、商店和分公司。

您可以從Adobe Illustrator中設計範本開始。在此範本中，詳細定義了常數和變數 (變數元件是可以自訂的組件)。例如，在對 Illustrator 檔案中的文字進行參數化之後，終端使用者可以輸入自己的文字。同樣，在將背景色彩參數化為一個變數組件之後，可以變換不同的背景色彩。

Dynamic Media Classic提供兩個範本發佈工作流程，一個用於基本使用案例，一個用於進階使用案例。基本使用案例包括在Adobe Illustrator中建立設計、上傳至Dynamic Media Classic，以及使用SPS中的參數定義變數元素。進階使用案例需要更加全面地定義可變性。進階使用案例會在Adobe Illustrator中建立變數元素，將檔案上傳至Dynamic Media Classic，並使用URL呼叫直接在XML層級控制這些元素。呼叫此藍本 *`*DOM manipulation*`*。

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . 將Zip檔案下載至本機硬碟並擷取其內容(Dynamic Media Classic-To-PrintPublishFlow Tutorial文件和教學課程資產)。

**快速入門**

本快速入門描述使用 Illustrator 檔案建立高品質、可自訂之列印產品的基本工作流程。

**1. 設計用於範本發佈的 Illustrator 檔案**

在 Illustrator 中設計您的範本。如果您要使用進階 DOM 操作方式自訂範本，請在 Illustrator 中定義變數元素的 s7:elementID。

請參閱[在 Illustrator 中建立初始範本](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)和 [DOM 操作](dom-manipulation.md#dom_manipulation)。

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud 使用者可以使用網路印刷的 Adobe Illustrator 外掛程式。此外掛程式可將範本轉換為Dynamic Media Classic FXG。如果範本包含字型，則在上載 FXG 檔案之前必須先將對應的字型檔案上載到 Scene7 Publishing System。

請參閱[上載用於範本發佈的檔案](upload-files-template-publishing.md#upload_files_for_template_publishing)。

**3. 在Dynamic Media Classic中檢視、定義或調整參數**

在「範本發佈預覽」和「範本發佈建置」畫面中，您可以透過參數定義和優化變數元素，預覽結果以及對結果進行測試。在這些畫面中，您可以執行以下操作:

* 建立和修改參數。
* 為參數特性和屬性指定預設值。
* 按一下「複製 URL」，將預覽 URL 複製到剪貼簿，並在瀏覽器視窗中預覽結果。

請參閱 [「動態媒體Classic中的參數化範本](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)」。

**4. 發佈 FXG 範本**

在您完成參數和屬性的定義和測試之後，發佈該檔案。發佈您的FXG範本會將它置於動態媒體影像伺服器，並啓動URL。

請務必發佈與 FXG 範本關聯的所有影像和字型。

請參閱[發佈 FXG 範本](dom-manipulation.md#publish_fxg_templates)。

**5. 取得 URL**

現在，範本可以透過其 URL 內嵌到您的網站中，以供終端使用者建立個人化的變數內容。

請參閱[將 FXG 範本連結到網頁](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page)。
