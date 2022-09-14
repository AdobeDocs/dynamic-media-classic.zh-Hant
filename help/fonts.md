---
title: 字型
description: 了解如何在Adobe Dynamic Media Classic中使用字型。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# 字型{#fonts}

有時，Adobe Dynamic Media Classic會要求您上傳字型檔案，以輸入或轉譯特定字型的文字。 例如，要在範本圖層上將特定的字型用於文字，請上載字型檔案。若要以特定的字型顯示 eCatalog 檢視器頁碼，請上載字型檔案。

Adobe Dynamic Media Classic支援下列字型類型：

* 所有 TrueType 字型
* PostScript®字型
* OpenType/TrueType 字型
* OpenType/PostScript 字型
* PhotoFont

上傳字型檔案後，您可以在「編輯資訊」畫面上變更其Adobe Dynamic Media Classic ID、字型名稱和輸入資訊。

>[!NOTE]
>
>如果您打算在範本圖層中使用字型，Adobe Dynamic Media Classic建議上傳所有字型樣式（粗體、斜體、粗體/斜體和規則）。 Adobe Dynamic Media Classic需要這些字型樣式來處理要求。 還建議上載與某種字型相關的所有 PostScript/ADOBE Type 1 檔案，因為其中的某些字型包含詳細的字距微調資訊。

## 上傳字型檔案 {#uploading-font-files}

使用與上載其他檔案相同的方法上載字型檔案。您可以將字型檔案儲存在任何Adobe Dynamic Media Classic資料夾中。 請參閱[上載檔案](uploading-files.md#uploading_your_files)。

## 編輯字型檔案資訊 {#editing-font-file-information}

您可以變更字型的ID名稱及其類型資訊。 編輯字型檔案有助於搜尋，並且使得字型更易於識別。

在「瀏覽」面板中，選擇要在「詳細資訊視圖」中編輯的字型檔案，然後選擇「檔案」>「編輯資訊」。 此時將開啟「編輯資訊」畫面。選擇以下選項，然後選擇 **[!UICONTROL 提交]**.

* **[!UICONTROL 字型名稱]**  — 此名稱在發佈時標識字型。

* **[!UICONTROL PostScript名稱]**  — 此名稱是字型的完整PostScript名稱。 它通常表示粗細或樣式。

* **[!UICONTROL RTF名稱]**  — 此名稱顯示在RTF編輯器的彈出菜單上，該菜單中建立了模板文本層。

* **[!UICONTROL 字型系列名稱]**  — 此名稱列出字型名稱，不帶樣式、粗細或字型類型指示器。

* **[!UICONTROL 字型樣式]**  — 選項為純、粗體、斜體和粗體斜體。

* **[!UICONTROL 字型類型]**  — 選項為TrueType和Adobe Type1。 如果使用其他名稱命名這些字型，可以輸入該名稱。

* **[!UICONTROL 字型類型縮寫]**  — 選項如下：

   * **[!UICONTROL TTF]**  — 用於PDF/PostScript呈現和影像服務的TrueType字型檔案。

   * **[!UICONTROL AFM]**  — 包含「Adobe字型量度」資訊且用於影像提供的Adobe PostScript字型檔案。

   * **[!UICONTROL PFM]**  — 包含二進位字型度量資訊的Adobe PostScript字型檔案。

   * **[!UICONTROL PFB]**  — 包含二進位字型輪廓資訊的Adobe PostScript字型檔案，用於PDF/PostScript呈現和影像服務。
