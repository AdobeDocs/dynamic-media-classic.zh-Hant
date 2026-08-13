---
title: 將提案集推送到Adobe Target Standard/Premium
description: 瞭解如何從Adobe Dynamic Media Classic將優惠方案集推送到Adobe Target Standard/Premium。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 8a9d304ced3a218ae6393961a278f5ab9581c229
workflow-type: tm+mt
source-wordcount: 283
ht-degree: 0%

---

# 將優惠方案集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

建立或編輯優惠方案集後，請依照下列步驟推送至Adobe Target Standard/Premium：

1. 在Test &amp; Target選件集畫面中，選取&#x200B;**[!UICONTROL 推送選件]**。
1. 輸入您的使用者端代碼和登入認證。
1. 選取&#x200B;**[!UICONTROL 登入]**。

在傳輸至Adobe Target Standard/Premium期間，前置詞`S7_`會自動新增至選件名稱的開頭。 前置詞已新增，以確保您可以在Test &amp; Target選件清單中輕鬆找到Adobe Dynamic Media Classic選件。 例如，選件會顯示為`S7_<name of offer set>_<offer name>`。

Adobe Dynamic Media Classic將Widget選件推送至Adobe Target Standard/Premium。 您可以使用Widget選件在Adobe Target Standard/Premium上託管所提供的內容。 Widget選件可與Adobe Target Standard/Premium託管的標準選件比較。 它們可讓Adobe Target Standard/Premium部署儲存在伺服器上的選件內容，實現更精細的動態使用。 Widget可讓您從URL擷取內容、快取該內容並提供兩小時的服務。 Widget提供一些動態內容產生功能，這是Adobe Target Standard/Premium外部的其他服務所沒有的。 如果提供選件的mbox包含mbox引數（例如`mboxProductID`和`mbox.offerId`），則會將`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL引數附加至要求的URL。 Widget選件URL提供的服務會使用這些引數，傳回Adobe Target Standard/Premium以外的內容（這些內容使用mbox中的產品或訂單資訊）。 您也可以透過API存取Widget選件，以便以程式設計方式在Adobe Target Standard/Premium以外建立選件。
