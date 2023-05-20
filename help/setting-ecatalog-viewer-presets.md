---
title: 設定eCatalog Viewer預設
description: 瞭解如何在Adobe Dynamic Media Classic設定eCatalog Viewer預設。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# 設定eCatalog Viewer預設{#setting-up-ecatalog-viewer-presets}

eCatalog 檢視器預設集會決定 eCatalog 檢視器的樣式、行為與外觀。Adobe Dynamic Media Classic提供eCatalog Viewer預設，如果您是管理員，也可以建立自己的eCatalog Viewer預設。

要建立預設，您可以從頭開始，或從Adobe Dynamic Media Classic提供的eCatalog Viewer預設開始，然後以新名稱保存。 您可以自行建立 eCatalog 檢視器預設集，以公司的色彩來呈現列印材料並設定色調。

eCatalog 檢視器預設集提供許多設定，可用來在頁面之間移動、縮放、搜尋和選擇外觀。這些控制項的外觀和查看器的顯示方式取決於您選擇的「eCatalog Viewer預設」。

按照以下步驟建立eCatalog Viewer預設（您必須是管理員）:

1. 在全局導航欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。
1. 如要建立 eCatalog 檢視器預設集，您可以在「檢視器預設集」畫面中從頭開始建立，或從現有 eCatalog 檢視器預設集開始:

   * **建立eCatalog查看器預設**  — 選擇 **[!UICONTROL 添加]**。 在「添加查看器預設」對話框中，選擇一個平台，選擇「目錄查看器」，然後選擇 **[!UICONTROL 添加]**。

   * **編輯eCatalog查看器預設**  — 選擇「eCatalog Viewer預設」，然後選擇 **[!UICONTROL 編輯]**。 選擇 **[!UICONTROL 另存為]** 建立完預設後。

1. 在「設定檢視器」畫面上輸入 eCatalog 檢視器預設集的名稱。
1. 在「設定檢視器」畫面，設定要使用的選項。

   選擇 **[!UICONTROL 資訊提示]** 表徵圖。

   在更新和更改設定時，「預覽」(Preview)頁面將顯示查看器。

1. （可選）在 **[!UICONTROL 資訊面板設定]**，也請參見Wiki頁。 **[!UICONTROL 資訊伺服器URL]** 選項可以包括以下特殊標籤，查看器可以使用這些標籤：

   | 標記 | 取代為 | 附註 |
   | --- | --- | --- |
   | `$1$` | rollover_key 值 | 來自的項標識符 `<area>` 的子菜單。 |
   | `$2$` | frame | 目前在影像集中顯示之影格的序號。 |
   | `$3$` | 影像根 | 在影像命令中指定之第一個項目的第一個路徑元素 (通常為指定影像集之目錄項目的影像目錄 ID)。 |

1. （可選）在 **[!UICONTROL 資訊面板設定]**，也請參見Wiki頁。 **[!UICONTROL 響應模板]** 框中，鍵入當Adobe Dynamic Media Classic在檢索影像映射資訊時遇到錯誤時要顯示的文本。 例如，如果系統收到公司名稱與 eCatalog 名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。

>[!NOTE]
>
>要使用此響應模板而不是eCatalog本身中定義的模板，請添加 `fmt=1` 到「資訊伺服器」URL的末尾。 例如: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 選擇 **[!UICONTROL 保存]**。
1. 選擇 **[!UICONTROL 預設]** 如果希望建立的eCatalog Viewer預設是用於在網頁上顯示eCatalogs的預設。

要刪除eCatalog Viewer預設，請在「查看器預設」螢幕上將其選中，然後選擇 **[!UICONTROL 刪除]**。

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

