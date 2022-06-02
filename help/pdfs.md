---
title: 使用PDF
description: 瞭解如何與Adobe Dynamic Media Classic的PDF合作。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 36%

---

# 使用PDF{#working-with-pdfs}

PDF（可移植文檔格式）檔案在Adobe Dynamic Media Classic最常用於建立eCatalogs。 在上載PDF檔案、Adobe Dynamic Media Classic柵格化或刪除時，預設情況下這些頁，以便這些頁可用於生成富媒體。

>[!NOTE]
>
>上載PDF以提取頁面時，Adobe會規定以下最佳做法准則和強制限制。
>
>* 每個PDF考慮提取的最大頁數
   >   * 最佳做法：100
   >   * 強制限制：1000（用於刷新上載）


## PDF 上載選項 {#pdf-upload-options}

上載 PDF 檔案時，您可以使用各種方法來設定 PDF 檔案的格式。您可以裁切其頁面、擷取搜尋字詞、輸入每英吋像素解析度，以及選擇色域。PDF 檔案有時會包含修剪邊界、裁切標記、對齊標記和其他印表機標記。您可以在上載 PDF 檔案時，從頁邊裁切這些標記。

上載PDF檔案的選項位於「上載」頁的「PDF選項」下。

### 處理選項

**[!UICONTROL 光柵化]**  — （預設）拆除PDF檔案中的頁面，並將向量圖形轉換為點陣圖影像。 要建立eCatalog，請選擇此選項。

**[!UICONTROL 提取搜索詞]**  — 從PDF檔案中提取字詞，以便在eCatalog Viewer中按關鍵字搜索檔案。

**[!UICONTROL 提取連結]**  — 從PDF檔案中提取連結，並將其轉換為在eCatalog Viewer中使用的影像映射。

**[!UICONTROL 使用多頁PDF自動生成電子目錄]**  — 自動從PDF檔案建立eCatalog。 上載 PDF 檔案後會命名 eCatalog。(僅在您上載 PDF 檔案並將其點陣化時，才可使用此選項。)

### 解析度

決定解析度設定。此設定決定 PDF 檔案中每英吋顯示的像素多寡。預設值為 150。

### 色域選項

選取「色域」選單，並為 PDF 檔案選擇色域。大多數的 PDF 檔案都會有 RGB 和 CMYK 色彩影像。RGB 色域較為適合線上檢視。

* **[!UICONTROL 自動檢測]**  — 保留PDF檔案的顏色空間。

* **[!UICONTROL 強制為RGB]**  — 轉換為RGB顏色空間。

* **[!UICONTROL 強制為CMYK]**  — 轉換為CMYK顏色空間。

* **[!UICONTROL 強制為灰度]**  — 轉換為灰度色空間。

### 顏色配置檔案選項

* **[!UICONTROL 轉換為sRGB]**  — 轉換為sRGB（標準紅綠藍）。 sRGB 是在網頁上顯示影像時建議使用的色域。

* **[!UICONTROL 保留原始顏色空間]**  — 保留原始顏色空間。

* **[!UICONTROL 自定義自]** > **[!UICONTROL 至]**  — 開啟菜單，以便選擇「轉換自」和「轉換至」顏色空間。 您可以選擇標準的Photoshop色彩空間或上載到Adobe Dynamic Media Classic的色彩空間。

請另參閱 [ICC 設定檔](/help/icc-profiles.md#icc_profiles)。

## 從PDF檔案裁剪空白 {#cropping-white-space-from-a-pdf-file}

1. 若要在上載 PDF 檔案時自動裁切其中的空白區域像素，請選取「裁切」選單並選擇「修剪」。
1. 指定下列選項:

   * **[!UICONTROL 基於]**  — 選擇是根據顏色還是透明度裁剪：

      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 然後選擇 **[!UICONTROL 角]** ，然後選擇PDF的角，該顏色最能代表要裁剪的空白顏色。

      * **[!UICONTROL 透明度]**  — 選擇「透明度」選項。
   * **[!UICONTROL 容差]**  — 拖動滑塊以指定0到1的公差。

   * **[!UICONTROL 基於顏色的修剪]**  — 指定0，僅當像素與您在PDF角部選擇的顏色完全匹配時，才裁剪像素。 數值越接近 1，允許的色彩差異就越大。

   * **[!UICONTROL 基於透明度的修剪]**  — 僅當像素透明時，指定0來裁剪像素；接近1的數字允許更透明。


## 從PDF頁的側面裁剪 {#cropping-from-the-sides-of-pdf-pages}

您可以在上載 PDF 檔案時，從頁邊手動移除印表機的標記。

1. 從「裁剪」菜單中，選擇 **[!UICONTROL 手動]**。
1. 在「上」、「右」、「下」及「左」文字方框中輸入像素設定，即可裁切頁面上緣、下緣及側邊。

裁切的頁面部分取決於您針對 PDF 檔案所輸入的「解析度像素/英吋」設定。例如，如果輸入150（預設值）作為「解析度PX/英吋」設定，並從頁面側面裁剪75個像素，則會裁剪半英吋；150像素/英吋，75像素等於半英吋。
