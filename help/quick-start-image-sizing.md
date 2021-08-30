---
title: '"快速入門: 影像調整大小"'
description: 簡介和影像調整快速入門，協助您快速上手並執行Dynamic Media Classic中的影像調整技術。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 31%

---

# 快速入門: 影像調整大小{#quick-start-image-sizing}

「影像大小調整」是指AdobeDynamic Media Classic根據單一高解析度影像建立多個衍生影像的功能。 您不需要手動為網站或應用程式建立數個影像（例如縮圖和放大檢視影像），而是提供單一主影像。 AdobeDynamic Media Classic會依您的要求產生所有修改的影像。 能夠動態地從單一主影像傳送影像有許多好處:

* 您不需手動建立不同大小的數個影像複本。您提供一個主影像以AdobeDynamic Media Classic，而AdobeDynamic Media Classic會從主影像產生不同大小的衍生影像。
* 您可以快速變更網站或應用程式內某個影像類型的大小。例如，若要變更所有的縮圖影像，您可以修改「縮圖」影像預設集。影像預設集類似巨集，它是一種大小和格式屬性的集合。您可以修改「縮圖」影像預設集，以變更網站或應用程式中所有縮圖影像的大小。
* 您無需在內部或外部管理任何內容或資產管理系統中的主版和所有各種衍生工具。

![您可以建立與同一高解析度主檔案大小不同的多個衍生影像。](/help/assets/is_derivative_sizes_popup.png)

本影像大小調整快速入門旨在協助您快速上手，並運用Dynamic Media Classic中的影像大小調整技術來Adobe。 請執行步驟1-5。 每一個步驟之後都有交互參照，可讓您在需要時尋找更多資訊。

## 1.上傳主影像

首先，請上傳主影像至AdobeDynamic Media Classic。 至於大小，AdobeDynamic Media Classic建議使用您預期在網站或應用程式中使用的最大大小影像。 例如，如果您想要檢視器縮放影像，請上傳大小最大且至少為2000像素的影像。 AdobeDynamic Media Classic支援許多影像檔案格式，但建議使用無損TIFF和PNG影像。

在全域導覽列上，選取&#x200B;**[!UICONTROL Upload]** ，將檔案從電腦上傳至Dynamic Media ClassicAdobe上的資料夾。 請參閱[上傳主影像](uploading-master-images.md#uploading_master_images)。

## 2.設定影像預設集

如同巨集，影像預設集是儲存於同一個名稱下的預先定義大小和格式命令集合。影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 如果您擁有公司管理員狀態，便可以自行設定影像預設集。AdobeDynamic Media Classic也隨附預設的影像預設集，您可以使用這些預設集動態傳送影像。

要建立影像預設集（如果您是管理員），請在全局導航欄上轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]**。 然後，選擇&#x200B;**[!UICONTROL Add]**&#x200B;以建立影像預設集，或選擇&#x200B;**[!UICONTROL Edit]**&#x200B;以更改現有的影像預設集。

您建立的影像預設集會新增至「預覽」頁面上的「影像預設集」功能表。 您可以使用新影像預設集，在網站和應用程式中動態顯示影像。請參閱[設定影像預設集](setting-image-presets.md#setting_up_image_presets)。

## 3.預覽影像預設集

下一步是以不同預設集大小預覽管理員所設定的影像預設集。

若要探索「影像預設集」，請在全域導覽列上前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**，然後瀏覽至影像預設集。

以不同的影像預設集進行實驗。了解以不同大小動態傳送影像至網站或應用程式時，影像的顯示方式。

請參閱「根據影像預設集預覽影像資產」。[](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

## 4.發佈主影像

發佈主影像檔案有兩個主要目的:

* 將主影像發佈至Dynamic Media影像伺服器，以便以動態方式將影像傳送至您的網站和應用程式。
* 發佈會啟用URL字串，用於從Dynamic Media影像伺服器呼叫您的網站或應用程式的影像。 發佈後，您可以視需要在網站或應用程式中複製並放置AdobeDynamic Media Classic產生的URL。

在全局導航欄上，選擇&#x200B;**[!UICONTROL Publish]**&#x200B;以啟動發佈作業。 在「發佈」對話框中，選擇「提交發佈」**[!UICONTROL 。]**&#x200B;請參閱[發佈主影像](publishing-master-images.md#publishing_master_images)。

## 5.將URL連結至您的Web應用程式

AdobeDynamic Media Classic會建立影像的URL圖說字串。 當您將影像發佈至Dynamic Media影像伺服器時，URL會變成作用中。 您可以從「瀏覽面板」（在「詳細資訊檢視」中）或「預覽」畫面複製這些URL字串。 複製 URL 字串後，您便可以在網站和應用程式中使用這些字串。影像調整大小的 URL 會將參照取代為網頁代碼中的靜態影像名稱。URL 會參照主影像名稱，而該名稱會被要顯示之新影像的資料庫取代。

使用影像預設集產生的 URL 字串會包含一個影像預設集的名稱。此名稱以貨幣符號括住(`$`)。 例如， `$thumbnail$`可以是設計為以縮圖大小顯示主影像的影像預設集。 請參閱[將URL連結到您的Web應用程式](linking-urls-web-application.md#linking_urls_to_your_web_application)。
