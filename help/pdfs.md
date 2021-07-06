---
title: 處理 PDF
description: 了解如何在Dynamic Media Classic中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic，資產管理
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 45%

---

# 處理 PDF{#working-with-pdfs}

Dynamic Media Classic最常使用PDF（可攜式檔案格式）檔案來建立eCatalog。 上傳PDF檔案、Dynamic Media Classic預設會柵格化或邊緣化頁面，以便這些頁面可用來建立多媒體。

## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF 檔案有時會包含修剪邊界、裁切標記、對齊標記和其他印表機標記。您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

上傳PDF檔案的選項位於「上傳」頁面的「PDF選項」下。

### 處理選項

**柵格化**  — （預設值）拆分PDF檔案中的頁面，並將向量圖形轉換為點陣圖影像。若要建立eCatalog，請選擇此選項。

**擷取搜尋字詞**  — 從PDF檔案擷取字詞，以便在eCatalog檢視器中依關鍵字搜尋檔案。

**提取連結**  — 從PDF檔案提取連結，並將其轉換為eCatalog檢視器中使用的影像地圖。

**使用多頁PDF自動產生eCatalog**  — 從PDF檔案自動建立eCatalog。上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

### 解析度

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

### 色域選項

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

* **自動檢測**  — 保留PDF檔案的顏色空間。

* **強制為RGB**  — 轉換為RGB色域。

* **強制為CMYK**  — 轉換為CMYK顏色空間。

* **強制為灰度**  — 轉換為灰度顏色空間。

### 色彩描述檔選項

* **轉換為sRGB**  — 轉換為sRGB（標準紅綠藍）。sRGB 是在網頁上顯示影像時建議使用的色域。

* **保留原始顏色空間**  — 保留原始顏色空間。

* **「自訂自」>「轉換為」**  — 開啟功能表，供您選擇「轉換自」和「轉換為顏色空間」。您可以選擇標準的Photoshop色彩空間或上傳至Dynamic Media Classic的色彩空間。

請另參閱 [ICC 設定檔](/help/icc-profiles.md#icc_profiles)。

## 從 PDF 檔案裁切空白區域 {#cropping-white-space-from-a-pdf-file}

1. 若要在上載 PDF 檔案時自動裁切其中的空白區域像素，請選取「裁切」選單並選擇「修剪」。
1. 指定下列選項:

   * **根據** 修剪掉 — 選擇根據顏色或透明度裁切：

   * **顏色**  — 選擇顏色選項。接著選取「邊角」選單，然後選擇對所要裁切之色彩呈現最佳空白區域色彩的 PDF 邊角。

   * **透明度**  — 選擇「透明度」選項。

   * **公差**  — 拖動滑塊以指定從0到1的公差。

   * **根據顏色修剪**  — 指定0，僅當像素與您在PDF的角部中選取的顏色完全匹配時，才裁切像素。數值越接近 1，允許的色彩差異就越大。

   * **根據透明度修剪**  — 指定0隻在像素為透明時裁切像素；接近1的數字使透明度更高。

## 從 PDF 頁面邊緣裁切 {#cropping-from-the-sides-of-pdf-pages}

您可以在上載 PDF 檔案時，從頁邊手動移除印表機的標記。

1. 在「裁切」菜單中，按一下「**[!UICONTROL 手動]**」。
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，如果您輸入150（預設值）作為「解析度PX/英吋」設定，並從頁面側邊裁切75像素，則會裁切半英吋；以150像素/英吋為單位，75像素等於半英吋。
