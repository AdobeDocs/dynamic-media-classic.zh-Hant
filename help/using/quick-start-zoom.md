---
title: '快速入門: 縮放'
description: 介紹和Zoom快速入門，協助您快速上手並執行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 19%

---

# 快速入門: 縮放{#quick-start-zoom}

縮放可讓您以互動方式檢視影像中的高解析度詳細資料。 例如，可以在動態的、可完全設定的整合檢視器中查看影像的色彩、選項、角度以及細節。此檢視器可內嵌在網頁上或顯示在快顯視窗中。 您可以在近距離稽核影像，並以高解析度平移影像，以仔細檢視它們。 縮放功能可以為您的客戶帶來豐富多彩的互動式視覺效果。

Adobe Dynamic Media Classic也提供引導式縮放，讓您強調影像中的重要功能。 例如，若要將檢視者的注意力集中於某個標誌上，可以為該標誌建立一個縮放目標。使用者選取此縮放目標時，會縮放至標誌。

所有縮放影像都是從單一主要影像、圖形和資料庫驅動屬性建立及提供的。 Adobe Dynamic Media Classic縮放可大幅減少製作和傳送影像的時間和成本。 您可以使用「縮放檢視器」來放大和縮小影像。 「縮放檢視器」有按鈕可供您選取來縮放和平移；您也可以拖曳到熒幕上來平移。 透過縮放檢視器預設集，可以設定要用於縮放影像的縮放檢視器。

請參閱[縮放目標： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS)和[縮放： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

下列「縮放快速入門」的設計目的，是要讓您快速上手並執行Adobe Dynamic Media Classic中的縮放技術。 依照步驟 1 至 6 執行。每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.上傳縮放影像

首先，將縮放影像上傳至Adobe Dynamic Media Classic。 為了達到最佳縮放效果，Adobe Dynamic Media Classic建議影像的最長大小至少為2000畫素。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，將影像從您的電腦或網路上傳至Adobe Dynamic Media Classic上的資料夾。 請參閱[上傳縮放影像](uploading-zoom-images.md#uploading_zoom_images)。

## 2.建立引導式縮放的縮放目標

縮放目標可用於反白顯示影像的特定部分。例如，您可以將注意力集中在影像與眾不同之處。在「縮放檢視器」視窗中，「縮放目標」會以縮圖影像的形式出現在影像的一側。 選取其中一個縮放目標縮圖，可自動縮放所指定的影像部分。

若要建立縮放目標，請選取&#x200B;**[!UICONTROL 編輯]**&#x200B;並選擇「縮放目標」，或在「詳細資料檢視」的「瀏覽」面板中開啟影像並選取&#x200B;**[!UICONTROL 縮放目標]**。 然後使用「縮放目標編輯器」頁面上的「縮放」工具，以便隔離部分影像作為目標。 請參閱[建立引導式縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。

## 3.設定縮放檢視器預設集

縮放檢視器預設集可確定縮放檢視器的樣式和行為。如果您是管理員，可以設定縮放檢視器預設集；Adobe Dynamic Media Classic也隨附預設的「最佳實務」縮放檢視器預設集。

若要建立縮放檢視器預設集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。 在[檢視器預設集]頁面上，選取&#x200B;**[!UICONTROL 新增]**，選擇平台和縮放檢視器，然後選取&#x200B;**[!UICONTROL 新增]**。 然後在`Configure Viewer`頁面上選擇選項。

Adobe Dynamic Media Classic提供&#x200B;**[!UICONTROL 縮放檢視器預設集]**&#x200B;選項，可讓您選取按鈕樣式和檢視器的整體外觀。 您也可以自訂網站的縮放設定。 請參閱[設定縮放檢視器預設集](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

## 4.使用縮放檢視器預覽影像

您可以在縮放檢視器中預覽影像，查看影像縮放時的縮放效果。

若要探索不同的縮放檢視器預設集及其呈現縮放體驗的方式，請在「瀏覽」面板中選取影像，然後選取「**[!UICONTROL 預覽]**」。 前往&#x200B;**[!UICONTROL 預設集]** > **[!UICONTROL 縮放]**，然後使用「縮放」功能表選取預設集。

此時會出現「縮放」按鈕。您可以檢視縮放影像在您網站上的外觀。 選取「縮放」按鈕（和「縮放目標」），以測試您所選取「縮放檢視器預設集」的設定。 檢視[使用不同縮放檢視器預覽影像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

## 5.發佈縮放影像

發佈縮放影像時，會將影像置於Dynamic Media影像伺服器上，以便傳遞至您的網站和應用程式。 在發佈程式中，Adobe Dynamic Media Classic會啟用URL字串。 這些URL字串會將Dynamic Media影像伺服器的縮放影像呼叫至您的網站或應用程式。

在全域導覽列上，選取&#x200B;**[!UICONTROL 發佈]**。 在[發佈]對話方塊中，選取&#x200B;**[!UICONTROL 送出發佈]**。 請參閱[發佈縮放影像](publishing-zoom-images.md#publishing_zoom_images)。

## 6.將縮放檢視器連結至您的網頁

Adobe Dynamic Media Classic會建立縮放影像所需的URL圖說文字字串，並在您將影像發佈至Dynamic Media影像伺服器時加以啟用。 您可以從&#x200B;**[!UICONTROL 預覽]**&#x200B;頁面複製這些URL字串。 複製URL字串後，您的網站和應用程式即可使用這些字串。 請參閱[將縮放檢視器連結至您的網頁](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)。
