---
title: 在Dynamic Media Classic中參數化範本
seo-title: 在Dynamic Media Classic中參數化範本
description: 'null'
seo-description: 瞭解如何在Dynamic Media Classic中參數化範本
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: 管理員
content-type: 參考
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTENDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 在Dynamic Media Classic中參數化範本{#parameterizing-a-template-in-scene}

將儲存為Dynamic Media Classic FXG的Illustrator範本上傳至Scene7 Publishing system後，您可以定義其變數元素。 透過在「範本發佈建置」和「範本發佈預覽」畫面中參數化變數元素來執行此操作。Dynamic Media Classic提供工具，可定義圖層上的文字和物件參數，以及它們各自的屬性。 您還可以建立範本的不同版本。

參數化 FXG 範本後，即可在範本中自訂文字、影像和圖形的可變性。例如，您可以參數化一行文字，以便終端使用者可以透過 Web 使用者介面修改該文字。您可以將空文字欄位定義為變數，以便終端使用者可以在這些欄位中填入個人化文字。您也可以在「動態媒體傳統範本發佈建置」畫面中，將設計元素的屬性和屬性參數化。

>[!NOTE]
>
>如果您打算使用DOM控制，則不需要在Dynamic Media Classic中參數化範本。

## 定義 FXG 範本中的參數 {#defining-parameters-in-fxg-templates}

請依照Dynamic Media Classic中的下列步驟，為FXG範本定義參數：

1. 在「瀏覽」視窗中，選取 FXG 檔案。
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   此時會開啟「範本發佈」畫面。

1. 選取LRCo\FXG\Welcome_Summit_10 （FXG檔案），然後按一下「建 **立** &gt;范 **本發佈」**。</p>

   ![](assets/wp_fxg_edit.png)

1. 在「範本發佈」畫面的「圖層」面板中，選取包含要參數化之元素的圖層。

   >[!NOTE]
   >
   >連續按眼睛圖示，確保您選取了正確的物件。

1. 在「屬性」面板中，按一下「名稱」欄 (用於參數化文字) 或「參數」欄 (用於參數化物件) 中的參數。

   * **在文**&#x200B;字欄位中按一下文字（捲動至「屬性」清單的底部以尋找文字）。 此時會出現「參數」對話框。Select the text that you want to parameterize and click **Add**. 您可以透過選取該文字的不同部分並為每個部分增加參數，從同一文字屬性建立多個參數。To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **對象**&#x200B;按一下「參數」(Parameter)列中的框。 此時會出現「編輯參數」對話框。Enter a name and click **OK**.
   若要使用相同值一次自訂多個屬性，請對每個屬性使用相同的參數名稱。例如，如果您的範本包含一個矩形和一個星形，您可以鍵入 `newcolor` 作為每項「純色」色彩屬性的參數名稱。每當您變更 `newcolor` 值時，矩形和星形就會變為新的色彩。

1. 在「值」或「資料」欄位中指定該屬性的預設值。設定所選物件的所有屬性，以指定所需的外觀。
1. (選擇性) 對要參數化的所有物件或圖層重複步驟 3 - 5。
1. 按一下「**儲存**」或「**另存新檔**」。
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## 在 FXG 範本中顯示或隱藏物件或圖層 {#show-or-hide-an-object-or-layer-in-the-fxg-template}

隱藏的物件和圖層不會顯示在預覽或輸出中，但並非已從檔案中刪除。您可以根據需要使其再次可見。可見性是一種可以成為變數的屬性。連續按眼睛圖示會為物件或圖層的可見性設定預設值。

1. 在「物件」面板中，按一下物件或圖層名稱旁邊的眼睛圖示，以將其隱藏在檔案中。
1. 再按一下，使該物件可見。

## 建立範本的不同版本 {#create-different-versions-of-a-template}

您可以編輯屬性以針對不同用途建立範本的不同版本。

在「範本發佈」畫面中，按一下「另存新檔」將該檔案儲存為新的 FXG 範本，而不覆寫原始 FXG 範本。

## 使用描邊文字 {#using-stroked-text}

描邊文字就是如何對屬性進行參數化的一個範例。Dynamic Media Classic支援下列筆畫文字功能：

* 描邊寬度
* 虛線描邊圖樣
* 不同連接樣式
* 不同端點樣式
* 描邊疊印
* 單獨對描邊進行色彩處理，包括特別色支援

下面表格描述支援描邊文字的屬性。

| 屬性 | 說明 |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | 指定是否為文字啟用填充。預設為 true。 |
| s7:stroke `<Boolean>` (S7FXG Only) | 指定是否為文字啟用描邊。預設為 false。 |
| s7:weight `<number>` (S7FXG Only) | 以點為單位指定文字的描邊粗細。預設為 1 點。 |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | 指定描邊的連接類型。預設為 round。 |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | 指定描邊的端類型。預設為 round。 |
| s7:miterLimit `<number>` (S7FXG Only) | 指定當連接為描邊尖角連接時的尖角限制。預設為 4。 |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | 指定是否為描邊啟用疊印。預設為 false。 |
| s7:strokeColorName (僅限 S7FXG) | 與 s7:colorName 相同，但是它定義描邊的色彩名稱。 |
| s7:strokeColorValue (僅限 S7FXG) | 與 s7:colorValue 相同，但是它定義描邊所用的色彩值。 |
| s7:strokeColorspace (僅限 S7FXG) | 與 s7:colorspace 相同，但是它定義描邊的色域。 |
| flm:dashPattern `<array>` (S7FXG Only) | 根據預設，沒有虛線和間隙圖樣。該屬性定義描邊的虛線/間隙圖樣。第一個值是描邊的虛線。第二個值是虛線之間的間隙。您可使用虛線和間隙的指定替代值，以同樣的方式來延伸多個值的陣列。 |

## 使用彎曲文字 {#using-warped-text}

彎曲文字可讓您使用波浪、旗幟、延伸等效果來修改文字外觀。

彎曲文字支援 RTF 物件。文字可以垂直或水平呈現，也可以是點文字、區域文字與路徑文字。必須先選取整個文字物件，才能套用彎曲文字。

您可以在 Adobe Illustrator 中建立彎曲文字。

使用彎曲文字時，您可以設定下列屬性:

* 樣式
* 方向
* 彎曲
* 水平扭曲
* 垂直扭曲

每個屬性都包含一組值。

| 屬性 | 值 | 預設 |
|--- |--- |--- |
| Styles7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | 無 |
| Directions7:warpDirection | horizontalvertical | 水平 |
| Bends7:warpBend | -1 至 1 | 0.5 |
| 水準扭曲7:warpHorizontalDistration | -1 至 1 | 0 |
| 垂直扭曲7:warpVerticalDistration | -1 至 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

如需更多有關建立與使用彎曲文字的資訊，請參閱Adobe Illustrator 文件。

>[!MORELIKETHIS]
>
>* [在 Illustrator 中建立初始範本](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Upload files for Template Publishing](upload-files-template-publishing.md#upload_files_for_template-publishing)

