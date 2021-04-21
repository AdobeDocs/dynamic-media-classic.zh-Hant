---
title: 處理 PDF
description: 瞭解如何在Dynamic Media經典中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media經典，資產管理
role: Business Practitioner
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 55%

---

# 處理 PDF{#working-with-pdfs}

PDF（可攜式檔案格式）檔案最常用於Dynamic MediaClassic建立eCatalog。 當您上傳PDF檔案、Dynamic Media經典點陣化(Metion Classic Rasterizes)或Rips時，預設會顯示頁面，讓這些頁面可用來建立多媒體。

## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF 檔案有時會包含修剪邊界、裁切標記、對齊標記和其他印表機標記。您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

您可以在「PDF 選項」下方的「上載」畫面中，找到用於上載 PDF 檔案的選項。

**處理**

「處理」選項如下:

**點陣化** （預設值）將PDF檔案中的頁面分割，並將向量圖形轉換為點陣圖影像。選擇此選項以建立 eCatalog。

**擷取搜** 尋字詞從PDF檔案擷取字詞，讓eCatalog檢視器中的關鍵字可搜尋檔案。

**摘取** 連結從PDF檔案擷取連結，並將其轉換為eCatalog檢視器中使用的影像地圖。

**使用多頁自動產生eCatalog從PDF** 檔案自動建立eCatalog。上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

**解析度**

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

**色域**

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

**自動** 偵測保留PDF檔案的色域。

**強制為** RGBC轉換為RGB色域。

**強制為** CMYKC轉換至CMYK色域。

**強制為灰** 階轉換為灰階色域。

**色彩設定檔**

選擇「色彩設定檔」選項:

**轉換為** sRGBConverts至sRGB（標準紅綠藍）。sRGB 是在網頁上顯示影像時建議使用的色域。

**保留原始色** 域保留原始色域。

**「自訂自」>「** 至開啟」功能表，您可以選擇「轉換自」和「轉換至顏色空間」。您可以選擇標準的Photoshop色域或您上傳至Dynamic Media經典的色域。

請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

## 從 PDF 檔案裁切空白區域 {#cropping-white-space-from-a-pdf-file}

1. 若要在上載 PDF 檔案時自動裁切其中的空白區域像素，請選取「裁切」選單並選擇「修剪」。
1. 指定下列選項:

   **根據修剪移** 除選擇是否根據顏色或透明度裁切：

   **顏** 色選擇顏色選項。接著選取「邊角」選單，然後選擇對所要裁切之色彩呈現最佳空白區域色彩的 PDF 邊角。

   **透明** 度選擇透明度選項。

   **公** 差拖動滑塊以指定0到1的公差：

   **根據顏色修** 剪指定0，只有在像素與您在PDF角落中選取的顏色完全相符時，才可裁切像素。數值越接近 1，允許的色彩差異就越大。

   **根據透明度修剪** 指定0，僅在像素完全透明時才裁切像素；接近1的數字使得透明度更高。

## 從 PDF 頁面邊緣裁切 {#cropping-from-the-sides-of-pdf-pages}

您可以在上載 PDF 檔案時，從頁邊手動移除印表機的標記。

1. 選取「裁切」選單，並且選擇「手動」。
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，如果您輸入 150 (預設值) 作為「解析度像素/英吋」設定，且從頁邊裁切 75 像素，則會裁切 半英吋，這是因為每英吋為 150 像素，而 75 像素等於半英吋。
