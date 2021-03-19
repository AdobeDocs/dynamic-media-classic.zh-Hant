---
title: 影像品質最佳化的最佳實踐
description: 瞭解最佳化影像品質的最佳範例。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media經典，資產管理
role: 業務從業人員
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1481'
ht-degree: 61%

---


# 影像品質最佳化的最佳實踐{#best-practices-for-optimizing-the-quality-of-your-images}

影像品質最佳化可能非常耗時，因為演算可接受的結果受許多因素影響。結果有點主觀，因為每個人對影像品質的認定不同。結構化實驗是關鍵。

Dynamic Media經典包含超過100種影像伺服指令，可用來調整和最佳化影像和轉換結果。 以下準則幫助您運用部分基本命令和最佳實踐來加速程序並快速達到滿意的結果。

另請參閱[Smart imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic)。

## 影像格式的最佳實踐 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 要讓影像呈現良好品質並具有可管理的大小和寬度，JPG 或 PNG 是最佳選擇。
* 如果URL中未提供格式命令，Dynamic Media影像伺服預設為JPG以傳送。
* JPG 以 10:1 的比例壓縮，通常會產生較小的檔案。PNG的壓縮比約為2:1，但在某些情況下除外，例如當影像包含空白背景時。 大致上 PNG 檔案的大小比 JPG 檔案更大。
* JPG 使用失真壓縮，意思就是在壓縮時會捨棄一些圖形元素 (像素)。PNG 另一方面會使用無失真壓縮。
* JPG 壓縮的相片影像通常比合成影像有更好的真實度，因為具有銳利的邊緣和對比。
* 如果您的影像具有透明度，請使用 PNG，因為 JPG 不支援透明度。

作為影像格式的最佳實務，請從最常見的設定`&fmt=JPG`開始。

## 影像大小的最佳實踐 {#best-practices-for-image-size}

動態縮小影像大小是Dynamic Media影像服務最常執行的工作之一。 它牽涉到指定大小，以及選擇性指定使用哪一個縮減取樣模式來縮減影像。

* 對於影像大小調整，最好也最直接的方法是使用`&wid=<value>`和`&hei=<value>`或僅使用`&hei=<value>`。 這些參數會根據外觀比例自動設定影像寬度。
* `&resMode=<value>` 控制用於縮減取樣的演算法。從`&resMode=sharp2`開始。 此值可提供最好的影像品質。雖然使用縮減取樣值`=bilin`的速度較快，但通常會導致不自然的鋸齒。

請使用`&wid=<value>&hei=<value>&resMode=sharp2`或`&hei=<value>&resMode=sharp2`來最佳調整影像大小

## 影像銳利化的最佳實踐 {#best-practices-for-image-sharpening}

影像銳利化是在網站上控制影像時最複雜的一環，常會發生許多錯誤。請花點時間參考下列有用資源，進一步瞭解銳利化和反銳化遮色片在Dynamic Media經典影像中的運作方式：

最佳實務白皮書[在Dynamic Media經典Adobe和影像伺服器上銳利化影像](/help/assets/s7_sharpening_images.pdf)。

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

有了Dynamic Media經典影像，您就可以在擷取、傳送或兩者上銳利化影像。 不過在大部分情況下，您應該只使用其中一種方法 (而非同時使用兩者) 將影像銳利化。傳送影像時在 URL 上銳利化影像，通常可以獲得最好的結果。

您可使用兩種方法將影像銳利化: 

* 簡單銳利化(`&op_sharpen`)-與Photoshop使用的銳利化濾鏡類似，簡單銳利化會在動態調整大小後將基本銳利化套用至影像的最終檢視。 不過，使用者無法設定這個方法。最佳實務是除非有需要，否則不使用`&op_sharpen`。
* 銳利化遮色片(`&op_USM`)-銳利化遮色片是業界標準的銳利化濾鏡。 最佳實踐就是遵守以下準則並利用遮色片銳利化調整將影像銳利化。遮色片銳利化調整可讓您控制以下三個參數: 

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5，效果的強度。)
      * `radius` (0-250，在銳利化之物件周圍繪製的「銳利化線條」寬度，其單位為像素。)

         請記住，`radius` 和 `amount` 參數互相消長。通過增加`amount`可以補償減小`radius`。 `Radius` 可以進行更精細的控制，因為較低的數值只會銳利化在邊緣的像素，而以較高的數值銳利化的像素範圍會比較寬。

      * `threshold` （0-255，效果敏感性）。

         此參數可決定銳化像素與周圍區域的差異程度，之後才會被視為邊緣像素，濾鏡會銳化這些像素。臨界值利用相似顏色 (如皮膚色調) 避免區域過度銳利化。例如，閾值為12會忽略膚色亮度的微小變化，以避免加上「雜訊」，同時仍會加上邊緣對比度至高對比區域，例如睫毛與皮膚相遇的區域。

         如需如何設定這三個參數的詳細資訊，包括搭配濾鏡使用的最佳實務，請參閱「在Adobe Scene7出版系統中銳利化影像」和「影像伺服器」上的「[」。](/help/assets/s7_sharpening_images.pdf)

      * Dynamic Media經典也可讓您控制第四個參數：單色(`0,1`)。 這個參數決定要將遮色片銳利化調整分別套用至每個色彩元件 (使用值 `0`) 或套用至影像亮度/飽和度 (使用值 `1`)。

