---
title: 自訂Media Portal畫面
description: 瞭解如何在Adobe Dynamic Media Classic中自訂Media Portal畫面。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 21%

---

# 自訂Media Portal畫面{#customizing-the-media-portal-screen}

Media Portal 樣式設定可讓您在 Media Portal 畫面置入公司標誌與色彩。使用樣式設定將您的公司品牌置於Media Portal上。

若要存取樣式設定，請前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 樣式設定]**. 請務必選取 **[!UICONTROL 儲存]** 以在完成設定後加以儲存。 您可以選取 **[!UICONTROL 還原]** 以恢復預設設定。 當您做出選擇時，「預覽」面板會顯示它們的顯示方式。

* **[!UICONTROL 標誌]**：選取 **[!UICONTROL 瀏覽]**，然後在「選取標誌影像」視窗中選擇圖形。

* **[!UICONTROL 應用]**：在「背景漸層顏色」選單中進行選擇，以建立漸層顏色混合。

* **[!UICONTROL 樹狀]**：選擇滑鼠指向效果顏色（將指標移到專案上時顯示的顏色）和選取範圍顏色（選取專案時顯示的顏色）。

* **[!UICONTROL 摺疊面板]**：針對在「詳細資訊」檢視畫面右側顯示的摺疊式功能表，選擇背景顏色、邊框樣式以及滑鼠指向效果與選取的顏色。

* **[!UICONTROL 收合式選單標題]**：選擇是否以收合式選單標題粗體顯示文字。

* **[!UICONTROL 資料格]**：選擇資料網格中標題列的顏色。

* **[!UICONTROL 警報]**：選擇警示訊息方塊的背景顏色。

* **[!UICONTROL 進度列]**：選擇列顏色，指出上傳和下載的進度。

若要Media Portal使用者檢視您選擇的樣式設定，他們必須附加 `?company=(company name)` 存取使用者存取Media Portal時使用的URL。 例如，若要查看樣式設定，使用以下 URL 存取 PortalCo 公司的 Media Portal 使用者:

`https://s7sps1.scene7.com/MediaPortal`

請改用以下URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

在URL中包含公司名稱可讓Media Portal識別使用者想要存取的公司，並據此套用公司的樣式設定。

您可以進一步瞭解 Media Portal 使用者的通訊 URL 變更，並設定「歡迎」電子郵件，使得新使用者可以收到正確的 Media Portal URL。

請參閱[設定 Media Portal 使用者的「歡迎」電子郵件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
