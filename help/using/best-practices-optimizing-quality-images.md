---
title: 影像品質最佳化准則
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
autotag-review: '2026-05-13T17:39:42.316Z'
TQID: 'https://experienceleague.adobe.com/kw-spdqv6ArVEWk8ID4mnQjYrS25RZntKOJ7-tESasY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: bbfeefce82fc757d71e5ad0038120752eb0683c1
workflow-type: tm+mt
source-wordcount: 1589
ht-degree: 27%

---

# 影像品質最佳化准則{#best-practices-for-optimizing-the-quality-of-your-images}

最佳化影像品質非常耗時。 呈現可接受結果的因素有很多。 結果有點主觀，因為每個人對影像品質的認定不同。 結構化的實驗是必要的。

Adobe Dynamic Media Classic包括用於調整和最佳化影像和演算結果的100多個影像伺服命令。 以下準則幫助您運用部分基本命令和最佳實踐來加速程序並快速達到滿意的結果。

另請參閱[智慧型影像處理](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-65/content/assets/dynamic/imaging-faq)。

>[!TIP]
>
>嘗試使用Dynamic Media [_快照_](https://snapshot.scene7.com/)，探索Dynamic Media影像修飾元和智慧型影像的優點。
>
> Snapshot是視覺化展示工具，旨在說明Dynamic Media最佳化及動態影像傳送的功能。 嘗試使用測試影像或Dynamic Media URL，以視覺化方式觀察各種Dynamic Media影像修飾元的輸出，以及針對下列專案的智慧型影像最佳化：
>
>* 檔案大小（含WebP和AVIF傳送）
>* 網路頻寬
>* DPR （裝置畫素比率）
>
>若要瞭解如何使用快照，請觀看[快照訓練影片](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) （3分17秒）。


## 影像格式的最佳實踐 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 要讓影像呈現良好品質並具有可管理的大小和寬度，JPG 或 PNG 是最佳選擇。
* 如果URL中未提供格式命令，則「動態媒體影像伺服」預設為JPG以進行傳送。
* JPG 以 10:1 的比例壓縮，通常會產生較小的檔案。 PNG以大約2:1的比例壓縮，除非影像包含透明背景。 PNG檔案通常比JPG檔案大。
* JPG 使用失真壓縮，意思就是在壓縮時會捨棄一些圖形元素 (像素)。 PNG 另一方面會使用無失真壓縮。
* JPG 壓縮的相片影像通常比合成影像有更好的真實度，因為具有銳利的邊緣和對比。
* 如果您的影像具有透明度，請使用 PNG，因為 JPG 不支援透明度。

作為影像格式的最佳作法，請從最常見的設定`&fmt=JPG`開始。

## 影像大小的最佳實踐 {#best-practices-for-image-size}

動態縮減影像大小是Dynamic Media影像伺服最常執行的工作之一。 它牽涉到指定大小，以及選擇性指定使用哪一個縮減取樣模式來縮減影像。

* 若要調整影像大小，請使用`&wid=<value>`和`&hei=<value>`。 這些引數會根據外觀比例自動設定影像寬度。
* `&resMode=<value>`控制縮減取樣所使用的演演算法。 從`&resMode=sharp2`開始。 此值可提供最好的影像品質。 使用縮減取樣值`bilin`的速度較快，但通常會導致鋸齒狀不自然感。

如需調整影像大小的最佳作法，請使用`&wid=<value>&hei=<value>&resMode=sharp2`。`&hei=<value>&resMode=sharp2`

## 影像銳利化的最佳實踐 {#best-practices-for-image-sharpening}

影像銳利化是控制網站上影像的最複雜方面，也會發生許多錯誤。 若要進一步瞭解銳利化和不銳利化遮色片在Adobe Dynamic Media Classic中的運作方式，請參閱下列實用資源：

PDF中的最佳做法白皮書，稱為[在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/using/assets/s7_sharpening_images.pdf)。

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

在Adobe Dynamic Media Classic中，您可以在擷取、傳送或兩者同時進行期間銳利化影像。 不過，通常您會使用一種方法來銳利化影像，但不會同時使用兩者。 透過URL傳送影像時銳利化通常能提供最佳結果。

您可以使用兩種影像銳利化方法：

* 簡單銳利化( `&op_sharpen`)：類似於Adobe Photoshop中使用的銳利化濾鏡，簡單銳利化會在動態調整大小後，將基本銳利化套用至影像的最終檢視。 不過，使用者無法設定這個方法。 除非必要，否則最佳實務是避免使用`&op_sharpen`。
* 遮色片銳利化(`&op_USM`)：遮色片銳利化是業界標準的銳利化濾鏡。 最佳實踐就是遵守以下準則並利用遮色片銳利化調整將影像銳利化。 遮色片銳利化調整可讓您控制以下三個參數:

  * `&op_sharpen=amount,radius,threshold`

    * `amount` （0-5，效果強度。）
    * `radius` (0-250，在銳利化物件周圍繪製的「銳利化線條」寬度（以畫素為單位）。

      請注意，引數`radius`和`amount`具有反向關係。 減少`radius`可以透過增加`amount`來補償。 `Radius`允許更細微的控制，因為較低的值只會銳利化邊緣畫素，而較高的值會銳利化較寬的畫素範圍。

    * `threshold` （0-255，效果敏感度。）

      這個參數決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素，濾鏡才會予以銳利化。 臨界值利用相似顏色 (如皮膚色調) 避免區域過度銳利化。 例如，閾值為12會忽略膚色亮度的微小變化，以避免加上「雜訊」，同時仍會加上邊緣對比度至高對比區域，例如睫毛與皮膚相遇的區域。

      如需如何設定這三個引數的詳細資訊，包括搭配濾鏡使用的最佳實務，請參閱[在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/using/assets/s7_sharpening_images.pdf)。

    * Adobe Dynamic Media Classic也可讓您控制第四個引數：單色( `0,1`)。 此引數決定使用值`0`將遮色片銳利化調整分別套用至每個色彩元件，或使用值`1`套用至影像亮度/強度。

最佳實踐就是從遮色片銳利化調整的 radius 參數著手。 您可以從以下的 radius 設定開始:

* 網站: 0.2-0.3 像素
* 相片列印 (250-300 ppi): 0.3-0.5 像素
* 偏移列印 (266-300 ppi): 0.7-1.0 像素
* 畫布列印 (150 ppi): 1.5-2.0 像素

將 amount 從 1.75 逐漸增加至 4。 如果銳利化仍不是想要的結果，請以小數增量增加半徑，然後再次將數量從1.75設定為4。 視需要重複執行

保留 monochrome 參數的設定值 0。

## JPEG壓縮的最佳作法(`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* 這個參數控制 JPG 編碼品質。 值愈大表示影像品質愈好，但檔案較大；相反地，值愈小表示影像品質愈差，但檔案較小。 此參數的範圍是 0-100。
* 若要將品質最佳化，請勿將此參數值設為 100。 設定90或95與100之間的差異幾乎無法察覺。 然而100會不必要地增加影像檔案的大小。 因此，若要最佳化品質但避免影像檔案變得太大，請將`qlt=`值設為90或95。
* 若要針對較小的影像檔案大小進行最佳化，但將影像品質維持在可接受的等級，請將`qlt=`值設定為80。 值低於70到75會造成顯著的影像品質降低。
* 若要停留在中間，請將`qlt=`值設定為85作為最佳實務。
* 使用色度旗標`qlt=`

  * `qlt=`引數有第二個設定，可讓您使用一般值`,0` （預設）開啟RGB色度縮減取樣，或使用值`,1`將其關閉。
  * 從關閉RGB色度縮減取樣開始( `,1`)。 此設定通常會得到較好的影像品質，特別是包含許多銳利邊緣和對比的合成影像。

JPG壓縮的最佳作法是使用`&qlt=85,0`。

## JPEG 大小調整的最佳實踐 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果您想要保證影像不會超過特定大小，引數`jpegSize`就相當實用。 此引數用於傳遞至記憶體有限的裝置。

* 此引數設定為KB ( `jpegSize=<size_in_kilobytes>`)。 它可定義影像傳送所允許的大小上限。
* `&jpegSize=`與JPG壓縮引數`&qlt=`互動。 如果具有指定JPG壓縮引數( `&qlt=`)的JPG回應未超過`jpegSize`值，則影像會依定義傳回`&qlt=`。 否則，`&qlt=`會逐漸減少，直到影像符合最大允許大小為止。 或者，如果系統無法符合影像，則會傳回錯誤。

最佳實務是，當您傳送JPG影像至記憶體有限的裝置時，請設定`&jpegSize=`並包含引數`&qlt=`。

## 最佳實踐摘要 {#best-practices-summary}

為了達到高影像品質和小檔案大小，最佳實務建議從下列參陣列合開始：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

在大多數情況下，這種設定組合會產生卓越的結果。

如果影像需要進一步最佳化，請從半徑設定為0.2或0.3開始，逐步微調銳利化（不銳利化遮色片）引數。 然後，逐漸將數量從1.75增加到最大值4 （等於[!DNL Adobe Photoshop]中的400%）。 查看是否得到想要的結果。

如果仍不滿意銳利化的結果，以小數遞增 radius。 對於每增加一個小數，請將數量重設為1.75，並逐漸增加到4。 重複這個程序，直到得到想要的結果為止。 雖然上述值是Creative Studio已驗證的方法，但請注意，您可以使用其他值並遵循其他程式。 結果是否令您滿意是主觀問題；因此，需要進行結構化的實驗。

實驗時，以下一般建議有助於最佳化您的工作流程：

* 直接在URL上或使用[!DNL Adobe Dynamic Media Classic]影像調整工具即時測試不同的引數。 後者提供調整作業的即時預覽。
* 如需參考最佳做法，請記得您可以將「動態媒體影像伺服」命令群組至影像預設集。 影像預設集是一組具有自訂預設集名稱（例如`$thumb_low$`和`$product_high$`）的URL命令巨集。 URL路徑中的自訂預設集名稱會呼叫這些預設集。 這類功能可協助您管理網站上不同影像使用模式的命令和品質設定，以及縮短 URL 的整體長度。
* Adobe Dynamic Media Classic也提供更進階的方式來調整影像品質，例如在擷取時套用影像銳利化。 對於可選擇進一步調整和最佳化演算結果的進階使用案例，Adobe Professional Services可協助您進行自訂insight和最佳實務。
