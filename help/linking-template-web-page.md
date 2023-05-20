---
title: 將範本連結至網頁
description: 瞭解如何將模板連結到Adobe Dynamic Media Classic的網頁。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 37%

---

# 將範本連結至網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式通過URL字串訪問Dynamic Media映像伺服器內容。 發佈模板後，Adobe Dynamic Media Classic將激活一個URL字串，該字串引用Dynamic Media影像伺服器上的模板。 您可以將這個 URL 貼至 Web 瀏覽器以進行測試。

要將URL字串置於網頁和應用程式中，請從Adobe Dynamic Media Classic複製。 要獲取使用影像預設生成的模板URL字串，請轉到「預覽」螢幕或「瀏覽面板」（在「詳細資訊視圖」中）。 然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 獲取模板URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。複製 URL 之後，該 URL 就會進入剪貼簿，讓您視需要貼上。要從「模板預覽」頁獲取使用「影像預設」生成的模板URL字串，請執行以下操作：

1. 選擇模板的滾動更新 **[!UICONTROL 預覽]** 按鈕 **[!UICONTROL 檔案]** > **[!UICONTROL 預覽]**。
1. 使用預設選單，選擇要用於傳送範本影像的影像預設集。「預覽」(Preview)頁面顯示從伺服器傳送模板時的樣式。
1. 選擇 **[!UICONTROL 複製URL]** 以便將URL複製到剪貼簿。

## 將模板URL添加到網頁 {#adding-template-urls-to-your-web-page}

要向網頁添加模板，請咨詢網頁開發團隊以修改 `<IMG>` HTML網頁代碼中的標籤。 使用Adobe Dynamic Media ClassicURL字串向Dynamic Media映像伺服器發出請求。 商務引擎或動態網頁代碼插入的範本影像符合為範本選擇的影像預設集所定義的大小及格式規格。

>[!MORELIKETHIS]
>
>* [向網頁添加動態影像](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

