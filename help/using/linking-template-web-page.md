---
title: 將範本連結至網頁
description: 瞭解如何將範本連結至Adobe Dynamic Media Classic中的網頁。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 37%

---

# 將範本連結至網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式會透過URL字串存取Dynamic Media Image Server內容。 在您發佈範本後，Adobe Dynamic Media Classic會啟動參考Dynamic Media影像伺服器上的範本的URL字串。 您可以將這個 URL 貼至 Web 瀏覽器以進行測試。

若要將URL字串放在網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得影像預設集產生的範本URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。 然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 取得範本URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。若要從「範本預覽」頁面取得以「影像預設集」產生的範本URL字串，請執行下列動作：

1. 選取範本的變換影像 **[!UICONTROL 預覽]** 按鈕或前往 **[!UICONTROL 檔案]** > **[!UICONTROL 預覽]**.
1. 使用預設選單，選擇要用於傳送範本影像的影像預設集。「預覽」頁面會顯示範本從伺服器傳送時的樣子。
1. 選取 **[!UICONTROL 複製URL]** 以便將URL複製到剪貼簿。

## 新增範本URL至您的網頁 {#adding-template-urls-to-your-web-page}

若要新增範本至網頁，請洽詢您的網頁開發團隊，以修改 `<IMG>` 標籤中的HTML網頁程式碼。 使用Adobe Dynamic Media Classic URL字串向Dynamic Media影像伺服器提出要求。 商務引擎或動態網頁代碼插入的範本影像符合為範本選擇的影像預設集所定義的大小及格式規格。

>[!MORELIKETHIS]
>
>* [將動態影像新增至網頁](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

