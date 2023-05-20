---
title: 影像品質最佳化的最佳實踐
description: 瞭解優化映像質量的最佳做法。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
source-git-commit: f3082fc6b66cf0903bf6cb1907a8615a12399fdc
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 50%

---

# 影像品質最佳化的最佳實踐{#best-practices-for-optimizing-the-quality-of-your-images}

影像品質最佳化可能非常耗時，因為演算可接受的結果受許多因素影響。結果有點主觀，因為每個人對影像品質的認定不同。結構化實驗是關鍵。

Adobe Dynamic Media Classic公司包括100多個影像服務命令，用於調整和優化影像和渲染結果。 以下準則幫助您運用部分基本命令和最佳實踐來加速程序並快速達到滿意的結果。

另請參閱 [智慧映像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic)。

>[!TIP]
>
>使用Dynamic Media，嘗試並瞭解Dynamic Media映像修改程式和智慧映像的優勢 [_快照_](https://snapshot.scene7.com/)。
>
> Snapshot是一種直觀的演示工具，旨在展示Dynamic Media在優化和動態影像傳輸方面的威力。 對test影像或Dynamic MediaURL進行實驗，以直觀地觀察各種Dynamic Media影像修飾符的輸出，並對以下各項進行智慧成像優化：
>* 檔案大小（使用WebP和AVIF交付）
>* 網路頻寬
>* DPR（設備像素比）
>
>要瞭解使用快照有多容易，請播放 [快照培訓視頻](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot.html?lang=en) （3分17秒）。


## 影像格式的最佳實踐 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 要讓影像呈現良好品質並具有可管理的大小和寬度，JPG 或 PNG 是最佳選擇。
* 如果URL中未提供format命令，則Dynamic Media影像服務預設為傳送JPG。
* JPG 以 10:1 的比例壓縮，通常會產生較小的檔案。PNG壓縮的比率約為2:1，有時影像包含空背景時除外。 大致上 PNG 檔案的大小比 JPG 檔案更大。
* JPG 使用失真壓縮，意思就是在壓縮時會捨棄一些圖形元素 (像素)。PNG 另一方面會使用無失真壓縮。
* JPG 壓縮的相片影像通常比合成影像有更好的真實度，因為具有銳利的邊緣和對比。
* 如果您的影像具有透明度，請使用 PNG，因為 JPG 不支援透明度。

作為影像格式的最佳做法，請從最常見的設定開始 `&fmt=JPG`。

## 影像大小的最佳實踐 {#best-practices-for-image-size}

動態縮小影像大小是Dynamic Media影像服務執行的最常見任務之一。 它牽涉到指定大小，以及選擇性指定使用哪一個縮減取樣模式來縮減影像。

* 對於影像大小調整，最好、最直接的方法是使用 `&wid=<value>` 和 `&hei=<value>` 或者 `&hei=<value>`。 這些參數會根據外觀比例自動設定影像寬度。
* `&resMode=<value>` 控制用於下採樣的算法。 開始於 `&resMode=sharp2`。 此值可提供最好的影像品質。使用縮減採樣值時 `=bilin` 速度更快，通常會導致偽像的混淆。

作為影像調整的最佳做法，請使用 `&wid=<value>&hei=<value>&resMode=sharp2` 或 `&hei=<value>&resMode=sharp2`

## 影像銳利化的最佳實踐 {#best-practices-for-image-sharpening}

影像銳利化是在網站上控制影像時最複雜的一環，常會發生許多錯誤。請花點時間，通過參考以下有用資源，瞭解銳化和反銳化掩碼在Adobe Dynamic Media Classic如何工作的更多資訊：

最佳做法白皮書 [在Adobe Dynamic Media Classic和影像伺服器上銳化影像](/help/assets/s7_sharpening_images.pdf)。

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

有了Adobe Dynamic Media Classic，你可以在攝入、遞送或兩者上銳化影像。 但是，通常只使用一種方法或另一種方法來銳化影像，但不同時使用兩種方法。 傳送影像時在 URL 上銳利化影像，通常可以獲得最好的結果。

可以使用兩種影像銳化方法：

* 簡單銳化( `&op_sharpen`) — 與在Photoshop使用的銳化濾鏡類似，簡單銳化將基本銳化應用於動態調整後影像的最終視圖。 不過，使用者無法設定這個方法。最好的做法是 `&op_sharpen` 除非需要。
* 反銳化掩碼( `&op_USM`) — 反銳化掩碼是用於銳化的行業標準篩選器。 最佳實踐就是遵守以下準則並利用遮色片銳利化調整將影像銳利化。遮色片銳利化調整可讓您控制以下三個參數: 

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5，效果的強度。)
      * `radius` (0-250，在銳利化之物件周圍繪製的「銳利化線條」寬度，其單位為像素。)

         請記住，`radius` 和 `amount` 參數互相消長。減少 `radius` 可以通過增加 `amount`。 `Radius` 可以進行更精細的控制，因為較低的數值只會銳利化在邊緣的像素，而以較高的數值銳利化的像素範圍會比較寬。

      * `threshold` （0-255，效果敏感。）

         這個參數決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素，濾鏡才會予以銳利化。臨界值利用相似顏色 (如皮膚色調) 避免區域過度銳利化。例如，臨界值 12 會忽略皮膚色調亮度的輕微變化，因此不會增加雜訊，同時會增加高反差區域的邊緣對比，例如睫毛和皮膚鄰接之處。

         有關如何設定這三個參數（包括與篩選器一起使用的最佳做法）的詳細資訊，請參見 [在Adobe Dynamic Media Classic和影像伺服器上銳化影像](/help/assets/s7_sharpening_images.pdf)。

      * Adobe Dynamic Media Classic還允許您控制第四個參數：單色(M) `0,1`)。 這個參數決定要將遮色片銳利化調整分別套用至每個色彩元件 (使用值 `0`) 或套用至影像亮度/飽和度 (使用值 `1`)。

