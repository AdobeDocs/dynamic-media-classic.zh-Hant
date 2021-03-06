---
title: 整合AdobeDynamic Media Classic與Adobe Target Standard/Premium
description: 了解如何整合AdobeDynamic Media Classic與Adobe Target Standard/Premium。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 整合AdobeDynamic Media Classic與Adobe Target Standard/Premium {#integrating-dmc-with-target}

您必須先在[!DNL Adobe Dynamic Media Classic] 「應用程式一般設定」畫面中輸入您的Target URL，才能將[!DNL Adobe Dynamic Media Classic]與[!DNL Target Standard/Premium]整合。 若要取得您的Target URL，並在「應用程式一般設定」頁面中輸入，請執行下列動作：

1. 在[!DNL Adobe Experience Cloud]中，登入您的[!DNL Target Standard/Premium]帳戶。
1. 登入後，在瀏覽器的位址列中，將URL複製到（包括`.com`）。

   例如，如果位址列中的&#x200B;*虛構* URL（URL路徑一律包含正斜線，而非如此範例中的反斜線）是`https:\\www.myfictionalsite.com/categories/admin/home.do`，請僅複製&#x200B;*虛構* URL的此部分：`https:\\www.myfictionalsite.com`。

1. 在[!DNL Adobe Dynamic Media Classic]中，轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**。
1. 在「應用程式一般設定」頁面的「**[!UICONTROL Test&amp;Target伺服器名稱]**」欄位中，貼上您在步驟2複製的URL。
1. 選擇&#x200B;**[!UICONTROL 關閉]**。
