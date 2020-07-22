---
title: 「快速入門： Target Standard/Premium整合」
seo-title: 「快速入門： Target Standard/Premium整合」
description: 'null'
seo-description: Adobe Target Standard/Premium的簡介和快速入門，可協助您快速上手使用Target Standard/Premium整合技術。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 19%

---


# 快速入門： Target Standard/Premium整合{#quick-start-target-integration}

Adobe Target Standard/Premium將控制權直接交由行銷人員掌控，以快速且持續地執行多個A/B和多變數測試、評估效率，並透過細分、鎖定和自動化個人化提高線上內容的相關性。

Dynamic Media Classic可讓您建立Target Standard/Premium促銷活動的選件和選件集。 例如，您可以建立包含相同豐富型媒體資產三種變化的選件集。 然後，您可以讓Target Standard/Premium決定哪個資產提供更佳的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。將選件集推送或儲存至Adobe Target Standard/Premium後，Target Standard/Premium可執行促銷活動，以判斷哪一種網站變化對點進和轉換效果最佳。

若要進一步自訂動態Dynamic Media Classic內容，請使用Target Standard/Premium HTML選件。 如需詳細資訊，請參閱Target Standard/Premium產品檔案。

>[!NOTE]
>
>必須有有效的Adobe Target Standard/Premium帳戶，才能搭配Dynamic Media Classic使用Target Standard/Premium。

**快速入門**

此快速入門功能可讓您快速啟動並執行Target Standard/Premium HTML選件集。 依照步驟 1 至 3 執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

**1. Enter your Target Standard/Premium URL in the Application General Settings screen.**

Dynamic Media Classic需要您的Target Standard/Premium URL與Target Standard/Premium整合。 Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. 請參 [閱整合Dynamic Media Classic與Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target)。

**2. 建立提案集**

使用參數化範本或影像來建立提案集。請在「Test&amp;Target 提案集」畫面上建立 HTML 提案集。To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

若要建立含範本的選件，請按一下「新 **增與預覽」**。 在「新增與預覽」畫面上，變更參數值。

若要使用影像建立提案，請將影像拖入「Test&amp;Target 提案集」畫面。Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

建立提案集後請將其儲存。

請參閱[建立提案集](creating-offer-set.md#creating_an_offer_set)。

**3. 將選件集推送至Target Standard/Premium**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. 請參 [閱推送選件集至Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
