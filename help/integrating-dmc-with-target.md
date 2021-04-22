---
title: 整合AdobeDynamic Media經典與Adobe Target標準版／高級版
description: 瞭解如何整合AdobeDynamic Media經典與Adobe Target標準版／高級版。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media經典
role: Data Engineer,Administrator,Business Practitioner
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 1%

---

# 整合AdobeDynamic Media經典與Adobe Target標準版／高級版{#integrating-dmc-with-target}

在將[!DNL Dynamic Media Classic]與[!DNL Target Standard/Premium]整合之前，您必須在[!DNL Dynamic Media Classic]應用程式一般設定畫面中輸入您的Target URL。 若要取得您的Target URL，並在「應用程式一般設定」頁面中輸入它，請執行下列動作：

1. 在[!DNL Adobe Experience Cloud]中，登入您的[!DNL Target Standard/Premium]帳戶。
1. 登入後，在瀏覽器的位址列中，將URL複製至並包含`.com`。

   例如，如果位址列中的&#x200B;*虛構* URL（URL路徑一律包含正斜線，而非如此範例中的反斜線）是`https:\\www.myfictionalsite.com/categories/admin/home.do`，則僅複製&#x200B;*虛構* URL的此部分：`https:\\www.myfictionalsite.com`。

1. 在[!DNL Dynamic Media Classic]中，按一下「Setup **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**」。
1. 在「應用程式一般設定」頁面的「**[!UICONTROL Test&amp;Target伺服器名稱]**」欄位中，貼上您在步驟2中複製的URL。
1. 按一下 **[!UICONTROL 關閉]**。
