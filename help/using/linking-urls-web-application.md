---
title: 將URL連結至您的網頁應用程式
description: 瞭解如何從Adobe Dynamic Media Classic將URL連結至您的網路應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 將URL連結至您的網頁應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式可透過URL字串存取Dynamic Media影像伺服器內容。 發佈影像後，Adobe Dynamic Media Classic會啟用參照Dynamic Media影像伺服器上影像預設集的URL字串。 您可以將這些 URL 貼至網路瀏覽器以進行測試。

若要將這些URL字串放入您的網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得影像預設集產生的URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。

## 取得影像預設集URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽取得影像預設集URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一影像資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一影像資產，然後在縮圖影像的右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.

1. （可選）在「影像預設集」清單的「產生複製URL的URL編碼」下拉式清單中，選取您要在複製影像資產的URL時套用的URL編碼。
1. 在「影像預設集清單」視窗中，在預覽窗格的右上角區域選取 **[!UICONTROL 複製URL]** 選取的預設集型別。
1. 在「影像預設集清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。

### 從瀏覽面板取得影像預設集URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 從瀏覽面板取得影像預設集 URL
1. 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**.
1. 選取 **[!UICONTROL URL]** 位於畫面右側的面板上，方便您展開影像預設集清單。
1. 選取 **[!UICONTROL 複製URL]** 影像預設集名稱旁的連結，以及您要複製到剪貼簿的URL。

## 關於影像預設集 URL 字串 {#about-image-preset-url-strings}

Dynamic Media影像伺服器的影像大小調整URL呼叫有以下基本語法：

*路徑*/*影像伺服器名稱*/*帳戶名稱*/*影像名稱*?*修飾元 1*&amp;*修飾元 2*&amp;...

在Dynamic Media影像伺服器URL中，伺服器的影像顯示指示會出現在問號(？)之後。 例如，此 URL 呼叫會傳送名為「背包」的影像，其寬度為 250 像素:

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

URL 中的影像預設集名稱皆包含在貨幣符號 ($) 中。當Dynamic Media影像伺服器遇到URL的影像預設集部分時( `Large` 在此情況下)，使用「大」影像預設集定義的大小和格式設定指示。

## 將動態影像新增至網頁 {#adding-dynamic-images-to-your-web-page}

若要將動態影像新增至網頁，請 `<IMG>` HTML網頁程式碼中的標籤通常會使用Adobe Dynamic Media Classic URL字串進行修改，以向Dynamic Media影像伺服器提出要求。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在使用 `<IMG>`標籤上的標籤，以使用對Adobe Dynamic Media Classic平台的影像預設集呼叫來取代靜態影像的參考。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此範例中，Dynamic Media影像伺服器「查詢」定義 `$thumbnail$` 並透過以下專案所定義的大小與格式規格，動態產生適當的影像： `thumbnail`影像預設集。 在 URL 字串中，除了產品影像檔案名稱 (在此範例中為 `backpack_trns`) 之外的所有項目，通常都會連接至頁面範本。唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
