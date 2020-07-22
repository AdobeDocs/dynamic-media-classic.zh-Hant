---
title: 整合Adobe Dynamic Media Classic與Adobe Target Classic
seo-title: 整合Adobe Dynamic Media Classic與Adobe Target Classic
description: 'null'
seo-description: 瞭解如何整合Adobe Dynamic Media Classic與Adobe Target Classic。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
translation-type: tm+mt
source-git-commit: 044c4fd8dc06369b7ac6b5eb65014835d2b84fee
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 9%

---


# 整合Adobe Dynamic Media Classic與Adobe Target Classic{#integrating-adobe-scene-with-adobe-target-classic}

您必須先在Dynamic Media Classic應用程式的「一般設定」畫面中輸入Target Classic URL，才能將Dynamic Media Classic與Target Classic整合。 請依照下列步驟取得Target Classic URL，並在「應用程式一般設定」畫面中輸入：

1. 請前往下列位址的「Target Classic登入」頁面： https://admin.testandtarget.omniture.com。
1. 輸入您的認證，然後按一下「登 **入」**。
1. 登入後，在瀏覽器的位址列中，複製 URL 中直到 *.com*(含)的部分。

   For example, if the *fictional* URL (URLs paths always contain forward slashes, not back slashes as in this example) in the address bar is `https:\\www.mysite.com/categories/admin/home.do`, copy only this portion of the *fictional* URL: `https:\\www.mysite.com`.

   在步驟5中，您會將複製的URL部分貼入「動態媒體傳統應用程式一般設定」畫面。

1. 在Dynamic Media Classic中，按一下「 **設定** >應 **用程式設定**」。
1. 在「應用程式一般設定」頁面的「 **[!UICONTROL Test&amp;Target伺服器名稱」欄位中]** ，貼上您在步驟3中複製的URL。
1. 按一下 **關閉**。

