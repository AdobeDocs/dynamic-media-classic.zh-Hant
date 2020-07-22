---
title: 建立 eCatalog
seo-title: 建立 eCatalog
description: 'null'
seo-description: 瞭解如何建立eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 78%

---


# 建立 eCatalog{#creating-an-ecatalog}

建立 eCatalog 必須進行下列步驟: 排序頁面、選擇頁面版面，以及透過繪製影像地圖、輸入滑鼠指向與超文字連結資料來連結頁面。或者，您也可以自訂目錄 (TOC)，如此一來，檢視者就會在 eCatalog 檢視器中看到頁面名稱，而非頁碼。

## 建立 eCatalog {#create}

您可以在 eCatalog 中包含影像檔案與 PDF 檔案。

建立 eCatalog 時，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 是否在儲存之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |
| 是 | 已發佈 | 已發佈 |
| 否 | 未發佈 | 集成員會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog**

1. 使用下列其中一個技巧來開始建立 eCatalog:

   **首先選取檔案** 。在「瀏覽面板」中，選取檔案，然後按一下「建立>eCatalogs」。

   **從eCatalog畫面開始** ，按一下「建立>eCatalogs」。 在資產庫中選取檔案夾，並將檔案從檔案夾中拖曳至「eCatalog」頁面的「排序頁面」頁面。

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. 為 eCatalog 選取整體版面。按一下「1 欄式」按鈕  以使用單一頁面，「2 欄式」按鈕  以使用雙頁式跨頁，或按一下「自訂」按鈕  以使用兩頁以上的跨頁。「更改 eCatalog 版面」對話框會出現。Select the All Spreads options and click **OK**.
1. 或者按一下個別頁面或跨頁，然後選擇「1 欄式」、「2 欄式」或「自訂」按鈕，以變更其版面。「更改 eCatalog 版面」對話框會出現。Select the Selected Spreads options and click **OK**.
1. 視需要使用下列其中一個技巧來重新排序頁面:

   **拖曳** 「將頁面或頁面跨頁拖曳至新位置」。 垂直列會顯示移動頁面的位置。

   **「移至」按鈕** 「選擇頁面跨頁」，按一下「移至」按鈕，然後在功能表上選擇您希望頁面之前顯示的頁面。

   **序列** #在清單視圖中，在序列號欄位中輸入頁碼。

1. 完成時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 按一下&#x200B;**「儲存」**。
1. 在「儲存」對話框中，選取一個檔案夾來儲存 eCatalog。在「檔案名稱」欄位中，輸入迴轉集名稱。
1. 按一下&#x200B;**「儲存」**。

   儲存 eCatalog 之後，您可以按一下「**預覽**」來預覽。

## 編輯 eCatalog {#editing-an-ecatalog}

根據您編輯的是已發佈的集或未發佈的集，「**儲存後發佈**」選項會以下列方式影響集與集成員:

| 已發佈集? | 是否在儲存編輯之前選取了「儲存後發佈」選項? | 儲存後集的狀態 | 儲存後集成員的狀態 |
|--- |--- |--- |--- |
| 是 | 是 | 已發佈 | 已發佈 |
| 是 | 否 | 已發佈 | 現有整合員將保留其已發佈狀態。在編輯期間添加的任何新整合員都將保留其已發佈或未發佈狀態。 |
| 否 | 是 | 已發佈 | 已發佈 |
| 否 | 否 | 未發佈 | 現有的集成員和在編輯期間加入的任何新的集成員，會保持已發佈或未發佈的狀態。 |

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**編輯 eCatalog**

1. 按一下 eCatalog 的滑鼠指向效果「**編輯**」按鈕。
1. 視需要進行變更。
1. 完成編輯時，在頁面右上角附近，請確保選取了「**儲存後發佈**」(預設)。
1. 按一下「**儲存**」，選取存放區檔案夾，輸入集名稱，然後按「**儲存**」。

## 刪除 eCatalog {#deleting-an-ecatalog}

刪除集時，便會將集本身移到垃圾桶。不過，該集中的成員 (或「子項」) 不會受到影響；而是會保持現有的已發佈或未發佈狀態。

另請參閱[手動發佈資產](publishing-files.md#manually_publishing_assets)和[手動取消發佈資產](publishing-files.md#manually_unpublishing_assets)。

**建立 eCatalog**

1. 在格點檢視、清單檢視或詳細資訊檢視中，選取一或多個 eCatalog。
1. 在全域導覽列上，按一下「**檔案** > **刪除** > **刪除**」。

## 自訂目錄 (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic會在eCatalog畫面的「訂購頁面」標籤上，在eCatalog中提供預設頁碼。 如需自訂頁面名稱，您可以變更組成目錄 (TOC) 的頁面標籤。建議重新命名封面與封底。例如，首頁可以讀取「封面」，而非「頁面0-1」。

您可以手動為 eCatalog 建立自訂的目錄 (TOC)，或從 CSV (僅限 Mac) 或 XML 檔案匯入頁面名稱。

>[!NOTE]
>
>若要還原預設頁面標題，請按一下「排序頁面」標籤上的「TOC 標籤」按鈕，然後選擇「還原預設值 (全部)」。

### 手動輸入頁面名稱 {#manually-entering-page-names}

若要逐次手動輸入頁面名稱，請前往「eCatalog」畫面的「排序頁面」標籤。然後在頁碼欄位中按一下，並輸入名稱。為每個要命名的頁面輸入名稱。

### 匯入頁面名稱 {#importing-page-names}

如果您處理的 eCatalog 包含多個頁面，建議使用匯入頁面名稱。您可以從 Tab 字元分隔檔案或 XML 檔案匯入名稱。

目錄標籤會儲存在影像的「使用者資料」欄位中； 格式化此資料為清單 `name=<value>`` pairs separated by two question marks “??” `。 例如，若要為名為tocEN &quot;的TOC欄位設定一個標籤，請將影像的「使用者資料」設定為：

tocEN=&lt;EN_page_label>

若要為名為 tocEN 與 tocFR 的 TOC 欄位設定分隔標籤:

tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>

若要在 Tab 字元分隔檔案中匯入「使用者資料」欄位，請包括欄位使用者資料:

| IPSID | 使用者資料 |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label> |

若要在 XML 檔案中匯入「使用者資料」欄位，請包括屬性 `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

若要從 Tab 字元分隔檔案或 XML 檔案匯入頁面名稱，請選取「TOC 標籤」按鈕，並選擇「匯入」。「上載中繼資料」對話框會出現。按一下「瀏覽」按鈕，並匯入將每個頁面與頁面名稱產生關聯之 CSV 檔案 (僅限 Mac) 或 XML 檔案。
