---
title: '快速入門: 影像調整大小'
description: 影像大小調整的簡介和快速入門，協助您快速上手，使用Adobe Dynamic Media Classic中的影像大小調整技術。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
autotag-review: '2026-05-13T20:09:57.533Z'
TQID: 'https://experienceleague.adobe.com/VGp4OQ03iRiobXKWuUERNtFwUMQ4z7a19wyOgHWuv3w'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 202f477d78272c66d0ac490e3a5041839b3e4f4d
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 5%

---

# 快速入門: 影像調整大小{#quick-start-image-sizing}

影像大小調整是指Adobe Dynamic Media Classic根據單一高解析度影像建立多個衍生影像的能力。 您提供的不是手動為網站或應用程式建立數個影像，而是單一主要影像。 Adobe Dynamic Media Classic會在您請求修改影像時產生所有影像。 從單一主要影像動態傳送影像有許多優點：

* 不需要手動建立多個不同大小的影像復本。 您提供一個主要影像給Adobe Dynamic Media Classic，它就會從主要影像產生不同大小的衍生物。
* 您可以在整個網站或應用程式中快速變更影像大小。 例如，若要變更所有縮圖影像，您可以修改「縮圖」影像預設集。 影像預設集是大小和格式屬性之集合。 若要變更整個網站或應用程式中所有縮圖影像的大小，您可以修改「縮圖」影像預設集。
* 您不需要管理任何內容或資產管理系統中的主要檔案或所有各種衍生專案。

![您可以建立多個衍生影像，其大小與相同的高解析度主要檔案不同](/help/using/assets/is_derivative_sizes_popup.png)。

請參閱[影像大小： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

下列影像大小調整快速入門旨在協助您開始使用Adobe Dynamic Media Classic中的影像大小調整技術。 完成步驟1-5。 每個步驟之後都會有互動參照，您可以在需要資訊時找到更多資訊。

## &#x200B;1. 上傳主要影像

將主要影像上傳至Adobe Dynamic Media Classic。 Adobe Dynamic Media Classic建議使用您預期在網站或應用程式上使用之最大大小的影像。 例如，如果您希望檢視器縮放影像，請上傳大小至少為2000畫素的影像。 Adobe Dynamic Media Classic支援許多影像檔案格式，但建議使用不失真TIFF和PNG影像。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。 請參閱[上傳主要影像](uploading-master-images.md#uploading_master_images)。

## &#x200B;2. 設定影像預設集

影像預設集是以名稱儲存的預定義大小和格式指令集合。 影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 如果您處於「公司管理員」狀態，可以獨立設定影像預設集。 您可以使用Adobe Dynamic Media Classic隨附的預設影像預設集，以動態方式傳送影像。

若要建立影像預設集（如果您是管理員），請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設集]**。 然後選取「**[!UICONTROL 新增]**」以建立影像預設集，或選取「**[!UICONTROL 編輯]**」以變更現有的影像預設集。

您建立的影像預設集會新增至「預覽」頁面上的「影像預設集」選單。 您可以使用新的影像預設集，在網站和應用程式上動態顯示影像。 請參閱[設定影像預設集](setting-image-presets.md#setting_up_image_presets)。

## &#x200B;3. 預覽影像預設集

下一步是以不同預設集大小預覽管理員所設定的影像預設集。

若要探索影像預設集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**，然後瀏覽至影像預設集。

測試不同的影像預設集。 判斷影像以不同大小動態方式傳送到您的網站或應用程式時影像的顯示方式。

請參閱[根據影像預設集預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)。

## &#x200B;4. 發佈您的主要影像

發佈主要影像檔案有兩個基本目的：

* 將您的主要影像發佈至Dynamic Media影像伺服器，以便影像可以動態傳遞至您的網站和應用程式。
* 發佈會啟用URL字串，以將影像從Dynamic Media影像伺服器呼叫至您的網站或應用程式。 發佈後，您可以視需要複製Adobe Dynamic Media Classic產生的URL，並將其放置在網站或應用程式中。

在全域導覽列上，選取&#x200B;**[!UICONTROL 發佈]**&#x200B;以開始發佈工作。 在[發佈]對話方塊中，選取&#x200B;**[!UICONTROL 送出發佈]**。 請參閱[發佈主要影像](publishing-master-images.md#publishing_master_images)。

## &#x200B;5. 將URL連結至您的網頁應用程式

Adobe Dynamic Media Classic會建立影像的URL圖說文字串。 將影像發佈至Dynamic Media影像伺服器時，URL會變成作用中。 您可以從「瀏覽」面板（在「詳細資料檢視」中）或「預覽」畫面複製這些URL字串。 複製URL字串後，即可在網站或應用程式中使用。 「調整影像大小」的URL會取代網頁程式碼中靜態影像名稱的參照。 URL會參照資料庫針對每個顯示的新影像所取代的主要影像名稱。

使用影像預設集產生的 URL 字串會包含一個影像預設集的名稱。 此名稱以美元符號(`$`)括住。 例如，`$thumbnail$`可以是設計成以縮圖大小顯示主要影像的影像預設集。 檢視[將URL連結至您的網頁應用程式](linking-urls-web-application.md#linking_urls_to_your_web_application)。
