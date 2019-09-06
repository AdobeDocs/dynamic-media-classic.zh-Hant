---
title: 將 URL 連結至網路應用程式
seo-title: 將 URL 連結至網路應用程式
description: 'null'
seo-description: 瞭解如何連結URL至您的Web應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186fb96
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENT_ PK/categories/image_ size
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 將 URL 連結至網路應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式會透過URL字串存取動態媒體影像伺服器內容。在您發佈影像後，Dynamic Media Classic會啓動參照動態媒體影像伺服器上影像預設集的URL字串。您可以將這些 URL 貼至網路瀏覽器以進行測試。

若要將這些 URL 字串置於網頁和應用程式中，請從 Scene7 Publishing System 複製。若要取得以影像預設集產生的 URL 字串，請前往「預覽」畫面或瀏覽面板 (在詳細檢視中)。

## 取得影像預設集 URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

***注意**：在您發佈資產之前，URL是無效的。*

### 從預覽取得影像預設集 URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗上方的工具列右側，按一下「格點檢視」。在「資產」視窗中，選取一項影像資產，然後在縮圖影像下方按一下「預覽 &gt; 影像預設集清單」。
   * 在「資產」視窗上方的工具列右側，按一下「清單檢視」。在「資產」視窗中，選取一項影像資產，然後在縮圖影像右側按一下「預覽 &gt; 影像預設集清單」。
   * 在「資產」視窗上方的工具列右側，按一下「詳細檢視」。在同一個工具列上，按一下「預覽 &gt; 影像預設集清單」。

1. (選擇性) 在「影像預設集清單」視窗中，位於底部之「產生複製 URL 的 URL 編碼」下拉式清單中，選取複製 URL 編碼時您要套用至影像資產 URL 的 URL 編碼。
1. 在「影像預設集清單」視窗的預覽窗格右上角中，針對選取的預設集類型按一下「複製 URL」。
1. 在「影像預設集清單」視窗右下角，按一下「關閉」即可返回「資產」畫面。

### 從瀏覽面板取得影像預設集 URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」視窗上方的工具列右側，按一下「格點檢視」。從瀏覽面板取得影像預設集 URL
1. 在「資產」視窗上方的工具列右側，按一下「詳細檢視」。
1. 按一下畫面右側面板上的 URL，以展開影像預設集清單。
1. 在含有您要複製至剪貼簿之 URL 的影像預設集名稱旁，按一下「複製 URL」連結。

## 關於影像預設集 URL 字串 {#about-image-preset-url-strings}

「動態媒體影像伺服器影像大小」的URL呼叫有下列基本語法：

*路徑*/*影像伺服器名稱*/*帳戶名稱*/*影像名稱*?*修飾元 1*&amp;*修飾元 2*&amp;...

在Dynamic Media Image Server URL中，顯示影像的伺服器指示會出現在問號(？)後面。例如，此 URL 呼叫會傳送名為「背包」的影像，其寬度為 250 像素:

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

URL 中的影像預設集名稱皆包含在貨幣符號 ($) 中。When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## 增加動態影像至網頁 {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
