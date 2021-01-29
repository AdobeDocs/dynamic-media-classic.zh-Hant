---
title: '"快速入門:迴轉集"'
description: 簡介和回轉集快速入門，協助您快速上手使用。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 68%

---


# 快速入門:迴轉集{#quick-start-spin-sets}

迴轉集用於模擬轉動物件進行查看時的真實動作。利用迴轉集能夠從任何角度查看項目，從而獲得任何角度的重要視覺詳細資訊。迴轉集會模擬 360 度的視覺效果。Dynamic Media Classic提供一維回轉集（檢視器可在其中旋轉項目）和二維回轉集（檢視器可在其中旋轉和翻轉項目）。 此外，使用者只需按幾下滑鼠，就可「自由格式」縮放和平移任何檢視。 透過這種方式，使用者能夠以特定的視點，更仔細地檢查項目。

![迴轉集的影像。](/help/assets/spin_set.png)

迴轉集也接受影像地圖。影像地圖就是迴轉集內顯示含文字之滑鼠指向面板的影像區域。使用者按一下「影像地圖」時，就會觸發某種動作。例如，啟動網頁讓使用者進一步瞭解產品。為了喚起對迴轉集內影像地圖的使用，當使用者將滑鼠指標移至影像地圖時，該影像地圖本身周圍就會顯示外框。

請參閱[建立影像地圖](creating-image-maps.md)。

**快速入門**

此回轉集快速入門旨在透過Dynamic Media Classic中的回轉集技術快速啟動及執行。 依照步驟 1 至 7 執行。每個步驟的結尾都有到主題標題的交互參照，您可以在其中找到更多資訊 (如果需要)。

**1. 建立和上載影像**

至少，一維自旋集需要8-12個項目鏡頭，二維自旋集需要16-24個項目鏡頭。 拍攝照片時必須間隔一定的角度，以便讓人感覺該項目正在旋轉和翻轉。例如，如果某個一維迴轉集中有 12 張照片，則每拍一張照片將項目旋轉 30 度 (360/12)。

選取全域導覽列上的「上傳」按鈕，將回轉影像從您的電腦或網路上傳至Dynamic Media Classic。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

**2.建立迴轉集**

若要建立迴轉集，請按一下「建置」按鈕，然後選擇「迴轉集」。在「迴轉集大小」對話框中，選擇需要的列和儲存格數，然後按一下「確定」。隨後將影像拖入迴轉集畫面上的格線中。

請參閱[建立迴轉集](creating-spin-set.md#creating-a-spin-set)。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06-245331fc135ab744793-8000">Including Image Maps in Spin Sets</a> to add clickable, hotspot regions, known as Image Maps, to images in a Spin Set. </p>

 -->

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See also <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06229f600f135ab7cc461-8000">Managing InfoPanel content</a>.</p>

 -->

**3.編輯迴轉集**

若要編輯某個迴轉集，請選取該迴轉集的「編輯」滑鼠指向按鈕。「迴轉集」畫面隨即開啟。增加、移除和變更影像的位置。您可以變更二維迴轉集中列的位置。

請參閱[編輯迴轉集](creating-spin-set.md#editing-a-spin-set)。

**4.設定迴轉集檢視器預設集**

管理員可以建立迴轉集檢視器預設集。這些預設集決定了迴轉集檢視器的外觀。若要設定新的迴轉集檢視器預設集，請在全域導覽列上選取「設定」按鈕。在「設定」畫面上，顯示「應用程式設定」選項，然後選取「檢視器預設集」。

在「檢視器預設集」畫面上，選取「增加」選單，然後在「增加檢視器預設集」對話框中選取「迴轉集檢視器」。接下來在「設定檢視器」畫面中選擇選項。

請參閱[設定迴轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

**5.預覽迴轉集**

在瀏覽面板中選取迴轉集，然後按一下其滑鼠指向「預覽」按鈕。在「預覽」畫面上，按住滑鼠按鈕並將指標往左或右拖曳，將項目「迴轉」視覺化。

請參閱[預覽迴轉集](previewing-spin-set.md#previewing-a-spin-set)。

**6.發佈迴轉集**

發佈回轉集會將它置於Dynamic Media Classic伺服器上，以便動態傳送至您的網站或應用程式。 它也會啟動URL字串，將「從動態媒體影像伺服器回轉集」呼叫至您的網站或應用程式。

若要發佈回轉集，請在「瀏覽面板」中選取其名稱旁的&#x200B;**標示為發佈**&#x200B;圖示，將其標示為發佈。 按一下全域導覽列上的&#x200B;**Publish**&#x200B;以啟動發佈。 在「發佈」畫面上，按一下「開始發佈」**。**

請參閱[發佈迴轉集](publishing-spin-set.md#publishing-a-spin-set)。

**7.將迴轉集連結到網頁**

Dynamic Media Classic會為回轉集建立URL圖說字串，並在您發佈後加以啟動。 您可以從「預覽」畫面複製這些 URL。

選擇「回轉集」，然後按一下「預覽」。 ****「預覽」畫面開啟。選取迴轉集檢視器預設集。然後按一下「複製URL」。****

請參閱[將迴轉集連結到網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
