---
title: 處理 PDF
seo-title: 處理 PDF
description: 'null'
seo-description: 瞭解如何在Dynamic Media Classic中處理PDF。
uuid: 26d70d28-9393-49b1-9051-d70456 deca67
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/master_ files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 處理 PDF{#working-with-pdfs}

PDF(可攜式文件格式)檔案最常用於Dynamic Media Classic，以建立eCatalogs。當您上傳PDF檔案時，Dynamic Media Classic會依照預設點陣化頁面，使頁面能夠用來建立豐富媒體。

## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF 檔案有時會包含修剪邊界、裁切標記、對齊標記和其他印表機標記。您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

您可以在「PDF 選項」下方的「上載」畫面中，找到用於上載 PDF 檔案的選項。

**處理**

「處理」選項如下:

**點陣化** (預設)套用PDF檔案中的頁面，並將向量圖形轉換為點陣圖影象。選擇此選項以建立 eCatalog。

**擷取搜尋字詞** 從PDF檔案擷取字詞，以便在eCatalog檢視器中依關鍵字搜尋檔案。

**摘取連結** 摘取PDF檔案中的連結，並將其涵蓋至eCatalog檢視器中使用的影像地圖。

**自動產生eCatalog具有多個頁面PDF** 自動從PDF檔案建立eCatalog。上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

**解析度**

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

**色域**

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

**偵測自動** 保留PDF檔案的色域。

**強制隨著RGB** 轉換為RGB色域。

**強制隨CMYK** 轉換為CMYK色域。

**「灰階」(Force** as Grayscale)轉換為灰階色域。

**色彩設定檔**

選擇「色彩設定檔」選項:

**轉換為sRGB** 轉換為sRGB(標準紅色綠色藍色)。sRGB 是在網頁上顯示影像時建議使用的色域。

**保留原始色域** 保留原始色域。

**自訂從&gt;「開啓** 」功能表，您可以選擇「轉換自」和「轉換為色域」。您可以選擇標準 Photoshop 色域，或是上載至 SPS 的色域。

請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

## 從 PDF 檔案裁切空白區域 {#cropping-white-space-from-a-pdf-file}

1. 若要在上載 PDF 檔案時自動裁切其中的空白區域像素，請選取「裁切」選單並選擇「修剪」。
1. 指定下列選項:

   **根據** 顏色或透明度選擇裁切以選擇裁切：

   **顏色** 選擇顏色選項。接著選取「邊角」選單，然後選擇對所要裁切之色彩呈現最佳空白區域色彩的 PDF 邊角。

   **透明度** 選擇透明度選項。

   **容許功能** 拖曳滑桿以指定從到1的容限：

   **根據顏色** 修剪只需將像素與您在PDF角落中選取的顏色完全相符，即可指定裁切像素。數值越接近 1，允許的色彩差異就越大。

   **以透明度為基礎的修剪** 只會在完全透明時指定裁切像素；數字接近1可提高透明度。

## 從 PDF 頁面邊緣裁切 {#cropping-from-the-sides-of-pdf-pages}

您可以在上載 PDF 檔案時，從頁邊手動移除印表機的標記。

1. 選取「裁切」選單，並且選擇「手動」。
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，如果您輸入 150 (預設值) 作為「解析度像素/英吋」設定，且從頁邊裁切 75 像素，則會裁切 半英吋，這是因為每英吋為 150 像素，而 75 像素等於半英吋。
