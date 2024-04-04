---
title: 將eCatalog連結至網頁
description: 瞭解如何將eCatalog連結至Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 38%

---

# 將eCatalog連結至網頁{#linking-an-ecatalog-to-a-web-page}

您的網站和應用程式可透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括eCatalog。 這些 URL 字串會在發佈程序中啟用。若要將eCatalog的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製eCatalog URL {#copying-an-ecatalog-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 目錄]**.
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之eCatalog 的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **複製URL**.

## 將eCatalog URL新增至網頁 {#adding-ecatalog-urls-to-your-web-page}

部署 eCatalog 最常見的方式，就是以 eCatalog 縮圖封面頁的形式，在網頁上放置連結。請與您的 IT 團隊合作，以確認 eCatalog 會在整潔、置中的彈出式視窗中啟動。要求您的 IT 團隊避免將工具列與位址列顯示在瀏覽器中。

如需詳細資訊和程式碼範例，請參閱 [Adobe檢視器參考指南中的內嵌HTML5 eCatalog檢視器](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 複製eCatalog檢視器的內嵌程式碼 {#copying-the-embed-code-of-an-ecatalog-viewer}

您可使用「內嵌程式碼」功能查看所選 eCatalog 的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製eCatalog檢視器的內嵌程式碼：**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 目錄]**.
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之eCatalog 的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL面板中，選取 **[!UICONTROL 內嵌程式碼]**.
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取 **[!UICONTROL 關閉]**.
