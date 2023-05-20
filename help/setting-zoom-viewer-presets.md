---
title: 設定縮放查看器預設
description: 瞭解如何在Adobe Dynamic Media Classic設定縮放查看器預設。
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 47%

---

# 設定縮放查看器預設{#setting-up-zoom-viewer-presets}

縮放檢視器預設集可確定縮放檢視器的樣式、行為和外觀。Adobe Dynamic Media Classic為定制和剝皮觀眾提供了多種選擇。 Adobe Dynamic Media Classic提供了預設的基本（快速）、彈出和自定義縮放查看器預設。 如果您是管理員，則可以建立公司「縮放查看器預設」或編輯預設預設並使用新名稱保存。

所有縮放檢視器都帶有用於放大、縮小、平移並在縮放後將影像重設為原始狀態的按鈕。這些按鈕的外觀和窗口本身的顯示方式取決於您選擇的「縮放查看器預設」。 您可以使用不同的色彩、邊框、字型及影像設定來設定縮放檢視器預設集。設定已導引縮放檢視器時，還可以選擇縮放目標的位置。縮放目標指的是使用者按一下後可縮放到指定區域的縮圖。

## 關於縮放檢視器預設集 {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic提供以下縮放查看器預設：

* **縮放查看器：基本**  — 提供原始影像的基本縮放。

* **縮放查看器：飛出**  — 在原始影像旁顯示縮放區域的第二個影像。 沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。彈出影像大小取決於主影像大小 (舞台寬度和高度) 和縮放係數。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

Adobe Dynamic Media Classic為「快速縮放查看器預設」建議以下參數：

* **放大的影像大小**  — 約1500 x 1500像素，不超過2000 x 2000像素。

* **影像大小** - 100 KB或更低，不超過150 KB（壓縮檔案使其保持在150 KB以下）。

* **縮放查看器：自定義**  — 提供有指導或未引導的影像縮放、具有多個視圖的影像集或顏色色板集。

## 建立和編輯縮放查看器預設 {#creating-and-editing-zoom-viewer-presets}

1. 在全局導航欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。
1. 進行以下一項操作:

   * **建立預設**  — 選擇 **[!UICONTROL 添加]**。 在「添加查看器預設」對話框中，選擇一個平台，選擇一個縮放查看器，然後選擇 **[!UICONTROL 添加]**。 在「預設名稱」框中輸入預設的名稱。

   * **編輯預設**  — 選擇縮放查看器預設，然後選擇 **[!UICONTROL 編輯]**。

1. 根據需要指定設定。

   要查看選項的說明，請選擇 **[!UICONTROL 資訊提示]** 表徵圖。

   在更新和更改設定時，「預覽」(Preview)頁面將顯示查看器。

1. 選擇 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存為]**。
1. 在「查看器預設」頁面上，檢查您建立的「縮放查看器預設」或「指導縮放查看器預設」。 如果需要調整，請選擇 **[!UICONTROL 編輯]**，更改「配置查看器」頁上的設定，然後選擇 **[!UICONTROL 保存]**。

有關在「檢視器預設集」畫面上管理檢視器預設集的資訊，請參閱[檢視器預設集](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [建立和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)

