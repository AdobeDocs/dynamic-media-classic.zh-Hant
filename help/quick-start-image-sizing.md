---
title: '"快速入門: 影像調整大小"'
seo-title: '"快速入門: 影像調整大小"'
description: 'null'
seo-description: 影像調整功能簡介和快速入門，協助您使用影像調整大小技術快速啓動和執行。
uuid: 6c4ad4b7-549d-4da-b6 b9-5997a8427 a8
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENT_ PK/categories/image_ size
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 快速入門: 影像調整大小{#quick-start-image-sizing}

影像調整大小是指Dynamic Media Classic能夠根據單一高解析度影像建立多個衍生影像的能力。您不需手動為網站或應用程式建立數個影像，例如縮圖和放大檢視影像，而是提供單一主影像。Dynamic Media Classic會隨著您要求，產生所有修改過的影像。能夠動態地從單一主影像傳送影像有許多好處:

* 您不需手動建立不同大小的數個影像複本。您可以提供一個主要影像至Dynamic Media Classic，而Dynamic Media Classic則會從主影像產生不同大小的衍生產品。
* 您可以快速變更網站或應用程式內某個影像類型的大小。例如，若要變更所有的縮圖影像，您可以修改「縮圖」影像預設集。影像預設集類似巨集，它是一種大小和格式屬性的集合。您可以修改「縮圖」影像預設集，以變更網站或應用程式中所有縮圖影像的大小。
* 您不需從內部或外部管理任何內容或資產管理系統中的主影像及所有衍生影像。

![您可以建立不同於相同高解析度主檔案的多個衍生影像。](/help/assets/is_derivative_sizes_popup.png)

**快速入門**

此「影像調整大小快速入門」的設計可讓您迅速熟練 Scene7 Publishing System 中的影像調整大小技術。遵循步驟1-5。每一個步驟之後都有交互參照，可讓您在需要時尋找更多資訊。

**1. 上載主影像**

先將您的主影像上載至 Scene7 Publishing System。就規模而言，Dynamic Media Classic建議您使用您預期在網站或應用程式中使用的最大大小影像。例如，如果您要檢視器縮放影像，請上載最大維度至少 2000 像素的影像。Dynamic Media Classic支援許多影像檔案格式，但是建議使用無失真TIFF和PNG影像。

選取全域導覽列上的「上載」按鈕，將您電腦的檔案上載至 Scene7 Publishing System 中的檔案夾。請參閱[上載主影像](uploading-master-images.md#uploading_master_images)。

**2. 設定影像預設集**

如同巨集，影像預設集是儲存於同一個名稱下的預先定義大小和格式命令集合。影像預設集管理從動態媒體影像伺服器傳送影像的大小和格式。如果您擁有公司管理員狀態，便可以自行設定影像預設集。Dynamic Media Classic也隨附預設的影像預設集，您可使用這些預設集來動態傳送影像。

若要建立影像預設集 (如果您是管理員)，請選擇「設定 &gt; 應用程式設定」。在「設定」畫面上，顯示「應用程式設定」選項，並選擇「影像預設集」。然後按一下 **「新增** 」或 **「編輯** 」以建立影像預設集。

您建立的影像預設集會增加至「預覽」畫面的「影像預設集」選單。您可以使用新影像預設集，在網站和應用程式中動態顯示影像。請參閱[設定影像預設集](setting-image-presets.md#setting_up_image_presets)。

**3. 預覽影像預設集**

下一步是以不同預設集大小預覽管理員所設定的影像預設集。

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

以不同的影像預設集進行實驗。看看您的影像在以不同大小動態傳送至網站或應用程式時的外觀。

請參閱[依據影像預設集來預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)。

**4. 發佈主影像**

發佈主影像檔案有兩個主要目的:

* 將您的主影像發佈至動態媒體影像伺服器，以便動態地將影像傳送至您的網站和應用程式。
* Publishing會啓動URL字串，以便從動態媒體影像伺服器呼叫影像至您的網站或應用程式。發佈後，您可以在網站或應用程式中複製並放置動態媒體Classic產生的URL。

選取全域導覽列上的「發佈」按鈕以啟動發佈。在「發佈」畫面上選取「開始發佈」按鈕。請參閱[發佈主影像](publishing-master-images.md#publishing_master_images)。

**5. 將 URL 連結至網路應用程式**

Dynamic Media Classic會建立影像的URL標記字串。當您將影像發佈至動態媒體影像伺服器時，URL會變成作用中。您可以從瀏覽面板(在詳細檢視中的)或「預覽」畫面複製這些 URL 字串。複製 URL 字串後，您便可以在網站和應用程式中使用這些字串。影像調整大小的 URL 會將參照取代為網頁代碼中的靜態影像名稱。URL 會參照主影像名稱，而該名稱會被要顯示之新影像的資料庫取代。

使用影像預設集產生的 URL 字串會包含一個影像預設集的名稱。This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. 請參閱[將 URL 連結至網路應用程式](linking-urls-web-application.md#linking_urls_to_your_web_application)。
