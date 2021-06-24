---
title: 將 URL 連結至網路應用程式
description: 了解如何將URL連結至您的Web應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 53%

---

# 將 URL 連結至網路應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式可透過URL字串存取Dynamic Media Image Server內容。 發佈影像後，Dynamic Media Classic會啟用參考Dynamic Media影像伺服器上的影像預設集的URL字串。 您可以將這些 URL 貼至網路瀏覽器以進行測試。

若要將這些URL字串放入您的網頁和應用程式中，請從Dynamic Media Classic複製。 若要取得以影像預設集產生的 URL 字串，請前往「預覽」畫面或瀏覽面板 (在詳細檢視中)。

## 取得影像預設集 URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽取得影像預設集 URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗上方的工具列右側，按一下「**[!UICONTROL 格點檢視]**」。在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方按一下「預覽&#x200B;**** > **[!UICONTROL 影像預設集清單]**」。
   * 在「資產」視窗上方的工具列右側，按一下「**[!UICONTROL 清單檢視]**」。在「資產」窗口中，選擇單個影像資產，然後按一下縮圖影像的右側，按一下「預覽&#x200B;**** > **[!UICONTROL 影像預設集清單]**」。
   * 在「資產」視窗上方的工具列右側，按一下「**[!UICONTROL 詳細檢視]**」。在相同工具列上，按一下「**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**」。

1. （可選）在「影像預設集清單」的「複製URL產生的URL編碼」下拉式清單中，選取複製影像資產時要套用至其URL的URL編碼。
1. 在「影像預設集清單」窗口的預覽窗格右上方區域，按一下所選預設集類型的「複製URL ]**」。**[!UICONTROL 
1. 在「影像預設集清單」視窗的右下角，按一下「**[!UICONTROL 關閉]**」以返回「資產」畫面。

### 從瀏覽面板取得影像預設集 URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」視窗上方的工具列右側，按一下「**[!UICONTROL 格點檢視]**」。從瀏覽面板取得影像預設集 URL
1. 在「資產」視窗上方的工具列右側，按一下「**[!UICONTROL 詳細檢視]**」。
1. 按一下畫面右側面板上的&#x200B;**[!UICONTROL URL]** ，展開影像預設集清單。
1. 按一下影像預設集名稱旁的&#x200B;**[!UICONTROL 複製URL]**&#x200B;連結，其中包含您要複製到剪貼簿的URL。

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

## 增加動態影像至網頁 {#adding-dynamic-images-to-your-web-page}

若要將動態影像新增至網頁，HTML網頁程式碼中的`<IMG>`標籤通常會使用Dynamic Media Classic URL字串來修改，以向Dynamic Media影像伺服器提出要求。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在可以使用`<IMG>`標籤，以對Dynamic Media Classic平台的「影像預設集」呼叫取代靜態影像的參考。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此範例中，Dynamic Media影像伺服器會「查詢」`$thumbnail$`的定義，並以`thumbnail`影像預設集所定義的大小和格式規格，動態產生適當的影像。 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
