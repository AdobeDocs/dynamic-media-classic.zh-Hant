---
title: 建立已導引縮放的縮放目標
description: 瞭解如何建立引導縮放的縮放目標。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 68%

---


# 建立已導引縮放的縮放目標{#creating-zoom-targets-for-guided-zoom}

縮放目標會將檢視器引導到影像的特定部分。除了隨意縮放之外，檢視者也可以按一下縮放目標縮圖，縮放到影像的重點部分。透過縮放目標，可反白顯示影像的有趣或誘人之處。

![Creating zoom targets for Guided Zoom](/help/assets/zo_guided_zoom.png)

## 關於縮放目標 {#about-zoom-targets}

縮放目目標最大縮放百分比是 100%。根據檢視器大小和影像大小的不同組合，最小縮放百分比也會有所不同，如下表格所示:

| 影像尺寸 | 檢視器大小 | 縮放百分比 |
|--- |--- |--- |
| 大碼 | 較小 | 最小縮放百分比較小 |
| 小碼 | 較大 | 最小縮放百分比較大 |

您可以變更縮放檢視器大小，使之與網頁上使用的大小相符。若要永久變更此設定，可以在「設定」畫面上變更檢視器大小 (如果您是管理員)。請參閱[設定縮放檢視器預設集](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

## 建立並編輯縮放目標 {#creating-and-editing-zoom-targets}

在「縮放目標編輯器」畫面上建立並編輯縮放目標。若要開啟該畫面，請選取一個影像並執行以下操作之一:

* 按一下變換&#x200B;**[!UICONTROL 編輯]**&#x200B;按鈕，然後選擇縮放目標。
* 在瀏覽面板中，在&#x200B;**[!UICONTROL 詳細資料檢視]**&#x200B;中顯示影像，然後按一下&#x200B;**[!UICONTROL 縮放目標]**。

在「縮放目標編輯器」螢幕上，按一下「選擇目標」按鈕（箭頭）以在更改目標大小或位置之前選擇目標。 ****&#x200B;按一下「新增目標」(****（矩形），在影像上建立縮放目標。 「縮放目標編輯器」畫面上也提供了用於刪除、複製和命名縮放目標的工具。

### 建立縮放目標  {#creating-a-zoom-target}

開啟「縮放目標編輯器」畫面，並按照以下步驟建立縮放目標:

1. 按一下「新增目標&#x200B;**[!UICONTROL （矩形）」，將指標移至影像上方，然後按一下縮放目標的位置。]**

   縮放目標的縮圖影像顯示在畫面右側的面板中。

1. 按一下「**[!UICONTROL 選擇目標]**（箭頭）」，按一下以選取您建立的縮放目標，並調整目標的大小和位置。

   * **調**
整大小將指標移至縮放目標的一角，然後拖曳以放大或縮小目標。

   * **定**
位將指標移至縮放目標上方，並拖曳至其他位置。

1. 在「名稱」方框中輸入縮放目標名稱。

   >[!NOTE]
   >
   >在「名稱」方框中輸入的不僅僅是名稱。使用者在縮放目標上移動指標時，將會看到您在「名稱」方框中輸入的內容。在「名稱」方框中輸入對縮放目標的簡要說明，以便使用者瞭解其可以縮放的內容。

1. 可以視情況在「使用者資料」欄位中輸入使用者資料。該欄位可供網站設計人員向縮放目標中增加資訊。
1. 按一下&#x200B;**[!UICONTROL 「儲存」]**。

   即可儲存縮放目標的座標和縮放等級。帶有您輸入的名稱的縮放目標縮圖顯示在畫面右側。

>[!NOTE]
>
>若要查看縮放目標在縮放檢視器中的顯示效果，請按一下「縮放目標編輯器」畫面的「預覽」按鈕，並在「預覽」畫面中選擇縮放檢視器。有關該畫面的資訊，請參閱[使用不同縮放檢視器預覽影像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

### 編輯縮放目標  {#editing-zoom-targets}

使用「縮放目標編輯器」畫面上的這些技術編輯縮放目標:

* **重**
新定位使用「選擇目標」按鈕（箭頭），按一下目標以選擇它。然後，將目標拖曳到其他位置。

* **調整**
大小使用「選擇目標」按鈕（箭頭），按一下目標以選取它。然後，從縮放目標的一角移動指標，並拖曳指標以放大或縮小目標。

* **刪**
除在畫面右側按一下目標的縮圖影像。然後按一下「刪除目標」。****

* **重**
新命名按一下畫面右側的目標縮圖影像。然後在**[!UICONTROL 名稱]**&#x200B;文字欄位中輸入名稱，然後按一下「儲存&#x200B;**[!UICONTROL a3/>」。]**

### 複製縮放目標 {#copying-zoom-targets}

可以將縮放目標從一個影像複製到另一個影像。如果兩個影像的內容相似且縮放目標位於同一位置，則可複製目標。請按照以下步驟將縮放目標複製到其他影像:

1. 在「縮放目標編輯器」畫面中開啟帶有要複製的縮放目標的影像。
1. 按一下「將目標複製到&#x200B;]**」。**[!UICONTROL 
1. 在「選擇影像」對話框中，選擇影像並按一下&#x200B;**[!UICONTROL 選擇]**。

