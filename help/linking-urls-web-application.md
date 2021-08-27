---
title: 將URL連結至您的Web應用程式
description: 了解如何從AdobeDynamic Media Classic將URL連結至您的Web應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 將URL連結至您的Web應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式可透過URL字串存取Dynamic Media Image Server內容。 發佈影像後，AdobeDynamic Media Classic會啟用參考Dynamic Media影像伺服器上的影像預設集的URL字串。 您可以將這些 URL 貼至網路瀏覽器以進行測試。

若要將這些URL字串放入您的網頁和應用程式中，請從AdobeDynamic Media Classic複製。 若要取得影像預設集產生的URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。

## 取得影像預設集URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽中取得影像預設集URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」窗口的右側，選擇「**[!UICONTROL 網格視圖]**」。 在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在「資產」窗口的右側，選擇「**[!UICONTROL 清單視圖]**」。 在「資產」窗口中，選擇單個影像資產，然後轉至縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在「資產」窗口的工具欄右側，選擇「**[!UICONTROL 詳細資訊視圖]**」。 在相同工具列上，前往「**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**」。

1. （可選）在「影像預設集清單」的「複製URL產生的URL編碼」下拉式清單中，選取複製影像資產時要套用至其URL的URL編碼。
1. 在「影像預設集清單」窗口的預覽窗格的右上方區域，為所選預設集類型選擇&#x200B;**[!UICONTROL 複製URL]**。
1. 在「影像預設集清單」視窗的右下角，選取&#x200B;**[!UICONTROL Close]**&#x200B;以返回「資產」畫面。

### 從「瀏覽」面板取得影像預設集URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」窗口的右側，選擇「**[!UICONTROL 網格視圖]**」。 從瀏覽面板取得影像預設集 URL
1. 在「資產」窗口的工具欄右側，選擇「**[!UICONTROL 詳細資訊視圖]**」。
1. 在螢幕右側的面板上選擇&#x200B;**[!UICONTROL URL]**，以便展開影像預設集清單。
1. 選取影像預設集名稱旁的&#x200B;**[!UICONTROL 複製URL]**&#x200B;連結，並附上您要複製到剪貼簿的URL。

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

URL 中的影像預設集名稱皆包含在貨幣符號 ($) 中。當Dynamic Media影像伺服器遇到URL的「影像預設集」部分（此例中為`Large`）時，使用「大」影像預設集定義的大小和格式指示。

## 將動態影像新增至網頁 {#adding-dynamic-images-to-your-web-page}

若要將動態影像新增至網頁，HTML網頁程式碼中的`<IMG>`標籤通常會使用AdobeDynamic Media Classic URL字串來修改，以向Dynamic Media影像伺服器提出要求。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在可以使用`<IMG>`標籤，以對AdobeDynamic Media Classic平台的「影像預設集」呼叫取代對靜態影像的參考。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此範例中，Dynamic Media影像伺服器會「查詢」`$thumbnail$`的定義，並以`thumbnail`影像預設集所定義的大小和格式規格，動態產生適當的影像。 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
