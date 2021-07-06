---
title: 上載主影像
description: 了解如何上傳主影像。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic，資產管理
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 19%

---

# 上載主影像{#uploading-master-images}

在將影像上傳至Dynamic Media Classic之前，請確定影像是最高品質的大小和格式。 Dynamic Media Classic建議上傳像素數充足的高品質影像（長度為1500到2000像素）。 此大小調整允許進行任何所需的動態影像處理。

如需上載影像的詳細資訊，請參閱[上載檔案](uploading-files.md#uploading_files)。

**準備主影像進行上載:**

將主影像檔案上傳至Dynamic Media Classic之前，請先準備這些檔案：

* **影像大小**  — 建立您預期使用的最大影像大小。一般影像大小最大為1500到2500像素。 如果您要使用縮放功能，Dynamic Media Classic建議使用大小最長至少為2000像素的影像，以獲得最佳的縮放詳細資料。 Dynamic Media Classic可以每個轉譯高達2500萬像素的影像。 例如，您可以使用5000 x 5000百萬像素影像或任何其它大小組合，最高2500萬像素。

* **檔案格式**  - Dynamic Media Classic支援所有標準影像檔案格式，包括TIFF、BMP、JPEG、PSD、GIF和EPS。建議使用不失真影像格式—TIFF 和 PNG。如果您使用JPEG影像，請使用最高品質的設定。

* **色域**  - RGB是Web影像呈現的色域；上傳時，常用於打印的CMYK影像會自動轉換為RGB。建議上載含有內嵌 ICC 色彩設定檔的 CMYK 影像，以供轉換為 RGB。請另參閱 [ICC 設定檔](/help/icc-profiles.md)。
