---
title: "快速入門: 影像調整大小"
description: 簡介和快速開始調整影像大小，幫助您快速啟動並運行Adobe Dynamic Media Classic的影像調整技術。
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

Image Sizing是指Adobe Dynamic Media Classic能夠根據單個高解析度影像建立多個導數影像。 您不會為網站或應用程式手動建立多個影像（例如縮略圖和放大視圖影像），而是提供單個主影像。 Adobe Dynamic Media Classic會根據您的請求生成所有修改的影像。 能夠從單個主映像動態提供映像有許多優點：

* 您不需手動建立不同大小的數個影像複本。您向Adobe Dynamic Media Classic提供一個主映像，而Adobe Dynamic Media Classic會從主映像生成不同大小的導數。
* 您可以快速變更網站或應用程式內某個影像類型的大小。例如，若要變更所有的縮圖影像，您可以修改「縮圖」影像預設集。影像預設集類似巨集，它是一種大小和格式屬性的集合。您可以修改「縮圖」影像預設集，以變更網站或應用程式中所有縮圖影像的大小。
* 您不必在內部或外部管理任何內容或資產管理系統中的主要檔案和所有衍生產品。

![您可以建立不同大小的多個衍生影像，這些影像與同一高解析度主檔案不同。](/help/assets/is_derivative_sizes_popup.png)

請參閱 [影像大小調整：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) 培訓視頻。

以下影像調整快速入門旨在通過Adobe Dynamic Media Classic的影像調整技術幫助您快速啟動和運行。 執行步驟1-5。 在每個步驟之後，都會有一個交叉引用，在該交叉引用中，您可以根據需要找到更多資訊。

## 1。上載主映像

首先將主映像上載到Adobe Dynamic Media Classic。 至於大小，Adobe Dynamic Media Classic建議使用您預期在網站或應用程式上使用的最大大小的影像。 例如，如果希望查看者縮放影像，請上載最大大小至少為2000像素的影像。 Adobe Dynamic Media Classic支援多種影像檔案格式，但建議使用無損TIFF和PNG影像。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 將檔案從電腦上傳到Adobe Dynamic Media Classic的資料夾。 請參閱 [上載主映像](uploading-master-images.md#uploading_master_images)。

## 2.設定影像預設

如同巨集，影像預設集是儲存於同一個名稱下的預先定義大小和格式命令集合。「影像預設」控制從Dynamic Media影像伺服器傳送影像的大小和格式。 如果您擁有公司管理員狀態，便可以自行設定影像預設集。Adobe Dynamic Media Classic還附帶了預設的「影像預設」，您可以使用它們動態傳送影像。

要建立「影像預設」（如果您是管理員），請在「全局導航」欄上轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設]**。 然後選擇 **[!UICONTROL 添加]** 建立影像預設，或選擇 **[!UICONTROL 編輯]** 更改現有影像預設。

您建立的「影像預設」將添加到「預覽」頁面的「影像預設」菜單。 您可以使用新影像預設集，在網站和應用程式中動態顯示影像。請參閱 [設定影像預設](setting-image-presets.md#setting_up_image_presets)。

## 3.預覽影像預設

下一步是以不同預設集大小預覽管理員所設定的影像預設集。

要瀏覽「影像預設」，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設]**，然後瀏覽到「影像預設」。

以不同的影像預設集進行實驗。瞭解以不同大小動態將影像傳送到網站或應用程式時的顯示方式。

請參閱 [根據影像預設預覽影像資源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)。

## 4.發佈主映像

發佈主映像檔案有兩個基本目的：

* 將主映像發佈到Dynamic Media映像伺服器，以便可以動態地將映像交付到您的網站和應用程式。
* 發佈激活URL字串，用於從Dynamic Media映像伺服器將映像調用到網站或應用程式。 發佈後，您可以在網站或應用程式中根據需要複製和放置Adobe Dynamic Media Classic生成的URL。

在全局導航欄上，選擇 **[!UICONTROL 發佈]** 來啟動發佈作業。 在「發佈」(Publish)對話框中，選擇 **[!UICONTROL 提交發佈]**。 請參閱 [發佈主映像](publishing-master-images.md#publishing_master_images)。

## 5.將URL連結到Web應用程式

Adobe Dynamic Media Classic為影像建立URL標注字串。 將影像發佈到Dynamic Media映像伺服器時，URL將變為活動狀態。 您可以從「瀏覽面板」（在「詳細資訊視圖」中）或「預覽」螢幕複製這些URL字串。 複製 URL 字串後，您便可以在網站和應用程式中使用這些字串。影像調整大小的 URL 會將參照取代為網頁代碼中的靜態影像名稱。該URL引用主映像名稱，該名稱由資料庫替換，用於顯示每個新映像。

使用影像預設集產生的 URL 字串會包含一個影像預設集的名稱。此名稱用美元符號括起來(`$`)。 比如說， `$thumbnail$` 可以是設計為以縮略圖大小顯示主影像的「影像預設」。 請參閱 [將URL連結到Web應用程式](linking-urls-web-application.md#linking_urls_to_your_web_application)。
