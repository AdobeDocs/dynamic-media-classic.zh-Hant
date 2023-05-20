---
title: 從Adobe Dynamic Media Classic出口資產
description: 瞭解如何從Adobe Dynamic Media Classic出口資產。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# 從Adobe Dynamic Media Classic出口資產{#exporting-assets-from-dmc}

您可以將在Adobe Dynamic Media Classic編輯的資產保存到本地網路驅動器。 匯出的資產會合併成 ZIP 檔案，適合下載或透過電子郵件傳送。

適用於匯出工作的壓縮 Zip 檔的檔案大小上限為 1 GB。此外，每個導出作業最多允許500個總資產。

Adobe Dynamic Media Classic在「作業」螢幕中記錄了出口作業。

**要從Adobe Dynamic Media Classic出口資產：**

1. 選擇要導出的資產，然後轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 導出]**。
1. 在「匯出選取的資產」視窗中，按一下「**[!UICONTROL 影像選項]**」，然後指定下列任一選項 (管理員會決定使用者可以使用哪些選項):

   * **[!UICONTROL 預設]**  — （可選）選擇「影像預設」以在導出資產時對其進行格式化。 如果選擇「影像預設集」，就無法使用其它格式化選項，因為資產會採用「影像預設集」所定義的格式。

   * **[!UICONTROL 轉換]**  — 轉換資產檔案或原始影像。

   * **[!UICONTROL 大小]**  — 您可以選擇標準大小。 或者，您可以選擇 **[!UICONTROL 其他]** 從 **[!UICONTROL 大小]** 下拉清單，選擇所需的度量單位，然後指定寬度和高度。

      另請參閱 [指定媒體門戶用戶可用的導出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

   * **[!UICONTROL 格式]**  — 選擇影像格式。

   * **[!UICONTROL 顏色]**  — 選擇RGB、CMYK或灰色。

   * **[!UICONTROL 解決]**  — 選擇72 ppi、150 ppi或300 ppi。

   * **[!UICONTROL 作業名稱]**  — 您可以為導出分配作業名稱。

   * **[!UICONTROL 發送電子郵件至]**  — （可選）如果您打算通過電子郵件發送資產，請輸入電子郵件地址。 電子郵件訊息會列出收件者可用來下載資產的 URL。

1. 選擇 **[!UICONTROL 導出]**。

支援三種基本匯出動作:

* 原始檔案 (匯出資產的原始檔案)
* 使用預設集轉換 (使用影像預設集來格式化資產)
* 不使用預設集轉換 (使用匯出對話框來指定影像修飾元)

無法匯出下列資產類型。所有其他產品都生成輸出。

* 影像集
* 演算集
* 迴轉集
* 媒體集
* 多比特率集
* eCatalog

此外，範本無法匯出成「原始檔案」。

您可以使用轉換來匯出下列資產類型:

* 影像
* 範本
* 調整過的影像
* PDF（生成轉換的頁）
* PostScript®

同時選取大量不同資產類型進行匯出時，會導致下列行為:

* 所有無法匯出的資產類型都會在送出工作之前從清單中移除
* 如果要求轉換，則會轉換所有可轉換的類型，而所有其它項目則會以原始形態匯出
