---
title: '快速入門: 影像集'
description: 影像集簡介和快速入門，可幫助您快速上手並執行Adobe Dynamic Media Classic中的影像集技術。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# 快速入門: 影像集{#quick-start-image-sets}

Adobe Dynamic Media Classic影像集為使用者提供整合式檢視體驗。 在動態影像集檢視器中，使用者可以透過選取縮圖影像來檢視專案的不同檢視。 「影像集」可讓您呈現專案的替代高解析度檢視。

影像集檢視器提供了縮放工具，以便近距離檢查影像。如有需要，您可以讓引導式「縮放目標」和「影像地圖」成為影像集的一部分。 影像集能創造更一致且緊密的檢視體驗。

請參閱[影像和迴轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)訓練影片。

建立影像集時，Adobe會建議下列最佳作法並強制進行下列限制：

| 限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| 每個集的重複資產數 | 無重複專案 | 20‡ |
| 每組影像的最大數量 | 每組5至10個影像 | 1000 |

‡最佳實務是不要在一個集中有重複的資產。 單一資產的限製為20個重複專案。 如果您為該資產新增另一個重複專案（在該集合內），請求會傳回錯誤或忽略重複專案。

另請參閱[Dynamic Media限制](/help/using/limitations.md)。

下列影像集快速入門的設計目的，是要讓您快速上手並執行Adobe Dynamic Media Classic中的影像集技術。

## 1.上傳多個檢視和色票的主要影像

請先為影像集上載影像。由於使用者可以在影像集檢視器中放大影像，因此在選擇影像時，請務必說明這個功能。 請確定影像的大小至少為2000畫素。 Adobe Dynamic Media Classic支援許多影像檔案格式，但建議使用不失真TIFF、PNG和EPS影像。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。

請參閱[準備影像集資產以進行上傳](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload)和[上傳您的檔案](uploading-files.md#uploading-your-files)。

## 2.建立影像集

在「影像集」中，使用者可在「影像集檢視器」中選取縮圖影像，以從不同側面或角度檢視影像。

若要建立影像集，請在全域導覽列上選取&#x200B;**[!UICONTROL 建置]**，然後選擇&#x200B;**[!UICONTROL 影像集]**。 在「影像集」視窗上，將影像拖曳至頁面以構成影像集。 視需求組織、新增和刪除影像。

請參閱[建立影像集](creating-image-set.md#creating-an-image-set)。

另請參閱[在影像集中包含縮放目標和影像地圖](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3.視需要準備影像集檢視器預設集

管理員可以建立或修改影像集檢視器預設集。Adobe Dynamic Media Classic隨附各種多媒體型別的預設檢視器預設集。 使用縮放檢視器： **[!UICONTROL 自訂]** > **[!UICONTROL 影像]**&#x200B;或&#x200B;**[!UICONTROL 影像集]**/**[!UICONTROL 多個檢視]**&#x200B;預設集來檢視您的影像集。

您可以從「應用程式設定」畫面新增或編輯檢視器預設集。

請參閱[建立和編輯檢視器預設集](application-setup.md#adding-and-editing-viewer-presets)。

## 4.預覽影像集

在[瀏覽]面板中選取[影像集]，然後選取[**[!UICONTROL 預覽]**]。 在「預覽」頁面中，選取縮圖圖示，以在選取的檢視器中檢查您的「影像集」。 您可以從「預設集」選單選擇不同的檢視器。

請參閱[預覽資產](previewing-asset.md#previewing-an-asset)。

## 5. Publish影像集

發佈影像集時會將其置於Adobe Dynamic Media Classic伺服器上並啟用URL字串。

>[!NOTE]
>
>如果您在建立並儲存影像集時於儲存&#x200B;**（預設）之後選取** Publish，則不需要執行此步驟。

在「瀏覽」面板中，選取名稱左側的&#x200B;**[!UICONTROL Publish標籤]**&#x200B;圖示。 然後選取&#x200B;**[!UICONTROL Publish]**。 在發佈頁面上，選取&#x200B;**[!UICONTROL 提交Publish]**。

檢視[Publish檔案](publishing-files.md#publishing-files)。

## 6.將影像集連結至您的網站

Adobe Dynamic Media Classic會為影像集建立URL呼叫，並在您發佈後加以啟用。 您可以從「預覽」畫面複製這些 URL。

選取影像集，然後選取&#x200B;**[!UICONTROL 預覽]**。 現在，請選取影像集檢視器預設集，然後按一下&#x200B;**[!UICONTROL 複製URL]**&#x200B;按鈕。

請參閱[將影像集連結至網頁](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page)。
