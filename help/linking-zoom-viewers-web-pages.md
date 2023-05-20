---
title: 將「縮放」查看器連結到網頁
description: 瞭解如何將縮放查看器連結到您在Adobe Dynamic Media Classic的網頁。
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

# 將「縮放」查看器連結到網頁{#linking-zoom-viewers-to-your-web-pages}

您的網站和應用程式通過URL字串或嵌入代碼訪問Dynamic Media影像伺服器內容，包括主影像和關聯的縮放目標以及縮放查看器預設。 這些 URL 字串會在發佈程序中啟用。要將這些URL字串或嵌入的代碼放在網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製縮放查看器URL {#copying-a-zoom-viewer-url}

1. 在左側的「資產庫」面板中，導覽至含有您要複製其 URL 之縮放檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]** 或 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和嵌入代碼」面板中，選擇 **[!UICONTROL 複製URL]** 按鈕。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

## 將縮放查看器URL添加到網頁 {#adding-zoom-viewer-urls-to-your-web-page}

通常，訪問者首先選擇「縮放」表徵圖（通常該表徵圖顯示放大鏡的影像），以縮放網站上的影像。 選取該圖示會啟動一個動態網頁 (ASP 或 JSP)，該網頁在彈出式視窗中顯示該影像。彈出式視窗是訪客實際縮放該影像的位置。

有關詳細資訊和代碼示例，請參閱 [《HTML查看器參考指南》中的「嵌入Adobe5基本縮放查看器」](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)。

## 複製縮放查看器的嵌入副本 {#copying-the-embed-copy-of-a-zoom-viewer}

您可使用「內嵌程式碼」功能查看所選「縮放檢視器」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。不可在「內嵌程式碼」對話框中編輯程式碼。

**複製縮放檢視器的內嵌程式碼:**

1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「縮放」檢視器的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和嵌入代碼」面板中，選擇 **[!UICONTROL 嵌入代碼]** 按鈕。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

1. 在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選擇 **[!UICONTROL 關閉]**。
