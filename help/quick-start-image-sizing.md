---
title: "快速入門: 影像調整大小"
description: 影像大小調整的簡介和快速入門，可協助您快速上手並執行Adobe Dynamic Media Classic中的影像大小調整技術。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 22%

---

# 快速入門: 影像調整大小{#quick-start-image-sizing}

影像大小調整是指Adobe Dynamic Media Classic根據單一高解析度影像建立多個衍生影像的能力。 您提供的不是手動為網站或應用程式建立多個影像（例如縮圖和放大檢視影像），而是單一主影像。 Adobe Dynamic Media Classic會依照您的要求產生所有修改的影像。 能夠從單個主映像動態地傳送映像有許多優點：

* 您不需手動建立不同大小的數個影像複本。您向Adobe Dynamic Media Classic提供一個主映像，而Adobe Dynamic Media Classic會從主映像生成不同大小的衍生工具。
* 您可以快速變更網站或應用程式內某個影像類型的大小。例如，若要變更所有的縮圖影像，您可以修改「縮圖」影像預設集。影像預設集類似巨集，它是一種大小和格式屬性的集合。您可以修改「縮圖」影像預設集，以變更網站或應用程式中所有縮圖影像的大小。
* 您不必在內部或外部管理任何內容或資產管理系統中的主要檔案和所有各種衍生工具。

![您可以建立與同一高解析度主檔案大小不同的多個衍生影像。](/help/assets/is_derivative_sizes_popup.png)

請參閱 [影像大小調整：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) 訓練影片。

以下「影像調整大小快速入門」旨在協助您使用Adobe Dynamic Media Classic中的「影像調整大小」技術快速上手並執行。 請執行步驟1-5。 在每個步驟之後，都會提供交叉參考，您可以在其中尋找更多資訊（如果需要）。

## 1.上傳主要影像

首先，請將主要影像上傳至Adobe Dynamic Media Classic。 至於大小，Adobe Dynamic Media Classic建議使用您預期在網站或應用程式中使用的最大大小影像。 例如，如果您想要檢視器縮放影像，請上傳大小最大且至少為2000像素的影像。 Adobe Dynamic Media Classic支援許多影像檔案格式，但建議使用無損TIFF和PNG影像。

在全局導航欄上，選擇 **[!UICONTROL 上傳]** 將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。 請參閱 [上傳主要影像](uploading-master-images.md#uploading_master_images).

## 2.設定影像預設集

如同巨集，影像預設集是儲存於同一個名稱下的預先定義大小和格式命令集合。影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 如果您擁有公司管理員狀態，便可以自行設定影像預設集。Adobe Dynamic Media Classic也隨附預設的影像預設集，您可以使用這些預設集來動態傳送影像。

若要建立影像預設集（如果您是管理員），請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設集]**. 然後選取 **[!UICONTROL 新增]** 建立影像預設集，或選擇 **[!UICONTROL 編輯]** 來更改現有的「影像預設集」。

您建立的影像預設集會新增至「預覽」頁面上的「影像預設集」功能表。 您可以使用新影像預設集，在網站和應用程式中動態顯示影像。請參閱 [設定影像預設集](setting-image-presets.md#setting_up_image_presets).

## 3.預覽影像預設集

下一步是以不同預設集大小預覽管理員所設定的影像預設集。

要瀏覽「影像預設集」，請在全局導航欄上轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**，然後瀏覽至影像預設集。

以不同的影像預設集進行實驗。了解以不同大小動態傳送影像至網站或應用程式時，影像的顯示方式。

請參閱 [根據影像預設集預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4.發佈主映像

發佈主要影像檔案有兩個重要用途：

* 將您的主要影像發佈至Dynamic Media影像伺服器，以便以動態方式將影像傳送至您的網站和應用程式。
* 發佈會啟用URL字串，用於從Dynamic Media影像伺服器呼叫您的網站或應用程式的影像。 發佈後，您可以視需要在網站或應用程式中複製並放置Adobe Dynamic Media Classic產生的URL。

在全局導航欄上，選擇 **[!UICONTROL 發佈]** 來啟動發佈作業。 在「發佈」(Publish)對話框中，選擇 **[!UICONTROL 提交發佈]**. 請參閱 [發佈主映像](publishing-master-images.md#publishing_master_images).

## 5.將URL連結至您的Web應用程式

Adobe Dynamic Media Classic會建立影像的URL圖說字串。 當您將影像發佈至Dynamic Media影像伺服器時，URL會變成作用中。 您可以從「瀏覽面板」（在「詳細資訊檢視」中）或「預覽」畫面複製這些URL字串。 複製 URL 字串後，您便可以在網站和應用程式中使用這些字串。影像調整大小的 URL 會將參照取代為網頁代碼中的靜態影像名稱。URL會參考主要影像名稱，而資料庫會取代該名稱，以顯示每個新影像。

使用影像預設集產生的 URL 字串會包含一個影像預設集的名稱。此名稱括在貨幣符號中(`$`)。 例如， `$thumbnail$` 可以是設計為以縮圖大小顯示主影像的影像預設集。 請參閱 [將URL連結至您的Web應用程式](linking-urls-web-application.md#linking_urls_to_your_web_application).
