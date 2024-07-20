---
title: 上傳PDF檔案
description: 瞭解如何在Adobe Dynamic Media Classic中上傳與eCatalog相關聯的PDF檔案。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# 上傳PDF檔案{#uploading-the-pdf-files}

通常Adobe PDF檔案是eCatalog的來源。 這些檔案包含所有影像資訊、字型和向量圖形。 您也可以建置含有影像的 eCatalog。在您準備好要上傳的PDF檔案後，請在全域導覽列上選取&#x200B;**[!UICONTROL 上傳]**&#x200B;以開始上傳PDF。

當您上傳頁面擷取的PDF時，Adobe會強制進行下列限制：

| PDF限制型別 | 強加的限制 | 2022年12月31日變更為限制 |
| --- | --- | --- |
| 要考慮進行擷取的PDF最大頁數 | 5000 （適用於新上傳） | 100 (適用於所有PDF) |

另請參閱[Dynamic Media限制](/help/using/limitations.md)。

## 準備PDF檔案

先準備PDF檔案，再上傳至Adobe Dynamic Media Classic：

* 若要讓檔案上傳更輕鬆，請將所有檔案放在電腦或網路上的相同資料夾中。
* 以字母數字順序，依照頁面為檔案命名。排序頁面會讓您在檔案上載後，能夠更輕鬆地依照適當順序來放置頁面。
* 若要檢視PDF頁面是否包含裁切標籤、註冊目標或色條，請檢查頁面。 這些標記會決定列印文件時，要在哪裡裁切紙張；將 eCatalog 放置在網路上之前，必須將這些標記移除。Adobe Dynamic Media Classic提供可在您上傳PDF檔案時裁切標籤的選項。
* 如果您希望檢視者依關鍵字搜尋eCatalog，請確定您的PDF檔案是否為「平面化」。 您無法從已平面化的 PDF 檔案中擷取搜尋字詞。若要檢視PDF是否平面化，請試著選取其內的文字。 如果您無法選取文字，PDF會平面化，且檢視器無法依您eCatalog中的關鍵字進行搜尋。
* 因為 PDF 檔案須列印，所以通常包含 CMYK 影像。依預設，Adobe Dynamic Media Classic可以聰明地偵測這些CMYK影像，並使用內部CMYK色彩設定檔來轉換影像。 不過，您也可以使用自訂色彩設定檔來轉換 CMYK 影像。

  請參閱[ICC （國際色彩聯盟）設定檔](icc-profiles.md#icc_profiles)。

## 最佳實務 PDF 上載選項 {#best-practice-pdf-upload-options}

如需關於各種上載方法的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_your_files)。

選取您要上傳的檔案，然後選取這&#x200B;*個最佳實務* PDF選項：

* **裁切選項**：在上傳工作選項對話方塊中，選取&#x200B;**[!UICONTROL 裁切選項]**。 如果PDF頁面包含裁切標籤、註冊標籤或其他標籤，請在&#x200B;**[!UICONTROL 裁切]**&#x200B;下拉式清單中選擇&#x200B;**[!UICONTROL 手動]**。 輸入要從頁面的上、右、下和左邊裁切的畫素數。 裁切標籤通常設定為半英吋邊界。 假設您選擇&#x200B;**[!UICONTROL 150]** （建議）作為每英吋畫素解析度。 然後在[上]、[右]、[下]和[左]文字方塊中輸入75、75、75、75。 在這種情況下，它會從邊界裁切半英吋（150 ppi，1的一半等於75畫素）。

* **處理中**：在上傳工作選項對話方塊中，選取&#x200B;**[!UICONTROL PDF選項]**。 在&#x200B;**[!UICONTROL 處理]**&#x200B;下拉式清單中，選擇&#x200B;**[!UICONTROL 點陣化]**。 必須將 PDF 檔案點陣化，才能讓所有頁面與影像顯示在 eCatalog 中。

* **擷取搜尋字詞（選擇性）**：在[上載工作選項]對話方塊中，選取&#x200B;**[!UICONTROL PDF選項]**。 如果要讓檢視者能夠在eCatalog中依關鍵字搜尋，請在「擷取」下拉式清單中選擇&#x200B;**[!UICONTROL 搜尋字詞]**。

* **從多頁PDF自動產生eCatalog （選用）**：在[上傳工作選項]對話方塊中，選取&#x200B;**[!UICONTROL PDF選項]**。 按一下&#x200B;**[!UICONTROL 從多頁PDF自動產生eCatalog]**，這樣您就可以在上傳時自動建立eCatalog。 您可以直接前往「eCatalog」畫面，並開始在 eCatalog 上作業 (不需要先選取 PDF 檔案)，然後選取「建置」命令。eCatalog 是根據 PDF 檔案來命名。

* **解析度**：在上傳工作選項對話方塊中，選取&#x200B;**[!UICONTROL PDF選項]**。 在&#x200B;**[!UICONTROL 解析度]**&#x200B;文字欄位中，輸入值。 Adobe Dynamic Media Classic建議每英吋150畫素。

* **色域**：在上傳工作選項對話方塊中，選取&#x200B;**[!UICONTROL PDF選項]**。 在「色域」下拉式清單中，選擇&#x200B;**[!UICONTROL 自動偵測]**。 通常針對列印輸出所建立的 PDF 是 CMYK 格式；針對線上檢視所建立的 PDF 則是 RGB。如果 PDF 同時使用兩個色域，則您可以選擇「強制為 RGB」或「強制為 CMYK」，來選取一個特定色域。例如，當頁面圖形使用 CMYK 色域，但圖片卻使用 RGB 時，PDF 會同時使用兩個色域。如果您上載了 ICC 設定檔，它的名稱便會顯示在「色域」選單上供您選擇。

  請參閱[ICC （國際色彩聯盟）設定檔](/help/using/icc-profiles.md)。

* **色彩設定檔選項**：在[上載工作選項]對話方塊中，選取&#x200B;**[!UICONTROL 色彩設定檔選項]**，然後選擇色彩設定檔選項：

   * **保留原始色域**：保留原始色域。

   * **自訂從>到**：開啟子功能表，讓您能夠選擇&#x200B;**[!UICONTROL 從]**&#x200B;轉換和&#x200B;**[!UICONTROL 轉換成]**&#x200B;色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

請參閱[ICC （國際色彩聯盟）設定檔](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>如需有關所有 PDF 選項的詳細資料，請參閱[PDF 上載選項](pdfs.md#pdf_upload_options)。
