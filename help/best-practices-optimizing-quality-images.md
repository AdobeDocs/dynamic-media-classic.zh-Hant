---
title: 影像品質最佳化的最佳實踐
seo-title: 影像品質最佳化的最佳實踐
description: 'null'
seo-description: 瞭解最佳化影像品質的最佳範例。
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: 管理員
content-type: 參考
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTENDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# 影像品質最佳化的最佳實踐{#best-practices-for-optimizing-the-quality-of-your-images}

影像品質最佳化可能非常耗時，因為演算可接受的結果受許多因素影響。結果有點主觀，因為每個人對影像品質的認定不同。結構化實驗是關鍵。

Dynamic Media Classic包含超過100個影像伺服指令，可用來調整和最佳化影像和轉譯結果。 以下準則幫助您運用部分基本命令和最佳實踐來加速程序並快速達到滿意的結果。

另請參閱 [智慧映像](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)。

## 影像格式的最佳實踐 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 要讓影像呈現良好品質並具有可管理的大小和寬度，JPG 或 PNG 是最佳選擇。
* 如果URL中未提供格式命令，則Dynamic Media Image Serving預設為JPG以進行傳送。
* JPG 以 10:1 的比例壓縮，通常會產生較小的檔案。除了一些情況 (例如影像有白色背景) 以外，PNG 會以大約 2:1 的比例壓縮。大致上 PNG 檔案的大小比 JPG 檔案更大。
* JPG 使用失真壓縮，意思就是在壓縮時會捨棄一些圖形元素 (像素)。PNG 另一方面會使用無失真壓縮。
* JPG 壓縮的相片影像通常比合成影像有更好的真實度，因為具有銳利的邊緣和對比。
* 如果您的影像具有透明度，請使用 PNG，因為 JPG 不支援透明度。

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## 影像大小的最佳實踐 {#best-practices-for-image-size}

動態縮小影像大小是動態媒體影像伺服最常執行的工作之一。 它牽涉到指定大小，以及選擇性指定使用哪一個縮減取樣模式來縮減影像。

* For image sizing, the best and most straightforward approach is to use `&wid=<value>` and `&hei=<value>` or just `&hei=<value>`. 這些參數會根據外觀比例自動設定影像寬度。
* `&resMode=<value>` 控制用於縮減取樣的演算法。 從開始 `&resMode=sharp2`。 此值可提供最好的影像品質。While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

作為調整影像大小、使用或 `&wid=<value>&hei=<value>&resMode=sharp2``&hei=<value>&resMode=sharp2`

## 影像銳利化的最佳實踐 {#best-practices-for-image-sharpening}

影像銳利化是在網站上控制影像時最複雜的一環，常會發生許多錯誤。請花點時間參考下列有用資源，進一步瞭解銳利化和反銳化遮色片在Dynamic Media Classic中的運作方式：

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

On Adobe TV, watch [Sharpening an image with unsharp mask](https://tv.adobe.com/watch/visual-design-cs6/sharpening-an-image-with-unsharp-mask/).

有了Dynamic Media Classic，您就可以在擷取、傳送或兩者上銳利化影像。 不過在大部分情況下，您應該只使用其中一種方法 (而非同時使用兩者) 將影像銳利化。傳送影像時在 URL 上銳利化影像，通常可以獲得最好的結果。

您可使用兩種方法將影像銳利化: 

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. 不過，使用者無法設定這個方法。The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. 最佳實踐就是遵守以下準則並利用遮色片銳利化調整將影像銳利化。遮色片銳利化調整可讓您控制以下三個參數: 

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5，效果的強度。)
      * `radius` (0-250，在銳利化之物件周圍繪製的「銳利化線條」寬度，其單位為像素。)

         請記住，`radius` 和 `amount` 參數互相消長。Reducing `radius` can be compensated by increasing `amount`. `Radius` 可以進行更精細的控制，因為較低的數值只會銳利化在邊緣的像素，而以較高的數值銳利化的像素範圍會比較寬。

      * `threshold` （0-255，效果敏感性）。

         這個參數決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素，濾鏡才會予以銳利化。臨界值利用相似顏色 (如皮膚色調) 避免區域過度銳利化。例如，臨界值 12 會忽略皮膚色調亮度的輕微變化，因此不會增加雜訊，同時會增加高反差區域的邊緣對比，例如睫毛和皮膚鄰接之處。
      如需如何設定這三個參數的詳細資訊，包括使用濾鏡的最佳實踐，請參閱以下資源: 

      銳利化影像的Dynamic Media Classic [說明主題](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html)。

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

   * Dynamic Media Classic也可讓您控制第四個參數：單色( `0,1`)。 這個參數決定要將遮色片銳利化調整分別套用至每個色彩元件 (使用值 `0`) 或套用至影像亮度/飽和度 (使用值 `1`)。


