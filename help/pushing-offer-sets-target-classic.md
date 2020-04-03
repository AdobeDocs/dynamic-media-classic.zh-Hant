---
title: 將選件集推送至Adobe Target Classic
seo-title: 將選件集推送至Adobe Target Classic
description: 'null'
seo-description: 瞭解如何將選件集推送至Adobe Target Classic。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 將選件集推送至Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

建立或編輯選件集後，請依照下列步驟將其推送至Target Classic:

1. 在「Target Classic選件集」畫面中，按一下「推播選件」按鈕。
1. 輸入登入憑證。
1. 按一下「登入」按鈕。

在傳輸至Target Classic期間，首碼S7_會自動附加至選件名稱的開頭。 附加此首碼，以確保您可在Target Classic選件清單中輕鬆找到Dynamic Media Classic選件。 例如，提案顯示為「S7_&lt;提案集名稱>_&lt;提案名稱>」。

SPS會推入Target Classic介面工具集選件。 您可以使用介面工具集選件，在Target Classic以外代管您自己的選件內容。 介面工具集選件類似於Target Classic以外代管的標準選件。 它們可讓Target Classic部署儲存在您伺服器上的選件內容，讓您更精密、更動態地使用。 介面工具集選件會擷取來自 URL 的內容、建立快取並提供大約兩個小時的內容。介面工具集選件提供一些動態內容產生功能，而Target Classic以外的其他選件則無法提供。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 這些參數可供介面工具集選件URL中的服務使用，以傳回使用您mbox中產品或訂單資訊的Target Classic以外的內容。 您也可透過API存取介面工具集選件，以程式設計方式在Target Classic外部建立選件。
