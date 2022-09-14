---
title: 將URL連結至您的Web應用程式
description: 了解如何從Adobe Dynamic Media Classic將URL連結至您的Web應用程式。
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

# 將URL連結至您的Web應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式可透過URL字串存取Dynamic Media Image Server內容。 發佈影像後，Adobe Dynamic Media Classic會啟動參考Dynamic Media影像伺服器上的影像預設集的URL字串。 您可以將這些 URL 貼至網路瀏覽器以進行測試。

若要將這些URL字串放入您的網頁和應用程式中，請從Adobe Dynamic Media Classic複製。 若要取得影像預設集產生的URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。

## 取得影像預設集URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽中取得影像預設集URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗上方，在工具列的右側，選取 **[!UICONTROL 網格視圖]**. 在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方，在工具列的右側，選取 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一影像資產，然後前往縮圖影像的右側 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方，在工具列的右側，選取 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.

1. （可選）在「影像預設集清單」的「複製URL產生的URL編碼」下拉式清單中，選取複製影像資產時要套用至其URL的URL編碼。
1. 在「影像預設集清單」窗口的預覽窗格右上方區域中，選擇 **[!UICONTROL 複製URL]** 的預設集類型。
1. 在「影像預設集清單」窗口的右下角，選擇 **[!UICONTROL 關閉]** 返回「資產」畫面。

### 從「瀏覽」面板取得影像預設集URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」視窗上方，在工具列的右側，選取 **[!UICONTROL 網格視圖]**. 從瀏覽面板取得影像預設集 URL
1. 在「資產」視窗上方，在工具列的右側，選取 **[!UICONTROL 詳細資料檢視]**.
1. 選擇 **[!UICONTROL URL]** 顯示在畫面右側的面板上，以便展開「影像預設集」清單。
1. 選擇 **[!UICONTROL 複製URL]** 連結至影像預設集名稱旁，以及您要複製到剪貼簿的URL。

## 關於影像預設集 URL 字串 {#about-image-preset-url-strings}

對Dynamic Media影像伺服器進行影像大小調整的URL呼叫具有下列基本語法：

*路徑*/*影像伺服器名稱*/*帳戶名稱*/*影像名稱*?*修飾元 1*&amp;*修飾元 2*&amp;...

在Dynamic Media影像伺服器URL中，顯示影像的指示會出現在問號(?)之後。 例如，此 URL 呼叫會傳送名為「背包」的影像，其寬度為 250 像素:

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

URL 中的影像預設集名稱皆包含在貨幣符號 ($) 中。當Dynamic Media影像伺服器遇到URL的「影像預設集」部分時( `Large` 在此情況下)，使用「大型」影像預設集所定義的大小和格式指示。

## 將動態影像新增至網頁 {#adding-dynamic-images-to-your-web-page}

若要將動態影像新增至您的網頁，請 `<IMG>` HTML網頁程式碼中的標籤通常會使用Adobe Dynamic Media Classic URL字串來修改，以向Dynamic Media影像伺服器提出要求。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在使用 `<IMG>`標籤，將對靜態影像的參考取代為對Adobe Dynamic Media Classic平台的「影像預設集」呼叫。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此範例中，Dynamic Media影像伺服器會「查詢」 `$thumbnail$` 並以 `thumbnail`影像預設集。 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
