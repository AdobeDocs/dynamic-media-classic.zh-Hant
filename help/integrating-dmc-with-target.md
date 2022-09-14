---
title: 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合
description: 了解如何整合Adobe Dynamic Media Classic與Adobe Target Standard/Premium。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合 {#integrating-dmc-with-target}

整合之前 [!DNL Adobe Dynamic Media Classic] with [!DNL Target Standard/Premium]，您必須在 [!DNL Adobe Dynamic Media Classic] 應用程式一般設定畫面。 若要取得您的Target URL，並在「應用程式一般設定」頁面中輸入，請執行下列動作：

1. 在 [!DNL Adobe Experience Cloud]，登入 [!DNL Target Standard/Premium] 帳戶。
1. 登入後，在瀏覽器的位址列中，將URL複製到（包括） `.com`.

   例如，若 *虛構* 位址列中的URL（URL路徑一律包含正斜線，而非如此範例所示的反斜線）為 `https:\\www.myfictionalsite.com/categories/admin/home.do`，僅複製 *虛構* URL: `https:\\www.myfictionalsite.com`.

1. 在 [!DNL Adobe Dynamic Media Classic]，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**.
1. 在「應用程式一般設定」頁面上， **[!UICONTROL Test&amp;Target伺服器名稱]** 欄位中填入您在步驟2複製的URL。
1. 選擇 **[!UICONTROL 關閉]**.
