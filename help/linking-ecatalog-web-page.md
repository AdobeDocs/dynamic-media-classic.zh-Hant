---
title: 將eCatalog連結至網頁
description: 了解如何在Adobe Dynamic Media Classic中將eCatalog連結至網頁。
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 38%

---

# 將eCatalog連結至網頁{#linking-an-ecatalog-to-a-web-page}

您的網站和應用程式可透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括eCatalog。 這些 URL 字串會在發佈程序中啟用。若要將eCatalog的URL字串或內嵌程式碼放入網頁和應用程式中，請從AdobeDynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製eCatalog URL {#copying-an-ecatalog-url}

1. 在「資產瀏覽」面板中，在「顯示」下拉清單中，選擇&#x200B;**[!UICONTROL Catalog]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之eCatalog 的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」和「內嵌程式碼」面板中，選取您要檢視器右側的「複製URL ]**」 。**[!UICONTROL 
   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL 複製URL]**。

   * 選擇&#x200B;**[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL 複製URL]**。

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**、**[!UICONTROL 清單視圖]**&#x200B;或&#x200B;**[!UICONTROL 詳細視圖]**。 在相同工具列上，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**複製URL**。

## 將eCatalog URL新增至您的網頁 {#adding-ecatalog-urls-to-your-web-page}

部署 eCatalog 最常見的方式，就是以 eCatalog 縮圖封面頁的形式，在網頁上放置連結。請與您的 IT 團隊合作，以確認 eCatalog 會在整潔、置中的彈出式視窗中啟動。要求您的 IT 團隊避免將工具列與位址列顯示在瀏覽器中。

如需更多詳細資訊和程式碼範例，請參閱Adobe檢視器參考指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)中的[內嵌HTML5 eCatalog檢視器。

## 複製eCatalog檢視器的內嵌程式碼 {#copying-the-embed-code-of-an-ecatalog-viewer}

您可使用「內嵌程式碼」功能查看所選 eCatalog 的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。「內嵌代碼」對話方塊中不允許編 輯代碼 。

**複製 eCatalog 檢視器的內嵌程式碼:**

1. 在「資產瀏覽」面板中，在「顯示」下拉清單中，選擇&#x200B;**[!UICONTROL Catalog]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之eCatalog 的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL」面板中，選取「**[!UICONTROL 內嵌程式碼]**」。
   * 選擇&#x200B;**[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

   * 選擇&#x200B;**[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

   * 選擇&#x200B;**[!UICONTROL 網格視圖]**、**[!UICONTROL 清單視圖]**&#x200B;或&#x200B;**[!UICONTROL 詳細視圖]**。 在相同工具列上，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

      在「查看器清單」頁的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

1. 在「內嵌代碼」對話方塊中，選取「**[!UICONTROL 複製到剪貼簿]**」。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選擇&#x200B;**[!UICONTROL 關閉]**。
