---
title: 上載PDF檔案
description: 瞭解如何上載與Adobe Dynamic Media Classic的eCatalog關聯的PDF檔案。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 38%

---

# 上載PDF檔案{#uploading-the-pdf-files}

通常，Adobe PDF檔案是eCatalog的源。 這些檔案包含所有影像資訊、字型和向量圖形。 您也可以建置含有影像的 eCatalog。準備好要上載的PDF檔案後，在全局導航欄上，選擇 **[!UICONTROL 上載]** 開始上傳PDF。

上載PDF以提取頁面時，Adobe強制實施以下限制：

| PDF限制類型 | 強加的限制 | 2022年12月31日變更上限 |
| --- | --- | --- |
| 要考慮提取的PDF的最大頁數 | 5000（用於新上載） | 100 |

另請參閱 [Dynamic Media限制](/help/limitations.md)。

<!-- 
>[!NOTE]
>
>When you upload a PDF for page extraction, Adobe imposes the following best practice guideline and enforced limit.d
>
>* Maximum page size of a PDF to be considered for extraction
>   * Best practice: 100
>   * Enforced limit: 1000 (for refresh uploads) -->

## 準備PDF檔案 {#preparing-your-pdf-files}

在將PDF檔案上載到Adobe Dynamic Media Classic之前，請準備這些檔案：

* 要使上傳檔案更容易，請將所有檔案放在電腦或網路上的同一資料夾中。
* 以字母數字順序，依照頁面為檔案命名。排序頁面會讓您在檔案上載後，能夠更輕鬆地依照適當順序來放置頁面。
* 要查看PDF頁是否包含裁剪標籤、註冊目標或顏色條，請檢查頁。 這些標記會決定列印文件時，要在哪裡裁切紙張；將 eCatalog 放置在網路上之前，必須將這些標記移除。Adobe Dynamic Media Classic提供了上載PDF檔案時裁剪標籤的選項。
* 如果您要檢視器依關鍵字搜尋 eCatalog，請檢查您的 PDF 檔案是否已「平面化」。您無法從已平面化的 PDF 檔案中擷取搜尋字詞。若要檢查 PDF 檔案是否已平面化，請嘗試選取其中的文字。如果無法選擇文本，則PDF將被展平，查看者無法按eCatalog中的關鍵字進行搜索。
* 因為 PDF 檔案須列印，所以通常包含 CMYK 影像。預設情況下，Adobe Dynamic Media Classic可以智慧地檢測這些CMYK影像，並使用內部CMYK顏色配置檔案進行轉換。 不過，您也可以使用自訂色彩設定檔來轉換 CMYK 影像。

   請參閱 [ICC（國際顏色聯盟）配置檔案](icc-profiles.md#icc_profiles)。

## 最佳實務 PDF 上載選項 {#best-practice-pdf-upload-options}

如需關於各種上載方法的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_your_files)。

選取要上載的檔案，然後選取以下 *最佳實務* PDF 選項:

* **裁剪選項**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL 裁剪選項]**。 如果PDF頁包含裁剪標籤、註冊標籤或其他標籤，則 **[!UICONTROL 裁剪]** 下拉清單，選擇 **[!UICONTROL 手動]**。 輸入要從頁面頂端、右方、底端與左方裁切掉的像素數。裁剪標籤通常設定為半英吋的邊距。 假設您選擇 **[!UICONTROL 150]** （推薦）作為像素/英吋解析度，並在「頂部」、「右」、「底部」和「左」文本框中輸入75、75、75、75。 在這種情況下，它從邊距（150 ppi,1的一半等於75像素）縮短半英吋。

* **處理**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 在 **[!UICONTROL 處理]** 下拉清單，選擇 **[!UICONTROL 光柵化]**。 必須將 PDF 檔案點陣化，才能讓所有頁面與影像顯示在 eCatalog 中。

* **提取搜索詞（可選）**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 在「提取」下拉清單中，選擇 **[!UICONTROL 搜索詞]** 的子菜單。

* **自動從多頁生成eCatalogPDF（可選）**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 選擇 **[!UICONTROL 自動從多頁生成eCatalogPDF]** 以在上載時自動建立eCatalog。 您可以直接前往「eCatalog」畫面，並開始在 eCatalog 上作業 (不需要先選取 PDF 檔案)，然後選取「建置」命令。eCatalog 是根據 PDF 檔案來命名。

* **解決**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 在 **[!UICONTROL 解決]** 文本欄位，輸入值。 Adobe Dynamic Media Classic推薦每英吋150像素。

* **色彩空間**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 在「顏色空間」下拉清單中，選擇 **[!UICONTROL 自動檢測]**。 通常針對列印輸出所建立的 PDF 是 CMYK 格式；針對線上檢視所建立的 PDF 則是 RGB。如果 PDF 同時使用兩個色域，則您可以選擇「強制為 RGB」或「強制為 CMYK」，來選取一個特定色域。例如，當頁面圖形使用 CMYK 色域，但圖片卻使用 RGB 時，PDF 會同時使用兩個色域。如果您上載了 ICC 設定檔，它的名稱便會顯示在「色域」選單上供您選擇。

   請參閱 [ICC（國際顏色聯盟）配置檔案](/help/icc-profiles.md)。

* **顏色配置檔案選項**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL 顏色配置檔案選項]**，然後選擇「顏色配置檔案」選項：

   * **保留原始顏色空間**  — 保留原始顏色空間。

   * **自定義自>自**  — 開啟子菜單，以便您 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 顏色空間。 您可以選擇標準的Photoshop色彩空間或上載到Adobe Dynamic Media Classic的色彩空間。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

請參閱 [ICC（國際顏色聯盟）配置檔案](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>如需有關所有 PDF 選項的詳細資料，請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。
