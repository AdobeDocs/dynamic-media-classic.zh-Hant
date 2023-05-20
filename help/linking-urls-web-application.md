---
title: 將URL連結到Web應用程式
description: 瞭解如何從Adobe Dynamic Media Classic將URL連結到Web應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 將URL連結到Web應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式通過URL字串訪問Dynamic Media映像伺服器內容。 發佈影像後，Adobe Dynamic Media Classic將激活引用Dynamic Media影像伺服器上的影像預設的URL字串。 您可以將這些 URL 貼至網路瀏覽器以進行測試。

要將這些URL字串放置到網頁和應用程式中，請從Adobe Dynamic Media Classic複製。 要獲取使用「影像預設」生成的URL字串，請轉到「預覽」螢幕或「瀏覽面板」（在「詳細資訊視圖」中）。

## 獲取影像預設URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽獲取影像預設URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」窗口的工具欄右側，選擇 **[!UICONTROL 網格視圖]**。 在「資產」窗口中，選擇單個影像資產，然後在縮覽圖影像下方，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設清單]**。
   * 在「資產」窗口的工具欄右側，選擇 **[!UICONTROL 清單視圖]**。 在「資產」窗口中，選擇單個影像資產，然後在縮覽圖影像的右側轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設清單]**。
   * 在「資產」窗口的工具欄右側，選擇 **[!UICONTROL 詳細資訊視圖]**。 在同一工具欄上，轉到 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設清單]**。

1. （可選）在「影像預設清單」的「複製URL生成的URL編碼」下拉清單中，選擇複製影像資產的URL時要應用的URL編碼。
1. 在「影像預設清單」窗口中，在預覽窗格的右上區域，選擇 **[!UICONTROL 複製URL]** 的子菜單。
1. 在「影像預設清單」窗口的右下角，選擇 **[!UICONTROL 關閉]** 返回「資產」螢幕。

### 從「瀏覽」面板獲取影像預設URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」窗口的工具欄右側，選擇 **[!UICONTROL 網格視圖]**。 從瀏覽面板取得影像預設集 URL
1. 在「資產」窗口的工具欄右側，選擇 **[!UICONTROL 詳細資訊視圖]**。
1. 選擇 **[!UICONTROL URL]** 顯示在螢幕右側的面板上，以便您可以展開「影像預設」清單。
1. 選擇 **[!UICONTROL 複製URL]** 連結，連結位於「影像預設」名稱旁邊，其中包含要複製到剪貼簿的URL。

## 關於影像預設集 URL 字串 {#about-image-preset-url-strings}

URL調用到Dynamic Media映像伺服器的映像大小具有以下基本語法：

*路徑*/*影像伺服器名稱*/*帳戶名稱*/*影像名稱*?*修飾元 1*&amp;*修飾元 2*&amp;...

在Dynamic Media影像伺服器URL中，在問號(?)後會顯示指向伺服器顯示影像的說明。 例如，此 URL 呼叫會傳送名為「背包」的影像，其寬度為 250 像素:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

影像預設集 URL 包含了所有以正確大小和格式規格呈現影像的修飾元指示。如果沒有影像預設集，請注意問號 (?) 後的所有修飾元指示 在此 URL 字串中:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

然而，在使用影像預設集產生的 URL 字串中，影像預設集的名稱會取代影像預設集所定義的指示。例如，根據上述的長 URL，URL 字串為:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

URL 中的影像預設集名稱皆包含在貨幣符號 ($) 中。當Dynamic Media影像伺服器遇到URL的影像預設部分時( `Large` 在本例中)，使用「大」影像預設定義的大小和格式說明。

## 向網頁添加動態影像 {#adding-dynamic-images-to-your-web-page}

要向網頁添加動態影像， `<IMG>` HTML網頁代碼中的標籤通常使用Adobe Dynamic Media ClassicURL字串進行修改，以向Dynamic Media映像伺服器發出請求。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

現在使用 `<IMG>`標籤，用到Adobe Dynamic Media Classic平台的「影像預設」調用替換對靜態影像的引用。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在本示例中，Dynamic Media映像伺服器「查找」 `$thumbnail$` 並動態生成具有由 `thumbnail`影像預設。 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
