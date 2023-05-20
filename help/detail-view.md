---
title: 詳細工作視圖
description: 瞭解如何在Adobe Dynamic Media Classic的「詳細視圖」中工作。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 21%

---

# 詳細工作視圖{#working-in-detail-view}

您可以通過在「詳細資訊視圖」中開啟資產來使用和瞭解資產。 在「詳細資訊視圖」中，您會看到資產大小、屬性、衍生項和元資料。 您還可以查看資產是否發佈以及何時發佈，以及您可以獲取已發佈資產的URL。 依據資產類型而定，您可以使用不同大小預覽資產、放大資產，以及執行銳利化、裁切及其它格式化作業。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![詳細資訊視圖](/help/assets/image_0.img.png)
*「資產庫」面板在左側隱藏為「詳細資訊視圖」。*

>[!NOTE]
>
>要開啟儲存資產的資料夾，可以在「資訊」面板頂部選擇資料夾路徑。

## 在詳細資訊視圖中開啟資產 {#open-an-asset-in-detail-view}

要仔細檢查、預覽或處理資產，可以在詳細資訊視圖中顯示它。

1. 在「瀏覽」面板中，執行下列任一操作：

   * 選取資產。在Adobe Dynamic Media Classic右上角，選擇 **[!UICONTROL 詳細資訊視圖]** 表徵圖
   * 在這個資產按兩下。
   * 選擇資產，然後轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 詳細資訊]**。

>[!NOTE]
>
>通過選擇「詳細資訊視圖」，您可以在同一資料夾中從資產到資產進行頁面 **[!UICONTROL 上一資產]** 或 **[!UICONTROL 下一資產]**。 這些按鈕位於「詳細資訊視圖」的右上角。

## 獲取詳細資訊視圖中的資訊 {#getting-information-in-detail-view}

詳細資訊視圖提供有關資產或檔案的資訊。 它顯示有關項目的以下資訊：儲存它的資料夾、其檔案名、項上載到Adobe Dynamic Media Classic的日期及其發佈歷史記錄。 您還可以在「詳細資訊視圖」中查看和編輯元資料以及添加資產的關鍵字。

您可以在「詳細資訊視圖」中獲取資產URL;但是，在您發佈資產之前，URL不處於活動狀態。 對於影像，「詳細資訊視圖」還提供生成和派生的資產和元資料的清單，如縮放目標和影像集。

## 在詳細資訊視圖中使用資產 {#working-with-assets-in-detail-view}

「詳細資訊視圖」提供了用於處理您開啟的資產的工具。 可用的工具取決於您正在使用的資產類型，但「詳細資訊視圖」始終提供以下功能：

* **發佈項**  — 選擇 **[!UICONTROL 發佈]** 表徵圖，或轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 發佈]** 或 **[!UICONTROL 檔案]** > **[!UICONTROL 取消發佈]**。

* **更名資產**  — 選擇名稱並輸入新名稱。

* **編輯和添加元資料**  — 選擇「元資料」面板，並根據需要進行更改。 請參閱 [查看、添加和導出元資料](/help/viewing-adding-exporting-metadata.md)。

* **編輯和添加關鍵字**  — 選擇「關鍵字」，然後根據需要添加或刪除它們。 請參閱[增加或編輯關鍵字](/help/viewing-adding-exporting-metadata.md)。

* **刪除資產**  — 轉到 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**。

對於離散檔案（例如影像、影像集和字型），可以在詳細資訊視圖中查看發佈和編輯歷史記錄，並檢查作業詳細資訊。

此表顯示了「詳細資訊視圖」中不同類型資產可用的其它選項。

| 資產類型 | 編輯/調整 | 預覽 |
| --- | --- | --- |
| 影像 | 增加影像地圖<br>添加縮放目標<br>裁剪<br>銳化<br>建立調整後視圖 | 是；縮放與影像影像預設集 |
| 機櫃和窗蓋影像 | 否 | 縮圖 |
| eCatalog | 編輯 | 是<br>「資訊」面板也可用 |
| 字型 | 編輯字體資訊 | 否 |
| FXG 檔案 | 編輯 | 是 |
| ICC 設定檔 | 編輯設定檔資訊 | 否 |
| Illustrator 檔案 | 無 (除非轉換成 FXG) | 否 |
| 影像集 | 編輯 | 是 |
| InDesign 檔案 | 無 (除非轉換成 FXG) | 否 |
| PDF 檔案 | 否 | 否 |
| PSD 檔案 | 是 (個別圖層) | 是 (個別圖層) |
| 迴轉集 | 編輯 | 是 |
| SVG 檔案 | 否 | 否 |
| 範本 | 編輯 | 是 |
| 視訊 | 否 | 是 |
| 暈映與演算後的暈映 | 否 | 顯示影像<br>可以以XML格式查看視頻的可呈現元素的內容和結構 |
| XML 檔案 | 否 | 已顯示內容 |
| ZIP 檔案 | 否 | 未顯示內容 |

>[!MORELIKETHIS]
>
>* [查看、添加和導出元資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

