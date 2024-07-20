---
title: 設定eCatalog檢視器預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定eCatalog檢視器預設集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# 設定eCatalog檢視器預設集{#setting-up-ecatalog-viewer-presets}

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式、行為與外觀。Adobe Dynamic Media Classic提供eCatalog檢視器預設集，如果您是管理員，也可以建立您自己的eCatalog檢視器預設集。

若要建立預設集，您可以從頭開始，或從Adobe Dynamic Media Classic提供的eCatalog檢視器預設集開始，然後以新名稱儲存。 您可以自行建立 eCatalog 檢視器預設集，以公司的色彩來呈現列印材料並設定色調。

eCatalog檢視器預設集提供許多設定，可用於在頁面之間移動、縮放、搜尋及選擇「外觀元素」。 這些控制項的外觀和檢視器的顯示方式取決於您選擇的eCatalog檢視器預設集。

請依照下列步驟進行，以建立eCatalog檢視器預設集（您必須是管理員）：

1. 在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。
1. 如要建立 eCatalog 檢視器預設集，您可以在「檢視器預設集」畫面中從頭開始建立，或從現有 eCatalog 檢視器預設集開始:

   * **建立eCatalog檢視器預設集**：選取&#x200B;**[!UICONTROL 新增]**。 在[新增檢視器預設集]對話方塊中，選擇平台，選擇[eCatalog檢視器]，然後選取[新增]****。

   * **編輯eCatalog檢視器預設集**：選取eCatalog檢視器預設集，然後選取&#x200B;**[!UICONTROL 編輯]**。 完成建立預設集後，選取&#x200B;**[!UICONTROL 另存新檔]**。

1. 在`Configure Viewer`頁面上，輸入eCatalog檢視器預設集的名稱。
1. 在`Configure Viewer`頁面上，設定您想要的選項。

   如果您想要閱讀其說明，請選取選項旁的&#x200B;**[!UICONTROL 資訊提示]**&#x200B;圖示。

   當您更新和變更設定時，「預覽」頁面會顯示檢視器。

1. （選擇性）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;中，**[!UICONTROL 資訊伺服器URL]**&#x200B;選項可以包含以下特殊權杖，檢視器會加以替代：

   | 標記 | 取代為 | 附註 |
   | --- | --- | --- |
   | `$1$` | rollover_key 值 | 對應之`<area>`專案的專案識別碼。 |
   | `$2$` | frame | 目前在影像集中顯示之影格的序號。 |
   | `$3$` | 影像根 | 在影像命令中指定之第一個項目的第一個路徑元素 (通常為指定影像集之目錄項目的影像目錄 ID)。 |

1. （選擇性）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;的&#x200B;**[!UICONTROL 回應範本]**&#x200B;方塊中，輸入Adobe Dynamic Media Classic擷取影像地圖資訊時發生錯誤，要顯示的文字。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。

>[!NOTE]
>
>若要使用此回應範本，而非eCatalog本身所定義的範本，請在資訊伺服器URL的結尾新增`fmt=1`。 例如： `https://.../$3$/$4$/$1$/?FMT=1`。

1. 選取&#x200B;**[!UICONTROL 儲存]**。
1. 選取「**[!UICONTROL 預設]**」，以便您建立的eCatalog檢視器預設集是用來在網頁上顯示eCatalog的。

若要刪除eCatalog檢視器預設集，請在[檢視器預設集]畫面中選取該預設集，然後選取&#x200B;**[!UICONTROL 刪除]**。

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
