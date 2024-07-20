---
title: 「快速入門：迴轉集」
description: 迴轉集簡介和快速入門可幫助您在Adobe Dynamic Media Classic中快速上手並執行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 21%

---

# 快速入門:迴轉集{#quick-start-spin-sets}

迴轉集用於模擬轉動物件進行查看時的真實動作。利用迴轉集能夠從任何角度查看項目，從而獲得任何角度的重要視覺詳細資訊。迴轉集會模擬 360 度的視覺效果。Adobe Dynamic Media Classic提供一維迴轉集（檢視器可旋轉專案）和二維迴轉集（檢視器可旋轉和翻轉專案）。 此外，使用者只要按幾下滑鼠即可隨意縮放及平移任何檢視。 透過這種方式，使用者能夠以特定的視點，更仔細地檢查項目。

迴轉集的![影像。](/help/using/assets/spin_set.png)

迴轉集也接受影像地圖。影像地圖就是迴轉集內顯示含文字之滑鼠指向面板的影像區域。當使用者選取影像地圖時，就會觸發某種動作。 例如，啟動網頁以便使用者進一步瞭解產品。 若要指出「迴轉集」中的「影像對映」，當使用者將滑鼠指標移到「影像對映」上時，就會在「影像對映」本身周圍出現輪廓。

請參閱[建立影像地圖](creating-image-maps.md)。

請參閱[影像和迴轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

當您建立「迴轉集」時，Adobe會建議下列最佳作法並強制執行下列限制：

| 迴轉集限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每個2D集的最大列/欄數 | 每組12至18個影像 | 1000 |

另請參閱[Dynamic Media限制](/help/using/limitations.md)。

此迴轉集快速入門旨在讓您快速上手並執行Adobe Dynamic Media Classic中的迴轉集技術。 依照步驟 1 至 7 執行。在每個步驟結束時，您可以選取主題連結以瞭解更多資訊。

## 1.建立及上傳影像

對於一維迴轉集，一個項目最少需要拍攝 8 到 12 張照片，對於二維迴轉集，最少需要 16 到 24 張照片。拍攝照片時必須間隔一定的角度，以便讓人感覺該項目正在旋轉和翻轉。例如，如果一維「迴轉集」包含12個鏡頭，則每個鏡頭應將專案旋轉30° (360/12)。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，從您的電腦或網路上傳迴轉影像至Adobe Dynamic Media Classic。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.建立迴轉集

若要建立迴轉集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL 迴轉集]**。 在「迴轉集大小」對話方塊中，選擇您要多少列和儲存格，並選取&#x200B;**[!UICONTROL 確定]**。 然後將影像拖曳至「迴轉集」頁面上的格線中。

請參閱[建立迴轉集](creating-spin-set.md#creating-a-spin-set)。

## 3.編輯迴轉集

若要編輯迴轉集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。 選取迴轉集，然後選取&#x200B;**[!UICONTROL 編輯]**。 增加、移除和變更影像的位置。您可以變更二維迴轉集中資料列的位置。

請參閱[編輯迴轉集](creating-spin-set.md#editing-a-spin-set)。

## 4.設定迴轉集檢視器預設集

管理員可以建立迴轉集檢視器預設集。這些預設集決定了迴轉集檢視器的外觀。若要設定新的迴轉集檢視器預設集，請在全域導覽列上，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。

在[檢視器預設集]頁面上，選取&#x200B;**[!UICONTROL 新增]**，然後從下拉式清單中選取&#x200B;**[!UICONTROL 迴轉集檢視器]**，然後選取&#x200B;**[!UICONTROL 新增]**。 在`Configure Viewer`頁面中選擇選項，然後選取&#x200B;**[!UICONTROL 儲存]**。

請參閱[設定迴轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.預覽迴轉集

在瀏覽面板中選取您的迴轉集，然後選取&#x200B;**[!UICONTROL 預覽]**。 在「預覽」頁面上，按住滑鼠鍵，向左或向右拖曳指標，以視覺化方式「旋轉」專案。

請參閱[預覽迴轉集](previewing-spin-set.md#previewing-a-spin-set)。

## 6. Publish a迴轉集

發佈迴轉集會將它置於Adobe Dynamic Media Classic伺服器上，以便動態傳遞至您的網站或應用程式。 這也會啟用URL字串，將迴轉集從Dynamic Media影像伺服器呼叫至您的網站或應用程式。

若要發佈迴轉集，請在「瀏覽」面板中選取其名稱旁的&#x200B;**[!UICONTROL 標籤為Publish]**&#x200B;圖示，將其標籤為發佈。 在全域導覽列上，選取&#x200B;**[!UICONTROL Publish]**&#x200B;以啟動發佈。 在發佈頁面上，選取&#x200B;**[!UICONTROL 提交Publish]**。

請參閱[Publish a迴轉集](publishing-spin-set.md#publishing-a-spin-set)。

## 7.將迴轉集連結至網頁

Adobe Dynamic Media Classic會為迴轉集建立URL圖說文字串，並在您發佈後加以啟用。 您可以從「預覽」頁面複製這些URL。

選取迴轉集，然後選取&#x200B;**[!UICONTROL 預覽]**。 選取迴轉集檢視器預設集。然後選取&#x200B;**[!UICONTROL 複製URL]**。

請參閱[將迴轉集連結至網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
