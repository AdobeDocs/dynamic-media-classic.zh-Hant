---
title: 使用PDF
description: 瞭解如何在Adobe Dynamic Media Classic中使用PDF。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 25%

---

# 使用PDF{#working-with-pdfs}

PDF（可攜式檔案格式）檔案最常用於Adobe Dynamic Media Classic建立eCatalog。 依預設，當您上傳PDF檔案時，Adobe Dynamic Media Classic會點陣化或Rip化頁面，以便使用這些頁面建置豐富媒體。

當您上傳頁面擷取的PDF時，Adobe會強制進行下列限制：

| 限制型別 | 強加的限制 | 2022年12月31日變更為限制 |
| --- | --- | --- |
| 要考慮進行擷取的PDF最大頁數 | 5000 （適用於新上傳） | 100 (適用於所有PDF) |

另請參閱 [Dynamic Media限制](/help/using/limitations.md).

## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF檔案通常包含裁切邊界、裁切標籤、對齊標籤和其他印表機標籤。 您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

上傳PDF檔案的選項位於「上傳」頁面的「PDF選項」下。

### 處理選項

**[!UICONTROL 點陣化]** - （預設）撕裂PDF檔案中的頁面，並將向量影象轉換為點陣圖影像。 若要建立eCatalog，請選擇此選項。

**[!UICONTROL 擷取搜尋字詞]**  — 從PDF檔案中擷取文字，以便在eCatalog檢視器中搜尋檔案中的關鍵字。

**[!UICONTROL 擷取連結]**  — 從PDF檔案中擷取連結，並將其轉換成eCatalog檢視器中使用的影像地圖。

**[!UICONTROL 使用多頁PDF自動產生eCatalog]**  — 自動從PDF檔案建立eCatalog。 上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

### 解析度

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

### 色域選項

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

* **[!UICONTROL 自動偵測]**  — 保留PDF檔案的色域。

* **[!UICONTROL 強製為RGB]**  — 轉換為RGB色域。

* **[!UICONTROL 強製為CMYK]**  — 轉換為CMYK色彩空間。

* **[!UICONTROL 強製為灰階]**  — 轉換為灰階色域。

### 色彩設定檔選項

* **[!UICONTROL 轉換為sRGB]**  — 轉換為sRGB （標準紅綠藍）。 sRGB是在網頁上顯示影像的建議色域。

* **[!UICONTROL 保留原始色域]**  — 保留原始色域。

* **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**  — 開啟選單，讓您能夠選擇「轉換自」和「轉換至」色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。

請另參閱 [ICC 設定檔](/help/using/icc-profiles.md#icc_profiles)。

## 裁切PDF檔案中的空格 {#cropping-white-space-from-a-pdf-file}

上傳檔案時，您可以自動裁切PDF檔案中的空白畫素。

1. 選取「裁切」選單，然後選擇「裁剪」。
1. 指定下列選項:

   * **[!UICONTROL 修剪依據]**  — 選擇根據顏色或透明度裁切：

      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 然後選取 **[!UICONTROL 邊角]** 功能表，然後以最能代表您要裁切之空白顏色的顏色，選擇PDF的角落。

      * **[!UICONTROL 透明度]**  — 選擇「透明度」選項。

   * **[!UICONTROL 容許度]**  — 拖曳滑桿以指定從0到1的公差。

   * **[!UICONTROL 根據色彩修剪]**  — 指定0只有在畫素完全符合您在PDF角落選取的顏色時，才會裁切畫素。 數值越接近 1，允許的色彩差異就越大。

   * **[!UICONTROL 根據透明度修剪]**  — 指定0以裁切透明畫素；數字越接近1則透明度越高。

## 從PDF頁面側面裁切 {#cropping-from-the-sides-of-pdf-pages}

上傳時，您可以手動從PDF檔案的頁面兩側移除印表機標籤。

1. 從「裁切」功能表中選取 **[!UICONTROL 手動]**.
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，假設您輸入150 （預設值）作為「解析度PX/英吋」設定。 然後裁切頁面兩側75畫素。 在這種情況下，請輸入0.5英吋 已裁切。 若每英吋150畫素，75畫素等於半英吋。
