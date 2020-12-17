---
title: 自訂 Media Portal 畫面
seo-title: 自訂 Media Portal 畫面
description: 'null'
seo-description: 瞭解如何自訂Media Portal畫面。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 53%

---


# 自訂 Media Portal 畫面{#customizing-the-media-portal-screen}

Media Portal 樣式設定可讓您在 Media Portal 畫面置入公司標誌與色彩。使用樣式設定即可將公司戳記放在 Media Portal 上。

若要存取樣式設定，請選擇&#x200B;**設定** > **Media Portal 設定** > **樣式設定**。 完成設定之後，請務必按一下「**儲存**」，以儲存的設定。您可以按一下「**還原**」來恢復預設設定。完成選擇之後，「預覽」面板會顯示您所作之選項所產生的外觀。

**標** 志按一下瀏覽，然後在選擇標誌影像窗口中選擇圖形。

**應用** 程式：在「背景漸層顏色」選單上進行選擇，以建立漸層顏色混合。

**樹選** 擇變換顏色（將指針移到項目上時顯示的顏色）和選擇顏色（選擇項目時顯示的顏色）。

**收合** 式面板為顯示在「詳細資訊」視圖中螢幕右側的收合式面板選擇背景顏色、邊框樣式、變換和選定顏色。

**Accordion頁** 首選擇是否在accordion頁首粗體中建立文字。

**數** 據網格選擇資料網格中標題行的顏色。

**警** 報為警報消息框選擇背景顏色。

**進度** 列選擇指示上載和下載進度的列的顏色。

Media Portal使用者若要查看您選擇的樣式設定，必須將`?company=(company name)`附加至存取Media Portal的URL。 例如，若要查看樣式設定，使用以下 URL 存取 PortalCo 公司的 Media Portal 使用者:

`https://s7sps1.scene7.com/MediaPortal`

會改用下列 URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

在 URL 中包含公司名稱，可讓 Media Portal 識別使用者要存取哪家公司，並據以套用該公司的樣式設定。

您可以進一步瞭解 Media Portal 使用者的通訊 URL 變更，並設定「歡迎」電子郵件，使得新使用者可以收到正確的 Media Portal URL。

請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
