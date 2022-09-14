---
title: "快速入門: 縮放"
description: 簡介和快速入門縮放功能可協助您快速上手並執行。
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 25%

---

# 快速入門: 縮放{#quick-start-zoom}

縮放可讓您以互動方式檢視影像中的高解析度詳細資訊。 例如，可以在動態的、可完全設定的整合檢視器中查看影像的色彩、選項、角度以及細節。此檢視器可以內嵌在網頁中，也可以顯示在彈出式視窗中。您可以在近距離審核影像，並以高解析度平移影像，以密切檢查影像。 縮放功能可以為您的客戶帶來豐富多彩的互動式視覺效果。

Adobe Dynamic Media Classic也提供引導式縮放功能，這是您反白標示影像重要功能的方式。 例如，若要將檢視者的注意力集中於某個標誌上，可以為該標誌建立一個縮放目標。當使用者選取此縮放目標時，會縮放至標誌。

所有縮放影像都是從單一主影像、圖形和資料庫驅動屬性建立並提供的。 Adobe Dynamic Media Classic縮放可大幅減少影像製作和傳送的時間和成本。 您可以使用縮放檢視器來放大和縮小影像。 縮放查看器中有一些按鈕可供選擇，以縮放和平移；您也可以在螢幕上拖曳進行平移。 透過縮放檢視器預設集，可以設定要用於縮放影像的縮放檢視器。

請參閱 [縮放目標：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS) 和 [縮放：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS) 訓練影片。

以下「縮放快速入門」是專為協助您快速上手而設計，其中包含Adobe Dynamic Media Classic中的「縮放」技術。 依照步驟 1 至 6 執行。在每個步驟之後，都會提供主題標題的交叉參考，您可在其中找到詳細資訊。

## 1.上傳縮放影像

首先，將縮放影像上傳至Adobe Dynamic Media Classic。 為獲得最佳縮放比例，Adobe Dynamic Media Classic建議影像大小最長至少為2000像素。

在全局導航欄上，選擇 **[!UICONTROL 上傳]** 將影像從您的電腦或網路上傳至Adobe Dynamic Media Classic上的資料夾。 請參閱 [上傳縮放影像](uploading-zoom-images.md#uploading_zoom_images).

## 2.建立縮放目標以進行引導式縮放

縮放目標可用於反白顯示影像的特定部分。例如，您可以將注意力集中在影像與眾不同之處。在「縮放檢視器」視窗中，縮放目標以縮圖影像的形式顯示在影像一側。選取其中一個縮放目標縮圖，可自動縮放所指定的影像部分。

若要建立縮放目標，請選取 **[!UICONTROL 編輯]** ，然後選擇「縮放目標」，或在「詳細資訊視圖」的「瀏覽面板」中開啟影像，然後選擇 **[!UICONTROL 縮放目標]**. 然後使用「縮放目標編輯器」頁上的縮放工具，以便將影像的一部分隔離為目標。 請參閱 [建立引導式縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

## 3.設定縮放檢視器預設集

縮放檢視器預設集可確定縮放檢視器的樣式和行為。如果您是管理員，可以設定縮放檢視器預設集；Adobe Dynamic Media Classic也隨附預設的「最佳實務」縮放檢視器預設集。

若要建立縮放檢視器預設集，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**. 在「查看器預設集」頁上，選擇 **[!UICONTROL 新增]**，選擇平台和縮放檢視器，然後選取 **[!UICONTROL 新增]**. 然後在「配置查看器」頁上選擇選項。

Adobe Dynamic Media Classic選件 **[!UICONTROL 縮放檢視器預設集]** 選項，可讓您選取檢視器的按鈕樣式和整體外觀。 您還可以自訂網站的縮放設定。請參閱 [設定縮放檢視器預設集](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 4.使用縮放檢視器預覽影像

您可以在縮放檢視器中預覽影像，查看影像縮放時的縮放效果。

若要探索不同的縮放檢視器預設集及其呈現縮放體驗的方式，請在「瀏覽」面板中選取影像，然後選取 **[!UICONTROL 預覽]**. 前往 **[!UICONTROL 預設集]** > **[!UICONTROL 縮放]**，然後選擇帶有「縮放」菜單的預設。

此時會出現「縮放」按鈕。可以查看縮放影像在網站上的外觀。選擇縮放按鈕（和縮放目標），以便您可以測試所選縮放查看器預設集的設定。 請參閱 [使用不同的縮放檢視器預覽影像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

## 5.發佈縮放影像

發佈縮放影像會將其置於Dynamic Media影像伺服器上，以便傳遞至您的網站和應用程式。 Adobe Dynamic Media Classic會在發佈程式中啟用URL字串。 這些URL字串會呼叫從Dynamic Media影像伺服器到您網站或應用程式的縮放影像。

在全局導航欄上，選擇 **[!UICONTROL 發佈]**. 在「發佈」(Publish)對話框中，選擇 **[!UICONTROL 提交發佈]**. 請參閱[發佈縮放影像](publishing-zoom-images.md#publishing_zoom_images)。

## 6.將縮放檢視器連結至您的網頁

Adobe Dynamic Media Classic會建立縮放影像所需的URL圖說字串，並在您將影像發佈至Dynamic Media影像伺服器時啟用它們。 您可以從 **[!UICONTROL 預覽]** 頁面。 複製 URL 字串之後，即可在網站和應用程式上使用。請參閱 [將縮放檢視器連結至您的網頁](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
