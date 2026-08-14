---
title: 快速入門:迴轉集
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
autotag-review: '2026-05-13T20:10:31.990Z'
TQID: 'https://experienceleague.adobe.com/dYjjsyvPAPOS5icw4Yi6Kpo93Nh2qvnCiW5-ih2hmDk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 1c15d2395e62ce41a298d25b973920963eef3a7a
workflow-type: tm+mt
source-wordcount: 820
ht-degree: 11%

---

# 快速入門:迴轉集{#quick-start-spin-sets}

「迴轉集」可提供物件的360度檢視。 「迴轉集」可讓您從任何角度檢視專案，從任何角度獲得視覺細節。 迴轉集會模擬 360 度的視覺效果。 Adobe Dynamic Media Classic提供一維迴轉集（檢視器可旋轉專案）和二維迴轉集（檢視器可旋轉和翻轉專案）。 此外，使用者可以縮放和平移任何檢視。 使用者可以從特定觀點更密切地檢查專案。

迴轉集的![影像](/help/using/assets/spin_set.png)

迴轉集也接受影像地圖。 「影像地圖」是旋轉組內影像上的區域，顯示包含文字的滑鼠指向效果面板。 當使用者選取影像地圖時，就會觸發動作。 例如，啟動網頁讓使用者進一步瞭解產品。 若要在「迴轉集」中指定「影像對映」，當使用者將指標移到「影像對映」上時，就會在「影像對映」本身周圍顯示輪廓。

請參閱[建立影像地圖](creating-image-maps.md)。

請參閱[影像和迴轉集： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

建立迴轉集時，Adobe會建議遵循下列准則並強制實施下列限制：

| 迴轉集限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每個2D集的最大列/欄數 | 每組12至18個影像 | 1000 |

另請參閱[Dynamic Media限制](/help/using/limitations.md)。

本指南旨在協助您快速開始使用Adobe Dynamic Media Classic中的迴轉集技術。 依照步驟 1 至 7 執行。 在每個步驟結束時，您可以選取主題連結以瞭解更多資訊。

## &#x200B;1. 建立及上傳影像

一維「迴轉集」至少需要8-12次專案快照，二維「迴轉集」至少需要16-24次專案快照。 拍攝必須定期進行，才能顯示專案旋轉和翻轉。 例如，如果一維「迴轉集」包含12個鏡頭，則每個鏡頭應將專案旋轉30° (360/12)。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，從您的電腦或網路上傳迴轉影像至Adobe Dynamic Media Classic。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## &#x200B;2. 建立迴轉集

若要建立迴轉集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL 迴轉集]**。 在「迴轉集大小」對話方塊中，選擇您要多少列和儲存格，並選取&#x200B;**[!UICONTROL 確定]**。 然後將影像拖曳至「迴轉集」頁面上的格線中。

請參閱[建立迴轉集](creating-spin-set.md#creating-a-spin-set)。

## &#x200B;3. 編輯迴轉集

若要編輯迴轉集，請在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。 選取迴轉集，然後選取&#x200B;**[!UICONTROL 編輯]**。 增加、移除和變更影像的位置。 您可以變更二維迴轉集中資料列的位置。

請參閱[編輯迴轉集](creating-spin-set.md#editing-a-spin-set)。

## &#x200B;4. 設定迴轉集檢視器預設集

管理員可以建立迴轉集檢視器預設集。 這些預設集決定了迴轉集檢視器的外觀。 若要設定新的迴轉集檢視器預設集，請在全域導覽列上，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。

在[檢視器預設集]頁面上，按一下[新增]&#x200B;**&#x200B;**，然後從下拉式清單中選取[迴轉集檢視器]&#x200B;**，然後選取[新增]**&#x200B;**。**&#x200B;在`Configure Viewer`頁面上選擇選項，然後按一下&#x200B;**[!UICONTROL 儲存]**。

請參閱[設定迴轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## &#x200B;5. 預覽迴轉集

在瀏覽面板中選取您的迴轉集，然後按一下&#x200B;**[!UICONTROL 預覽]**。 在「預覽」頁面上，按住按鈕並向左或向右拖曳指標，以視覺化方式旋轉專案。

請參閱[預覽迴轉集](previewing-spin-set.md#previewing-a-spin-set)。

## &#x200B;6. 發佈迴轉集

發佈迴轉集會將它置於Adobe Dynamic Media Classic伺服器上，以便動態傳遞至您的網站或應用程式。 這也會啟用URL字串，從Dynamic Media影像伺服器呼叫迴轉集至您的網站或應用程式。

若要發佈迴轉集，請在「瀏覽」面板中選取其名稱旁的&#x200B;**[!UICONTROL 標籤為發佈]**&#x200B;圖示，將其標籤為發佈。 在全域導覽列上，按一下&#x200B;**[!UICONTROL 發佈]**&#x200B;以啟動發佈。 在發佈頁面上，按一下&#x200B;**[!UICONTROL 送出發佈]**。

請參閱[發佈迴轉集](publishing-spin-set.md#publishing-a-spin-set)。

## &#x200B;7. 將迴轉集連結至網頁

Adobe Dynamic Media Classic會為迴轉集建立URL圖說文字串，並在您發佈後加以啟用。 您可以從「預覽」頁面複製這些URL。

選取迴轉集，然後按一下[預覽]。**&#x200B;** 選取迴轉集檢視器預設集。 然後按一下&#x200B;**[!UICONTROL 複製URL]**。

請參閱[將迴轉集連結至網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
