---
title: 將影像集連結至網頁
description: 瞭解如何將影像集連結至Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 17%

---

# 將影像集連結至網頁{#linking-an-image-set-to-a-web-page}

發佈影像集後，您可以複製其相關URL或其內嵌程式碼，以用於您的網站或應用程式。 接著，您可以部署URL，或視需要貼上內嵌程式碼，讓使用者檢視您網站或應用程式上的影像集。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製影像集URL {#copying-an-image-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 影像集]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的影像集。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 複製URL]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

## 將影像集URL新增至網頁 {#adding-image-set-urls-to-your-web-page}

部署影像集的最常見方式是在網頁上放置連結（透過導覽圖示）。 選取時，連結會啟動動態頁面(JSP)，在彈出式縮放視窗中顯示「影像集」。 縮放連結會開啟一個彈出式視窗，其中包含實際的縮放功能。

如需詳細資訊和程式碼範例，請參閱HTML檢視器參考指南](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)中的[內嵌Adobe5縮放檢視器。

## 複製影像集檢視器的內嵌程式碼 {#copying-the-embed-code-of-an-image-set-viewer}

您可使用「內嵌程式碼」功能查看所選「影像集」的檢視器程式碼。您也可以將程式碼複製到剪貼簿，以便貼到網頁中來部署檢視器。 不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製影像集檢視器的內嵌程式碼：**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 影像集]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的影像集。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL面板中，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**清單檢視**&#x200B;或&#x200B;**詳細檢視**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

1. 在「內嵌程式碼」對話方塊中，選取&#x200B;**[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取&#x200B;**[!UICONTROL 關閉]**。

>[!MORELIKETHIS]
>
>* [Publish](publishing-files.md#publishing_files)
