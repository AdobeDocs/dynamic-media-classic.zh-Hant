---
title: 從Dynamic Media Classic匯出資產
description: 了解如何從Dynamic Media Classic匯出資產。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 52%

---

# 從Dynamic Media Classic匯出資產{#exporting-assets-from-dmc}

您可以將在Dynamic Media Classic中編輯的資產儲存至本機網路磁碟。 匯出的資產會合併成 ZIP 檔案，適合下載或透過電子郵件傳送。

適用於匯出工作的壓縮 Zip 檔的檔案大小上限為 1 GB。此外，每個匯出工作最多可允許500個資產。

Dynamic Media Classic會在「工作」畫面中保留匯出工作的記錄。

**若要從Dynamic Media Classic匯出資產：**

1. 選取您要匯出的資產，然後前往&#x200B;**[!UICONTROL File]** > **[!UICONTROL Export]**。
1. 在「匯出選取的資產」視窗中，按一下「**[!UICONTROL 影像選項]**」，然後指定下列任一選項 (管理員會決定使用者可以使用哪些選項):

   * **[!UICONTROL 預設]**  — （可選）選擇影像預設集，以在您匯出資產時設定資產的格式。如果選擇「影像預設集」，就無法使用其它格式化選項，因為資產會採用「影像預設集」所定義的格式。

   * **[!UICONTROL 轉換]**  — 轉換資產檔案或原始影像。

   * **[!UICONTROL 大小]**  — 您可以選取標準大小。或者，您可以從&#x200B;**[!UICONTROL Size]**&#x200B;下拉清單中選擇&#x200B;**[!UICONTROL Other]**，選擇所需的度量單位，然後指定寬度和高度。

      另請參閱[指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

   * **[!UICONTROL 格式]**  — 選擇影像格式。

   * **[!UICONTROL 顏色]**  — 選擇RGB、CMYK或灰色。

   * **[!UICONTROL 解析度]**  — 選擇72 ppi、150 ppi或300 ppi。

   * **[!UICONTROL 作業名稱]**  — 您可以為匯出指派作業名稱。

   * **[!UICONTROL 傳送電子郵件至]**  — （可選）如果您要透過電子郵件傳送資產，請輸入電子郵件地址。電子郵件訊息會列出收件者可用來下載資產的 URL。

1. 選擇&#x200B;**[!UICONTROL 導出]**。

支援三種基本匯出動作:

* 原始檔案 (匯出資產的原始檔案)
* 使用預設集轉換 (使用影像預設集來格式化資產)
* 不使用預設集轉換 (使用匯出對話框來指定影像修飾元)

無法匯出下列資產類型。其他所有項目都會產生匯出。

* 影像集
* 演算集
* 迴轉集
* 媒體集
* 多個位元速率設定
* eCatalog

此外，範本無法匯出成「原始檔案」。

您可以使用轉換來匯出下列資產類型:

* 影像
* 範本
* 調整過的影像
* PDF（生成轉換的頁面）
* PostScript®

同時選取大量不同資產類型進行匯出時，會導致下列行為:

* 所有無法匯出的資產類型都會在送出工作之前從清單中移除
* 如果要求轉換，則會轉換所有可轉換的類型，而所有其它項目則會以原始形態匯出
