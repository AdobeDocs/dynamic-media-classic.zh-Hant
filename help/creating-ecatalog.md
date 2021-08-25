---
title: 建立eCatalog
description: 了解如何在Dynamic Media Classic中建立eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic，檢視器，eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 57%

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

   * **首先選取檔案**  — 在「瀏覽」面板中，選取檔案，然後前往「建 **[!UICONTROL 置]**  >  **[!UICONTROL eCatalog」]**。

   * **從eCatalog畫面開始**  — 前往 **[!UICONTROL 建置]**  >  **[!UICONTROL eCatalog]**。在資產庫中選取檔案夾，並將檔案從檔案夾中拖曳至「eCatalog」頁面的「排序頁面」頁面。

      >[!NOTE]
      >
      >若要依名稱 (而非縮圖) 來檢視資產庫中的項目，請為「個人設定」中的「預設資產庫視圖」選取「名稱」選項。

1. 為 eCatalog 選取整體版面。為單頁選擇&#x200B;**[!UICONTROL 1 Up]**，為雙頁跨頁選擇&#x200B;**[!UICONTROL 2 Up]**，為超過兩頁的跨頁選擇&#x200B;**[!UICONTROL Custom]**。 在&#x200B;**[!UICONTROL 更改eCatalog佈局]**&#x200B;對話框中，選擇&#x200B;**[!UICONTROL 所有跨頁]**&#x200B;選項，然後選擇&#x200B;**[!UICONTROL 確定]**。
1. （可選）通過選擇單個頁面或頁面跨頁，然後選擇&#x200B;**[!UICONTROL 1 Up]**、**[!UICONTROL 2 Up]**&#x200B;或&#x200B;**[!UICONTROL Custom]**&#x200B;按鈕，來更改其佈局。 在&#x200B;**[!UICONTROL 更改eCatalog佈局]**&#x200B;對話框中，選擇&#x200B;**[!UICONTROL 選擇的跨頁]**&#x200B;選項，然後選擇&#x200B;**[!UICONTROL 確定]**。
1. 視需要使用下列其中一個技巧來重新排序頁面:

   * **拖曳**  — 拖曳頁面或頁面跨頁至新位置。垂直列會顯示移動頁面的位置。

   * **「移至」按鈕**  — 選擇頁面或頁面跨頁，選擇 **[!UICONTROL 「移至」]**，然後在您希望頁面之前顯示的功能表中選擇頁面。

   * **序列** 號 — 在清單檢視中，在序列號欄位中輸入頁碼。

1. 完成時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇&#x200B;**[!UICONTROL 保存]**。
1. 在「儲存」對話框中，選取一個檔案夾來儲存 eCatalog。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選擇&#x200B;**[!UICONTROL 保存]**。

   儲存後，您可以選取&#x200B;**[!UICONTROL 預覽]**&#x200B;來預覽eCatalog。

## 編輯eCatalog {#editing-an-ecatalog}

無論您編輯已發佈的集還是未發佈的集，**[!UICONTROL 儲存後發佈]**&#x200B;選項都會以下列方式影響集和整合員：

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯 eCatalog:**

1. 選擇eCatalog的滾動&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕。
1. 視需要進行變更。
1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇&#x200B;**[!UICONTROL 保存]**，選擇儲存資料夾，輸入該集的名稱，然後選擇&#x200B;**[!UICONTROL 保存]**。

## 刪除eCatalog {#deleting-an-ecatalog}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個 eCatalog。
1. 在全局導航欄上，轉至&#x200B;**[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**。

## 自訂目錄(TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic會在eCatalog畫面的「訂購頁面」標籤上，提供eCatalog中的預設頁碼。 如需自訂頁面名稱，您可以變更組成目錄 (TOC) 的頁面標籤。建議重新命名封面與封底。例如，封面可以是「封面」，而非「頁面0-1」。

您可以手動為 eCatalog 建立自訂的目錄 (TOC)，或從 CSV (僅限 Mac) 或 XML 檔案匯入頁面名稱。

>[!NOTE]
>
>要恢復預設頁面標題，請在&#x200B;**[!UICONTROL 訂購頁面]**&#x200B;頁簽上，選擇&#x200B;**[!UICONTROL 目錄標籤]**，然後選擇&#x200B;**[!UICONTROL 還原預設值（全部）]**。

### 手動輸入頁面名稱 {#manually-entering-page-names}

若要逐次手動輸入頁面名稱，請前往「eCatalog」畫面的「排序頁面」標籤。然後，在頁碼欄位中，輸入您要命名的每個頁面的名稱。

### 匯入頁面名稱 {#importing-page-names}

如果您處理的 eCatalog 包含多個頁面，建議使用匯入頁面名稱。您可以從 Tab 字元分隔檔案或 XML 檔案匯入名稱。

TOC標籤儲存在影像的「使用者資料」欄位中；將此資料格式化為`name=<value>` ` pairs separated by two question marks “??” `清單。 例如，若要為名為 `tocEN` 的 TOC 欄位設定一個標籤，請將影像的「使用者資料」設定為:

`tocEN=&lt;EN_page_label>`

要為名為`tocEN`和`tocFR`的目錄欄位設定單獨的標籤：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

若要匯入以Tab分隔的檔案中的「使用者資料」欄位，請納入欄位使用者資料：

| IPSID | 使用者資料 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

若要在 XML 檔案中匯入「使用者資料」欄位，請包括屬性 `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要從以制表符分隔的或XML檔案導入頁面名稱，請選擇&#x200B;**[!UICONTROL TOC標籤]**&#x200B;按鈕並選擇&#x200B;**[!UICONTROL 導入]**。 在「上載元資料」對話框中，選擇&#x200B;**[!UICONTROL Browse]**，然後導入CSV檔案（僅Mac）或將每個頁面與頁面名稱關聯的XML檔案。
