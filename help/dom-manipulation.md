---
title: DOM 操作
seo-title: DOM 操作
description: 'null'
seo-description: 瞭解DOM控制。
uuid: 275cd49d-2a55-41f9-80b0-e147 d0 cd2907
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/category/範本發佈
discoiquuid: 890ca93e-3146-4347-864b-bd5 e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM 操作{#dom-manipulation}

DOM (文件物件模型) 操作是一種透過直接控制設計檔案的 XML 代碼來編輯設計檔案的方法。DOM 操作可使您更佳控制變數設計元素 (包括變更其內容和外觀)；您甚至可以根據需要建立新元素。

Dynamic Media Classic可讓您在發佈範本後，透過URL命令操作Dynamic Media Classic FXG範本的DOM。FXG 範本中的設計元素是透過 URL 傳遞命令來進行處理。這樣您就可以動態處理屬性以及對圖形增加屬性。

若要使用DOM控制，您可以建立s7：您可以在Illustrator檔案中使用Elementis，然後將它轉換為Dynamic Media Classic FXG檔案並將它上傳至SPS。

>[!NOTE]
>
>使用 DOM 操作命令時，所有傳入值都必須進行 URL 編碼。

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## 在 Illustrator 檔案中建立 s7:elementID {#creating-s-elementids-in-illustrator-files}

若要在 Illustrator 中建立的設計中使用 DOM 操作，請在您的 Illustrator 設計中建立 s7:elementID。建立 s7:elementID 可以在範本發佈之後使用 URL 命令來修改設計元素。

### 為文字 DOM 操作建立 s7:elementID {#creating-s-elementids-for-dom-manipulation-of-text}

若要為文字物件的 DOM 操作建立一個 s7:elementID，請在 Illustrator 中開啟「圖層」面板。然後，在包含變數文字的文字圖層上，使用 s7:elementID 命名該圖層。To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. 以下是 s7:elementID 文字圖層名稱的範例:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### 為物件 DOM 操作建立 s7:elementID {#creating-s-elementids-for-dom-manipulation-of-objects}

如果您希望終端使用者能夠變更物件的屬性，請為物件建立 s7:elementID。物件可以構成整個文字框、圖形和影像。彩色背景是物件元素 ID 的一個範例。當季節改變時，終端使用者可以變換海報的背景色彩，使海報順應季節。

在 Illustrator 中為某個物件建立 s7:element ID 之前，請先為該物件建立一個單獨的圖層。

在 Illustrator 中按照以下步驟為物件建立 s7:elementID:

1. 選取物件。
1. 按一下 **「視窗** &gt; **圖層**」。
1. 在「圖層」面板中，將物件圖層命名為s7：OpenEnd.To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. 以下是 s7:elementID 物件圖層名稱的範例:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## 發佈 FXG 範本 {#publish-fxg-templates}

發佈您的FXG範本會將它放置在動態媒體Classic伺服器上，可供您的網站和應用程式使用。在發佈過程期間，Scene7 Publishing System 會啟用您的網站或應用程式所需的 URL。

>[!NOTE]
>
>若要使用 FXG 範本，請發佈其所含的所有內容，包括字型和影像。如果未包括所有必要檔案，則在發佈時會出現錯誤訊息。

### 將 FXG 範本標記為發佈 {#mark-fxg-templates-for-publish}

範本及其所有支援檔案必須標示為發佈，以便放置在動態媒體影像伺服器上。

1. 在瀏覽面板中，選取 FXG 範本以及所用的所有圖形、影像和字型。
1. 按一下 **「標記為發佈**」。

### 發佈 FXG 範本 {#publish-your-fxg-template}

1. 在「全域導覽」列上按一下「**發佈**」。
1. 選取「時間」選項，並選擇性輸入發佈工作的名稱。
1. Click **Start Publish**.

### 文字溢出指示器顯示 {#text-overflow-indicator-display}

當文字超出在文字框內為其分配的空間 (或者，如果是串連的文字，則為在最後一個文字框中分配的空間) 時，會顯示&#x200B;*文字溢出指示器*。該指示器是一個內含加號的紅色方塊。SPS 上的文字溢出指示器始終處於啟用狀態。

文字溢出指示器透過 `markOverflowingTextFrame` 修飾元進行控制。如下所示使用該修飾元:

| 修飾元/值 | 說明 |
|--- |--- |
| markOverlowingTextFrame=0,1 | 值為 1 時表示顯示文字流量指示器。預設為 0。(雖然預設為 0，但是 SPS 中的文字溢出指示器始終處於啟用狀態。) 請注意 markOverflowingTextFrame 修飾元區分大小寫。 |

>[!MORELIKETHIS]
>
>* [定義可變性: 參數化與 DOM 操作](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publishing](publishing-files.md#publishing_files)

