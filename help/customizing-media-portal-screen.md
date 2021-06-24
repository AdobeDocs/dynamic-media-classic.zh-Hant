---
title: 自訂 Media Portal 畫面
description: 了解如何自訂Media Portal畫面。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic，協作，資產管理
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# 自訂 Media Portal 畫面{#customizing-the-media-portal-screen}

Media Portal 樣式設定可讓您在 Media Portal 畫面置入公司標誌與色彩。使用樣式設定將公司品牌推廣到媒體入口網站。

若要存取樣式設定，請選擇&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL Media Portal 設定]** > **[!UICONTROL 樣式設定]**。 完成設定之後，請務必按一下「**[!UICONTROL 儲存]**」，以儲存的設定。您可以按一下「**[!UICONTROL 還原]**」來恢復預設設定。完成選擇之後，「預覽」面板會顯示您所作之選項所產生的外觀。

* **徽標**  — 按一下「 **** 瀏覽」，然後在「選擇徽標影像」窗口中選擇圖形。

* **應用**  — 通過在「背景漸變顏色」菜單上進行選擇來建立漸變顏色混合。

* **樹**  — 選擇變換顏色（將指針移動到項目上時顯示的顏色）和選擇顏色（選擇項目時顯示的顏色）。

* **折疊式功能表**  — 為顯示在「詳細資訊」檢視畫面右側的折疊式功能表選擇背景顏色、邊框樣式、變換及選取的顏色。

* **折疊式面板標題**  — 選擇是否在折疊式面板標題粗體中建立文字。

* **資料格**  — 為資料格線中的標題列選擇顏色。

* **警報**  — 為警報訊息方塊選擇背景顏色。

* **進度條**  — 為指示上載和下載進度的條選擇一個顏色。

Media Portal使用者若要查看您選取的樣式設定，必須將`?company=(company name)`附加至其存取Media Portal的URL。 例如，若要查看樣式設定，使用以下 URL 存取 PortalCo 公司的 Media Portal 使用者:

`https://s7sps1.scene7.com/MediaPortal`

請改用下列URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

在 URL 中包含公司名稱，可讓 Media Portal 識別使用者要存取哪家公司，並據以套用該公司的樣式設定。

您可以進一步瞭解 Media Portal 使用者的通訊 URL 變更，並設定「歡迎」電子郵件，使得新使用者可以收到正確的 Media Portal URL。

請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
