---
title: 字型
seo-title: 字型
description: 'null'
seo-description: 瞭解如何在Dynamic Media Classic中使用字體。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/support_ files
discoiquuid: 97cdc6a-30aa-44Fe-a611-fd71 b02 b2 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 字型{#fonts}

在某些情況下，Scene7 Publishing System 要求您上載字型檔案，以便使用特定的字型輸入或演算文字。例如，要在範本圖層上將特定的字型用於文字，請上載字型檔案。若要以特定的字型顯示 eCatalog 檢視器頁碼，請上載字型檔案。

Dynamic Media Classic支援以下字型類型：

* 所有 TrueType 字型
* PostScript®字體
* OpenType/TrueType 字型
* OpenType/PostScript 字型
* PhotoFont

上載字型檔案之後，您可以在「編輯資訊」畫面中變更其 SPS ID、字型名稱和類型資訊。

>[!NOTE]
>
>Dynamic Media Classic建議您在範本圖層中使用字體時，上傳所有字體樣式(粗體、斜體、粗體/斜體)。Dynamic Media Classic需要這些字型樣式來處理要求。還建議上載與某種字型相關的所有 PostScript/ADOBE Type 1 檔案，因為其中的某些字型包含詳細的字距微調資訊。

## 上載字型檔案 {#uploading-font-files}

使用與上載其他檔案相同的方法上載字型檔案。您可以將字型檔案儲存在任何 SPS 檔案夾中。請參閱[上載檔案](uploading-files.md#uploading_your_files)。

## 編輯字型檔案資訊 {#editing-font-file-information}

您可以變更字型的 ID 名稱及其類型資訊。編輯字型檔案有助於搜尋，並且使得字型更易於識別。

在瀏覽面板中，選取您要在詳細檢視中編輯的字型檔案，然後選取「檔案 &gt; 編輯資訊」。此時將開啟「編輯資訊」畫面。選擇以下選項，然後選取「送出」按鈕。

**字型名稱** ：此名稱會在發佈字體時識別。

**PostScript名稱** 此名稱為字體的完整PostScript名稱。它通常表示粗細或樣式。

**RTF名稱** 此名稱會顯示在RTF編輯器的快顯功能表上，其中會建立範本文字圖層。

**字型系列名稱** 此名稱會列出字體名稱，而沒有樣式、粗細或字體類型指標。

**字型樣式** ：選項為「純」、「粗體」、「斜體」和「粗體」。

**字型類型** ：選項為TrueType和Adobe Type1。如果使用其他名稱命名這些字型，可以輸入該名稱。

**字型類型縮寫** 選項如下所示：

**TTF** TrueType字型檔案，用於PDF/PostScript轉譯和影像伺服。

**包含** Adobe字型度量資訊並用於影像服務的AFM Adobe PostScript字體檔案。

**包含二進位字體度量資訊的PFM** Adobe PostScript字體檔案。

**包含二進位字型外框資訊的PFB** Adobe PostScript字體檔案，並用於PDF/PostScript演算和影像伺服。
