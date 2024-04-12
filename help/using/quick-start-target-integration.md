---
title: 「快速入門：Adobe Target Standard/Premium整合」
description: Adobe Target Standard/Premium簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速啟動和執行Adobe Target Standard/Premium整合技術。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 7%

---

# 快速入門：Adobe Target Standard/Premium整合{#quick-start-target-integration}

Adobe Target Standard/Premium可讓行銷人員直接掌控，透過細分、目標定位和Automated Personalization快速並持續執行多個A/B和多變數測試、衡量效益並提高線上內容的關聯性。

Adobe Dynamic Media Classic可讓您建立Adobe Target Standard/Premium行銷活動的優惠方案和優惠方案集。 例如，您可以建立包含相同多媒體資產的三個變體的選件集。 接著，您可以讓Adobe Target Standard/Premium判斷哪個資產可提供較好的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。優惠方案集推送或儲存至Adobe Target Standard/Premium （優惠方案與mbox和體驗相關聯）後，Adobe Target Standard/Premium就可以執行行銷活動。 這些行銷活動會決定網站的哪些變數最適合點進和轉換。

若要進一步自訂動態Adobe Dynamic Media Classic內容，請使用Adobe Target Standard/PremiumHTML選件。 請參閱 [Adobe Target Standard/Premium產品檔案](https://experienceleague.adobe.com/en/docs/target) 以取得詳細資訊。

>[!NOTE]
>
>若要搭配使用Adobe Target Standard/Premium和Adobe Dynamic Media Classic，必須使用有效的Adobe Target Standard/Premium帳戶。

本快速入門旨在協助您快速上手Adobe Target Standard/PremiumHTML選件集。 依照步驟 1 至 3 執行。每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.在「應用程式一般設定」頁面中輸入您的Adobe Target Standard/Premium URL

Adobe Dynamic Media Classic需要您的Adobe Target Standard/Premium URL才能與Adobe Target Standard/Premium整合。 複製您的Adobe Target Standard/Premium URL部分，最多到並且包括 `.com`，並在Adobe Dynamic Media Classic中輸入 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組， **[!UICONTROL Test&amp;Target伺服器名稱]** 文字欄位。 另請參閱 [將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2.建立優惠方案集

使用參數化範本或影像來建立提案集。您可以在Test&amp;Target選件集頁面上建立HTML選件集。 若要開啟此頁面，請選取您的範本或影像，然後在全域導覽列上，前往 **[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**.

若要使用範本建立優惠方案，請選取 **[!UICONTROL 新增並預覽]**. 在新增和預覽頁面，變更引數值。

若要建立含有影像的選件，請將影像拖曳至Test&amp;Target選件集頁面。 選取 **[!UICONTROL 預覽]** 並為影像或選件集中的所有影像選擇影像預設集。

建立提案集後請將其儲存。

另請參閱 [建立優惠方案集](creating-offer-set.md#creating_an_offer_set).

## 3.將優惠方案集推送至Adobe Target Standard/Premium

在Test&amp;Target選件集頁面中，選取 **[!UICONTROL 推送優惠方案]**，並在Test&amp;Target登入對話方塊中輸入您的登入認證。 另請參閱 [將優惠方案集推送到Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
