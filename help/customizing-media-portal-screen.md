---
title: 自訂 Media Portal 畫面
description: 瞭解如何在Adobe Dynamic Media Classic自定義媒體門戶螢幕。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# 自訂 Media Portal 畫面{#customizing-the-media-portal-screen}

Media Portal 樣式設定可讓您在 Media Portal 畫面置入公司標誌與色彩。使用樣式設定將公司品牌推廣放在媒體門戶上。

要訪問樣式設定，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 媒體門戶設定]** > **[!UICONTROL 樣式設定]**。 確保選擇 **[!UICONTROL 保存]** 來保存設定。 可以選擇 **[!UICONTROL 還原]** 來恢復預設設定。 在您進行選擇時，「預覽」面板將顯示它們的顯示方式。

* **[!UICONTROL 標識]**  — 選擇 **[!UICONTROL 瀏覽]**，然後在「選擇徽標影像」窗口中選擇圖形。

* **[!UICONTROL 應用程式]**  — 通過在「背景漸變顏色」菜單上進行選擇來建立漸變顏色混合。

* **[!UICONTROL 樹]**  — 選擇滾動顏色（將指針移到項目上時顯示的顏色）和選擇顏色（選擇項目時顯示的顏色）。

* **[!UICONTROL 手風琴]**  — 為「詳細資訊」視圖中螢幕右側顯示的折疊面板選擇背景顏色、邊框樣式、滾動和選定顏色。

* **[!UICONTROL 折疊式標題]**  — 選擇是否在折疊面板標題粗體中生成文本。

* **[!UICONTROL 達塔格里德]**  — 為資料網格中的標題行選擇顏色。

* **[!UICONTROL 警報]**  — 為警報消息框選擇背景顏色。

* **[!UICONTROL 進度欄]**  — 為指示上載和下載進度的欄選擇顏色。

要讓媒體門戶用戶查看您選擇的樣式設定，他們必須追加 `?company=(company name)` 訪問媒體門戶的URL。 例如，若要查看樣式設定，使用以下 URL 存取 PortalCo 公司的 Media Portal 使用者:

`https://s7sps1.scene7.com/MediaPortal`

請改用以下URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

在 URL 中包含公司名稱，可讓 Media Portal 識別使用者要存取哪家公司，並據以套用該公司的樣式設定。

您可以進一步瞭解 Media Portal 使用者的通訊 URL 變更，並設定「歡迎」電子郵件，使得新使用者可以收到正確的 Media Portal URL。

請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
