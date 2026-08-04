---
title: 將迴轉集連結至網頁
description: 瞭解如何將迴轉集連結至Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:03:03.240Z'
TQID: 'https://experienceleague.adobe.com/wOviDM-OY9nHBF9RnPXwsCQ2psd6UsxVVppf5kyS0y0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 98c2209424b1ad028b194d1bdf7c71d77b16b50d
workflow-type: tm+mt
source-wordcount: 729
ht-degree: 16%

---

# 將迴轉集連結至網頁{#linking-a-spin-set-to-a-web-page}

網站和應用程式使用URL字串或內嵌程式碼來存取Dynamic Media影像伺服器內容，包括迴轉集。 這些URL字串會在發佈程式期間啟用。 若要將迴轉集的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製迴轉集URL {#copying-a-spin-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 迴轉集]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的迴轉集。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。 在右側的「URL和內嵌程式碼」面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 複製URL]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

## 將迴轉集URL新增至網頁 {#adding-spin-set-urls-to-your-web-page}

使用在縮放視窗中顯示迴轉集的動態頁面（ASP或JSP），像所有縮放檢視器一樣部署迴轉集。 Adobe Dynamic Media Classic平台的URL要求使用與縮放檢視器相同的通訊協定。 不過，「檢視器預設集」名稱取決於管理員定義為預設「迴轉集檢視器預設集」的預設集。 例如，下列URL語法範例（未上線）包含名為`viewer.jsp`的預設集名稱，而SKU引數現在是迴轉集名稱：

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此URL語法範例中（連結未上線），請參閱SKU編號( `sku=backpack_spin`)。 `sku=`之後的字串是迴轉集名稱( `backpack spin`)。

## 複製迴轉集檢視器的內嵌程式碼 {#copying-the-embed-code-of-a-spin-set-viewer}

使用內嵌程式碼功能可讓您檢閱所選迴轉集的檢視器程式碼。 您也可以將程式碼複製到剪貼簿，以便貼到網頁中來部署檢視器。 不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製迴轉集檢視器的內嵌程式碼：**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 迴轉集]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的迴轉集。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。 在右側的URL和內嵌程式碼面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 內嵌程式碼]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

1. 在「內嵌程式碼」對話方塊中，選取&#x200B;**[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取&#x200B;**[!UICONTROL 關閉]**。
