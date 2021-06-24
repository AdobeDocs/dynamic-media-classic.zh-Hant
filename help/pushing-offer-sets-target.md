---
title: 推送優惠方案集至Adobe Target Standard/Premium
description: 了解如何將選件集推送至Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 6%

---

# 推送優惠方案集至Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

建立或編輯優惠方案集後，請依照下列步驟將其推送至Adobe Target Standard/Premium:

1. 在「Test&amp;Target選件集」畫面中，按一下「**[!UICONTROL 推播選件]**」。
1. 輸入您的用戶端代碼和登入憑證。
1. 按一下&#x200B;**[!UICONTROL 「登入」]**。

在傳輸至Adobe Target Standard/Premium期間，首碼`S7_`會自動附加至優惠方案名稱的開頭。 此首碼的附加目的，是確保您可以輕鬆在Test&amp;Target選件清單中找到Dynamic Media Classic選件。 例如，選件會顯示為`S7_<name of offer set>_<offer name>`。

Dynamic Media Classic推播至Adobe Target Standard/Premium Widget選件。 您可以使用介面工具集選件，在Adobe Target Standard/Premium以外托管您自己的選件內容。 介面工具集選件類似於在Adobe Target Standard/Premium以外托管的標準選件。 它們可讓Adobe Target Standard/Premium部署儲存在伺服器上的選件內容，以提供更複雜且動態的使用方式。 介面工具集選件會擷取來自 URL 的內容、建立快取並提供大約兩個小時的內容。介面工具集選件提供一些動態內容產生功能，但Adobe Target Standard/Premium以外的其他選件則不提供。 如果提供選件的mbox包含mbox參數，例如`mboxProductID`和`mbox.offerId`，則`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL參數會附加至請求的URL。 這些參數可供介面工具集選件URL上可用的服務使用，以在Adobe Target Standard/Premium以外傳回內容，這些內容會使用mbox的產品或訂單資訊。 您也可透過API存取介面工具集選件，以程式設計方式在Adobe Target Standard/Premium以外建立選件。