最佳實踐就是從遮色片銳利化調整的 radius 參數著手。您可以從以下的 radius 設定開始: 

* 網站: 0.2-0.3 像素
* 相片列印 (250-300 ppi): 0.3-0.5 像素
* 偏移列印 (266-300 ppi): 0.7-1.0 像素
* 畫布列印 (150 ppi): 1.5-2.0 像素

將 amount 從 1.75 逐漸增加至 4。如果銳利化仍未產生您想要的樣子，以小數遞增 radius，並再次將 amount 從 1.75 增加至 4。視需要重複執行

保留 monochrome 參數的設定值 0。

## JPEG 壓縮的最佳實踐 (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* 這個參數控制 JPG 編碼品質。值愈大表示影像品質愈好，但檔案較大；相反地，值愈小表示影像品質愈差，但檔案較小。此參數的範圍是 0-100。
* 若要將品質最佳化，請勿將此參數值設為 100。設為 90、95 或 100 的差異微乎其微，但 100 會不必要的增加影像檔案的大小。因此，要優化質量，同時避免影像檔案過大，請設定 `qlt=` 值為90或95。
* 要優化較小的影像檔案大小，但將影像質量保持在可接受的級別，請設定 `qlt=` 值為80。 低於 70 至 75 的值會導致影像品質大幅下滑。
* 作為最佳實踐，要在中間， `qlt=` 值85以保持中間位置。
* 在 `qlt=` = 中使用色度旗幟

   * 的 `qlt=` 參數具有第二個設定，允許您使用法線值開啟RGB色度下採樣 `,0` （預設值），或使用值關閉 `,1`。
   * 要保持其簡單性，請先關閉RGB色度下採樣( `,1`)。 此設定通常會得到較好的影像品質，特別是包含許多銳利邊緣和對比的合成影像。

作為JPG壓縮使用的最佳做法 `&qlt=85,0`。

## JPEG 大小調整的最佳實踐 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

參數 `jpegSize` 如果您希望確保映像不會超過某個大小，以便傳輸到記憶體有限的設備，則此功能非常有用。

* 此參數以千位元組( `jpegSize=<size_in_kilobytes>`)。 它可定義影像傳送所允許的大小上限。
* `&jpegSize=` 與JPG壓縮參數交互 `&qlt=`。 如果JPG響應具有指定的JPG壓縮參數( `&qlt=`)不超過 `jpegSize` 值，影像返回時 `&qlt=` 定義。 否則， `&qlt=` 會逐漸減少，直到映像達到允許的最大大小，或直到系統確定它無法適應並返回錯誤。

作為最佳做法， `&jpegSize=` 並添加參數 `&qlt=` 將JPG映像交付到記憶體有限的設備。

## 最佳實踐摘要 {#best-practices-summary}

達到高影像品質和小型檔案的最佳實踐，就是從以下的參數組合開始: 

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

這個設定組合在大多數環境中可獲得極佳的結果。

如果影像需要進一步最佳化，可逐漸微調銳利化 (遮色片銳利化調整) 參數，從 radius 設為 0.2 或 0.3 開始。接著，將 amount 從 1.75 逐漸增加至最大值 4 (相當於 Photoshop 中的 400%)。查看是否得到想要的結果。

如果仍不滿意銳利化的結果，以小數遞增 radius。每一次小數增量，amount 就從 1.75 重新開始逐漸增加至 4。重複這個程序，直到得到想要的結果為止。上述值是經過 Creative Studios 驗證的方法，請記住您可以依循其他策略並從其他值開始。您對於結果的滿意度很主觀，因此，結構化實驗是關鍵。

在您進行實驗時，以下一般性建議有助於優化工作流：

* 直接在URL上或使用Adobe Dynamic Media Classic的影像調整功能，即時嘗試並test不同的參數。 後者提供用於調整操作的即時預覽。
* 作為最佳做法，請記住，可以將「Dynamic Media影像服務」命令分組到影像預設中。 影像預設基本上是具有自定義預設名稱(如 `$thumb_low$` 和 `&product_high$`。 URL路徑中的自定義預設名稱將調用這些預設。 這類功能可協助您管理網站上不同影像使用模式的命令和品質設定，以及縮短 URL 的整體長度。
* Adobe Dynamic Media Classic還提供了更先進的影像質量調整方法，例如對攝取應用影像銳化。 對於可以選擇進一步調整和優化渲染結果的高級使用情形，Adobe Professional Services可以幫助您定制洞察力和最佳實踐。
