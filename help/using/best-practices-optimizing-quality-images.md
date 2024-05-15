---
title: 影像品質最佳化的最佳實踐
description: 瞭解影像品質最佳化的最佳實務。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 40%

---

# 影像品質最佳化的最佳實踐{#best-practices-for-optimizing-the-quality-of-your-images}

最佳化影像品質可能會耗費大量時間。 呈現可接受結果的因素有很多。 結果有點主觀，因為每個人對影像品質的認定不同。結構化實驗是關鍵。

Adobe Dynamic Media Classic包括用於調整和最佳化影像和演算結果的100多個影像伺服命令。 以下準則幫助您運用部分基本命令和最佳實踐來加速程序並快速達到滿意的結果。

另請參閱 [智慧型影像](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>嘗試使用Dynamic Media來探索Dynamic Media影像修飾元和智慧型影像處理的優點 [_快照_](https://snapshot.scene7.com/).
>
> Snapshot是視覺化展示工具，旨在說明Dynamic Media在最佳化及動態影像傳送方面的強大功能。 嘗試使用測試影像或Dynamic Media URL，以視覺化方式觀察各種Dynamic Media影像修飾元的輸出，以及針對下列專案的智慧型影像最佳化：
>
>* 檔案大小（含WebP和AVIF傳送）
>* 網路頻寬
>* DPR （裝置畫素比率）
>
>若要瞭解使用Snapshot的簡易性，請播放 [快照訓練影片](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) （3分17秒）。


## 影像格式的最佳實踐 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 要讓影像呈現良好品質並具有可管理的大小和寬度，JPG 或 PNG 是最佳選擇。
* 如果URL中未提供任何格式命令，Dynamic Media影像伺服預設為JPG進行傳送。
* JPG 以 10:1 的比例壓縮，通常會產生較小的檔案。PNG會以大約2:1的比率壓縮，除非有時影像包含空白背景。 大致上 PNG 檔案的大小比 JPG 檔案更大。
* JPG 使用失真壓縮，意思就是在壓縮時會捨棄一些圖形元素 (像素)。PNG 另一方面會使用無失真壓縮。
* JPG 壓縮的相片影像通常比合成影像有更好的真實度，因為具有銳利的邊緣和對比。
* 如果您的影像具有透明度，請使用 PNG，因為 JPG 不支援透明度。

影像格式的最佳作法是從最常見的設定開始 `&fmt=JPG`.

## 影像大小的最佳實踐 {#best-practices-for-image-size}

動態縮減影像大小是Dynamic Media Image Serving最常執行的工作之一。 它牽涉到指定大小，以及選擇性指定使用哪一個縮減取樣模式來縮減影像。

* 調整影像大小的最佳且最直接的方法是使用 `&wid=<value>` 和 `&hei=<value>` 或只是 `&hei=<value>`. 這些參數會根據外觀比例自動設定影像寬度。
* `&resMode=<value>` 控制縮減取樣所使用的演演算法。 開始於 `&resMode=sharp2`. 此值可提供最好的影像品質。使用縮減取樣值時 `=bilin` 速度更快，通常會導致鋸齒狀不自然感。

如需調整影像大小的最佳作法，請使用 `&wid=<value>&hei=<value>&resMode=sharp2` 或 `&hei=<value>&resMode=sharp2`

## 影像銳利化的最佳實踐 {#best-practices-for-image-sharpening}

影像銳利化是在網站上控制影像時最複雜的一環，常會發生許多錯誤。請參考下列實用資源，以花時間進一步瞭解銳利化和遮色片銳利化在Adobe Dynamic Media Classic中的運作方式：

最佳實務白皮書 [在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

有了Adobe Dynamic Media Classic，您可以在內嵌和/或傳送時銳利化影像。 不過，通常您只會使用一種方法或另一種方法來銳利化影像，但不會同時使用兩者。 傳送影像時在 URL 上銳利化影像，通常可以獲得最好的結果。

您可以使用兩種影像銳利化方法：

* 簡單銳利化( `&op_sharpen`) — 類似於Photoshop中使用的銳利化濾鏡，簡單銳利化會在動態調整大小後，將基本銳利化套用至影像的最終檢視。 不過，使用者無法設定這個方法。最佳實務是避免使用 `&op_sharpen` 除非必要。
* 不銳利化遮色片( `&op_USM`) — 不銳利化遮色片是業界標準的銳利化濾鏡。 最佳實踐就是遵守以下準則並利用遮色片銳利化調整將影像銳利化。遮色片銳利化調整可讓您控制以下三個參數: 

   * `&op_sharpen=amount,radius,threshold`

      * `amount` （0-5，效果強度。）
      * `radius` (0-250，在銳利化物件周圍繪製的「銳利化線條」寬度（以畫素為測量單位）。

        請記住，引數 `radius` 和 `amount` 互相抵抗。 減少 `radius` 可以通過增加 `amount`. `Radius` 當值越低，只會銳利化邊緣畫素，而值越高會銳利化較寬的畫素範圍，因此可讓您使用更精細的控制項。

      * `threshold` （0-255，效果敏感度。）

        這個參數決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素，濾鏡才會予以銳利化。臨界值利用相似顏色 (如皮膚色調) 避免區域過度銳利化。例如，閾值為12會忽略膚色亮度的微小變化，以避免加上「雜訊」，同時仍會加上邊緣對比度至高對比區域，例如睫毛與皮膚相遇的區域。

        如需如何設定這三個引數的詳細資訊，包括篩選使用的最佳實務，請參閱 [在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/using/assets/s7_sharpening_images.pdf).

      * Adobe Dynamic Media Classic也可讓您控制第四個引數：單色( `0,1`)。 此引數會決定是否使用值將遮色片銳利化調整分別套用至每個色彩元件 `0` 或使用值調整至影像亮度/強度 `1`.

最佳實踐就是從遮色片銳利化調整的 radius 參數著手。您可以從以下的 radius 設定開始: 

* 網站: 0.2-0.3 像素
* 相片列印 (250-300 ppi): 0.3-0.5 像素
* 偏移列印 (266-300 ppi): 0.7-1.0 像素
* 畫布列印 (150 ppi): 1.5-2.0 像素

將 amount 從 1.75 逐漸增加至 4。如果銳利化仍未產生您想要的樣子，以小數遞增 radius，並再次將 amount 從 1.75 增加至 4。視需要重複執行

保留 monochrome 參數的設定值 0。

## JPEG壓縮的最佳作法(`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* 這個參數控制 JPG 編碼品質。值愈大表示影像品質愈好，但檔案較大；相反地，值愈小表示影像品質愈差，但檔案較小。此參數的範圍是 0-100。
* 若要將品質最佳化，請勿將此參數值設為 100。設定90或95與100之間的差異幾乎無法察覺。 然而100會不必要地增加影像檔案的大小。 因此，若要最佳化品質但避免影像檔案變得太大，請設定 `qlt=` 值為90或95。
* 若要針對較小的影像檔案大小進行最佳化，但將影像品質維持在可接受的等級，請設定 `qlt=` 值為80。 低於 70 至 75 的值會導致影像品質大幅下滑。
* 作為最佳實務，若要保持在中間，請將 `qlt=` 值設為85，則維持在中間。
* 在中使用色度旗標 `qlt=`

   * 此 `qlt=` 引數有第二個設定，可讓您使用一般值開啟RGB色度縮減取樣 `,0` （預設），或使用值將其關閉 `,1`.
   * 為了保持簡單，請從RGB色度縮減取樣關閉( `,1`)。 此設定通常會得到較好的影像品質，特別是包含許多銳利邊緣和對比的合成影像。

使用JPG壓縮作為最佳實務 `&qlt=85,0`.

## JPEG 大小調整的最佳實踐 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

引數 `jpegSize` 如果您想要保證影像不會超過傳送至記憶體有限之裝置的特定大小，這個選項就十分實用。

* 此引數是以KB為單位( `jpegSize=<size_in_kilobytes>`)。 它可定義影像傳送所允許的大小上限。
* `&jpegSize=` 會與JPG壓縮引數互動 `&qlt=`. 如果JPG回應具有指定的JPG壓縮引數( `&qlt=`)不可超過 `jpegSize` 值，則影像會以 `&qlt=` 依定義。 否則， `&qlt=` 會逐漸減少，直到影像符合最大允許大小為止。 或者，直到系統判斷它無法容納並傳回錯誤為止。

最佳實務是，設定 `&jpegSize=` 並新增引數 `&qlt=` 如果您要將JPG影像傳送至記憶體有限的裝置。

## 最佳實踐摘要 {#best-practices-summary}

為了達到高影像品質和小檔案大小，最佳實務建議從下列參陣列合開始：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

在大多數情況下，這種設定組合會產生卓越的結果。

如果影像需要進一步最佳化，可逐漸微調銳利化 (遮色片銳利化調整) 參數，從 radius 設為 0.2 或 0.3 開始。接著，將 amount 從 1.75 逐漸增加至最大值 4 (相當於 Photoshop 中的 400%)。查看是否得到想要的結果。

如果仍不滿意銳利化的結果，以小數遞增 radius。每一次小數增量，amount 就從 1.75 重新開始逐漸增加至 4。重複這個程序，直到得到想要的結果為止。上述值是經過 Creative Studios 驗證的方法，請記住您可以依循其他策略並從其他值開始。您對於結果的滿意度很主觀，因此，結構化實驗是關鍵。

實驗時，以下一般建議有助於最佳化您的工作流程：

* 請直接在URL上或使用Adobe Dynamic Media Classic的影像調整功能，即時試用並測試不同的引數。 後者提供調整作業的即時預覽。
* 如需參考最佳做法，請記得您可以將「Dynamic Media影像伺服」命令群組至影像預設集。 影像預設集基本上是URL指令巨集，其中包含自訂預設集名稱，例如 `$thumb_low$` 和 `&product_high$`. URL路徑中的自訂預設集名稱會呼叫這些預設集。 這類功能可協助您管理網站上不同影像使用模式的命令和品質設定，以及縮短 URL 的整體長度。
* Adobe Dynamic Media Classic也提供更進階的方式來調整影像品質，例如在擷取時套用影像銳利化。 對於可選擇進一步調整和最佳化演算結果的進階使用案例，Adobe Professional Services可協助您提供自訂分析和最佳實務。
