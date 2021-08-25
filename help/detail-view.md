---
title: 在詳細資訊視圖中工作
description: 了解如何在Dynamic Media Classic的「詳細檢視」中運作。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: 47845c30311fb9afb3fffb8502b6e7c534e4bfdb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 24%

---

# 在詳細資訊視圖中工作{#working-in-detail-view}

您可以在「詳細資訊檢視」中開啟資產，以使用資產並了解資產。 在「詳細資訊檢視」中，您會看到資產大小、屬性、衍生項目和中繼資料。 您也會看到資產的發佈狀況與發佈時間，並取得已發佈資產的 URL。依據資產類型而定，您可以使用不同大小預覽資產、放大資產，以及執行銳利化、裁切及其它格式化作業。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Detail ](/help/assets/image_0.img.png)
*ViewDetail視圖，左側的「資產庫」面板隱藏在視圖中。*

>[!NOTE]
>
>若要開啟儲存資產的資料夾，您可以在「資訊」面板頂端選取資料夾路徑。

## 在「詳細資訊檢視」中開啟資產 {#open-an-asset-in-detail-view}

若要仔細檢查、預覽或處理資產，您可以在「詳細資訊檢視」中顯示資產。

1. 在「瀏覽」面板中，執行下列任一操作：

   * 選取資產。在Dynamic Media Classic的右上角附近，選取&#x200B;**[!UICONTROL Detail View]**&#x200B;圖示。
   * 在這個資產按兩下。
   * 選取資產，然後前往&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 詳細資料]**。

>[!NOTE]
>
>您可以在「詳細資料檢視」中選取&#x200B;**[!UICONTROL 上一個資產]**&#x200B;或&#x200B;**[!UICONTROL 下一個資產]**，從資產頁面到同一個資料夾中的資產。 這些按鈕位於「詳細資訊視圖」的右上角。

## 在詳細資訊檢視中取得資訊 {#getting-information-in-detail-view}

詳細資訊檢視提供資產或檔案的相關資訊。 它會顯示項目的下列資訊：儲存該項目的資料夾、其檔案名稱、項目上傳至Dynamic Media Classic的日期，及其發佈記錄。 您也可以在「詳細資料檢視」中檢視及編輯中繼資料，以及新增資產的關鍵字。

您可以在「詳細資料檢視」中取得資產URL;不過，在您發佈資產之前，URL不會啟用。 對於影像，「詳細資訊檢視」也提供組建和衍生資產與中繼資料的清單，例如縮放目標與影像集。

## 在「詳細資訊檢視」中使用資產 {#working-with-assets-in-detail-view}

詳細資料檢視選件工具，可用於使用您開啟的資產。 可用的工具取決於您使用的資產類型，但「詳細資訊檢視」一律提供下列功能：

* **要發佈的項目**  — 選取名 **** 稱左側的「發佈」，或前往 **[!UICONTROL 「檔案]**  >  **** 發佈 **[!UICONTROL 者檔案]**  >  **[!UICONTROL 取消發佈」]**。

* **重新命名資產**  — 選取名稱並輸入新名稱。

* **編輯和新增中繼資料**  — 選取「中繼資料」面板，並視需要變更。請參閱[檢視、新增和匯出中繼資料](/help/viewing-adding-exporting-metadata.md)。

* **編輯和新增關鍵字**  — 選取「關鍵字」，並視需要新增或移除關鍵字。請參閱[增加或編輯關鍵字](/help/viewing-adding-exporting-metadata.md)。

* **刪除資產**  — 前往 **[!UICONTROL 檔案]**  >  **[!UICONTROL 刪除]**。

對於離散檔案（例如影像、影像集和字型），您可以在「詳細資訊視圖」中查看發佈和編輯歷史記錄，並檢查任務詳細資訊。

此表格顯示「詳細資料檢視」中，不同資產類型可使用的其他選項。

| 資產類型 | 編輯/調整 | 預覽 |
| --- | --- | --- |
| 影像 | 增加影像地圖<br>新增縮放目<br><br><br>標裁切銳利化建立調整後的檢視 | 是；縮放與影像影像預設集 |
| 封包與視窗涵蓋範圍影像 | 否 | 縮圖 |
| eCatalog | 編輯 | 是<br>資訊面板也可用 |
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
| 暈映與演算後的暈映 | 否 | 如所示<br>您可以以XML格式查看暈映的可呈現元素的內容和結構 |
| XML 檔案 | 否 | 已顯示內容 |
| ZIP 檔案 | 否 | 未顯示內容 |

>[!MORELIKETHIS]
>
>* [檢視、新增和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

