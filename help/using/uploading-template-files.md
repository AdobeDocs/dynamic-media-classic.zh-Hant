---
title: 上傳範本檔案
description: 瞭解如何在Adobe Dynamic Media Classic中上傳範本檔案。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 32%

---

# 上傳範本檔案{#uploading-template-files}

在開始建立範本之前，請將範本所需的檔案上傳到Adobe Dynamic Media Classic。 您可以從Adobe®Photoshop®PSD或影像檔案建立範本。 建議使用 TIFF 和 PNG 影像，因為它們允許設定透明度。

>[!NOTE]
>
>Adobe Dynamic Media Classic建議您在範本中使用透明的TIFF或PSD影像，且大小應與您要顯示於網站上的大小完全相同。 發佈範本時，呼叫的影像所帶的影像預設集大小亦相同。請注意，此大小可確保範本的大小不會調整 (重新取樣) 為大於或小於設計尺寸。

可以使用 Adobe Photoshop PSD 檔案或影像檔案建立範本。

如需上傳檔案的詳細說明，請參閱 [上傳檔案](uploading-files.md#uploading_files). 上載範本檔案時請注意以下事項:

* 如果您要上傳PSD檔案，可從中建立範本。 Adobe Dynamic Media Classic會為PSD中的每個圖層建立個別影像。 在「上載工作選項」對話方塊中，選取 **[!UICONTROL Photoshop選項]**，並選取 **[!UICONTROL 保留圖層]** 和 **[!UICONTROL 建立範本]**. 然後，從 **[!UICONTROL 圖層命名]** 下拉式清單，用於命名Adobe Dynamic Media Classic從PSD圖層建立的影像。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [上傳檔案](uploading-files.md#uploading_your_files)
>* [使用PSD檔案](psd-files.md#working_with_psd_files)
