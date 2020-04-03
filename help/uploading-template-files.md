---
title: 上載範本檔案
seo-title: 上載範本檔案
description: 'null'
seo-description: 瞭解如何上傳範本檔案。
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 上載範本檔案{#uploading-template-files}

將範本所需的檔案上載到 Scene7 Publishing System，然後開始建置範本。可以從 Adobe® Photoshop® PSD 或影像檔案建置範本。建議使用 TIFF 和 PNG 影像，因為它們允許設定透明度。

>[!NOTE]
>
>Dynamic Media Classic建議在範本中使用透明TIFF或PSD影像，其大小與您要在網站上顯示的影像大小完全相同。 發佈範本時，呼叫的影像所帶的影像預設集大小亦相同。請注意，此大小可確保範本的大小不會調整 (重新取樣) 為大於或小於設計尺寸。

可以使用 Adobe Photoshop PSD 檔案或影像檔案建立範本。

有關上載檔案的詳細指示，請參閱[上載檔案](uploading-files.md#uploading_files)。上載範本檔案時請注意以下事項:

* 如果上載的是 PSD 檔案，則可以從該檔案建立範本。Dynamic Media Classic會為PSD中的每個圖層建立個別的影像。 在「上載工作選項」對話框中，選取「Photoshop 選項」，選取「保留圖層」選項，然後選取「建立範本」選項。然後，在「圖層命名」選單中選擇選項，以命名Dynamic Media Classic從PSD的圖層建立的影像。 請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。
* 如果上載的是影像，則可以從其剪裁路徑建立遮色片。此選項適用於使用影像編輯應用程式所建立而具有剪裁路徑的影像。在「上載工作選項」對話框中，選取「影像編輯選項」，然後選取「從剪裁路徑建立遮色片」選項。請參閱[上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)。

>[!MORELIKETHIS]
>
>* [上載檔案](uploading-files.md#uploading_your_files)
>* [使用 PSD 檔案](psd-files.md#working_with_psd_files)

