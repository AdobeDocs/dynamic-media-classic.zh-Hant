---
title: 設定縮放檢視器預設集
seo-title: 設定縮放檢視器預設集
description: 'null'
seo-description: 瞭解如何設定縮放檢視器預設集。
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categores/縮放
discoiquuid: 5023a933-e229-4d3 c-8e91-3ac5 e9 f4970 b
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 設定縮放檢視器預設集{#setting-up-zoom-viewer-presets}

縮放檢視器預設集可確定縮放檢視器的樣式、行為和外觀。Dynamic Media Classic提供許多自訂和外觀設定檢視器的選項。Dynamic Media Classic隨附預設基本(快速)、飛出和自訂縮放檢視器預設集。如果您是管理員，則可以建立新的公司縮放檢視器預設集，或編輯預設預設集並儲存為新名稱。

所有縮放檢視器都帶有用於放大、縮小、平移並在縮放後將影像重設為原始狀態的按鈕。按鈕和視窗的顯示效果取決於所選的縮放檢視器預設集。您可以使用不同的色彩、邊框、字型及影像設定來設定縮放檢視器預設集。設定已導引縮放檢視器時，還可以選擇縮放目標的位置。縮放目標指的是使用者按一下後可縮放到指定區域的縮圖。

## 關於縮放檢視器預設集 {#about-zoom-viewer-presets}

Dynamic Media Classic提供這些縮放檢視器預設集：

**縮放檢視器：基本** 在原始影像上提供基本縮放。

**縮放檢視器：飛出** 顯示原始影像旁縮放區域的第二張影像。沒有控制項可供使用，使用者僅需將選取範圍移動至要檢視的區域上。

決定此檢視器的完整頻寬使用情況時，請考量檢視器會同時處理主要影像和彈出影像。彈出影像大小取決於主影像大小 (舞台寬度和高度) 和縮放係數。若要避免彈出檔案大小過大，請平衡以下兩個值: 如果您的主要影像較大，請降低「縮放係數」值。(「彈出寬度」和「彈出高度」會決定彈出視窗的大小，但不會決定提供給檢視器之彈出影像的大小。)

例如，如果您的主影像大小為 350 x 350 像素且「縮放係數」為 3，則產生的彈出影像為 1050 x 1050 像素。如果您的主影像大小為 300 x 300 像素且「縮放係數」為 4，則彈出影像為 1200 x 1200 像素。視 JPEG 品質設定 (建議設定為 80-90 之間) 而定，您可以顯著地降低檔案大小。建議的縮放係數為 2.5 至 4，視主影像大小而定。

Dynamic Media Classic建議這些參數用於彈出式縮放檢視器預設集：

**放大影像大小** 大約1500x1500像素，不超過2000像素。

**影像大小100** KB或以下，不超過150KB(壓縮檔案將檔案保持在150KB以下)。

**縮放檢視器：自訂** 提供含影像引導或未引導縮放功能、含多重檢視的影像集或色票集。

## 建立和編輯縮放檢視器預設集 {#creating-and-editing-zoom-viewer-presets}

請按照以下步驟建立或編輯縮放檢視器預設集:

1. 按一下「**設定**」&gt;「**檢視器預設集**」。
1. 進行以下一項操作:

   **建立預設集** 按一下新增。在「新增檢視器預設集」對話方塊中，選擇平台、選擇縮放檢視器，然後按一下「新增」。在預設名稱方塊中輸入預設集的名稱。

   **編輯預設集** 選取縮放檢視器預設集，然後按一下 **編輯**。

1. 根據需要指定設定。

   若要查看選項描述，請按一下選項旁的「資訊提示」圖示 。

   預覽畫面會在您更新並變更設定時顯示檢視器。

1. 按一下「**儲存**」或「**另存新檔**」。
1. 在「檢視器預設集」畫面上，檢查建立的縮放檢視器預設集或已導引縮放檢視器預設集。If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

有關在「檢視器預設集」畫面上管理檢視器預設集的資訊，請參閱[檢視器預設集](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [Creating and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets)

