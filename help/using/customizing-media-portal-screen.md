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
autotag-review: '2026-05-13T19:43:32.877Z'
TQID: 'https://experienceleague.adobe.com/tIJ90TIWEvVbRT1LR-z8ajTrx2zEXg33V8Q9SgOfzKY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 00d087b14c6c030473ecfee92ec879e705a9b197
workflow-type: tm+mt
source-wordcount: 329
ht-degree: 5%

---

# 自訂Media Portal畫面{#customizing-the-media-portal-screen}

Media Portal 樣式設定可讓您在 Media Portal 畫面置入公司標誌與色彩。 使用樣式設定將您的公司品牌套用至Media Portal。

若要存取樣式設定，請移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 樣式設定]**。 確定選取&#x200B;**[!UICONTROL 儲存]**，在設定完成後儲存設定。 您可以選取&#x200B;**[!UICONTROL 還原]**&#x200B;以重設為預設值。 當您做出選擇時，「預覽」面板會顯示它們的顯示方式。

* **[!UICONTROL 標誌]**：選取&#x200B;**[!UICONTROL 瀏覽]**，然後在[選取標誌影像]視窗中選擇圖形。

* **[!UICONTROL 應用程式]**：選取「背景漸層顏色」選單上的選項，以設定漸層顏色混合。

* **[!UICONTROL 樹狀結構]**：選擇滑鼠指向效果顏色和選取範圍顏色。

* **[!UICONTROL 摺疊式功能表]**：選擇背景顏色、邊框樣式，以及在[詳細資料]檢視畫面右側顯示的摺疊式功能表所選取的滑鼠指向效果顏色。

* **[!UICONTROL 收合式選單標題]**：選擇是否要以收合式選單標題粗體顯示文字。

* **[!UICONTROL Datagrid]**：選擇資料網格中標題列的色彩。

* **[!UICONTROL 警示]**：選擇警示訊息方塊的背景顏色。

* **[!UICONTROL 進度列]**：選擇指示上傳和下載進度的進度列色彩。

若要讓Media Portal使用者檢視您選擇的樣式設定，他們必須在存取Media Portal的URL中附加`?company=(company name)`。 例如，若要檢視樣式設定，存取PortalCo公司的Media Portal使用者可以使用以下URL：

`https://s7sps1.scene7.com/MediaPortal`

請改用以下URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

在URL中包含公司名稱可讓Media Portal識別使用者想要存取的公司，並據此套用公司的樣式設定。

您可以進一步瞭解如何與Media Portal使用者通訊URL變更，以及設定歡迎電子郵件訊息，好讓新使用者接收正確的Media Portal URL。

請參閱[為Media Portal使用者設定歡迎電子郵件訊息](adding-media-portal-users.md#setting_up_the_welcome_email_message_for_media_portal_users)。
