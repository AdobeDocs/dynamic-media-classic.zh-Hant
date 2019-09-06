---
title: 設定 eCatalog 檢視器預設集
seo-title: 設定 eCatalog 檢視器預設集
description: 'null'
seo-description: 瞭解如何設定eCatalog檢視器預設集。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
discoiquuid: 6c123f85-3bc4-4392-a7 fb-55618127c65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 設定 eCatalog 檢視器預設集{#setting-up-ecatalog-viewer-presets}

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式、行為與外觀。Dynamic Media Classic提供eCatalog檢視器預設集，而且您也可以建立自己的eCatalog檢視器預設集，如果您是管理員。

若要建立新預設集，您可以從頭開始或從Dynamic Media Classic提供的eCatalog檢視器預設集開始，並以新名稱儲存它。您可以自行建立 eCatalog 檢視器預設集，以公司的色彩來呈現列印材料並設定色調。

eCatalog 檢視器預設集提供許多設定，可用來在頁面之間移動、縮放、搜尋和選擇外觀。這些控制項的外觀與檢視器本身的外觀取決於您對 eCatalog 檢視器預設集的選擇。

遵循下列步驟即可建立 eCatalog 檢視器預設集 (您必須是管理員):

1. 按一下「**設定**」&gt;「**檢視器預設集**」。
1. 如要建立 eCatalog 檢視器預設集，您可以在「檢視器預設集」畫面中從頭開始建立，或從現有 eCatalog 檢視器預設集開始:

   **建立eCatalog檢視器預設集** 按一下新增。In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **編輯eCatalog檢視器預設集** 選取eCatalog檢視器預設集，然後按一下「編輯」。Click **Save As** after you finish creating the preset.

1. 在「設定檢視器」畫面上輸入 eCatalog 檢視器預設集的名稱。
1. 在「設定檢視器」畫面，設定要使用的選項。

   按一下選項旁的「資訊提示」圖示以查看其描述。

   預覽畫面會在您更新並變更設定時顯示檢視器。

1. (選擇性) 在「資訊面板設定」中，「資訊伺服器 URL」選項可以包含下列特殊標記，檢視器會加以替代:

   | 標記 | 取代為 | 附註 |
   |--- |--- |--- |
   | `$1$` | rollover_key 值 | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | 目前在影像集中顯示之影格的序號。 |
   | `$3$` | imageroot | 在影像命令中指定之第一個項目的第一個路徑元素 (通常為指定影像集之目錄項目的影像目錄 ID)。 |

1. (選擇性)在資訊面板設定中，在「回應範本」方塊中，如果Dynamic Media Classic遇到影像地圖擷取資訊時發生錯誤，請輸入您要顯示的文字。例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。

>[!NOTE]
>
>若要使用此「回應範本」而非 eCatalog 本身定義的範本，請在資訊伺服器 URL 的末端加上「fmt=1」。例如: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 按一下&#x200B;**「儲存」**。
1. 如果要讓您建立的 eCatalog 檢視器預設集成為用來在網頁上顯示 eCatalog 的內容，請按一下「預設」。

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
