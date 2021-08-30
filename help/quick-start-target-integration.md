---
title: 「快速入門：Adobe Target Standard/Premium整合」
description: Adobe Target Standard/Premium的簡介和快速入門，可協助您在Adobe Dynamic Media Classic中使用Adobe Target Standard/Premium整合技術快速上手並執行。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 10%

---

# 快速入門：Adobe Target Standard/Premium整合{#quick-start-target-integration}

Adobe Target Standard/Premium可讓行銷人員直接控制，以快速且持續執行多個A/B和多變數測試、評估成效，並透過細分、鎖定目標和Automated Personalization提高線上內容的相關性。

AdobeDynamic Media Classic可讓您建立Adobe Target Standard/Premium促銷活動的選件和選件集。 例如，您可以建立一個選件集，其中包含相同多媒體資產的三個變體。 接著，您可以讓Adobe Target Standard/Premium判斷哪個資產可提供更好的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。將選件集推送或儲存至Adobe Target Standard/Premium後（其中選件與mbox和體驗相關聯）,Adobe Target Standard/Premium便可執行促銷活動。 這些促銷活動會決定哪個網站的變異在點進次數和轉換中表現最佳。

若要進一步自訂動態AdobeDynamic Media Classic內容，請使用Adobe Target Standard/Premium HTML選件。 如需詳細資訊，請參閱[Adobe Target Standard/Premium產品檔案](https://experienceleague.adobe.com/docs/target.html)。

>[!NOTE]
>
>若要搭配使用Adobe Target Standard/Premium與Adobe Dynamic Media Classic，必須具備有效的Adobe Target Standard/Premium帳戶。

此快速入門功能可協助您快速上手並執行Adobe Target Standard/Premium HTML選件集。 依照步驟 1 至 3 執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

## 1.在「應用程式一般設定」頁面中輸入您的Adobe Target Standard/Premium URL

AdobeDynamic Media Classic需要您的Adobe Target Standard/Premium URL才能與Adobe Target Standard/Premium整合。 將您的Adobe Target Standard/Premium URL的部分複製到`.com`（含），然後在「AdobeDynamic Media Classic **[!UICONTROL 應用程式一般設定]**」頁面的「**[!UICONTROL 伺服器]**」群組的「**[!UICONTROL Test&amp;Target伺服器名稱]**」文字欄位中輸入。 請參閱[整合AdobeDynamic Media Classic與Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target)。

## 2.建立優惠方案集

使用參數化範本或影像來建立提案集。您可以在Test&amp;Target選件集頁面上建立HTML選件集。 若要開啟此頁面，請選取您的範本或影像，然後在全域導覽列上，前往&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target選件集]**。

若要使用範本建立選件，請選取&#x200B;**[!UICONTROL 新增並預覽]**。 在「新增和預覽」頁面上，變更參數值。

若要建立含有影像的選件，請將影像拖曳至Test&amp;Target選件集頁面。 選取&#x200B;**[!UICONTROL 預覽]**，然後為影像或選件集中的所有影像選擇影像預設集。

建立提案集後請將其儲存。

請參閱[建立選件集](creating-offer-set.md#creating_an_offer_set)。

## 3.推送選件集至Adobe Target Standard/Premium

在「Test&amp;Target選件集」頁面中，選取「**[!UICONTROL 推送選件]**」，然後在「Test&amp;Target登入」對話方塊中輸入您的登入憑證。 請參閱[將選件集推送至Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
