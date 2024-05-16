---
title: 建立引導式縮放的縮放目標
description: 瞭解如何在Adobe Dynamic Media Classic中建立引導式縮放的縮放目標。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 27%

---

# 建立引導式縮放的縮放目標{#creating-zoom-targets-for-guided-zoom}

縮放目標會將檢視器引導到影像的特定部分。除了自由格式縮放以外，檢視者還可以選取縮放目標縮圖，並縮放至您要其聚焦的影像部分。 透過縮放目標，可反白顯示影像的有趣或誘人之處。

![建立引導式縮放的縮放目標](/help/using/assets/zo_guided_zoom.png)

## 關於縮放目標 {#about-zoom-targets}

縮放目標的最大縮放百分比為100%。 根據檢視器大小和影像大小的不同組合，最小縮放百分比也會有所不同，如下表格所示:

| 影像尺寸 | 檢視器大小 | 縮放百分比 |
| --- | --- | --- |
| 大碼 | 較小 | 最小縮放百分比較小 |
| 小碼 | 較大 | 最小縮放百分比較大 |

您可以變更縮放檢視器的大小，以符合網頁上使用的大小。 您可以透過變更[設定]畫面上的檢視器大小來永久變更此設定（如果您是管理員）。 另請參閱 [設定縮放檢視器預設集](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 建立及編輯縮放目標 {#creating-and-editing-zoom-targets}

在縮放目標編輯器畫面中建立和編輯縮放目標。 若要開啟該畫面，請選取一個影像並執行以下操作之一:

* 選取變換影像 **[!UICONTROL 編輯]** 按鈕，然後選擇「縮放目標」。
* 在「瀏覽」面板中，將影像顯示於 **[!UICONTROL 詳細資料檢視]**，然後選取 **[!UICONTROL 縮放目標]**.

在「縮放目標編輯器」畫面上，選取 **[!UICONTROL 選取目標]** 按鈕（箭頭）以在變更目標大小或位置之前選取目標。 若要在影像上建立縮放目標，請選取 **[!UICONTROL 新增目標]** （矩形）。 「縮放目標編輯器」頁面也提供刪除、複製和命名縮放目標的工具。

### 建立縮放目標 {#creating-a-zoom-target}

若要建立縮放目標，請開啟「縮放目標編輯器」頁面，並執行下列動作：

1. 選取 **[!UICONTROL 新增目標]** （矩形），將指標移到影像上，然後選取縮放目標的位置。

   縮放目標的縮圖影像顯示在畫面右側的面板中。

1. 選取 **[!UICONTROL 選取目標]** （箭頭），然後選取您建立的縮放目標，並調整目標的大小和位置。

   * **調整大小**：將指標移至縮放目標的角落上，並拖曳以放大或縮小目標。

   * **位置**：將指標移至縮放目標上方，並將其拖曳至其他位置。

1. 在「名稱」方框中輸入縮放目標名稱。

   >[!NOTE]
   >
   >在「名稱」方框中輸入的不僅僅是名稱。使用者在縮放目標上移動指標時，將會看到您在「名稱」方框中輸入的內容。在「名稱」方框中輸入對縮放目標的簡要說明，以便使用者瞭解其可以縮放的內容。

1. 可以視情況在「使用者資料」欄位中輸入使用者資料。此欄位可供網站設計人員新增資訊至縮放目標。
1. 選取 **[!UICONTROL 儲存]**.

   即可儲存縮放目標的座標和縮放等級。帶有您輸入的名稱的縮放目標縮圖顯示在畫面右側。

>[!NOTE]
>
>若要在縮放檢視器中檢視縮放目標的外觀，請選取 **[!UICONTROL 預覽]** 「縮放目標編輯器」畫面中的按鈕。 然後在「預覽」畫面中選擇「縮放檢視器」。 如需有關此畫面的詳細資訊，請參閱 [使用不同的縮放檢視器預覽影像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### 編輯縮放目標 {#editing-zoom-targets}

若要編輯「縮放目標」，請在「縮放目標編輯器」頁面上使用下列技術：

* **重新定位**：使用選取目標按鈕（箭頭）選取目標。 然後，將目標拖曳到其他位置。

* **調整大小**：使用選取目標按鈕（箭頭）選取目標。 若要放大或縮小目標，請將指標移至縮放目標的角落並拖曳。

* **刪除**：選取畫面右側的目標縮圖影像。 然後選取 **[!UICONTROL 刪除目標]**.

* **重新命名**：選取畫面右側的目標縮圖影像。 然後，在 **[!UICONTROL 名稱]** 文字欄位並選取 **[!UICONTROL 儲存]**.

### 複製縮放目標 {#copying-zoom-targets}

您可將縮放目標從一個影像複製到另一個影像。 當兩個影像呈現類似內容且其縮放目標屬於相同位置時，複製目標。 若要將「縮放目標」複製到另一個影像，請執行下列動作：

1. 在「縮放目標編輯器」畫面中，使用您要複製的縮放目標開啟影像。
1. 選取 **[!UICONTROL 將目標複製到]**.
1. 在「選取影像」對話方塊中，選取影像並選取 **[!UICONTROL 選取]**.
