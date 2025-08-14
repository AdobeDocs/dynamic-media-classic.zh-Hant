---
title: 將縮放檢視器連結至您的網頁
description: 瞭解如何將縮放檢視器連結至您在Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 23%

---

# 將縮放檢視器連結至您的網頁{#linking-zoom-viewers-to-your-web-pages}

您的網站和應用程式可透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容。 該存取權包括主要影像和相關聯的縮放目標。 其中也包含縮放檢視器預設集。 這些 URL 字串會在發佈程序中啟用。若要將這些URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製縮放檢視器URL {#copying-a-zoom-viewer-url}

1. 在左側的「資產庫」面板中，導覽至含有您要複製其 URL 之縮放檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**&#x200B;或&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 複製URL]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

## 將縮放檢視器URL新增至您的網頁 {#adding-zoom-viewer-urls-to-your-web-page}

通常，訪客會先選取「縮放」圖示（通常該圖示會顯示放大鏡的影像），以縮放網站上的影像。 選取此圖示會啟動動態網頁（ASP或JSP），在快顯視窗中顯示影像。 彈出式視窗是訪客實際縮放該影像的位置。

如需詳細資訊和程式碼範例，請參閱HTML檢視器參考指南中的[內嵌Adobe5 Basic Zoom Viewer ](https://experienceleague.adobe.com/zh-hant/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)。

## 複製縮放檢視器的內嵌副本 {#copying-the-embed-copy-of-a-zoom-viewer}

您可使用「內嵌程式碼」功能查看所選「縮放檢視器」的檢視器程式碼。您也可以將程式碼複製到剪貼簿，以便貼到網頁中來部署檢視器。 不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製縮放檢視器的內嵌程式碼：**

1. 在左側的「資產庫」面板中，導覽至包含您要複製其內嵌程式碼的縮放檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL和內嵌程式碼面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 內嵌程式碼]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

1. 在「內嵌程式碼」對話方塊中，選取&#x200B;**[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取&#x200B;**[!UICONTROL 關閉]**。
