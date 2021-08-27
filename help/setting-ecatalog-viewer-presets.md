---
title: 設定 eCatalog 檢視器預設集
description: 了解如何設定eCatalog檢視器預設集。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 42%

---

# 設定 eCatalog 檢視器預設集{#setting-up-ecatalog-viewer-presets}

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式、行為與外觀。AdobeDynamic Media Classic提供eCatalog檢視器預設集，如果您是管理員，也可以建立自己的eCatalog檢視器預設集。

若要建立預設集，您可以從草稿開始，或從AdobeDynamic Media Classic提供的eCatalog檢視器預設集開始，並以新名稱儲存。 您可以自行建立 eCatalog 檢視器預設集，以公司的色彩來呈現列印材料並設定色調。

eCatalog 檢視器預設集提供許多設定，可用來在頁面之間移動、縮放、搜尋和選擇外觀。這些控制項的外觀和查看器的顯示方式取決於您選擇的eCatalog查看器預設集。

請依照下列步驟操作，以建立eCatalog檢視器預設集（您必須是管理員）:

1. 在全局導航欄上，按一下「**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**」。
1. 如要建立 eCatalog 檢視器預設集，您可以在「檢視器預設集」畫面中從頭開始建立，或從現有 eCatalog 檢視器預設集開始:

   * **建立eCatalog檢視器預設集**  — 按一下 **[!UICONTROL 「新增」]**。在「添加查看器預設集」對話框中，選擇平台，選擇eCatalog查看器，然後按一下「**[!UICONTROL 添加]**」。

   * **編輯eCatalog檢視器預設集**  — 選取eCatalog檢視器預設集，然後按一下「編輯」。建立完預設集後，按一下「**[!UICONTROL 另存新檔」。]**

1. 在「設定檢視器」畫面上輸入 eCatalog 檢視器預設集的名稱。
1. 在「設定檢視器」畫面，設定要使用的選項。

   如果要閱讀選項的說明，請按一下選項旁的&#x200B;**[!UICONTROL 資訊提示]**&#x200B;圖示。

   預覽頁面會在您更新和變更設定時顯示檢視器。

1. （選用）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;中，**[!UICONTROL 資訊伺服器URL]**&#x200B;選項可包含下列特殊代號，供檢視器取代：

   | 標記 | 取代為 | 附註 |
   |--- |--- |--- |
   | `$1$` | rollover_key 值 | 來自地圖的`<area>`元素的項目識別碼。 |
   | `$2$` | frame | 目前在影像集中顯示之影格的序號。 |
   | `$3$` | imageroot | 在影像命令中指定之第一個項目的第一個路徑元素 (通常為指定影像集之目錄項目的影像目錄 ID)。 |

1. （可選）在&#x200B;**[!UICONTROL 資訊面板設定]**&#x200B;中，在&#x200B;**[!UICONTROL 回應範本]**&#x200B;方塊中，輸入如果AdobeDynamic Media Classic在擷取影像地圖的資訊時遇到錯誤，您要顯示的文字。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。

>[!NOTE]
>
>要使用此響應模板，而不是eCatalog本身中定義的模板，請將`fmt=1`添加到資訊伺服器URL的末尾。 例如: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 按一下&#x200B;**「儲存」**。
1. 如果要讓您建立的 eCatalog 檢視器預設集成為用來在網頁上顯示 eCatalog 的內容，請按一下「預設」。

若要刪除eCatalog檢視器預設集，請在「檢視器預設集」畫面上選取該預設集，然後按一下&#x200B;**[!UICONTROL Delete]**。

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