最佳實踐就是從遮色片銳利化調整的 radius 參數著手。您可以從以下的 radius 設定開始: 

* 網站: 0.2-0.3 像素
* 相片列印 (250-300 ppi): 0.3-0.5 像素
* 偏移列印 (266-300 ppi): 0.7-1.0 像素
* 畫布列印 (150 ppi): 1.5-2.0 像素

將 amount 從 1.75 逐漸增加至 4。如果銳利化仍未產生您想要的樣子，以小數遞增 radius，並再次將 amount 從 1.75 增加至 4。視需要重複執行

保留 monochrome 參數的設定值 0。

## JPEG 壓縮的最佳實踐 (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* 這個參數控制 JPG 編碼品質。值愈大表示影像品質愈好，但檔案較大；相反地，值愈小表示影像品質愈差，但檔案較小。此參數的範圍是 0-100。
* 若要將品質最佳化，請勿將此參數值設為 100。設為 90、95 或 100 的差異微乎其微，但 100 會不必要的增加影像檔案的大小。因此，若要最佳化品質，但避免影像檔案變得過大，請將`qlt=`值設為90或95。
* 若要最佳化小型影像檔案大小，但將影像品質維持在可接受的水準，請將`qlt=`值設為80。 低於 70 至 75 的值會導致影像品質大幅下滑。
* 最佳實務是，若要保持在中間位置，請將`qlt=`值設為85以保持在中間位置。
* 在 `qlt=` = 中使用色度旗幟

   * `qlt=`參數有第二個設定，可讓您使用正常值`,0`（預設值）開啟RGB色度縮減採樣，或使用值`,1`關閉它。
   * 要保持其簡單性，請先關閉RGB色度下採樣(`,1`)。 此設定通常會得到較好的影像品質，特別是包含許多銳利邊緣和對比的合成影像。

JPG壓縮的最佳實務是使用`&qlt=85,0`。

## JPEG 大小調整的最佳實踐 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果您想要確保影像不會超過特定大小，以便傳送至記憶體有限的裝置，`jpegSize` 是實用的參數。

* 此參數以千位元組(`jpegSize=<size_in_kilobytes>`)為單位設定。 它可定義影像傳送所允許的大小上限。
* `&jpegSize=` 與JPG壓縮參數互動 `&qlt=`。如果具有指定JPG壓縮參數(`&qlt=`)的JPG回應未超過`jpegSize`值，則會傳回已定義的`&qlt=`影像。 否則，`&qlt=`會逐漸縮小，直到影像符合允許的最大大小，或直到系統判斷它無法符合併傳回錯誤為止。

如果您要將JPG影像傳送至記憶體有限的裝置，請設定`&jpegSize=`並新增參數`&qlt=`。

## 最佳實踐摘要 {#best-practices-summary}

達到高影像品質和小型檔案的最佳實踐，就是從以下的參數組合開始: 

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

這個設定組合在大多數環境中可獲得極佳的結果。

如果影像需要進一步最佳化，可逐漸微調銳利化 (遮色片銳利化調整) 參數，從 radius 設為 0.2 或 0.3 開始。接著，將 amount 從 1.75 逐漸增加至最大值 4 (相當於 Photoshop 中的 400%)。查看是否得到想要的結果。

如果仍不滿意銳利化的結果，以小數遞增 radius。每一次小數增量，amount 就從 1.75 重新開始逐漸增加至 4。重複這個程序，直到得到想要的結果為止。上述值是經過 Creative Studios 驗證的方法，請記住您可以依循其他策略並從其他值開始。您對於結果的滿意度很主觀，因此，結構化實驗是關鍵。

在實驗時，您可能也會發現以下的一般性建議對於您的工作流程最佳化很實用: 

* 直接在Dynamic Media經典URL上或使用Dynamic Media經典影像調整功能（提供調整作業的即時預覽），即時嘗試並測試不同的參數。
* 請記住，您可以將「Dynamic Media影像伺服」指令群組至影像預設集。 影像預設集基本上是具有自訂預設集名稱（例如`$thumb_low$`和`&product_high$`）的URL命令巨集。 URL 路徑中的自訂預設集名稱會呼叫這些預設集。這類功能可協助您管理網站上不同影像使用模式的命令和品質設定，以及縮短 URL 的整體長度。
* Dynamic Media經典也提供更進階的影像品質調整方式，例如在擷取時套用銳利化影像。 在進階使用案例中，這是進一步調整及最佳化演算結果的方法之一，Adobe Professional Services 可協助您進行自訂分析和最佳實踐。
