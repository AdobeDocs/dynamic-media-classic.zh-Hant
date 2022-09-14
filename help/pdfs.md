---
title: 使用PDF
description: 了解如何使用Adobe Dynamic Media Classic中的PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# 使用PDF{#working-with-pdfs}

PDF（可攜式檔案格式）檔案在Adobe Dynamic Media Classic中最常用來建立eCatalog。 上傳PDF檔案、Adobe Dynamic Media Classic模擬或邊欄時，依預設會產生頁面，以便用來建立多媒體。

當您上傳PDF以擷取頁面時，Adobe會強制執行下列限制：

| 限制類型 | 限制 | 2022年12月31日上限的變更 |
| --- | --- | --- |
| 要考慮提取的PDF的最大頁數 | 5000（適用於新上傳） | 100(適用於所有PDF) |

另請參閱 [Dynamic Media限制](/help/limitations.md).

## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF 檔案有時會包含修剪邊界、裁切標記、對齊標記和其他印表機標記。您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

上傳PDF檔案的選項位於「上傳」頁面的「PDF選項」下。

### 處理選項

**[!UICONTROL 光柵化]**  — （預設）拆分PDF檔案中的頁面，並將向量圖形轉換為點陣圖影像。 若要建立eCatalog，請選擇此選項。

**[!UICONTROL 擷取搜尋字詞]**  — 從PDF檔案中擷取字詞，以便在eCatalog檢視器中按關鍵字搜尋檔案。

**[!UICONTROL 擷取連結]**  — 從PDF檔案中提取連結，並將其轉換為eCatalog檢視器中使用的影像地圖。

**[!UICONTROL 使用多頁自動產生eCatalogPDF]**  — 從PDF檔案自動建立eCatalog。 上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

### 解析度

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

### 色域選項

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

* **[!UICONTROL 自動檢測]**  — 保留PDF檔案的顏色空間。

* **[!UICONTROL 強制為RGB]**  — 轉換為RGB顏色空間。

* **[!UICONTROL 強制為CMYK]**  — 轉換為CMYK顏色空間。

* **[!UICONTROL 強制為灰度]**  — 轉換為灰度顏色空間。

### 色彩描述檔選項

* **[!UICONTROL 轉換為sRGB]**  — 轉換為sRGB（標準紅綠藍）。 sRGB 是在網頁上顯示影像時建議使用的色域。

* **[!UICONTROL 保留原始顏色空間]**  — 保留原始顏色空間。

* **[!UICONTROL 自訂來源]** > **[!UICONTROL 結束日期]**  — 開啟菜單，以便選擇「轉換自」和「轉換至」顏色空間。 您可以選擇標準的Photoshop色域或您上傳至Adobe Dynamic Media Classic的色域。

請另參閱 [ICC 設定檔](/help/icc-profiles.md#icc_profiles)。

## 從PDF檔案中裁切空白字元 {#cropping-white-space-from-a-pdf-file}

1. 若要在上載 PDF 檔案時自動裁切其中的空白區域像素，請選取「裁切」選單並選擇「修剪」。
1. 指定下列選項:

   * **[!UICONTROL 根據]**  — 根據顏色或透明度選擇裁切：

      * **[!UICONTROL 顏色]**  — 選擇顏色選項。 然後選取 **[!UICONTROL 角]** ，然後選取PDF的角，其顏色最能代表您要裁切的空白顏色。

      * **[!UICONTROL 透明度]**  — 選擇透明度選項。
   * **[!UICONTROL 容許度]**  — 拖動滑塊以指定從0到1的公差。

   * **[!UICONTROL 基於顏色的修剪]**  — 指定0，僅當像素與您在PDF的角中選定的顏色完全匹配時才裁剪像素。 數值越接近 1，允許的色彩差異就越大。

   * **[!UICONTROL 基於透明度的修剪]**  — 指定0，只有在像素為透明時才裁切像素；接近1的數字使透明度更高。


## 從PDF頁面的側邊裁切 {#cropping-from-the-sides-of-pdf-pages}

您可以在上載 PDF 檔案時，從頁邊手動移除印表機的標記。

1. 從「裁切」功能表中，選取 **[!UICONTROL 手動]**.
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，假設您輸入150（預設值）作為「解析度PX/英吋」設定。 接著，您會從頁面側邊裁切75個像素。 在這種情況下，0.5英吋。 被裁切。 150像素/英吋，75像素等於半英吋。
