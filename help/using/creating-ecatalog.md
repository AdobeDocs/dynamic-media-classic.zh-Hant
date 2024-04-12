---
title: 建立eCatalog
description: 瞭解如何在Adobe Dynamic Media Classic中建立eCatalog。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 44%

---

# 建立 eCatalog {#creating-an-ecatalog}

建立 eCatalog 必須進行下列步驟: 排序頁面、選擇頁面版面，以及透過繪製影像地圖、輸入滑鼠指向與超文字連結資料來連結頁面。或者，您也可以自訂目錄 (TOC)，如此一來，檢視者就會在 eCatalog 檢視器中看到頁面名稱，而非頁碼。

## 建立eCatalog {#create}

您可以在eCatalog中包含影像檔案和PDF檔案。

建立 eCatalog 時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| 儲存前是否已選取「儲存後發佈」選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要建立eCatalog：**

1. 使用下列其中一個技巧來開始建立 eCatalog:

   * **請先選取檔案**  — 在「瀏覽」面板中，選取檔案，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**.

   * **從eCatalog畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**. 在資產庫中選取檔案夾，並將檔案從檔案夾中拖曳至「eCatalog」頁面的「排序頁面」頁面。

     >[!NOTE]
     >
     >若要依名稱 (而非縮圖) 來檢視資產庫中的項目，請為「個人設定」中的「預設資產庫視圖」選取「名稱」選項。

1. 為 eCatalog 選取整體版面。選取 **[!UICONTROL 1欄式]** 若為單一頁面， **[!UICONTROL 2欄式]** 適用於雙頁跨頁，或 **[!UICONTROL 自訂]** 適用於超過兩頁的頁面跨頁。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 全部展開]** 選項並選取 **[!UICONTROL 確定]**.
1. 或者，您可以選取個別頁面或跨頁頁面，然後選擇 **[!UICONTROL 1欄式]**， **[!UICONTROL 2欄式]**，或 **[!UICONTROL 自訂]** 按鈕。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 展開選取專案]** 選項並選取 **[!UICONTROL 確定]**.
1. 視需要使用下列其中一個技巧來重新排序頁面:

   * **拖曳**  — 將頁面或跨頁拖曳到新位置。 垂直列會顯示移動頁面的位置。

   * **移至按鈕**  — 選取頁面或跨頁，選取 **[!UICONTROL 移至]**，然後在功能表中選擇您想讓頁面在之前顯示的頁面。

   * **序號**  — 在清單檢視中，在「序號」欄位中輸入頁碼。

1. 完成時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**.
1. 在「儲存」對話框中，選取一個檔案夾來儲存 eCatalog。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選取 **[!UICONTROL 儲存]**.

   在儲存eCatalog後，您可以選取 **[!UICONTROL 預覽]**.

## 編輯eCatalog {#editing-an-ecatalog}

無論您是編輯已發佈集合還是未發佈集合， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響集合與設定成員：

| 已發佈集? | 儲存編輯內容前，是否已選取「儲存後發佈」選項？ | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員會保留其已發佈狀態。 在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要編輯eCatalog：**

1. 選取eCatalog的變換 **[!UICONTROL 編輯]** 按鈕。
1. 視需要進行變更。
1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除eCatalog

刪除集時，便會將集本身移到垃圾桶。不過，該集內的成員（或「子系」）不受影響；相反地，它們各自保留其現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**若要刪除eCatalog：**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個 eCatalog。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.

## 自訂目錄（目錄） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic會在eCatalog畫面的「訂購頁面」標籤上，提供eCatalog中的預設頁碼。 如需自訂頁面名稱，您可以變更組成目錄 (TOC) 的頁面標籤。建議重新命名封面與封底。例如，封面可以閱讀「封面」而非「第0-1頁」。

您可以手動建立eCatalog的自訂目錄(TOC)，或是從CSV (僅限Mac)或XML檔案匯入頁面名稱。

>[!NOTE]
>
>若要還原預設頁面標題，請在 **[!UICONTROL 排序頁面]** 索引標籤，選取 **[!UICONTROL TOC標籤]**，然後選取 **[!UICONTROL 還原預設值（全部）]**.

### 手動輸入頁面名稱 {#manually-entering-page-names}

若要逐次手動輸入頁面名稱，請前往「eCatalog」畫面的「排序頁面」標籤。然後，在頁碼欄位中，輸入您要命名之各頁面的名稱。

### 匯入頁面名稱 {#importing-page-names}

如果您處理的 eCatalog 包含多個頁面，建議使用匯入頁面名稱。您可以從 Tab 字元分隔檔案或 XML 檔案匯入名稱。

TOC標籤儲存在影像的「使用者資料」欄位中；將此資料格式化為 `name=<value>` ` pairs separated by two question marks "??" `. 例如，為名為的目錄欄位設定一個標籤 `tocEN`，將影像的使用者資料設為：

`tocEN=&lt;EN_page_label>`

若要為命名的TOC欄位設定個別標籤 `tocEN` 和 `tocFR`：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

若要以定位字元分隔的檔案匯入「使用者資料」欄位，請包含該欄位使用者資料：

| IPSID | 使用者資料 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

若要在XML檔案中匯入「使用者資料」欄位，請包含屬性 `vc_userdata`：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

若要從定位字元分隔或XML檔案匯入頁面名稱，請選取 **[!UICONTROL TOC標籤]** 按鈕並選取 **[!UICONTROL 匯入]**. 在「上載中繼資料」對話方塊中，選取 **[!UICONTROL 瀏覽]**，然後匯入CSV檔案(僅限Mac)或將每個頁面與頁面名稱建立關聯的XML檔案。
