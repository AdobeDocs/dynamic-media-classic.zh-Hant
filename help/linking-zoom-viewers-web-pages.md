---
title: 將縮放檢視器連結至您的網頁
description: 了解如何在Adobe Dynamic Media Classic中將縮放檢視器連結至您的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# 將縮放檢視器連結至您的網頁{#linking-zoom-viewers-to-your-web-pages}

您的網站和應用程式可透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括主要影像和相關的縮放目標，以及縮放檢視器預設集。 這些 URL 字串會在發佈程序中啟用。若要將這些URL字串或內嵌程式碼放入您的網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製縮放檢視器URL {#copying-a-zoom-viewer-url}

1. 在左側的「資產庫」面板中，導覽至含有您要複製其 URL 之縮放檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」和「內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 右邊。
   * 選擇 **[!UICONTROL 網格視圖]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**.

   * 選擇 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**.

   * 選擇 **[!UICONTROL 網格視圖]**, **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 複製URL]**.

## 將縮放檢視器URL新增至網頁 {#adding-zoom-viewer-urls-to-your-web-page}

通常，訪客會先選取「縮放」圖示來縮放網站上的影像（通常圖示會顯示放大鏡的影像）。 選取該圖示會啟動一個動態網頁 (ASP 或 JSP)，該網頁在彈出式視窗中顯示該影像。彈出式視窗是訪客實際縮放該影像的位置。

如需詳細資訊和程式碼範例，請參閱 [「HTML檢視器參考指南」中的內嵌Adobe5基本縮放檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 複製縮放檢視器的內嵌副本 {#copying-the-embed-copy-of-a-zoom-viewer}

您可使用「內嵌程式碼」功能查看所選「縮放檢視器」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。「內嵌代碼」對話方塊中不允許編 輯代碼 。

**複製縮放檢視器的內嵌程式碼:**

1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「縮放」檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」和「內嵌程式碼」面板中，選取 **[!UICONTROL 內嵌程式碼]** 右邊。
   * 選擇 **[!UICONTROL 網格視圖]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**.

   * 選擇 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**.

   * 選擇 **[!UICONTROL 網格視圖]**, **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「查看器清單」頁的表的「操作」列下，選擇 **[!UICONTROL 內嵌程式碼]**.

1. 在「內嵌程式碼」對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選擇 **[!UICONTROL 關閉]**.
