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
autotag-review: '2026-05-13T19:52:27.080Z'
TQID: 'https://experienceleague.adobe.com/c1Un6UFrYZh-tqwPp98shMiTUEEMhkEn1vmxEl2rVq0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f55e82148ae9d11c54dda28351743b02c1fb58a4
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 11%

---

# 將範本連結至網頁{#linking-a-template-to-a-web-page}

您的網站和應用程式會使用URL字串存取Dynamic Media影像伺服器內容。 在您發佈範本後，Adobe Dynamic Media Classic會啟用在Dynamic Media影像伺服器上參考範本的URL字串。 您可以將此URL貼到網頁瀏覽器以進行測試。

若要將URL字串置入網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得使用影像預設集產生的範本URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。 然後選取「影像預設集」並選取「複製 URL」按鈕。

>[!NOTE]
>
>在發佈資產之前，URL 不會產生作用。

## 取得範本URL {#obtaining-a-template-url}

您可以在「範本預覽」畫面上取得使用影像預設集產生的範本 URL 字串。 在您複製URL後，該URL會儲存到剪貼簿，以便您視需要貼上。 若要從「範本預覽」頁面取得使用「影像預設集」產生的範本URL字串，請執行下列動作：

1. 選取範本的&#x200B;**[!UICONTROL 預覽]**&#x200B;按鈕，或移至&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 預覽]**。
1. 使用「預設」選單，選擇您要用來傳送範本的「影像預設」。 「預覽」頁面會在範本從伺服器傳送時顯示範本。
1. 選取「**[!UICONTROL 複製URL]**」，以便將URL複製到剪貼簿。

## 新增範本URL至您的網頁 {#adding-template-urls-to-your-web-page}

若要新增範本至您的網頁，請洽詢您的網頁開發團隊，以修改HTML網頁程式碼中的`<IMG>`標籤。 使用Adobe Dynamic Media Classic URL字串傳送要求給Dynamic Media影像伺服器。 商務引擎或動態網頁程式碼會以您為範本選擇的影像預設集定義的大小和格式規格，插入範本影像。

>[!MORELIKETHIS]
>
>* [新增動態影像至您的網頁](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
