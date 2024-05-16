---
title: 從Adobe Dynamic Media Classic匯出資產
description: 瞭解如何從Adobe Dynamic Media Classic匯出資產。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 38%

---

# 從Adobe Dynamic Media Classic匯出資產{#exporting-assets-from-dmc}

您可以在Adobe Dynamic Media Classic中編輯的資產儲存至本機網路磁碟機。 匯出的資產會合併成 ZIP 檔案，適合下載或透過電子郵件傳送。

適用於匯出工作的壓縮 Zip 檔的檔案大小上限為 1 GB。此外，每個匯出作業最多允許500個總資產。

Adobe Dynamic Media Classic會保留「工作」畫面中匯出工作的記錄。

**若要從Adobe Dynamic Media Classic匯出資產：**

1. 選取您要匯出的資產，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯出]**.
1. 在「匯出選取的資產」視窗中，按一下「**[!UICONTROL 影像選項]**」，然後指定下列任一選項 (管理員會決定使用者可以使用哪些選項):

   * **[!UICONTROL 預設集]**：您可選擇在匯出資產時，選擇影像預設集來格式化資產。 如果選擇「影像預設集」，就無法使用其它格式化選項，因為資產會採用「影像預設集」所定義的格式。

   * **[!UICONTROL 轉換]**：轉換資產檔案或原始影像。

   * **[!UICONTROL 大小]**：您可以選取標準大小。 或者，您可以選取 **[!UICONTROL 其他]** 從 **[!UICONTROL 大小]** 從下拉式清單中選擇所需的度量單位，然後指定寬度和高度。

     另請參閱 [指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL 格式]**：選擇影像格式。

   * **[!UICONTROL 顏色]**：選擇「RGB」、「CMYK」或「灰色」。

   * **[!UICONTROL 解析度]**：選擇72 ppi、150 ppi或300 ppi。

   * **[!UICONTROL 工作名稱]**：您可以指派工作名稱給匯出。

   * **[!UICONTROL 傳送電子郵件至]**：選填。 如果您要透過電子郵件傳送資產，請輸入電子郵件地址。 電子郵件訊息會列出收件者可用來下載資產的 URL。

1. 選取 **[!UICONTROL 匯出]**.

支援三種基本匯出動作:

* 原始檔案 (匯出資產的原始檔案)
* 使用預設集轉換（使用影像預設集來格式化資產）
* 不使用預設集轉換 (使用匯出對話框來指定影像修飾元)

無法匯出下列資產類型。所有其他會產生匯出。

* 影像集
* 演算集
* 迴轉集
* 媒體集
* 多位元速率集
* eCatalog

此外，範本無法匯出為「原始檔案」。

您可以使用轉換來匯出下列資產類型:

* 影像
* 範本
* 調整過的影像
* PDF（產生轉換的頁面）
* PostScript®

同時選取大量不同資產類型進行匯出時，會導致下列行為:

* 所有無法匯出的資產型別都會在工作提交前從清單中移除
* 如果要求轉換，所有可轉換的型別都會被匯出，而其他所有型別則會匯出為原始型別
