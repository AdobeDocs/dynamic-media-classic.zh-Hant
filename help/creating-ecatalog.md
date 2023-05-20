---
title: 建立電子目錄
description: 瞭解如何在Adobe Dynamic Media Classic建立eCatalog。
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

## 建立電子目錄 {#create}

您可以在eCatalog中包括影像檔案和PDF檔案。

建立 eCatalog 時，「**[!UICONTROL 儲存後發佈]**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog:**

1. 使用下列其中一個技巧來開始建立 eCatalog:

   * **首先選擇檔案**  — 在「瀏覽面板」中，選擇檔案，然後轉到 **[!UICONTROL 生成]** > **[!UICONTROL 電子目錄]**。

   * **從eCatalog螢幕開始**  — 轉到 **[!UICONTROL 生成]** > **[!UICONTROL 電子目錄]**。 在資產庫中選取檔案夾，並將檔案從檔案夾中拖曳至「eCatalog」頁面的「排序頁面」頁面。

      >[!NOTE]
      >
      >若要依名稱 (而非縮圖) 來檢視資產庫中的項目，請為「個人設定」中的「預設資產庫視圖」選取「名稱」選項。

1. 為 eCatalog 選取整體版面。選擇 **[!UICONTROL 1上]** 單頁， **[!UICONTROL 2個]** 用於雙頁跨頁，或 **[!UICONTROL 自定義]** 頁面跨頁。 在 **[!UICONTROL 更改電子目錄佈局]** 對話框，選擇 **[!UICONTROL 所有跨頁]** 選項，選擇 **[!UICONTROL 確定]**。
1. （可選）通過選擇單個頁面或頁面跨頁，然後選擇 **[!UICONTROL 1上]**。 **[!UICONTROL 2個]**&#x200B;或 **[!UICONTROL 自定義]** 按鈕 在 **[!UICONTROL 更改電子目錄佈局]** 對話框，選擇 **[!UICONTROL 所選跨頁]** 選項，選擇 **[!UICONTROL 確定]**。
1. 視需要使用下列其中一個技巧來重新排序頁面:

   * **拖動**  — 將頁面或頁面跨頁拖到新位置。 垂直列會顯示移動頁面的位置。

   * **「移至」按鈕**  — 選擇頁面或頁面跨頁，選擇 **[!UICONTROL 移到]**，然後選擇希望頁面在前面顯示的菜單上的頁面。

   * **序列號**  — 在清單視圖中，在序列號欄位中輸入頁碼。

1. 完成時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 保存]**。
1. 在「儲存」對話框中，選取一個檔案夾來儲存 eCatalog。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 選擇 **[!UICONTROL 保存]**。

   保存電子目錄後，可通過選擇 **[!UICONTROL 預覽]**。

## 編輯電子目錄 {#editing-an-ecatalog}

無論您編輯已發佈集還是未發佈集， **[!UICONTROL 保存後發佈]** 選項通過以下方式影響集和整合員：

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
| --- | --- | --- | --- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有集成員會保持已發佈的狀態。在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯 eCatalog:**

1. 選擇eCatalog的滾動更新 **[!UICONTROL 編輯]** 按鈕
1. 視需要進行變更。
1. 完成編輯時，在頁面右上角附近，請確保選取了「**[!UICONTROL 儲存後發佈]**」(預設)。
1. 選擇 **[!UICONTROL 保存]**，選擇儲存資料夾，輸入集的名稱，然後選擇 **[!UICONTROL 保存]**。

## 刪除電子目錄 {#deleting-an-ecatalog}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog:**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個 eCatalog。
1. 在全局導航欄上，轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**。

## 自定義目錄(TOC) {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic在「eCatalog」螢幕的「訂單頁」頁籤上的「eCatalog」中提供預設頁碼。 如需自訂頁面名稱，您可以變更組成目錄 (TOC) 的頁面標籤。建議重新命名封面與封底。例如，封面可以讀「封面」，而不是「頁0-1」。

您可以手動為 eCatalog 建立自訂的目錄 (TOC)，或從 CSV (僅限 Mac) 或 XML 檔案匯入頁面名稱。

>[!NOTE]
>
>要恢復預設頁面標題，請在 **[!UICONTROL 訂單頁]** 頁籤 **[!UICONTROL 目錄標籤]**，然後選擇 **[!UICONTROL 恢復預設值（全部）]**。

### 手動輸入頁面名稱 {#manually-entering-page-names}

若要逐次手動輸入頁面名稱，請前往「eCatalog」畫面的「排序頁面」標籤。然後，在頁碼欄位中，為要命名的每頁輸入名稱。

### 導入頁名 {#importing-page-names}

如果您處理的 eCatalog 包含多個頁面，建議使用匯入頁面名稱。您可以從 Tab 字元分隔檔案或 XML 檔案匯入名稱。

TOC標籤儲存在影像的「用戶資料」欄位中；將此資料格式化為 `name=<value>` ` pairs separated by two question marks “??” `。 例如，若要為名為 `tocEN` 的 TOC 欄位設定一個標籤，請將影像的「使用者資料」設定為:

`tocEN=&lt;EN_page_label>`

為名為的目錄欄位設定單獨的標籤 `tocEN` 和 `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

要在制表符分隔的檔案中導入「用戶資料」欄位，請包括該欄位的用戶資料：

| IPSID | 用戶資料 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

若要在 XML 檔案中匯入「使用者資料」欄位，請包括屬性 `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要從制表符分隔或XML檔案導入頁名，請選擇 **[!UICONTROL 目錄標籤]** 按鈕 **[!UICONTROL 導入]**。 在「上載元資料」對話框中，選擇 **[!UICONTROL 瀏覽]**，然後導入將每頁與頁名關聯的CSV檔案(僅Mac)或XML檔案。
