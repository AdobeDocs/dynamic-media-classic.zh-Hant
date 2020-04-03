---
title: 「快速入門：Target Classic整合」
seo-title: 「快速入門：Target Classic整合」
description: 'null'
seo-description: Adobe Target Classic的簡介和快速入門，可協助您使用Target Classic整合技術快速上手使用。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 快速入門：Target Classic整合{#quick-start-target-classic-integration}

Adobe Target Classic將控制權直接交給行銷人員，以便快速且持續地執行多個A/B和多變數測試、評估效率，並透過細分、鎖定和自動化個人化提高線上內容的相關性。

Scene7 Publishing System可讓您建立Target Classic促銷活動的選件和選件集。 例如，您可以建立包含相同豐富型媒體資產三種變化的選件集。 然後，您可以讓Target Classic決定哪個資產可提供更佳的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。將選件集推送或儲存至Adobe Target Classic後，選件會與mbox和體驗產生關聯，Target Classic可以執行促銷活動，以判斷哪些網站變數對點進和轉換效果最佳。

若要進一步自訂動態Dynamic Media Classic內容，請使用Target Classic HTML選件。 如需詳細資訊，請參閱Target Classic產品檔案。

>[!NOTE]
>
>您必須有有效的Adobe Target Classic帳戶，才能搭配Scene7 Publishing System使用Target Classic。

**快速入門**

此快速入門旨在讓您快速啟動並執行Target Classic HTML選件集。 依照步驟 1 至 3 執行。每個步驟之後都有連接至某個主題標題的交戶參照，您可以在其中尋找更多資訊。

**1. Enter your Target Classic URL in the Application General Settings screen.**

Dynamic Media Classic需要您的Target Classic URL與Target Classic整合。 Copy the portion of your Target Classic URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. 請參 [閱整合Dynamic Media Classic與Target Classic](integrating-scene7-target-classic.md#integrating_scene7_with_target_classic)。

**2. 建立提案集**

使用參數化範本或影像來建立提案集。您可在Target Classic選件集螢幕上建立HTML選件集。 To open this screen, select your template or images, and click **Build** > **Target Classic Offer Set**.

若要建立含範本的選件，請按一下「新 **增與預覽」**。 在「新增與預覽」畫面上，變更參數值。

若要建立包含影像的選件，請將影像拖曳至Target Classic選件集畫面。 Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

建立提案集後請將其儲存。

請參閱[建立提案集](creating-offer-set.md#creating_an_offer_set)。

**3. Push the offer set to Target Classic**

In the Target Classic Offer Set screen, click **Push Offers**, and enter your login credentials in the Target Classic Login dialog box. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).
