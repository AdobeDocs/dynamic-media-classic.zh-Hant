---
title: 將範本連結到網頁
description: 瞭解如何將範本連結至網頁。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 68%

---


# 將範本連結到網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式會透過URL字串存取Dynamic Media影像伺服器內容。 發佈範本後，Dynamic Media經典會啟動參考Dynamic Media影像伺服器上範本的URL字串。 您可以將這個 URL 貼至 Web 瀏覽器以進行測試。

若要將URL字串置於您的網頁和應用程式中，請從Dynamic Media經典複製。 若要取得使用影像預設集產生的範本 URL 字串，請移至「預覽」畫面或瀏覽面板 (在詳細檢視中)。然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 取得範本 URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。請按照以下步驟在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串:

1. 按一下範本的滑鼠指向「預覽」按鈕或選擇「檔案 > 預覽」。「預覽」畫面開啟。
1. 使用預設選單，選擇要用於傳送範本影像的影像預設集。「預覽」畫面可顯示從伺服器傳送後的範本效果。
1. 按一下「複製 URL」按鈕，將 URL 複製到剪貼簿。

## 將範本 URL 增加到網頁中  {#adding-template-urls-to-your-web-page}

若要將範本新增至網頁，請洽詢您的網頁開發團隊，以使用Dynamic Media經典URL字串修改HTML網頁程式碼中的`<IMG>`標籤，以向Dynamic Media影像伺服器提出要求。 商務引擎或動態網頁代碼插入的範本影像符合為範本選擇的影像預設集所定義的大小及格式規格。

>[!MORELIKETHIS]
>
>* [增加動態影像至網頁](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

