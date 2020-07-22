---
title: 將選件集推送至Adobe Target Standard/Premium
seo-title: 將選件集推送至Adobe Target Standard/Premium
description: 'null'
seo-description: 瞭解如何將選件集推送至Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 10%

---


# 將選件集推送至Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

建立或編輯選件集後，請依照下列步驟將其推送至Target Standard/Premium:

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. 輸入您的用戶端代碼和登入認證。
1. 按一下&#x200B;**[!UICONTROL 「登入」]**。

在傳輸至Target Standard/Premium期間，首碼S7_會自動附加至選件名稱的開頭。 附加此首碼，以確保您能在Test&amp;Target選件清單中輕鬆找到Dynamic Media Classic選件。 例如，提案顯示為「S7_&lt;提案集名稱>_&lt;提案名稱>」。

Dynamic Media Classic推入Target Standard/Premium Widget選件。 您可以使用介面工具集選件，在Target Standard/Premium以外代管您自己的選件內容。 介面工具集選件類似於Target Standard/Premium以外代管的標準選件。 它們可讓Target Standard/Premium部署儲存在您伺服器上的選件內容，讓您更精密、更動態地使用。 介面工具集選件會擷取來自 URL 的內容、建立快取並提供大約兩個小時的內容。介面工具集選件提供一些動態內容產生功能，而Target Standard/Premium以外的其他選件則無法提供。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 這些參數可供介面工具集選件URL中的服務使用，以傳回Target Standard/Premium以外的內容，這些內容會使用您mbox中的產品或訂單資訊。 您也可透過API存取介面工具集選件，以程式設計方式在Target Standard/Premium以外建立選件。