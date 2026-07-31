---
title: 字型
description: 瞭解如何在Adobe Dynamic Media Classic中使用字型。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:28.929Z'
TQID: 'https://experienceleague.adobe.com/g-A6M8KM6VT4m-JVyDp6KMMN82CtGTXcoUFVvQsoLps'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: aff765628275d5725ace65a497424effb8213c37
workflow-type: tm+mt
source-wordcount: 431
ht-degree: 16%

---

# 字型{#fonts}

有時候，Adobe Dynamic Media Classic會要求您上傳字型檔案，以輸入或轉譯特定字型的文字。 例如，要在範本圖層上將特定的字型用於文字，請上載字型檔案。 若要以特定的字型顯示 eCatalog 檢視器頁碼，請上載字型檔案。

Adobe Dynamic Media Classic支援下列字型型別：

* 所有 TrueType 字型
* PostScript®字型
* OpenType/TrueType 字型
* OpenType/PostScript 字型
* PhotoFont

上傳字型檔案後，您可以變更其Adobe Dynamic Media Classic ID、字型名稱，並在「編輯資訊」畫面上輸入資訊。

>[!NOTE]
>
>如果您打算在範本圖層中使用字型，Adobe Dynamic Media Classic建議您上傳所有字型樣式（粗體、斜體、粗體/斜體及一般字型）。 Adobe Dynamic Media Classic需要這些字型樣式來處理請求。 也建議上傳與某個字型關聯的所有`PostScript/Adobe Type1`檔案，因為其中某些字型包含特定的字距微調資料。

## 上傳字型檔案 {#uploading-font-files}

使用與上載其他檔案相同的方法上載字型檔案。 您可以將字型檔案儲存在任何Adobe Dynamic Media Classic資料夾中。 請參閱[上載檔案](uploading-files.md#uploading_your_files)。

## 編輯字型檔案資訊 {#editing-font-file-information}

您可以變更字型的ID名稱及其型別資訊。 編輯字型檔案有助於搜尋，並讓字型更容易識別。

在「瀏覽」面板中，選取要在「詳細檢視」中編輯的字型檔案，然後選擇「檔案>編輯資訊」。 此時將開啟「編輯資訊」畫面。 選擇下列選項，然後選取&#x200B;**[!UICONTROL 提交]**。

* **[!UICONTROL 字型名稱]**：此名稱可識別發佈時的字型。

* **[!UICONTROL PostScript名稱]**：此名稱是字型的完整PostScript名稱。 它通常表示粗細或樣式。

* **[!UICONTROL RTF名稱]**：此名稱會出現在建立範本文字圖層的RTF編輯器中的彈出式選單上。

* **[!UICONTROL 字型系列名稱]**：此名稱列出字型名稱，但沒有樣式、粗細或字型型別指示器。

* **[!UICONTROL 字型樣式]**：選項為純、粗體、斜體及粗斜體。

* **[!UICONTROL 字型型別]**：選項為TrueType和Adobe Type 1。 如果您以其他名稱呼叫這些字型，則可以輸入這些名稱。

* **[!UICONTROL 字型型別縮寫]**：選項如下：

  * **[!UICONTROL TTF]**：用於PDF/PostScript轉譯與影像伺服的TrueType字型檔案。

  * **[!UICONTROL AFM]**：包含Adobe字型度量資訊且用於影像伺服的Adobe PostScript字型檔案。

  * **[!UICONTROL PFM]**：包含二進位字型量度資訊的Adobe PostScript字型檔案。

  * **[!UICONTROL PFB]**：包含二進位字型外框資訊的Adobe PostScript字型檔案，用於PDF/PostScript轉譯及影像伺服。
