---
title: 設定 eCatalog 檢視器預設集
description: 瞭解如何設定eCatalog檢視器預設集。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media經典，檢視器，檢視器預設集，eCatalog
role: Business Practitioner
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
translation-type: tm+mt
source-git-commit: 6f3801a71dd2a5f162acacf7d8199dbf8c3520f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 42%

---

# 設定 eCatalog 檢視器預設集{#setting-up-ecatalog-viewer-presets}

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式、行為與外觀。Dynamic Media·Classic提供eCatalog檢視器預設集，如果您是管理員，也可以建立您自己的eCatalog檢視器預設集。

若要建立預設集，您可以從頭開始，或從Dynamic MediaClassic提供的eCatalog檢視器預設集開始，然後以新名稱儲存。 您可以自行建立 eCatalog 檢視器預設集，以公司的色彩來呈現列印材料並設定色調。

eCatalog 檢視器預設集提供許多設定，可用來在頁面之間移動、縮放、搜尋和選擇外觀。這些控制項的外觀和檢視器的顯示方式取決於您選擇的eCatalog檢視器預設集。

請遵循下列步驟，以建立eCatalog檢視器預設集（您必須是管理員）:

1. 在全域導覽列上，按一下「設定&#x200B;**** > **[!UICONTROL 檢視器預設集]**」。
1. 如要建立 eCatalog 檢視器預設集，您可以在「檢視器預設集」畫面中從頭開始建立，或從現有 eCatalog 檢視器預設集開始:

   * **建立eCatalog檢視器預設集** -按一下「 **[!UICONTROL 新增]**」。在「新增檢視器預設集」對話方塊中，選擇平台、選擇eCatalog檢視器，然後按一下「新增&#x200B;****」。

   * **編輯eCatalog檢視器預設集** -選取eCatalog檢視器預設集，然後按一下「編輯」。完成預設集建立後，按一下「另存為」。****

1. 在「設定檢視器」畫面上輸入 eCatalog 檢視器預設集的名稱。
1. 在「設定檢視器」畫面，設定要使用的選項。

   如果要讀取選項的說明，請按一下選項旁的&#x200B;**[!UICONTROL 資訊提示]**&#x200B;表徵圖。

   「預覽」頁面會在您更新和變更設定時顯示檢視器。

1. （選擇性）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;中，**[!UICONTROL 資訊伺服器URL]**&#x200B;選項可包含下列檢視器替代的特殊Token:

   | 標記 | 取代為 | 附註 |
   |--- |--- |--- |
   | `$1$` | rollover_key 值 | 映射的`<area>`元素中的項目標識符。 |
   | `$2$` | frame | 目前在影像集中顯示之影格的序號。 |
   | `$3$` | imageroot | 在影像命令中指定之第一個項目的第一個路徑元素 (通常為指定影像集之目錄項目的影像目錄 ID)。 |

1. （可選）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;的&#x200B;**[!UICONTROL 回應範本]**&#x200B;方塊中，輸入當Dynamic Media經典在擷取影像地圖資訊時遇到錯誤時要顯示的文字。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。

>[!NOTE]
>
>要使用此響應模板而不是eCatalog本身中定義的模板，請將`fmt=1`添加到資訊伺服器URL的末尾。 例如: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 按一下&#x200B;**「儲存」**。
1. 如果要讓您建立的 eCatalog 檢視器預設集成為用來在網頁上顯示 eCatalog 的內容，請按一下「預設」。

若要刪除eCatalog檢視器預設集，請在「檢視器預設集」畫面上選取它，然後按一下「刪除&#x200B;****」。

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

