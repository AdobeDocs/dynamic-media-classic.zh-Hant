---
title: '"快速入門:迴轉集"'
description: 簡介和快速開始回轉集可協助您快速上手使用。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media經典，觀眾，旋轉集
role: Business Practitioner
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 32%

---

# 快速入門:迴轉集{#quick-start-spin-sets}

迴轉集用於模擬轉動物件進行查看時的真實動作。利用迴轉集能夠從任何角度查看項目，從而獲得任何角度的重要視覺詳細資訊。迴轉集會模擬 360 度的視覺效果。Dynamic Media經典提供一維回轉集（檢視器可在其中旋轉項目）和二維回轉集（檢視器可在其中旋轉和翻轉項目）。 此外，使用者只需按幾下滑鼠，就可「自由格式」縮放和平移任何檢視。 透過這種方式，使用者能夠以特定的視點，更仔細地檢查項目。

![迴轉集的影像。](/help/assets/spin_set.png)

迴轉集也接受影像地圖。影像地圖就是迴轉集內顯示含文字之滑鼠指向面板的影像區域。使用者按一下「影像地圖」時，就會觸發某種動作。例如，啟動網頁讓使用者進一步瞭解產品。若要指出回轉集中的影像地圖，當使用者將滑鼠指標移至影像地圖上時，影像地圖本身周圍會出現外框。

請參閱[建立影像地圖](creating-image-maps.md)。

此回轉集快速入門旨在利用Dynamic Media經典公司的回轉集技術快速啟動和運行。 依照步驟 1 至 7 執行。在每個步驟結束時，您可以按一下主題連結以進一步瞭解。

## 1.建立和上傳影像

至少，一維自旋集需要8-12個項目鏡頭，二維自旋集需要16-24個項目鏡頭。 拍攝照片時必須間隔一定的角度，以便讓人感覺該項目正在旋轉和翻轉。例如，如果一維回轉集包含12個鏡頭，請針對每個鏡頭旋轉項目30°(360/12)。

在全域導覽列上，按一下&#x200B;**[!UICONTROL Upload]**，將回轉影像從您的電腦或網路上傳至Dynamic Media經典。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.建立回轉集

若要建立回轉集，請在全域導覽列上按一下「建立&#x200B;**** > **[!UICONTROL 回轉集]**」。 在「回轉集大小」對話框中，選擇所需的行和單元格數，然後按一下「確定」****。 然後將影像拖曳至「回轉集」頁面的格線中。

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

## 3.編輯回轉集

若要編輯回轉集，請在全域導覽列上按一下「設定&#x200B;**** > **[!UICONTROL 檢視器預設集]**」。 選擇回轉集，然後按一下&#x200B;**[!UICONTROL 編輯]**。 增加、移除和變更影像的位置。您可以變更二維迴轉集中列的位置。

請參閱[編輯迴轉集](creating-spin-set.md#editing-a-spin-set)。

## 4.設定回轉集檢視器預設集

管理員可以建立迴轉集檢視器預設集。這些預設集決定了迴轉集檢視器的外觀。若要設定新的回轉集檢視器預設集，請在全域導覽列上按一下「設定&#x200B;**** > **[!UICONTROL 檢視器預設集]**」。

在「檢視器預設集」頁面上，按一下「新增&#x200B;****」，然後從下拉式清單中選取「回轉集檢視器」，然後按一下「新增&#x200B;****」。 ****&#x200B;在「配置查看器」頁中選擇選項，然後按一下&#x200B;**[!UICONTROL 保存]**。

請參閱[設定迴轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.預覽回轉集

在「瀏覽面板」中選取「回轉集」，然後按一下「預覽」。 ****&#x200B;在「預覽」頁面上，按住滑鼠按鈕並向左或向右拖曳指標，以視覺化方式「回轉」項目。

請參閱[預覽迴轉集](previewing-spin-set.md#previewing-a-spin-set)。

## 6.發佈回轉集

發佈回轉集會將它放置在Dynamic Media經典伺服器上，以便動態傳遞至您的網站或應用程式。 它也會啟動URL字串，從Dynamic Media影像伺服器呼叫回轉集至您的網站或應用程式。

若要發佈回轉集，請在「瀏覽面板」中選取其名稱旁的&#x200B;**[!UICONTROL 標示為發佈]**&#x200B;圖示，將其標示為發佈。 在全域導覽列上，按一下「**[!UICONTROL 發佈]**」以啟動發佈。 在「發佈」畫面上，按一下「提交發佈」。****

請參閱[發佈迴轉集](publishing-spin-set.md#publishing-a-spin-set)。

## 7.將回轉集連結至網頁

Dynamic Media經典會建立回轉集的URL圖說字串，並在您發佈後加以啟動。 您可以從「預覽」頁面複製這些URL。

選擇「回轉集」，然後按一下「預覽」。 ****&#x200B;選取迴轉集檢視器預設集。然後按一下「複製URL」。****

請參閱[將迴轉集連結到網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
