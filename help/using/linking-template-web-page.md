---
title: 將範本連結至網頁
description: 瞭解如何將範本連結至Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 16%

---

# 將範本連結至網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式會透過URL字串存取Dynamic Media影像伺服器內容。 在您發佈範本後，Adobe Dynamic Media Classic會啟用參考Dynamic Media影像伺服器上的範本的URL字串。 您可以將此URL貼到網頁瀏覽器以進行測試。

若要將URL字串置入網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得使用影像預設集產生的範本URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。 然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 取得範本URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。若要從「範本預覽」頁面取得使用「影像預設集」產生的範本URL字串，請執行下列動作：

1. 選取範本的滑鼠指向效果&#x200B;**[!UICONTROL 預覽]**&#x200B;按鈕，或移至&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 預覽]**。
1. 使用「預設」選單，選擇您要用來傳送範本影像的「影像預設」。 「預覽」頁面會顯示範本從伺服器傳送時的外觀。
1. 選取「**[!UICONTROL 複製URL]**」，以便將URL複製到剪貼簿。

## 新增範本URL至您的網頁 {#adding-template-urls-to-your-web-page}

若要新增範本至您的網頁，請洽詢您的網頁開發團隊，以修改HTML網頁程式碼中的`<IMG>`標籤。 使用Adobe Dynamic Media Classic URL字串向Dynamic Media影像伺服器提出要求。 商務引擎或動態網頁程式碼會以您為範本選擇的影像預設集所定義的大小和格式規格，插入範本影像。

>[!MORELIKETHIS]
>
>* [新增動態影像至您的網頁](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
