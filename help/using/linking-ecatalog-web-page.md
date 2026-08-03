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
autotag-review: '2026-05-13T19:52:09.030Z'
TQID: 'https://experienceleague.adobe.com/cAIaFvlJ3jYoqu1LeLRILuuYsfvuYH6f-N8PqqkHkrk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: a6b941f1da5843a57d082f6bebc4a75a6c2ee65c
workflow-type: tm+mt
source-wordcount: 683
ht-degree: 16%

---

# 將eCatalog連結至網頁{#linking-an-ecatalog-to-a-web-page}

您的網站和應用程式會使用URL字串或內嵌程式碼來存取Dynamic Media影像伺服器內容，包括eCatalog。 這些 URL 字串會在發佈程序中啟用。 若要將eCatalog的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製eCatalog URL {#copying-an-ecatalog-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 目錄]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的eCatalog。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。 在右側的「URL和內嵌程式碼」面板中，選取您想要的檢視器右側的&#x200B;**[!UICONTROL 複製URL]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**[!UICONTROL 複製URL]**」。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在「檢視器清單」頁面中，在表格的「動作」欄下，選取「**複製URL**」。

## 將eCatalog URL新增至網頁 {#adding-ecatalog-urls-to-your-web-page}

部署eCatalog的標準方法是使用網頁上的eCatalog縮圖封面來新增連結。 若要確保eCatalog會在置中的快顯視窗啟動，請連絡您的IT部門。 若要隱藏工具列和位址列，請設定瀏覽器。

如需詳細資訊和程式碼範例，請參閱「HTML檢視器參考」中的[內嵌Adobe5 eCatalog檢視器](https://experienceleague.adobe.com/zh-hant/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)。

## 複製eCatalog檢視器的內嵌程式碼 {#copying-the-embed-code-of-an-ecatalog-viewer}

內嵌程式碼功能可讓您檢閱所選eCatalog的檢視器程式碼。 您也可以將程式碼複製到剪貼簿，以便貼到網頁中來部署檢視器。 不可在「內嵌程式碼」對話框中編輯程式碼。

**若要複製eCatalog檢視器的內嵌程式碼：**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取&#x200B;**[!UICONTROL 目錄]**。
1. 在左側的「資產庫」面板中，導覽至資產資料夾，該資料夾包含您要複製其內嵌程式碼的eCatalog。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。 在右側的URL面板中，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。
   * 選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

   * 選取&#x200B;**[!UICONTROL 格線檢視]**、**[!UICONTROL 清單檢視]**&#x200B;或&#x200B;**[!UICONTROL 詳細檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

     在[檢視器清單]頁面的[動作]資料表欄下，選取&#x200B;**[!UICONTROL 內嵌程式碼]**。

1. 在「內嵌程式碼」對話方塊中，選取&#x200B;**[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取&#x200B;**[!UICONTROL 關閉]**。
