---
title: 將優惠方案集推送到Adobe Target Standard/Premium
description: 瞭解如何從Adobe Dynamic Media Classic將優惠方案集推送到Adobe Target Standard/Premium。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# 將優惠方案集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

建立或編輯優惠方案集後，請依照下列步驟推送至Adobe Target Standard/Premium：

1. 在Test&amp;Target選件集畫面中，選取&#x200B;**[!UICONTROL 推送選件]**。
1. 輸入您的使用者端代碼和登入認證。
1. 選取&#x200B;**[!UICONTROL 登入]**。

在傳輸至Adobe Target Standard/Premium期間，前置詞`S7_`會自動附加至選件名稱的開頭。 前置詞是附加的，以確保您可以在Test&amp;Target選件清單中輕鬆找到Adobe Dynamic Media Classic選件。 例如，選件會顯示為`S7_<name of offer set>_<offer name>`。

Adobe Dynamic Media Classic深入探討Adobe Target Standard/Premium Widget選件。 您可以使用Widget選件在Adobe Target Standard/Premium上託管您自己的選件內容。 Widget選件類似於Adobe Target Standard/Premium託管的標準選件。 它們可讓Adobe Target Standard/Premium部署儲存在伺服器上的選件內容，允許更精細的動態使用。 Widget選件可從URL擷取內容、快取該內容，並提供約兩個小時的服務。 Widget提供一些動態內容產生功能，這是Adobe Target Standard/Preimium以外其他提供所沒有的功能。 如果提供選件的mbox包含`mboxProductID`和`mbox.offerId`等mbox引數，則會將`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL引數附加至要求的URL。 這些引數是由Widget選件URL提供的服務所使用，用來傳回Adobe Target Standard/Premium以外使用您mbox中的產品或訂單資訊的內容。 您也可以透過API存取Widget選件，以便以程式設計方式在Adobe Target Standard/Premium以外建立選件。
