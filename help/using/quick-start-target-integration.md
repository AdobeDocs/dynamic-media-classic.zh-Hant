---
title: 快速入門：Adobe Target Standard/Premium整合
description: Adobe Target Standard/Premium簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速啟動和執行Adobe Target Standard/Premium整合技術。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T19:56:29.690Z'
TQID: 'https://experienceleague.adobe.com/urNoJw6SrzPpsfpoTtudKndZfJOmWsZKtBZ3Za4aE0I'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 0f0abef2ec6e1d0743eca66e59673547f70ad7b0
workflow-type: tm+mt
source-wordcount: 529
ht-degree: 1%

---

# 快速入門：Adobe Target Standard/Premium整合{#quick-start-target-integration}

Adobe Target Standard/Premium為行銷團隊提供管理控制權。 此功能可協助您快速持續執行多個A/B和多變數測試，並評估其成效。 此外，它也可以透過細分、目標定位和Automated Personalization增加線上內容的相關性。

Adobe Dynamic Media Classic可讓您建立Adobe Target Standard/Premium行銷活動的優惠方案和優惠方案集。 例如，您可以建立包含相同多媒體資產的三個變數的選件集。 接著，您可以讓Adobe Target Standard或Premium判斷哪個資產可提供較佳的轉換效能。 您可以從基本範本或個別影像建立優惠方案和優惠方案集。 優惠方案集推送或儲存至Adobe Target Standard/Premium （優惠方案與mbox和體驗相關聯）後，Adobe Target Standard/Premium就可以執行行銷活動。 這些行銷活動會決定網站的哪些變體最適合點進和轉換。

若要進一步自訂動態Adobe Dynamic Media Classic內容，請使用Adobe Target Standard/Premium HTML選件。 如需詳細資訊，請參閱[Adobe Target Standard/Premium產品檔案](https://experienceleague.adobe.com/en/docs/target)。

>[!NOTE]
>
>若要搭配使用Adobe Target Standard/Premium和Adobe Dynamic Media Classic，必須使用有效的Adobe Target Standard/Premium帳戶。

本指南旨在協助您快速開始使用Adobe Target Standard/Premium HTML Offer Set。 依照步驟 1 至 3 執行。 每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## &#x200B;1. 在「應用程式一般設定」頁面中輸入您的Adobe Target Standard/Premium URL

Adobe Dynamic Media Classic需要您的Adobe Target Standard/Premium URL才能與Adobe Target Standard/Premium整合。 將您的Adobe Target Standard/Premium URL部分複製到並包括`.com`，並在Adobe Dynamic Media Classic **[!UICONTROL 應用程式一般設定]**&#x200B;頁面上的&#x200B;**[!UICONTROL 伺服器]**&#x200B;群組內的&#x200B;**[!UICONTROL Test&amp;Target伺服器名稱]**&#x200B;文字欄位中輸入該部分。 請參閱[整合Adobe Dynamic Media Classic與Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target)。

## &#x200B;2. 建立優惠方案集

使用引數化範本或影像來建立選件集。 您可以在Test&amp;Target選件集頁面上建立HTML選件集。 若要開啟此頁面，請選取您的範本或影像，然後在全域導覽列上，移至&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**。

若要使用範本建立優惠方案，請選取&#x200B;**[!UICONTROL 新增並預覽]**。 在新增和預覽頁面，變更引數值。

若要建立含有影像的選件，請將影像拖曳至Test&amp;Target選件集頁面。 選取「**[!UICONTROL 預覽]**」並選擇影像的影像預設集，或選件集中的所有影像。

建立選件集後儲存選件集。

請參閱[建立優惠方案集](creating-offer-set.md#creating_an_offer_set)。

## &#x200B;3. 將優惠方案集推送到Adobe Target Standard/Premium

在Test&amp;Target選件集頁面中，選取&#x200B;**[!UICONTROL 推送選件]**，然後在Test&amp;Target登入對話方塊中輸入您的登入認證。 請參閱[將選件集推送至Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
