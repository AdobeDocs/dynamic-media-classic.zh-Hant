---
title: '"快速入門:迴轉集"'
description: 介紹和回轉集快速入門，協助您在Adobe Dynamic Media Classic中快速上手並執行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 23%

---

# 快速入門:迴轉集{#quick-start-spin-sets}

迴轉集用於模擬轉動物件進行查看時的真實動作。利用迴轉集能夠從任何角度查看項目，從而獲得任何角度的重要視覺詳細資訊。回轉集模擬360°的檢視體驗。 Adobe Dynamic Media Classic提供可讓檢視器旋轉項目的一維回轉集，以及可讓檢視器旋轉及翻轉項目的二維回轉集。 此外，使用者只需按幾下滑鼠，即可「自由格式」縮放及平移任何檢視。 透過這種方式，使用者能夠以特定的視點，更仔細地檢查項目。

![迴轉集的影像。](/help/assets/spin_set.png)

迴轉集也接受影像地圖。影像地圖就是迴轉集內顯示含文字之滑鼠指向面板的影像區域。使用者按一下「影像地圖」時，就會觸發某種動作。例如，啟動網頁讓使用者進一步瞭解產品。為了在回轉集中指出影像映射，當用戶將滑鼠指針移到影像映射上時，該影像映射本身周圍會出現一個輪廓。

請參閱[建立影像映射](creating-image-maps.md)。

請參閱[影像和回轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

此回轉集快速入門旨在透過Adobe Dynamic Media Classic中的回轉集技術，協助您快速上手並執行。 依照步驟 1 至 7 執行。在每個步驟結束時，您可以選取主題連結以深入了解。

## 1.建立和上傳影像

一維自旋集至少需要8-12個項目的鏡頭，二維自旋集至少需要16-24個。 拍攝照片時必須間隔一定的角度，以便讓人感覺該項目正在旋轉和翻轉。例如，如果一維度回轉集包含12個鏡頭，請為每個鏡頭旋轉項目30°(360°/12)。

在全域導覽列上，選取&#x200B;**[!UICONTROL Upload]** ，將回轉影像從您的電腦或網路上傳至Adobe Dynamic Media Classic。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.建立回轉集

若要建立回轉集，請在全域導覽列上前往&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**。 在「回轉集大小」對話方塊中，選擇所需的列數和儲存格數，然後選取&#x200B;**[!UICONTROL 確定]**。 然後將影像拖曳至回轉集頁面上的格線中。

請參閱[建立回轉集](creating-spin-set.md#creating-a-spin-set)。

## 3.編輯回轉集

若要編輯回轉集，請在全域導覽列上前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。 選取回轉集，然後選取&#x200B;**[!UICONTROL Edit]**。 增加、移除和變更影像的位置。您可以變更二維迴轉集中列的位置。

請參閱[編輯回轉集](creating-spin-set.md#editing-a-spin-set)。

## 4.設定回轉集檢視器預設集

管理員可以建立迴轉集檢視器預設集。這些預設集決定了迴轉集檢視器的外觀。若要設定新的回轉集檢視器預設集，請在全域導覽列上前往&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。

在「查看器預設集」頁上，選擇&#x200B;**[!UICONTROL Add]**，然後從下拉清單中選擇&#x200B;**[!UICONTROL Spin Set Viewer]**，然後選擇&#x200B;**[!UICONTROL Add]**。 在「配置查看器」頁中選擇選項，然後選擇&#x200B;**[!UICONTROL 保存]**。

請參閱[設定回轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.預覽回轉集

在「瀏覽」面板中選取「回轉集」，然後選取「**[!UICONTROL 預覽]**」。 在「預覽」頁面上，按住滑鼠按鈕，並向左或向右拖曳指標，以視覺化方式「回轉」項目。

請參閱[預覽回轉集](previewing-spin-set.md#previewing-a-spin-set)。

## 6.發佈回轉集

發佈回轉集會將其置於Adobe Dynamic Media Classic伺服器上，以便動態傳遞至您的網站或應用程式。 它也會啟動URL字串，該URL字串會從Dynamic Media影像伺服器呼叫回轉集至您的網站或應用程式。

若要發佈回轉集，請在「瀏覽」面板中選取其名稱旁的&#x200B;**[!UICONTROL 標示為發佈]**&#x200B;圖示，將其標示為發佈。 在全域導覽列中，選取&#x200B;**[!UICONTROL Publish]**&#x200B;以起始發佈。 在「發佈」螢幕上，選擇「**[!UICONTROL 提交發佈]**」。

請參閱[發佈回轉集](publishing-spin-set.md#publishing-a-spin-set)。

## 7.將回轉集連結至網頁

Adobe Dynamic Media Classic會為回轉集建立URL圖說字串，並在您發佈後啟用它們。 您可以從預覽頁面複製這些URL。

選擇回轉集，然後選擇&#x200B;**[!UICONTROL 預覽]**。 選取迴轉集檢視器預設集。然後選擇&#x200B;**[!UICONTROL 複製URL]**。

請參閱[將回轉集連結至網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
