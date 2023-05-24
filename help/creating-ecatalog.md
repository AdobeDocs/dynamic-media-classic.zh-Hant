---
title: 建立eCatalog
description: 瞭解如何在Adobe Dynamic Media Classic中建立eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 56%

---

# 建立 eCatalog {#creating-an-ecatalog}

建立 eCatalog 必須進行下列步驟: 排序頁面、選擇頁面版面，以及透過繪製影像地圖、輸入滑鼠指向與超文字連結資料來連結頁面。或者，您也可以自訂目錄 (TOC)，如此一來，檢視者就會在 eCatalog 檢視器中看到頁面名稱，而非頁碼。

## 建立eCatalog {#create}

您可以在eCatalog中包含影像檔案和PDF檔案。

建立 eCatalog 時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog:**

1. 使用下列其中一個技巧來開始建立 eCatalog:

   * **先選取檔案**  — 在「瀏覽」面板中，選取檔案，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**.

   * **從eCatalog畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**. 在資產庫中選取檔案夾，並將檔案從檔案夾中拖曳至「eCatalog」頁面的「排序頁面」頁面。

      >[!NOTE]
      >
      >若要依名稱 (而非縮圖) 來檢視資產庫中的項目，請為「個人設定」中的「預設資產庫視圖」選取「名稱」選項。

1. 為 eCatalog 選取整體版面。選取 **[!UICONTROL 1欄式]** 若為單一頁面， **[!UICONTROL 2欄式]** 適用於雙頁跨頁，或 **[!UICONTROL 自訂]** 適用於超過兩頁的頁面跨頁。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 所有跨頁]** 選項並選取 **[!UICONTROL 確定]**.
1. 或者，您可以選取個別頁面或頁面跨頁，然後選擇 **[!UICONTROL 1欄式]**， **[!UICONTROL 2欄式]**，或 **[!UICONTROL 自訂]** 按鈕。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 選取的跨頁]** 選項並選取 **[!UICONTROL 確定]**.
1. 視需要使用下列其中一個技巧來重新排序頁面:

   * **拖曳**  — 將頁面或跨頁拖曳到新位置。 垂直列會顯示移動頁面的位置。

   * **移動至按鈕**  — 選取頁面或跨頁，選取 **[!UICONTROL 移至]**，然後在功能表中選擇您想要頁面顯示在其前面的頁面。

   * **序號**  — 在「清單檢視」的「序號」欄位中輸入頁碼。

1. 完成時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**.
1. 在「儲存」對話框中，選取一個檔案夾來儲存 eCatalog。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選取 **[!UICONTROL 儲存]**.

   儲存eCatalog後，您可以選取 **[!UICONTROL 預覽]**.

## 編輯eCatalog {#editing-an-ecatalog}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯 eCatalog:**

1. 選取eCatalog的變換 **[!UICONTROL 編輯]** 按鈕。
1. 視需要進行變更。
1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除eCatalog {#deleting-an-ecatalog}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個 eCatalog。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.

## 自訂目錄（目錄） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic會在eCatalog畫面的「訂購頁面」標籤上，提供eCatalog中的預設頁碼。 如需自訂頁面名稱，您可以變更組成目錄 (TOC) 的頁面標籤。建議重新命名封面與封底。例如，封面可以閱讀「封面」而非「第0-1頁」。

您可以手動為 eCatalog 建立自訂的目錄 (TOC)，或從 CSV (僅限 Mac) 或 XML 檔案匯入頁面名稱。

>[!NOTE]
>
>若要還原預設頁面標題，請在 **[!UICONTROL 排序頁面]** 索引標籤，選取 **[!UICONTROL TOC標籤]**，然後選取 **[!UICONTROL 還原預設值（全部）]**.

### 手動輸入頁面名稱 {#manually-entering-page-names}

若要逐次手動輸入頁面名稱，請前往「eCatalog」畫面的「排序頁面」標籤。然後，在頁碼欄位中，為每一個要命名的頁面輸入名稱。

### 匯入頁面名稱 {#importing-page-names}

如果您處理的 eCatalog 包含多個頁面，建議使用匯入頁面名稱。您可以從 Tab 字元分隔檔案或 XML 檔案匯入名稱。

TOC標籤儲存在影像的「使用者資料」欄位中；將此資料格式化為 `name=<value>` ` pairs separated by two question marks “??” `. 例如，若要為名為 `tocEN` 的 TOC 欄位設定一個標籤，請將影像的「使用者資料」設定為:

`tocEN=&lt;EN_page_label>`

若要為命名的TOC欄位設定個別標籤 `tocEN` 和 `tocFR`：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

若要匯入Tab字元分隔檔案中的「使用者資料」欄位，請包含該欄位使用者資料：

| IPSID | 使用者資料 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

若要在 XML 檔案中匯入「使用者資料」欄位，請包括屬性 `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

若要從定位字元分隔或XML檔案匯入頁面名稱，請選取 **[!UICONTROL TOC標籤]** 按鈕並選取 **[!UICONTROL 匯入]**. 在「上傳中繼資料」對話方塊中，選取 **[!UICONTROL 瀏覽]**，然後匯入CSV檔案(僅限Mac)或將每個頁面與頁面名稱建立關聯的XML檔案。
