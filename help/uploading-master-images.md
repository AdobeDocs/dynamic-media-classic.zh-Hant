---
title: 上載主映像
description: 瞭解如何將主映像上載到Adobe Dynamic Media Classic。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 2%

---

# 上載主映像{#uploading-master-images}

在將影像上傳到Adobe Dynamic Media Classic之前，請確保它們是最高質量的大小和格式。 Adobe Dynamic Media Classic建議上傳具有足夠像素數（1500到2000像素長）的高質量影像。 此大小調整允許任何需要的Dynamic Imaging。

有關上載影像的詳細資訊，請參閱 [上載檔案](uploading-files.md#uploading_files)。

**準備要上載的主映像：**

在將主映像檔案上載到Adobe Dynamic Media Classic之前，請先準備它們：

* **影像大小**  — 建立您預期使用的最大大小影像。 典型影像大小在1500到2500像素之間，最長大小。 如果要使用「縮放」功能，Adobe Dynamic Media Classic建議使用最長大小至少為2000像素的影像來優化縮放細節。 Adobe Dynamic Media Classic可以每張2500萬像素的影像。 例如，您可以使用5000 x 5000 MP的映像或任何其他大小組合，最多25 MP。

* **檔案格式** -Adobe Dynamic Media Classic支援所有標準影像檔案格式，包括TIFF、BMP、JPEG、PSD、GIF和EPS。 建議使用不失真影像格式—TIFF 和 PNG。如果使用的是JPEG影像，請使用最高質量的設定。

* **顏色空間** -RGB是Web影像演示的顏色空間；在上載常用於打印的CMYK影像時，它們會自動轉換為RGB。 建議上載具有嵌入的ICC（國際顏色聯盟）顏色配置檔案的CMYK影像，以便轉換為RGB。 另請參閱 [ICC（國際顏色聯盟）配置檔案](/help/icc-profiles.md)。
