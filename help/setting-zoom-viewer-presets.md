---
title: 設定縮放檢視器預設集
description: 了解如何在AdobeDynamic Media Classic中設定縮放檢視器預設集。
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 47%

---

# 設定縮放檢視器預設集{#setting-up-zoom-viewer-presets}

縮放檢視器預設集可確定縮放檢視器的樣式、行為和外觀。AdobeDynamic Media Classic提供許多自訂和外觀檢視器的選項。 AdobeDynamic Media Classic隨附預設的基本（快速）、快速退出和自訂縮放檢視器預設集。 如果您是管理員，可以建立公司「縮放檢視器預設集」或編輯預設的預設集，並以新名稱儲存。

所有縮放檢視器都帶有用於放大、縮小、平移並在縮放後將影像重設為原始狀態的按鈕。這些按鈕的外觀和窗口本身的顯示方式取決於您選擇的縮放查看器預設集。 您可以使用不同的色彩、邊框、字型及影像設定來設定縮放檢視器預設集。設定已導引縮放檢視器時，還可以選擇縮放目標的位置。縮放目標指的是使用者按一下後可縮放到指定區域的縮圖。

## 關於縮放檢視器預設集 {#about-zoom-viewer-presets}

AdobeDynamic Media Classic提供下列縮放檢視器預設集：

* **縮放檢視器：基本**  — 提供原始影像的基本縮放。

* **縮放檢視器：飛出**  — 在原始影像旁邊顯示縮放區域的第二個影像。沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。彈出影像大小取決於主影像大小 (舞台寬度和高度) 和縮放係數。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

AdobeDynamic Media Classic建議使用下列參數進行快速縮小檢視器預設集：

* **放大影像大**  — 約1500 x 1500像素，不超過2000 x 2000像素。

* **影像大小** - 100 KB或以下，不超過150 KB（壓縮檔案以使其保持在150 KB以下）。

* **縮放檢視器：自訂**  — 提供有影像的引導式或未引導式縮放、有多個檢視的影像集或色票集。

## 建立和編輯縮放檢視器預設集 {#creating-and-editing-zoom-viewer-presets}

1. 在全局導航欄上，轉到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。
1. 進行以下一項操作:

   * **建立預設集**  — 選取 **[!UICONTROL 「新增」]**。在「添加查看器預設集」對話框中，選擇平台，選擇縮放查看器，然後選擇&#x200B;**[!UICONTROL 添加]**。 在「預設集名稱」方塊中輸入預設集的名稱。

   * **編輯預設集**  — 選取「縮放檢視器預設集」，然後選取「 **[!UICONTROL 編輯]**」。

1. 根據需要指定設定。

   若要查看選項的說明，請選取選項旁的&#x200B;**[!UICONTROL 資訊提示]**&#x200B;圖示。

   預覽頁面會在您更新和變更設定時顯示檢視器。

1. 選擇「**[!UICONTROL 保存]**」或「**[!UICONTROL 另存為]**」。
1. 在「查看器預設集」頁上，檢查您建立的「縮放查看器預設集」或「引導式縮放查看器預設集」。 如果需要調整，請選擇&#x200B;**[!UICONTROL Edit]**，更改「配置查看器」頁上的設定，然後選擇&#x200B;**[!UICONTROL Save]**。

有關在「檢視器預設集」畫面上管理檢視器預設集的資訊，請參閱[檢視器預設集](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [建立和編輯查看器預設集](application-setup.md#adding_and_editing_viewer_presets)

