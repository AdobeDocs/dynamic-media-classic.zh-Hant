---
title: 向Adobe Target標準/高級版推送優惠
description: 瞭解如何向Adobe Target標準/高級版推出優惠套件。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 向Adobe Target標準/高級版推送優惠 {#pushing-offer-sets-to-target}

建立或編輯聘用集後，按以下步驟將其推送至Adobe Target標準/高級版：

1. 在「Test和目標優惠集」螢幕中，選擇 **[!UICONTROL 推送服務]**。
1. 輸入您的客戶端代碼和登錄憑據。
1. 選擇 **[!UICONTROL 登錄]**。

在傳輸到Adobe Target標準/高級版時，前置詞 `S7_` 自動附加到優惠名稱的開始。 附加此前置詞是為了確保您可以在「Test和目標」優惠清單中輕鬆找到Adobe Dynamic Media Classic優惠。 例如，此優惠顯示為 `S7_<name of offer set>_<offer name>`。

Adobe Dynamic Media Classic推出Adobe Target標準/高級小部件產品。 您可以使用Widget產品在Adobe Target標準/高級版之外托管您自己的產品內容。 Widget產品與托管在Adobe Target標準/優先版之外的標準產品類似。 它們允許Adobe Target標準/高級版部署儲存在您伺服器上的內容，從而實現更複雜和動態的使用。 Widget提供的內容可以從URL中檢索內容，快取並服務該內容大約兩個小時。 Widget提供的功能提供了一些動態內容生成功能，而Adobe Target標準版/Preimium之外的其他功能則不提供。 如果提供服務的mbox包含mbox參數，如 `mboxProductID` 和 `mbox.offerId`，也請參見Wiki頁。 `productId=[PRODUCT_ID]`和 `offerID=[OFFERID]` URL參數將附加到請求的URL。 這些參數可由小部件提供URL上的可用服務使用，以返回使用您框中的產品或訂單資訊的Adobe Target標準/高級版以外的內容。 Widget產品還可通過API以寫程式方式在Adobe Target標準/高級版之外建立產品。
