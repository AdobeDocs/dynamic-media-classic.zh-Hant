---
title: 上載 PDF 檔案
description: 了解如何上傳與eCatalog相關聯的PDF檔案。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic，檢視器，eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 44%

---

# 上載 PDF 檔案{#uploading-the-pdf-files}

通常，Adobe PDF檔案是eCatalog的來源。 這些檔案包含所有影像資訊、字型和向量圖形。 您也可以建置含有影像的 eCatalog。準備好要上傳的PDF檔案後，在全域導覽列上，按一下&#x200B;**[!UICONTROL Upload]**&#x200B;以開始上傳PDF。

## 準備 PDF 檔案 {#preparing-your-pdf-files}

先準備PDF檔案，再將其上傳至Dynamic Media Classic:

* 為了更輕鬆地上傳檔案，請將所有檔案放置在電腦或網路上的相同資料夾中。
* 以字母數字順序，依照頁面為檔案命名。排序頁面會讓您在檔案上載後，能夠更輕鬆地依照適當順序來放置頁面。
* 要查看PDF頁面是否包含裁切標籤、註冊目標或顏色條，請檢查頁面。 這些標記會決定列印文件時，要在哪裡裁切紙張；將 eCatalog 放置在網路上之前，必須將這些標記移除。Dynamic Media Classic提供上傳PDF檔案時的裁切標籤選項。
* 如果您要檢視器依關鍵字搜尋 eCatalog，請檢查您的 PDF 檔案是否已「平面化」。您無法從已平面化的 PDF 檔案中擷取搜尋字詞。若要檢查 PDF 檔案是否已平面化，請嘗試選取其中的文字。如果您無法選取文字，PDF會平面化，而檢視器無法依eCatalog中的關鍵字搜尋。
* 因為 PDF 檔案須列印，所以通常包含 CMYK 影像。預設情況下，Dynamic Media Classic可以智慧地檢測這些CMYK影像，並使用內部CMYK顏色配置檔案進行轉換。 不過，您也可以使用自訂色彩設定檔來轉換 CMYK 影像。

   請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

## 最佳實務 PDF 上載選項 {#best-practice-pdf-upload-options}

如需關於各種上載方法的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_your_files)。

選取要上載的檔案，然後選取以下 *最佳實務* PDF 選項:

* **裁切選項**  — 在「上傳工作選項」對話方塊上，按一下「 **[!UICONTROL 裁切選項]**」。如果PDF頁面包含裁切標籤、註冊標籤或其他標籤，請在&#x200B;**[!UICONTROL Crop]**&#x200B;下拉式清單中，選擇&#x200B;**[!UICONTROL Manual]**。 輸入要從頁面頂端、右方、底端與左方裁切掉的像素數。裁切標籤通常設定為半英吋邊距。 假設您選擇&#x200B;**[!UICONTROL 150]**（建議）作為每英吋像素解析度，然後在「頂」、「右」、「底」和「左」文本框中輸入75、75、75、75。 在這種情況下，它會從邊緣裁切半英吋（150 ppi,1的半數等於75像素）。

* **處理**  — 在「上傳工作選項」對話方塊中，按一 **[!UICONTROL 下PDF選項]**。在&#x200B;**[!UICONTROL Processing]**&#x200B;下拉式清單中，選擇&#x200B;**[!UICONTROL Rasterize]**。 必須將 PDF 檔案點陣化，才能讓所有頁面與影像顯示在 eCatalog 中。

* **提取搜尋字詞（選用）**  — 在「上傳工作選項」對話方塊上，按一下「 **[!UICONTROL PDF選項」]**。如果您希望檢視器能夠依eCatalog中的關鍵字來搜尋，請在「擷取」下拉式清單中選擇&#x200B;**[!UICONTROL 搜尋字詞]**。

* **從多頁PDF自動產生eCatalog（可選）**  — 在「上傳工作選項」對話方塊上，按一下「 **[!UICONTROL PDF選項」]**。選擇&#x200B;**[!UICONTROL 從多頁自動生成eCatalog PDF]**&#x200B;以在您上傳時自動建立eCatalog。 您可以直接前往「eCatalog」畫面，並開始在 eCatalog 上作業 (不需要先選取 PDF 檔案)，然後選取「建置」命令。eCatalog 是根據 PDF 檔案來命名。

* **解決**  — 在「上傳工作選項」對話方塊中，按一 **[!UICONTROL 下PDF選項]**。在&#x200B;**[!UICONTROL Resolution]**&#x200B;文本欄位中，輸入一個值。 Dynamic Media Classic建議使用150像素/英吋。

* **Colorspace**  — 在「上傳工作選項」對話方塊上，按一 **[!UICONTROL 下PDF選項]**。在「Colorspace」下拉清單中，選擇「自動檢測」**[!UICONTROL 。]**&#x200B;通常針對列印輸出所建立的 PDF 是 CMYK 格式；針對線上檢視所建立的 PDF 則是 RGB。如果 PDF 同時使用兩個色域，則您可以選擇「強制為 RGB」或「強制為 CMYK」，來選取一個特定色域。例如，當頁面圖形使用 CMYK 色域，但圖片卻使用 RGB 時，PDF 會同時使用兩個色域。如果您上載了 ICC 設定檔，它的名稱便會顯示在「色域」選單上供您選擇。

   請參閱[ICC 設定檔](/help/icc-profiles.md)。

* **顏色配置檔案選項**  — 在「上載作業選項」對話框中，按一下「顏 **[!UICONTROL 色配置檔案選項」]**，然後選擇「顏色配置檔案」選項：

   * **保留原始顏色空間**  — 保留原始顏色空間。

   * **「自訂自」>「轉換為」**  — 開啟子功能表，以便選擇「轉 **[!UICONTROL 換]** 自」和「 **[!UICONTROL 轉換]** 為顏色空間。您可以選擇標準的Photoshop色彩空間或上傳至Dynamic Media Classic的色彩空間。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>如需有關所有 PDF 選項的詳細資料，請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。
