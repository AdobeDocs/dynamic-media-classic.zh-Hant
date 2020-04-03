---
title: 從 Scene7 Publishing System 匯出資產
seo-title: 從 Scene7 Publishing System 匯出資產
description: 'null'
seo-description: 瞭解如何從Scene7 Publishing System匯出資產。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 從 Scene7 Publishing System 匯出資產{#exporting-assets-from-scene-publishing-system}

您可以將您在 Scene7 Publishing System 中編輯的資產儲存到本機網路磁碟。匯出的資產會合併成 ZIP 檔案，適合下載或透過電子郵件傳送。

適用於匯出工作的壓縮 Zip 檔的檔案大小上限為 1 GB。另外，請注意，每個匯出工作的總資產上限為 500 個。

Dynamic Media Classic會在「工作」畫面中保留匯出工作的記錄。

**將資產從 Scene7 Publishing System 匯出**

1. 選取要匯出的資產，然後按一下「**檔案** > **匯出**」。
1. 在「匯出選取的資產」視窗中，按一下「**影像選項**」，然後指定下列任一選項 (管理員會決定使用者可以使用哪些選項):

   * **預設**&#x200B;集（可選）在匯出資產時，選擇影像預設集以設定其格式。 如果選擇「影像預設集」，就無法使用其它格式化選項，因為資產會採用「影像預設集」所定義的格式。

   * **轉換**&#x200B;轉換資產檔案或原始影像。

   * **大小**&#x200B;您可以選擇標準大小。 或者，您可以從「大小」下拉式清單按一下「其他」，選擇所需的度量單位，然後指定寬度和高度。

      另請參閱[指定 Media Portal 使用者可使用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

   * **格式**&#x200B;選擇影像格式。

   * **顏色**&#x200B;選擇RGB、CMYK或灰色。

   * **解析**&#x200B;度選擇72、150或300 ppi。

   * **作業名**&#x200B;稱您可以為導出分配作業名稱。

   * **傳送電子郵**&#x200B;件至（可選）輸入電子郵件地址以透過電子郵件傳送資產。 電子郵件訊息會列出收件者可用來下載資產的 URL。

1. 按一下「**匯出**」。

支援三種基本匯出動作:

* 原始檔案 (匯出資產的原始檔案)
* 使用預設集轉換 (使用影像預設集來格式化資產)
* 不使用預設集轉換 (使用匯出對話框來指定影像修飾元)

無法匯出下列資產類型。所有其它項目都應該會產生匯出。

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
* PDF (會產生轉換的頁面)
* Postscript

同時選取大量不同資產類型進行匯出時，會導致下列行為:

* 所有無法匯出的資產類型都會在送出工作之前從清單中移除
* 如果要求轉換，則會轉換所有可轉換的類型，而所有其它項目則會以原始形態匯出

