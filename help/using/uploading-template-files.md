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
autotag-review: '2026-05-13T19:58:21.817Z'
TQID: 'https://experienceleague.adobe.com/pwmEOjYzNJNV-yxeBfOz3xQBT3rJ9u9imU6cdNgQLDA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 9c30d97a0a8b110f966eec5901c6e1dc84590951
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 12%

---

# 上傳範本檔案{#uploading-template-files}

在開始建立範本之前，請將範本所需的檔案上傳到Adobe Dynamic Media Classic。 您可以從®Photoshop®PSD或影像檔案建置範本。 建議使用 TIFF 和 PNG 影像，因為它們允許設定透明度。

>[!NOTE]
>
>Adobe Dynamic Media Classic建議您在範本中使用透明的TIFF或PSD影像，且大小應與您要顯示在網站上的大小相同。 發佈範本時，請使用相同大小的影像預設集呼叫影像。 留意大小可確保範本不會調整大小（重新取樣）至大於或小於設計時的大小。

可以使用 Adobe Photoshop PSD 檔案或影像檔案建立範本。

如需上傳檔案的詳細說明，請參閱[上傳檔案](uploading-files.md#uploading_files)。 上傳範本檔案時，請考量下列事項：

* 如果您上傳PSD檔案，可從中建立範本。 Adobe Dynamic Media Classic會為PSD中的每個圖層建立個別的影像。 在「上載工作選項」對話方塊中，選取&#x200B;**[!UICONTROL Photoshop選項]**，然後選取&#x200B;**[!UICONTROL 維護圖層]**&#x200B;和&#x200B;**[!UICONTROL 建立範本]**。 然後從&#x200B;**[!UICONTROL 圖層命名]**&#x200B;下拉式清單中選擇選項，以命名Adobe Dynamic Media Classic從PSD的圖層建立的影像。
請參閱[PSD 上載選項](psd-files.md#psd_upload_options)。

<!--
THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). 
-->

>[!MORELIKETHIS]
>
>* [上傳您的檔案](uploading-files.md#uploading_your_files)
>* [使用PSD檔案](psd-files.md#working_with_psd_files)
