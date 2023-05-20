---
title: "快速入門: 影像集"
description: 介紹和快速啟動映像集，幫助您快速啟動和運行Adobe Dynamic Media Classic的映像集技術。
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

Adobe Dynamic Media Classic影像集為用戶提供綜合的觀看體驗。 在動態影像集檢視器中，使用者按一下縮圖影像，就可以查看項目的不同檢視。「影像集」(Image Sets)用於顯示項目的替代高解析度視圖。

影像集檢視器提供了縮放工具，以便近距離檢查影像。如果您想要，也可以讓已導引縮放目標和影像地圖成為您影像集的一部分。影像集能創造更一致且緊密的檢視體驗。

請參閱 [影像和旋轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 培訓視頻。

建立映像集時，Adobe建議採用以下最佳做法並強制實施以下限制：

| 限制類型 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每集重複的資產數 | 無重複項 | 20 |
| 每集的最大影像數 | 每組5-10頁影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md)。

以下映像集快速啟動旨在利用Adobe Dynamic Media Classic的映像集技術快速啟動和運行。

## 1。上載多個視圖和色板的主影像

請先為影像集上載影像。由於用戶可以在「影像集查看器」中放大影像，因此在選擇影像時，請確保考慮此功能。 確保影像在最大大小中至少為2000像素。 Adobe Dynamic Media Classic支援多種影像檔案格式，但建議使用無損TIFF、PNG和EPS影像。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 將檔案從電腦上傳到Adobe Dynamic Media Classic的資料夾。

請參閱 [準備映像集資產以供上載](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 和 [上載檔案](uploading-files.md#uploading-your-files)。

## 2.建立映像集

在「影像集」中，用戶在「影像集查看器」中選擇縮略圖，以從不同的側面或角度查看影像。

要建立影像集，請在全局導航欄上選擇 **[!UICONTROL 生成]**，然後選擇 **[!UICONTROL 影像集]**。 在「影像集」窗口中，將影像拖到頁面上以合成影像集。 視需求組織、新增和刪除影像。

請參閱 [建立映像集](creating-image-set.md#creating-an-image-set)。

另請參閱 [在影像集中包括縮放目標和影像映射](/help/including-zoom-targets-image-maps-image-sets.md)

## 3.根據需要準備影像集查看器預設

管理員可以建立或修改影像集檢視器預設集。Adobe Dynamic Media Classic為每個富媒體類型都提供預設的查看器預設。 使用縮放查看器： **[!UICONTROL 自定義]** > **[!UICONTROL 影像]** 或 **[!UICONTROL 影像集]**/**[!UICONTROL 多個視圖]** 影像集。

您可以從「應用程式設定」畫面增加或編輯檢視器預設集。

請參閱 [建立和編輯查看器預設](application-setup.md#adding-and-editing-viewer-presets)。

## 4.預覽影像集

在「瀏覽」面板中選擇「影像集」，然後選擇 **[!UICONTROL 預覽]**。 在「預覽」頁中，選擇縮略圖表徵圖以檢查選定查看器中的影像集。 您可以從「預設集」選單選擇不同的檢視器。

請參閱 [預覽資產](previewing-asset.md#previewing-an-asset)。

## 5.發佈映像集

發佈映像集將其放在Adobe Dynamic Media Classic伺服器上並激活URL字串。

>[!NOTE]
>
>如果在您建立和儲存影像集時選取了「**[!UICONTROL 儲存後發佈]**」(預設)，則此步驟並非必要。

選擇 **[!UICONTROL 標籤為發佈]** 表徵圖。 然後，選擇 **[!UICONTROL 發佈]**。 在「發佈」頁面上，選擇 **[!UICONTROL 提交發佈]**。

請參閱 [發佈檔案](publishing-files.md#publishing-files)。

## 6。將映像集連結到您的網站

Adobe Dynamic Media Classic建立映像集的URL調用，並在您發佈後激活它們。 您可以從「預覽」畫面複製這些 URL。

選擇影像集，然後選擇 **[!UICONTROL 預覽]**。 現在選擇影像集查看器預設，然後選擇 **[!UICONTROL 複製URL]**。

請參閱 [將影像集連結到網頁](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page)。
