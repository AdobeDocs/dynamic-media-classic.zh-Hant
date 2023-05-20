---
title: 將影像集連結到網頁
description: 瞭解如何將影像集連結到Adobe Dynamic Media Classic的網頁。
uuid: 8153a228-b2ec-4bc2-8996-266113a83df5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 40f4abab-9059-4d92-a761-f6d573b42e00
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 42%

---

# 將影像集連結到網頁{#linking-an-image-set-to-a-web-page}

發佈影像集後，您便可以在網站或應用程式中複製其 URL 或內嵌程式碼。然後，您可以視需要部署 URL 或貼上內嵌程式碼，以便使用者在您的網站或應用程式中檢視「影像集」。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製影像集URL {#copying-an-image-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉清單中，選擇 **[!UICONTROL 影像集]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「影像集」的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和嵌入代碼」面板中，選擇 **[!UICONTROL 複製URL]** 按鈕。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

## 增加影像集 URL 至網頁 {#adding-image-set-urls-to-your-web-page}

部署影像集最普遍的方式是在網頁上放置連結 (透過導覽圖示)。按一下後，連結將啟動動態頁(JSP)，該頁在彈出式縮放窗口中顯示「影像集」。 縮放連結會開啟包含實際縮放功能的快顯視窗。

有關詳細資訊和代碼示例，請參閱 [《HTML查看器參考指南》中的「嵌入Adobe5縮放查看器」](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)。

## 複製影像集查看器的嵌入代碼 {#copying-the-embed-code-of-an-image-set-viewer}

您可使用「內嵌程式碼」功能查看所選「影像集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。不可在「內嵌程式碼」對話框中編輯程式碼。

**複製「影像集」檢視器的內嵌程式碼:**

1. 在「資產瀏覽」面板的「顯示」下拉清單中，選擇 **[!UICONTROL 影像集]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「影像集」的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的URL面板中，選擇 **[!UICONTROL 嵌入代碼]**。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **清單視圖**&#x200B;或 **詳細資訊視圖**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 嵌入代碼]**。

1. 在「嵌入代碼」對話框中，選擇 **[!UICONTROL 複製到剪貼簿]**。

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選擇 **[!UICONTROL 關閉]**。

>[!MORELIKETHIS]
>
>* [發佈](publishing-files.md#publishing_files)

