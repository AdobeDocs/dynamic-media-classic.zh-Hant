---
title: 「快速啟動：混合媒體集"
description: 介紹和混合媒體集快速入門，幫助您在Adobe Dynamic Media Classic快速啟動和運行。
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 34%

---

# 快速入門: 混合媒體集{#quick-start-mixed-media-sets}

 混合媒體集為使用者提供整合式的檢視體驗。混合媒體集可能包含影像、影像集、色票集、迴轉集和視訊。用戶可以在混合媒體查看器中選擇不同的頁籤，以查看不同查看器中的項。 如果未指定任何標籤，則所有的資產都會一併顯示於色票列中。

混合媒體集檢視器預設集包含了社群選項，可供終端使用者內嵌編碼、複製 URL 和連結至主網站。使用者可以使用這些選項，在個人網站或社交網站上分享產品資訊。

此混合媒體集快速啟動旨在通過混合媒體集技術在Adobe Dynamic Media Classic快速啟動和運行。

## 1。上載影像、色板檔案和視頻

先為混合媒體集上載影像、色票檔案和視訊。由於用戶可以在混合媒體集查看器中放大影像，因此在選擇影像時，請確保您考慮了此功能。 確保影像在最大大小中至少為2000像素。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 將檔案從電腦上傳到Adobe Dynamic Media Classic的資料夾。

請參閱 [上載檔案](uploading-files.md#uploading-your-files)。

## 2.建立介質集以在混合介質集中使用

您可以增加影像、影像集、色票集、迴轉集和視訊至混合媒體集。請先準備好媒體集，再將其增加至混合媒體集。

請參閱 [建立映像集](creating-image-set.md#creating-an-image-set)。 [建立色板集](creating-swatch-set.md#creating-a-swatch-set), [建立旋轉集](creating-spin-set.md#creating-a-spin-set)。

## 3.建立混合媒體集

在全局導航欄上，轉到 **[!UICONTROL 生成]** > **[!UICONTROL 混合媒體集]**。 將影像、色板集、影像集和視頻拖到「混合媒體集」頁上。 若要增加音軌，請將音訊檔案拖曳至「音軌」方框。

請參閱 [建立混合媒體集](creating-mixed-media-set.md#creating-a-mixed-media-set)。

## 4.設定混合媒體查看器預設

Adobe Dynamic Media Classic提供了混合媒體集的預設查看器預設。 管理員可以建立或修改混合媒體集檢視器預設集。

設定「混合媒體集」查看器預設時，請為您集中的所有其他資產添加查看器預設。 例如，如果您的混合媒體集包含視訊，則請增加視訊檢視器預設集至混合媒體集檢視器預設集。您也可以增加音軌至檢視器。音軌會在檢視器開啟時播放，但不會在視訊進行的同時播放。

請參閱 [設定混合媒體集查看器預設](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) 和 [建立和編輯查看器預設](application-setup.md#adding-and-editing-viewer-presets)。

另請參閱 [查看器預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 培訓視頻。

## 5.預覽混合媒體集

選擇混合媒體集 **[!UICONTROL 預覽]** 按鈕 可以選擇縮略圖和色板表徵圖，以在混合媒體集查看器中檢查混合媒體集。 您可以從「預設集」選單選擇不同的檢視器。

請參閱 [預覽資產](previewing-asset.md#previewing-an-asset)。

## 6。發佈混合媒體集

發佈混合媒體集將其放置在Adobe Dynamic Media Classic伺服器上並激活URL字串。

您需要將混合媒體集同時發佈至&#x200B;**視訊伺服器**&#x200B;與&#x200B;**影像伺服器**。您可以使用&#x200B;**視訊伺服器**&#x200B;來發佈標示為發佈的實際視訊，你用 **映像伺服器** 發佈相關資產（如視頻縮略圖），並設定任何自適應視頻集的資訊。

請參閱 [發佈混合媒體集](publishing-mixed-media-set.md#publishing-a-mixed-media-set)。

## 7。將混合媒體集連結到網頁

Adobe Dynamic Media Classic在您發佈混合媒體集後激活URL調用。 可以從「預覽」頁複製這些URL。

選擇混合媒體集，然後選擇 **[!UICONTROL 預覽]**。 在「預覽」頁中，選擇「混合媒體集查看器預設」，然後選擇 **[!UICONTROL 複製URL]**。 請參閱[將混合媒體集連結至網頁](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page)。
