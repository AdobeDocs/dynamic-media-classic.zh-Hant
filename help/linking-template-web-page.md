---
title: 將範本連結到網頁
seo-title: 將範本連結到網頁
description: 'null'
seo-description: 瞭解如何將範本連結至網頁。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/template_ basics
discoiquuid: 989dba07-448a-45b1-b157-af50 abb5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 將範本連結到網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式會透過URL字串存取動態媒體影像伺服器內容。在您發佈範本後，Dynamic Media Classic會啓動參照動態媒體影像伺服器上範本的URL字串。您可以將這個 URL 貼至 Web 瀏覽器以進行測試。

若要將 URL 字串置於網頁或應用程式，請從 Scene7 Publishing System 複製。若要取得使用影像預設集產生的範本 URL 字串，請移至「預覽」畫面或瀏覽面板 (在詳細檢視中)。然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 取得範本 URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。請按照以下步驟在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串:

1. 按一下範本的滑鼠指向「預覽」按鈕或選擇「檔案 &gt; 預覽」。「預覽」畫面開啟。
1. 使用預設選單，選擇要用於傳送範本影像的影像預設集。「預覽」畫面可顯示從伺服器傳送後的範本效果。
1. 按一下「複製 URL」按鈕，將 URL 複製到剪貼簿。

## 將範本 URL 增加到網頁中 {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 商務引擎或動態網頁代碼插入的範本影像符合為範本選擇的影像預設集所定義的大小及格式規格。

>[!MORELIKETHIS]
>
>* [增加動態影像至網頁](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
