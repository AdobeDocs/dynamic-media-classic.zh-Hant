---
title: '"快速入門:迴轉集"'
description: 簡介和快速啟動到旋轉集，幫助您在Adobe Dynamic Media Classic快速啟動並運行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 5040b1916794d3b54f952a1df5f060be2f31006a
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 22%

---

# 快速入門:迴轉集{#quick-start-spin-sets}

迴轉集用於模擬轉動物件進行查看時的真實動作。利用迴轉集能夠從任何角度查看項目，從而獲得任何角度的重要視覺詳細資訊。「旋轉集」(Spin Set)模擬360°的觀看體驗。 Adobe Dynamic Media Classic公司提供一維旋轉集和二維旋轉集，觀看者可以旋轉項目。 此外，用戶只需點擊幾下滑鼠即可「自由格式」縮放和平移任何視圖。 透過這種方式，使用者能夠以特定的視點，更仔細地檢查項目。

![迴轉集的影像。](/help/assets/spin_set.png)

迴轉集也接受影像地圖。影像地圖就是迴轉集內顯示含文字之滑鼠指向面板的影像區域。使用者按一下「影像地圖」時，就會觸發某種動作。例如，啟動網頁讓使用者進一步瞭解產品。要指出旋轉集中的影像映射，當用戶將滑鼠指針移到影像映射本身周圍時，將顯示輪廓。

請參閱 [建立影像映射](creating-image-maps.md)。

請參閱 [影像和旋轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 培訓視頻。

>[!NOTE]
>
>建立「旋轉集」時，Adobe建議使用以下最佳實踐准則和強制限制。
>
>* 每2D旋轉集的最大行/列數
   > 
   >   * 最佳做法：1000
   >   * 強制限制：1000


本「旋轉集快速啟動」旨在通過Adobe Dynamic Media Classic的「旋轉集」技術幫助您快速啟動和運行。 依照步驟 1 至 7 執行。在每個步驟的末尾，您可以選擇主題連結以瞭解詳細資訊。

## 1。建立和上載映像

對於一維自旋集，至少需要8-12個項的投影，對於二維自旋集，需要16-24個投影。 拍攝照片時必須間隔一定的角度，以便讓人感覺該項目正在旋轉和翻轉。例如，如果一維自旋集包含12個鏡頭，則對每個鏡頭旋轉項目30°(360°/12)。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 將旋轉映像從您的電腦或網路上傳到Adobe Dynamic Media Classic。

請參閱[迴轉集影像拍攝準則](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.建立旋轉集

要建立旋轉集，請在全局導航欄上，轉到 **[!UICONTROL 生成]** > **[!UICONTROL 旋轉集]**。 在「旋轉集大小」對話框中，選擇所需的行和單元格數，然後選擇 **[!UICONTROL 確定]**。 然後將影像拖到「旋轉集」頁上的網格中。

請參閱 [建立旋轉集](creating-spin-set.md#creating-a-spin-set)。

## 3.編輯旋轉集

要編輯旋轉集，請在全局導航欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。 選擇旋轉集，然後選擇 **[!UICONTROL 編輯]**。 增加、移除和變更影像的位置。您可以變更二維迴轉集中列的位置。

請參閱 [編輯旋轉集](creating-spin-set.md#editing-a-spin-set)。

## 4.設定旋轉集查看器預設

管理員可以建立迴轉集檢視器預設集。這些預設集決定了迴轉集檢視器的外觀。要設定新的「旋轉集查看器預設」，請轉至「全局導航」欄 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。

在「查看器預設」頁面上，選擇 **[!UICONTROL 添加]**，然後選擇 **[!UICONTROL 旋轉集查看器]** 從下拉清單中，然後選擇 **[!UICONTROL 添加]**。 在「配置查看器」頁中選擇選項，然後選擇 **[!UICONTROL 保存]**。

請參閱 [設定旋轉集查看器預設](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.預覽旋轉集

在「瀏覽面板」中選擇「旋轉集」，然後選擇 **[!UICONTROL 預覽]**。 在「預覽」頁面上，按住滑鼠按鈕，然後向左或向右拖動指針以可視地「旋轉」項目。

請參閱 [預覽旋轉集](previewing-spin-set.md#previewing-a-spin-set)。

## 6。發佈旋轉集

發佈Spin Set將其放置在Adobe Dynamic Media Classic伺服器上，以便可以動態地將其提交到您的網站或應用程式。 它還激活URL字串，該字串將從Dynamic Media映像伺服器調用到網站或應用程式的Spin Set。

要發佈旋轉集，請通過選擇 **[!UICONTROL 標籤為發佈]** 表徵圖。 在全局導航欄上，選擇 **[!UICONTROL 發佈]** 啟動發佈。 在「發佈」螢幕上，選擇 **[!UICONTROL 提交發佈]**。

請參閱 [發佈旋轉集](publishing-spin-set.md#publishing-a-spin-set)。

## 7。將旋轉集連結到網頁

Adobe Dynamic Media Classic為「旋轉集」建立URL標注字串，並在發佈它們後激活它們。 可以從「預覽」頁複製這些URL。

選擇「旋轉集」，然後選擇 **[!UICONTROL 預覽]**。 選取迴轉集檢視器預設集。然後選擇 **[!UICONTROL 複製URL]**。

請參閱 [將旋轉集連結到網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
