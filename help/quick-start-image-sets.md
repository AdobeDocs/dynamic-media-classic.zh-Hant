---
title: "快速入門: 影像集"
description: 影像集簡介和快速入門，可協助您使用Adobe Dynamic Media Classic中的影像集技術快速上手並執行。
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# 快速入門: 影像集{#quick-start-image-sets}

Adobe Dynamic Media Classic影像集可為使用者提供整合的檢視體驗。 在動態影像集檢視器中，使用者按一下縮圖影像，就可以查看項目的不同檢視。影像集可讓您呈現項目的替代高解析度檢視。

影像集檢視器提供了縮放工具，以便近距離檢查影像。如果您想要，也可以讓已導引縮放目標和影像地圖成為您影像集的一部分。影像集能創造更一致且緊密的檢視體驗。

請參閱 [影像和回轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 訓練影片。

當您建立影像集時，Adobe會建議下列最佳作法並強制執行下列限制：

| 限制類型 | 最佳實務 | 限制 |
| --- | --- | --- |
| 每組重複資產數 | 無重複項目 | 20 |
| 每組影像的最大數量 | 每組5-10頁影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

以下「影像集快速入門」旨在通過Adobe Dynamic Media Classic中的「影像集」技術快速啟動並運行。

## 1.上傳多個檢視和色票的主要影像

請先為影像集上載影像。由於使用者可以在影像集檢視器中放大影像，因此在選擇影像時，請務必說明這項功能。 請確定影像大小最大時至少為2000像素。 Adobe Dynamic Media Classic支援許多影像檔案格式，但建議使用無損TIFF、PNG和EPS影像。

在全局導航欄上，選擇 **[!UICONTROL 上傳]** 將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。

請參閱 [準備影像集資產以供上傳](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 和 [上傳您的檔案](uploading-files.md#uploading-your-files).

## 2.建立影像集

在「影像集」中，用戶在「影像集查看器」中選擇縮圖影像，以從不同的側面或角度查看影像。

要建立影像集，請在全局導航欄上，選擇 **[!UICONTROL 建置]**，然後選擇 **[!UICONTROL 影像集]**. 在「影像集」視窗中，將影像拖曳至頁面以組成影像集。 視需求組織、新增和刪除影像。

請參閱 [建立影像集](creating-image-set.md#creating-an-image-set).

另請參閱 [在影像集中包含縮放目標和影像映射](/help/including-zoom-targets-image-maps-image-sets.md)

## 3.視需要準備影像集檢視器預設集

管理員可以建立或修改影像集檢視器預設集。Adobe Dynamic Media Classic隨附每個多媒體類型的預設檢視器預設集。 使用縮放檢視器： **[!UICONTROL 自訂]** > **[!UICONTROL 影像]** 或 **[!UICONTROL 影像集]**/**[!UICONTROL 多次檢視]** 用於查看影像集的預設集。

您可以從「應用程式設定」畫面增加或編輯檢視器預設集。

請參閱 [建立和編輯查看器預設集](application-setup.md#adding-and-editing-viewer-presets).

## 4.預覽影像集

在「瀏覽」面板中選擇「影像集」，然後選擇 **[!UICONTROL 預覽]**. 在「預覽」頁面中，選取縮圖圖示以檢查所選檢視器中的影像集。 您可以從「預設集」選單選擇不同的檢視器。

請參閱 [預覽資產](previewing-asset.md#previewing-an-asset).

## 5.發佈影像集

發佈影像集會將其置於Adobe Dynamic Media Classic伺服器上並啟用URL字串。

>[!NOTE]
>
>如果在您建立和儲存影像集時選取了「**[!UICONTROL 儲存後發佈]**」(預設)，則此步驟並非必要。

選擇 **[!UICONTROL 標籤為發佈]** 表徵圖。 然後，選取 **[!UICONTROL 發佈]**. 在「發佈」頁面上，選取 **[!UICONTROL 提交發佈]**.

請參閱 [發佈檔案](publishing-files.md#publishing-files).

## 6.將影像集連結至您的網站

Adobe Dynamic Media Classic會建立影像集的URL呼叫，並在您發佈後啟用它們。 您可以從「預覽」畫面複製這些 URL。

選取影像集，然後選取 **[!UICONTROL 預覽]**. 現在，請選取「影像集檢視器預設集」，然後選取 **[!UICONTROL 複製URL]**.

請參閱 [將影像集連結至網頁](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
