---
title: 上載 PDF 檔案
seo-title: 上載 PDF 檔案
description: 'null'
seo-description: 瞭解如何上傳與eCatalog相關的PDF檔案。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 上載 PDF 檔案{#uploading-the-pdf-files}

Adobe PDF 檔案通常是 eCatalog 的來源；這些 PDF 檔案包含所有影像資訊及字型與向量圖形。您也可以建置含有影像的 eCatalog。準備好供上載用的 PDF 檔案之後，請選取全域導覽列上的「上載」按鈕，開始上載 PDF。

## 準備 PDF 檔案 {#preparing-your-pdf-files}

將 PDF 檔案上載至 Scene7 Publishing System 前，請先準備 PDF 檔案:

* 將所有檔案放置於電腦或網路上的同一個檔案夾中，即可更輕鬆上載檔案。
* 以字母數字順序，依照頁面為檔案命名。排序頁面會讓您在檔案上載後，能夠更輕鬆地依照適當順序來放置頁面。
* 檢視 PDF 頁面，即可查看其中是否包含裁切標記、對齊目標或色彩條。這些標記會決定列印文件時，要在哪裡裁切紙張；將 eCatalog 放置在網路上之前，必須將這些標記移除。Dynamic Media Classic提供在您上傳PDF檔案時裁切標籤的選項。
* 如果您要檢視器依關鍵字搜尋 eCatalog，請檢查您的 PDF 檔案是否已「平面化」。您無法從已平面化的 PDF 檔案中擷取搜尋字詞。若要檢查 PDF 檔案是否已平面化，請嘗試選取其中的文字。如果無法選取文字，就表示 PDF 已平面化，且檢視器無法在 eCatalog 中依關鍵字搜尋。
* 因為 PDF 檔案須列印，所以通常包含 CMYK 影像。根據預設，SPS 可以智慧地偵測這些 CMYK 影像，並使用內部 CMYK 色彩設定檔來轉換它們。不過，您也可以使用自訂色彩設定檔來轉換 CMYK 影像。

   請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

## 最佳實務 PDF 上載選項 {#best-practice-pdf-upload-options}

如需關於各種上載方法的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_your_files)。

選取要上載的檔案，然後選取以下 *最佳實務* PDF 選項:

* **裁切**&#x200B;選取「裁切」功能表，如果頁面包含裁切標籤、註冊標籤或其他標籤，則選擇「手動」。 輸入要從頁面頂端、右方、底端與左方裁切掉的像素數。裁切標記通常設為半英吋邊界。假設您選擇每英吋 150 像素的解析度 (建議設定)，那麼在「上」、「右」、「下」與「左」文字方框中輸入 75、75、75、75 時，會裁切從邊界算起的半英吋區域 (在 150 ppi 時，半英吋相當於 75 個像素)。

* **處理**&#x200B;選擇「處理」菜單，然後選擇「柵格化」。 必須將 PDF 檔案點陣化，才能讓所有頁面與影像顯示在 eCatalog 中。

* **摘取搜尋字詞（選用）**&#x200B;如果您希望檢視者能夠在eCatalog中依關鍵字搜尋，請選取這個選項。

* **從多頁自動產生eCatalog（可選）選**&#x200B;取此選項，在您上傳時自動建立eCatalog。 您可以直接前往「eCatalog」畫面，並開始在 eCatalog 上作業 (不需要先選取 PDF 檔案)，然後選取「建置」命令。eCatalog 是根據 PDF 檔案來命名。

* **解析度** Dynamic Media Classic建議每英吋150像素。

* **Colorspace** Dynamic Media Classic建議選擇「自動偵測」。 通常針對列印輸出所建立的 PDF 是 CMYK 格式；針對線上檢視所建立的 PDF 則是 RGB。如果 PDF 同時使用兩個色域，則您可以選擇「強制為 RGB」或「強制為 CMYK」，來選取一個特定色域。例如，當頁面圖形使用 CMYK 色域，但圖片卻使用 RGB 時，PDF 會同時使用兩個色域。如果您上載了 ICC 設定檔，它的名稱便會顯示在「色域」選單上供您選擇。

   請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

* **顏色描述檔**&#x200B;選擇顏色描述檔選項：

* **轉換為SRGB**&#x200B;轉換為SRGB（標準紅綠藍）。 SRGB 是在網頁上顯示影像時建議使用的色域。

* **保留原始色域**&#x200B;保留原始色域。

* **「自訂自」>「至**&#x200B;開啟」功能表，您可以選擇「轉換自」和「轉換至顏色空間」。 您可以選擇標準 Photoshop 色域，或是上載至 SPS 的色域。

請參閱[ICC 設定檔](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>如需有關所有 PDF 選項的詳細資料，請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。

