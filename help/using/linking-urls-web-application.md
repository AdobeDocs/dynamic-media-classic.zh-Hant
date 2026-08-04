---
title: 將URL連結至您的網頁應用程式
description: 瞭解如何將URL從Adobe Dynamic Media Classic連結至您的網頁應用程式。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:48.579Z'
TQID: 'https://experienceleague.adobe.com/c8e722KVmasJVtoVl8k7-5vGjvs4Lm-GZavm-TF9fk0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1960799e4144942d4d9443196e6db425f87c7686
workflow-type: tm+mt
source-wordcount: 821
ht-degree: 16%

---

# 將URL連結至您的網頁應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式會使用URL字串存取Dynamic Media影像伺服器內容。 發佈影像後，Adobe Dynamic Media Classic會啟用參照Dynamic Media影像伺服器上影像預設集的URL字串。 您可以在網頁瀏覽器中使用這些URL進行測試。

若要將這些URL字串放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得影像預設集產生的URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。

## 取得影像預設集URL {#obtaining-an-image-preset-url}

您可以從「預覽」或詳細檢視取得由影像預設集產生的 URL 字串。 在您複製URL後，該URL會儲存到剪貼簿，以便您視需要貼上。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

### 從預覽取得影像預設集URL {#obtaining-an-image-preset-url-from-preview}

1. 在左側的「資產庫」面板中，導覽至包含要預覽之影像資產的資產資料夾。
1. 進行以下一項操作:

   * 在Assets視窗上方、工具列右側，選取&#x200B;**[!UICONTROL 格線檢視]**。 在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在Assets視窗上方、工具列右側，選取&#x200B;**[!UICONTROL 清單檢視]**。 在「資產」視窗中，選取單一影像資產，然後在縮圖影像的右側，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在Assets視窗上方、工具列右側，選取&#x200B;**[!UICONTROL 詳細資料檢視]**。 在相同工具列上，移至&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。

1. （選用）在「影像預設集」清單的「產生複製URL的URL編碼」下拉式清單中，選取URL編碼，以在複製影像資產時套用至該資產的URL。
1. 在「影像預設集清單」視窗中，在預覽窗格的右上角區域中，為選取的預設集型別選取「**[!UICONTROL 複製URL]**」。
1. 在「影像預設集清單」視窗的右下角，選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回Assets畫面。

### 從瀏覽面板取得影像預設集URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左側的「資產庫」面板中，導覽至包含您要預覽之影像資產的資產資料夾。
1. 在Assets視窗上方、工具列右側，選取&#x200B;**[!UICONTROL 格線檢視]**。 從瀏覽面板取得影像預設集 URL
1. 在Assets視窗上方、工具列右側，選取&#x200B;**[!UICONTROL 詳細資料檢視]**。
1. 在右側面板上選取&#x200B;**[!UICONTROL URL]**&#x200B;以顯示影像預設集清單。
1. 選取影像預設集名稱旁的&#x200B;**[!UICONTROL 複製URL]**&#x200B;連結，以及您要複製到剪貼簿的URL。

## 影像預設集URL字串概觀 {#about-image-preset-url-strings}

在Dynamic Media影像伺服器上調整影像大小的URL呼叫有以下基本語法：

*路徑*/*影像伺服器的名稱*/*帳戶名稱*/*影像名稱*？*修飾元1*&amp;*修飾元2*&amp;...

在Dynamic Media影像伺服器URL中，伺服器的影像顯示指示會遵循問號(？)。 例如，此URL呼叫會傳送名為「揹包」的影像，寬度為250畫素：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

影像預設集 URL 包含了所有以正確大小和格式規格呈現影像的修飾元指示。 如果沒有影像預設集，請注意問號(？)後面的所有修飾元指示 在此 URL 字串中:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

不過，在「影像預設集」產生的URL字串中，「影像預設集」名稱會取代由「影像預設集」定義的指示。 例如，根據上述的長 URL，URL 字串為:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

URL中的影像預設集名稱使用貨幣符號($)。 當Dynamic Media影像伺服器處理URL的影像預設集部分（在此例中為`Large`）時，會使用「大」影像預設集所定義的大小和格式設定指示。

## 將動態影像新增至網頁 {#adding-dynamic-images-to-your-web-page}

將動態影像新增至您的網頁時，`<IMG>`標籤通常會使用Adobe Dynamic Media Classic URL字串進行修改，以從Dynamic Media影像伺服器要求影像。 此字串會按照影像預設集所定義的大小和格式規格來產生影像。

例如，您不需使用一般呼叫即可開啟靜態影像，如

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在可以使用`<IMG>`標籤，以對Adobe Dynamic Media Classic平台的影像預設集呼叫來取代靜態影像的參考。 範例呼叫的外觀如下:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

在此範例中，Dynamic Media影像伺服器會擷取`$thumbnail$`的定義，並以`thumbnail`影像預設集所定義的尺寸與格式規格，動態產生適當的影像。 在URL字串中，產品影像檔案名稱（在此案例中為`backpack_trns`）以外的所有專案通常都是針對頁面範本所設定。 唯一自動從商務伺服器插入頁面範本的元素是 IPS ID 或影像名稱。
