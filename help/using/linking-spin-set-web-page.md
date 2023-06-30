---
title: 將迴轉集連結至網頁
description: 瞭解如何將迴轉集連結至Adobe Dynamic Media Classic中的網頁。
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# 將迴轉集連結至網頁{#linking-a-spin-set-to-a-web-page}

網站和應用程式會透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括迴轉集。 這些 URL 字串會在發佈程序中啟用。若要將迴轉集的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製迴轉集URL {#copying-a-spin-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 迴轉集]**.
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「迴轉集」的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

## 將迴轉集URL新增至網頁 {#adding-spin-set-urls-to-your-web-page}

迴轉集的部署方式與所有縮放檢視器一樣，即透過在縮放視窗中顯示迴轉集的動態頁面 (ASP 或 JSP) 部署。對Adobe Dynamic Media Classic平台的URL呼叫遵循縮放檢視器上的相同通訊協定。 不過，「檢視器預設集」名稱取決於管理員定義為預設「迴轉集檢視器預設集」的預設集。例如，以下非線上的 URL 語法範例包括名為 `viewer.jsp` 的預設集名稱，而現在 SKU 參數為迴轉集名稱:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此 URL 語法範例 (非線上連結) 中，注意 SKU 號碼 (`sku=backpack_spin`)。之後的字串 `sku=` 是迴轉集名稱( `backpack spin`)。

## 複製迴轉集檢視器的內嵌程式碼 {#copying-the-embed-code-of-a-spin-set-viewer}

您可使用「內嵌程式碼」功能查看所選「迴轉集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。不可在「內嵌程式碼」對話框中編輯程式碼。

**複製迴轉集檢視器的內嵌程式碼:**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 迴轉集]**.
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「迴轉集」的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 內嵌程式碼]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

     在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   不可在「內嵌程式碼」對話框中編輯程式碼。

1. 選取 **[!UICONTROL 關閉]**.
