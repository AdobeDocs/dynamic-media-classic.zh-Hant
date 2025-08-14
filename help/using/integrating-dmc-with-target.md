---
title: 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合
description: 瞭解如何將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合 {#integrating-dmc-with-target}

您必須先在「[!DNL Adobe Dynamic Media Classic]應用程式一般設定」畫面中輸入目標URL，才能將[!DNL Target Standard/Premium]與[!DNL Adobe Dynamic Media Classic]整合。 若要取得Target URL並在「應用程式一般設定」頁面中輸入，請執行下列動作：

1. 在[!DNL Adobe Experience Cloud]中，登入您的[!DNL Target Standard/Premium]帳戶。
1. 登入後，在瀏覽器的位址列中，將URL複製到並包括`.com`。

   例如，如果位址列中的&#x200B;*虛構* URL （URL路徑一律包含正斜線，而非此範例中的反斜線）是`https:\\www.myfictionalsite.com/categories/admin/home.do`，則僅複製&#x200B;*虛構* URL的這個部分： `https:\\www.myfictionalsite.com`。

1. 在[!DNL Adobe Dynamic Media Classic]中，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**。
1. 在「應用程式一般設定」頁面的&#x200B;**[!UICONTROL Test&amp;Target伺服器名稱]**&#x200B;欄位中，貼上您在步驟2中複製的URL。
1. 選取&#x200B;**[!UICONTROL 關閉]**。
