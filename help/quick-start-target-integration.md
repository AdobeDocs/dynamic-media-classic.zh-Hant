---
title: 「快速入門：Adobe Target標準版／高級版整合」
description: Adobe Target標準版／高級版的簡介和快速入門，可協助您使用Adobe Target標準版／高級版整合技術快速上手使用。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media經典
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 11%

---

# 快速入門：Adobe Target標準版／高級版整合{#quick-start-target-integration}

Adobe Target標準版/Premium將控制權直接交給行銷人員，以快速且持續地執行多個A/B和多變數測試，衡量成效，並透過細分、鎖定和自動化個人化提高線上內容的相關性。

Dynamic Media經典可讓您建立Adobe Target標準版／高級版促銷活動的選件和選件集。 例如，您可以建立包含相同豐富型媒體資產三種變化的選件集。 然後，您就可以讓Adobe Target標準版／高級版決定哪個資產提供更佳的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。將選件集推送或儲存至Adobe Target標準版／高級版（其中選件與mbox和體驗相關聯）後，Adobe Target標準版／高級版可以執行促銷活動。 這些促銷活動會決定哪些網站變數對點進次數和轉換效果最佳。

若要進一步自訂動態Dynamic Media經典內容，請使用Adobe Target標準版／優質HTML選件。 如需詳細資訊，請參閱[Adobe Target標準版／高級版產品檔案](https://experienceleague.adobe.com/docs/target.html)。

>[!NOTE]
>
>必須有有效的Adobe Target標準版／高級版帳戶才能搭配使用Adobe Target標準版／高級版與Dynamic Media經典版。

此快速入門功能可讓您快速上手使用Adobe Target標準版／高級版HTML選件集。 依照步驟 1 至 3 執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

## 1.在「應用程式一般設定」頁面中輸入您的Adobe Target標準版／高級版URL

Dynamic MediaClassic需要您的Adobe TargetStandard/Premium URL與Adobe TargetStandard/Premium整合。 將您的Adobe Target標準／高級URL的部分複製到`.com`（包括&#x200B;**[!UICONTROL ），然後在**[!UICONTROL &#x200B;伺服器&#x200B;]**組**[!UICONTROL  Test&amp;Target伺服器名稱&#x200B;]**文本欄位中的「Dynamic Media標準／高級URL」頁中輸入。]**&#x200B;請參閱[整合Dynamic Media經典與Adobe Target標準版／高級版](integrating-dmc-with-target.md#integrating-dmc-with-target)。

## 2.建立選件集

使用參數化範本或影像來建立提案集。您可在Test&amp;Target的「選件集」頁面上建立HTML選件集。 若要開啟此頁面，請選取範本或影像，然後在全域導覽列上，按一下「建置&#x200B;**[!UICONTROL > >**[!UICONTROL  Test&amp;Target選件集&#x200B;]**」。]**

若要建立含範本的選件，請按一下「新增與預覽」。 ****&#x200B;在「新增與預覽」頁面上，變更參數值。

若要建立包含影像的選件，請將影像拖曳至「Test&amp;Target選件集」頁面。 按一下「預覽」，然後為影像或選件集中的所有影像選擇影像預設集。****

建立提案集後請將其儲存。

請參閱[建立提案集](creating-offer-set.md#creating_an_offer_set)。

## 3.將選件推送至Adobe Target標準版／高級版

在「Test&amp;Target選件集」頁面中，按一下「推送選件&#x200B;]**」，然後在「Test&amp;Target登入」對話方塊中輸入您的登入認證。**[!UICONTROL &#x200B;請參閱[將選件集推送至Adobe Target標準版／高級版](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