最佳實踐就是從遮色片銳利化調整的 radius 參數著手。您可以從以下的 radius 設定開始: 

* 網站: 0.2-0.3 像素
* 相片列印 (250-300 ppi): 0.3-0.5 像素
* 偏移列印 (266-300 ppi): 0.7-1.0 像素
* 畫布列印 (150 ppi): 1.5-2.0 像素

將 amount 從 1.75 逐漸增加至 4。如果銳利化仍未產生您想要的樣子，以小數遞增 radius，並再次將 amount 從 1.75 增加至 4。視需要重複執行

保留 monochrome 參數的設定值 0。

## JPEG 壓縮的最佳實踐 (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* 這個參數控制 JPG 編碼品質。值愈大表示影像品質愈好，但檔案較大；相反地，值愈小表示影像品質愈差，但檔案較小。此參數的範圍是 0-100。
* 若要將品質最佳化，請勿將此參數值設為 100。設為 90、95 或 100 的差異微乎其微，但 100 會不必要的增加影像檔案的大小。Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. 低於 70 至 75 的值會導致影像品質大幅下滑。
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* 在 `qlt=` = 中使用色度旗幟

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * To keep it simple, start with RGB chromaticity downsampling turned off ( `,1`). 此設定通常會得到較好的影像品質，特別是包含許多銳利邊緣和對比的合成影像。

As a best practice for JPG compression use `&qlt=85,0`.

## JPEG 大小調整的最佳實踐 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果您想要確保影像不會超過特定大小，以便傳送至記憶體有限的裝置，`jpegSize` 是實用的參數。

* This parameter is set in kilobytes ( `jpegSize=<size_in_kilobytes>`). 它可定義影像傳送所允許的大小上限。
* `&jpegSize=` 與JPG壓縮參數互動 `&qlt=`。 If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## 最佳實踐摘要 {#best-practices-summary}

達到高影像品質和小型檔案的最佳實踐，就是從以下的參數組合開始: 

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

這個設定組合在大多數環境中可獲得極佳的結果。

如果影像需要進一步最佳化，可逐漸微調銳利化 (遮色片銳利化調整) 參數，從 radius 設為 0.2 或 0.3 開始。接著，將 amount 從 1.75 逐漸增加至最大值 4 (相當於 Photoshop 中的 400%)。查看是否得到想要的結果。

如果仍不滿意銳利化的結果，以小數遞增 radius。每一次小數增量，amount 就從 1.75 重新開始逐漸增加至 4。重複這個程序，直到得到想要的結果為止。上述值是經過 Creative Studios 驗證的方法，請記住您可以依循其他策略並從其他值開始。您對於結果的滿意度很主觀，因此，結構化實驗是關鍵。

在實驗時，您可能也會發現以下的一般性建議對於您的工作流程最佳化很實用: 

* 直接在Dynamic Media Classic URL上或使用Scene7 Publishing system的影像調整功能（提供調整作業的即時預覽），即時嘗試並測試不同的參數。
* 請記住，您可以將「動態媒體影像伺服」指令群組至影像預設集。 An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. URL 路徑中的自訂預設集名稱會呼叫這些預設集。這類功能可協助您管理網站上不同影像使用模式的命令和品質設定，以及縮短 URL 的整體長度。
* Dynamic Media Classic也提供更進階的方式來調整影像品質，例如在擷取時套用銳利化影像。 在進階使用案例中，這是進一步調整及最佳化演算結果的方法之一，Adobe Professional Services 可協助您進行自訂分析和最佳實踐。

