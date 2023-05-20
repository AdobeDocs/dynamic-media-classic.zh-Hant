---
title: 將旋轉集連結到網頁
description: 瞭解如何將旋轉集連結到Adobe Dynamic Media Classic的網頁。
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# 將旋轉集連結到網頁{#linking-a-spin-set-to-a-web-page}

網站和應用程式通過URL字串或嵌入代碼訪問Dynamic Media映像伺服器內容，包括旋轉集。 這些 URL 字串會在發佈程序中啟用。要將「旋轉集」的URL字串或嵌入代碼放入網頁和應用程式中，請從Adobe Dynamic Media Classic複製它。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 複製旋轉集URL {#copying-a-spin-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉清單中，選擇 **[!UICONTROL 旋轉集]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「迴轉集」的資產資料夾。
1. 在工具列右側的「資產瀏覽」面板上方，執行下列任一操作:

   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，按兩下單一資產以在「詳細檢視」中開啟。在右側的「URL和嵌入代碼」面板中，選擇 **[!UICONTROL 複製URL]** 按鈕。
   * 選擇 **[!UICONTROL 網格視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮覽圖影像下，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 清單視圖]**。 在「資產瀏覽」面板中，選擇單個資產，然後在縮略圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

   * 選擇 **[!UICONTROL 網格視圖]**。 **[!UICONTROL 清單視圖]**&#x200B;或 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 查看器清單]**。

      在「查看器清單」頁中，在表的「操作」列下，選擇 **[!UICONTROL 複製URL]**。

## 將旋轉集URL添加到網頁 {#adding-spin-set-urls-to-your-web-page}

迴轉集的部署方式與所有縮放檢視器一樣，即透過在縮放視窗中顯示迴轉集的動態頁面 (ASP 或 JSP) 部署。對Adobe Dynamic Media Classic平台的URL調用遵循縮放查看器上的相同協定。 不過，「檢視器預設集」名稱取決於管理員定義為預設「迴轉集檢視器預設集」的預設集。例如，以下非線上的 URL 語法範例包括名為 `viewer.jsp` 的預設集名稱，而現在 SKU 參數為迴轉集名稱:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此 URL 語法範例 (非線上連結) 中，注意 SKU 號碼 (`sku=backpack_spin`)。後面的字串 `sku=` 是旋轉集名稱( `backpack spin`)。

## 複製旋轉集查看器的嵌入代碼 {#copying-the-embed-code-of-a-spin-set-viewer}

您可使用「內嵌程式碼」功能查看所選「迴轉集」的檢視器程式碼。您也可以將該程式碼複製到剪貼簿，然後在您的網頁中貼上，以便部署檢視器。不可在「內嵌程式碼」對話框中編輯程式碼。

**複製迴轉集檢視器的內嵌程式碼:**

1. 在「資產瀏覽」面板的「顯示」下拉清單中，選擇 **[!UICONTROL 旋轉集]**。
1. 在左側的「資產庫」面板中，導覽至含有您要複製其內嵌程式碼之「迴轉集」的資產資料夾。
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
