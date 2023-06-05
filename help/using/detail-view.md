---
title: 在「詳細資訊」檢視中進行工作
description: 瞭解如何在Adobe Dynamic Media Classic的「詳細資料檢視」中運作。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 21%

---

# 在「詳細資訊」檢視中進行工作{#working-in-detail-view}

您可以在「詳細資料檢視」中開啟資產，以使用及瞭解資產。 在「詳細資料檢視」中，您會看到資產大小、屬性、衍生工具和中繼資料。 您也可以檢視資產是否發佈及何時發佈，以及取得已發佈資產的URL。 依據資產類型而定，您可以使用不同大小預覽資產、放大資產，以及執行銳利化、裁切及其它格式化作業。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![詳細資料檢視](/help/using/assets/image_0.img.png)
*「詳細資料檢視」，「資產庫」面板隱藏於左側檢視中。*

>[!NOTE]
>
>若要開啟儲存資產的資料夾，您可以選取「資訊」面板頂端的資料夾路徑。

## 在「詳細資料檢視」中開啟資產 {#open-an-asset-in-detail-view}

若要深入檢查、預覽或處理資產，您可以在「詳細資料檢視」中顯示資產。

1. 在「瀏覽」面板中，執行下列任一項作業：

   * 選取資產。在Adobe Dynamic Media Classic的右上角附近，選取 **[!UICONTROL 詳細資料檢視]** 圖示。
   * 在這個資產按兩下。
   * 選取資產，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 詳細資料]**.

>[!NOTE]
>
>在「詳細資料檢視」中，您可以在相同資料夾中選取資產，在不同資產間進行分頁 **[!UICONTROL 上一個資產]** 或 **[!UICONTROL 下一個資產]**. 這些按鈕位於「詳細資料檢視」的右上角。

## 在「詳細資料檢視」中取得資訊 {#getting-information-in-detail-view}

「詳細資料檢視」提供有關資產或檔案的資訊。 它會顯示專案的相關資訊：儲存專案的資料夾、其檔案名稱、專案上傳至Adobe Dynamic Media Classic的日期及其發佈歷史記錄。 您也可以在「詳細資料檢視」中檢視和編輯中繼資料，以及新增資產的關鍵字。

您可以在「詳細資料檢視」中取得資產URL，但該URL要等到您發佈資產後才會啟用。 對於影像，「詳細資料檢視」也會提供建置和衍生的資產和中繼資料清單，例如縮放目標和影像集。

## 在「詳細資料檢視」中使用資產 {#working-with-assets-in-detail-view}

「詳細資料檢視」提供處理您所開啟之資產的工具。 可用的工具取決於您使用的資產型別，但「詳細資料檢視」一律會提供下列功能：

* **要發佈的專案**  — 選取 **[!UICONTROL 發佈]** 圖示或前往「 」 **[!UICONTROL 檔案]** > **[!UICONTROL 發佈]** 或 **[!UICONTROL 檔案]** > **[!UICONTROL 取消發佈]**.

* **重新命名資產**  — 選取名稱並輸入新名稱。

* **編輯和新增中繼資料**  — 選取「中繼資料」面板，並視需要變更。 另請參閱 [檢視、新增和匯出中繼資料](/help/using/viewing-adding-exporting-metadata.md).

* **編輯和新增關鍵字**  — 選取關鍵字，並視需要新增或移除關鍵字。 請參閱[增加或編輯關鍵字](/help/using/viewing-adding-exporting-metadata.md)。

* **刪除資產**  — 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**.

對於離散檔案（例如，影像、影像集和字型），您可以檢視發佈和編輯歷史記錄，並在「詳細資訊檢視」中檢查作業詳細資訊。

此表格顯示「詳細資料檢視」中不同資產型別可用的其他選項。

| 資產類型 | 編輯/調整 | 預覽 |
| --- | --- | --- |
| 影像 | 增加影像地圖<br>新增縮放目標<br>裁切<br>銳利化<br>建立調整後的檢視 | 是；縮放與影像影像預設集 |
| 機櫃和視窗涵蓋影像 | 否 | 縮圖 |
| eCatalog | 編輯 | 是<br>資訊面板也可供使用 |
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
| 暈映與演算後的暈映 | 否 | 顯示影像<br>您可以以XML格式檢視暈映的可轉譯元素的內容和結構 |
| XML 檔案 | 否 | 已顯示內容 |
| ZIP 檔案 | 否 | 未顯示內容 |

>[!MORELIKETHIS]
>
>* [檢視、新增和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

