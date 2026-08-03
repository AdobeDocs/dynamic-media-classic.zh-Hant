---
title: 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合
description: 瞭解如何將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:50.750Z'
TQID: 'https://experienceleague.adobe.com/csg3qawhCOMv6niWQHp9vyGgpJBcVuOOhExioDeURuA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: c8b39b658f09de6bb598277c5a0a4e1ce3a8bc9a
workflow-type: tm+mt
source-wordcount: 137
ht-degree: 0%

---

# 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合 {#integrating-dmc-with-target}

您必須先在「[!DNL Adobe Dynamic Media Classic]應用程式一般設定」畫面中輸入目標URL，才能將[!DNL Adobe Dynamic Media Classic]與[!DNL Target Standard/Premium]整合。 若要取得Target URL並在「應用程式一般設定」頁面中輸入，請執行下列動作

1. 在[!DNL Adobe Experience Cloud]中，登入您的[!DNL Target Standard/Premium]帳戶。
1. 登入後，在瀏覽器的位址列中，將URL複製到並包括`.com`。

   如果位址列中的URL （URL路徑一律包含正斜線，而非反斜線）是`https://www.myfictionalsite.com/categories/admin/home.do`，請複製此部分： `https://www.myfictionalsite.com`。

1. 在[!DNL Adobe Dynamic Media Classic]中，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**。
1. 在「應用程式一般設定」頁面的&#x200B;**[!UICONTROL Test&amp;Target伺服器名稱]**&#x200B;欄位中，貼上您在步驟2中複製的URL。
1. 選取&#x200B;**[!UICONTROL 關閉]**。
