---
title: 上載PDF檔案
description: 瞭解如何上載與Adobe Dynamic Media Classic的eCatalog關聯的PDF檔案。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 36%

---

# 上載PDF檔案{#uploading-the-pdf-files}

通常，Adobe PDF檔案是eCatalog的源。 這些檔案包含所有影像資訊、字型和向量圖形。 您也可以建置含有影像的 eCatalog。準備好要上載的 PDF 檔案後，請在全域導覽列上選取 **[!UICONTROL 「上載]** 」以開始上傳 pdf。

上傳頁面摘取的 PDF 時，Adobe Systems 會強制實施下列限制：

| PDF 限制類型 | 限制已施加 | 2022年12月31日變更 |
| --- | --- | --- |
| 要考慮 PDF 的最大頁面數摘取 | 5000（用於新上傳） | 100(所有PDF) |

另請參閱 [Dynamic Media限制](/help/limitations.md)。

## 準備PDF檔案 {#preparing-your-pdf-files}

在將PDF檔案上載到Adobe Dynamic Media Classic之前，請準備這些檔案：

* 若要輕鬆上傳檔案，請將所有檔案放在電腦或網路的相同資料夾中。
* 以字母數字順序，依照頁面為檔案命名。排序頁面會讓您在檔案上載後，能夠更輕鬆地依照適當順序來放置頁面。
* 若要查看 PDF 頁面是否包含裁切標記、註冊目標或顏色條，請檢查頁面。 這些標記會決定列印文件時，要在哪裡裁切紙張；將 eCatalog 放置在網路上之前，必須將這些標記移除。Adobe Systems 動態媒體經典提供上傳 PDF 檔案時裁切標記的選項。
* 如果您要檢視器依關鍵字搜尋 eCatalog，請檢查您的 PDF 檔案是否已「平面化」。您無法從已平面化的 PDF 檔案中擷取搜尋字詞。若要檢查 PDF 檔案是否已平面化，請嘗試選取其中的文字。如果您無法選取文字，PDF 會被拼合，且檢視器無法搜尋 eCatalog 中的關鍵字。
* 因為 PDF 檔案須列印，所以通常包含 CMYK 影像。預設情況下，Adobe Dynamic Media Classic可以智慧地檢測這些CMYK影像，並使用內部CMYK顏色配置檔案進行轉換。 不過，您也可以使用自訂色彩設定檔來轉換 CMYK 影像。

   請參閱 [ICC（國際顏色聯盟）配置檔案](icc-profiles.md#icc_profiles)。

## 最佳實務 PDF 上載選項 {#best-practice-pdf-upload-options}

如需關於各種上載方法的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_your_files)。

選取您要上傳的檔案，然後選取這些 *最佳實務* PDF 選項：

* **裁切選項** -在「上載工作選項」對話方塊中，選取 **[!UICONTROL 裁切選項]** 。 如果 PDF 頁面包含裁切標記、註冊標記或其他標記，請在「裁切 ]**下拉式清單中**[!UICONTROL  ，選擇 **[!UICONTROL 「手動]** 」。輸入要從頁面頂端、右方、底端與左方裁切掉的像素數。裁切標記通常設為半英寸邊距。 假設您選擇 **[!UICONTROL 150]** （建議）作為每英吋像素的解析度，然後在上、右、下、左文字方塊中輸入75、75、75、75。 在這種情況下，它會從頁邊距中裁切半英寸（150 ppi，一半等於75圖元）。

* **處理** -在「上載工作選項」對話方塊中，選擇 **[!UICONTROL PDF 選項]** 。 **[!UICONTROL 在處理]** 下拉式清單中，選擇 **[!UICONTROL 「光柵]** 化」。必須將 PDF 檔案點陣化，才能讓所有頁面與影像顯示在 eCatalog 中。

* **提取搜索詞（可選）**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 在「提取」下拉清單中，選擇 **[!UICONTROL 搜索詞]** 的子菜單。

* **自動從多頁生成eCatalogPDF（可選）**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL PDF選項]**。 選擇 **[!UICONTROL 自動從多頁生成eCatalogPDF]** 以在上載時自動建立eCatalog。 您可以直接前往「eCatalog」畫面，並開始在 eCatalog 上作業 (不需要先選取 PDF 檔案)，然後選取「建置」命令。eCatalog 是根據 PDF 檔案來命名。

* **解決方案** -在「上載工作選項」對話方塊中，選擇 **[!UICONTROL PDF 選項]** 。 **[!UICONTROL 在解析度]** 文字欄位中輸入值。Adobe Systems 動態媒體經典建議150圖元/英寸。

* **色域選** -在「上載工作選項」對話方塊中，選擇 **[!UICONTROL PDF 選項]** 。 在色域選下拉式清單中，選擇 **[!UICONTROL 「自動]** 偵測」。 通常針對列印輸出所建立的 PDF 是 CMYK 格式；針對線上檢視所建立的 PDF 則是 RGB。如果 PDF 同時使用兩個色域，則您可以選擇「強制為 RGB」或「強制為 CMYK」，來選取一個特定色域。例如，當頁面圖形使用 CMYK 色域，但圖片卻使用 RGB 時，PDF 會同時使用兩個色域。如果您上載了 ICC 設定檔，它的名稱便會顯示在「色域」選單上供您選擇。

   請參閱 [ ICC （國際顏色聯合會）設定檔 ](/help/icc-profiles.md) 。

* **顏色配置檔案選項**  — 在「上載作業選項」對話框上，選擇 **[!UICONTROL 顏色配置檔案選項]**，然後選擇「顏色配置檔案」選項：

   * **保留原始顏色空間**  — 保留原始顏色空間。

   * **自定義自>自**  — 開啟子菜單，以便您 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 顏色空間。 您可以選擇標準的Photoshop色彩空間或上載到Adobe Dynamic Media Classic的色彩空間。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

請參閱 [ICC（國際顏色聯盟）配置檔案](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>如需有關所有 PDF 選項的詳細資料，請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。
