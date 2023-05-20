---
title: 上載模板檔案
description: 瞭解如何在Adobe Dynamic Media Classic上載模板檔案。
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 38%

---

# 上載模板檔案{#uploading-template-files}

在開始構建模板之前，將模板所需的檔案上載到Adobe Dynamic Media Classic。 可以從 Adobe® Photoshop® PSD 或影像檔案建置範本。建議使用 TIFF 和 PNG 影像，因為它們允許設定透明度。

>[!NOTE]
>
>Adobe Dynamic Media Classic建議在模板中使用透明TIFF或PSD影像，其大小與您希望在網站上顯示的大小相同。 發佈範本時，呼叫的影像所帶的影像預設集大小亦相同。請注意，此大小可確保範本的大小不會調整 (重新取樣) 為大於或小於設計尺寸。

可以使用 Adobe Photoshop PSD 檔案或影像檔案建立範本。

有關上載檔案的詳細說明，請參見 [上載檔案](uploading-files.md#uploading_files)。 上載範本檔案時請注意以下事項:

* 如果正在上載PSD檔案，則可以從該檔案建立模板。 Adobe Dynamic Media Classic為PSD中的每個圖層建立單獨的影像。 在「上載作業選項」對話框中，選擇 **[!UICONTROL Photoshop選項]**，然後選擇 **[!UICONTROL 維護層]** 和 **[!UICONTROL 建立模板]**。 然後，從 **[!UICONTROL 層命名]** 下拉清單，用於命名Adobe Dynamic Media Classic從PSD的圖層建立的影像。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [上載檔案](uploading-files.md#uploading_your_files)
>* [使用PSD檔案](psd-files.md#working_with_psd_files)

