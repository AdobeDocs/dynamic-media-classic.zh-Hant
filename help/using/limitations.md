---
title: Dynamic Media限制
description: 瞭解建立影像集或迴轉集或上傳PDF時的最佳實務和強制限制。 另外還能瞭解不支援的Dynamic Media網頁瀏覽器和作業系統組合。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---

# Dynamic Media限制

以下各節說明Dynamic Media的限制。

本主題包含下列章節：

* [Dynamic Media對資產型別的最佳實務和強制執行限制](#best-practice-enforced-limits)
* [Dynamic Media不支援的網頁瀏覽器和作業系統組合](#unsupported-browser-os)

## Dynamic Media對資產型別的最佳實務和強制執行限制 {#best-practice-enforced-limits}

當您建立迴轉集或影像集，或上傳頁面擷取的PDF時，Adobe會建議下列最佳作法。 Adobe也會強制實行下列限制：

| 資產：限制型別 | 最佳實務 | 強加的限制 |
| --- | --- | --- |
| **影像**：每個影像的智慧型裁切數目 | 5 | 100 |
| **所有集合**：每個集合的重複資產數目 | 無重複專案 | 20‡ |
| **所有集合**：每個集合的資產數量上限 | 每組5至10個影像 | 1000 |
| **迴轉集**：每個2D集的列/欄數上限 | 每組12至18個影像 | 1000 |
| **PDF**：要考慮擷取之PDF的最大頁數 |  | 100 (適用於所有PDF) |

‡最佳實務是不要在一個集中有重複的資產。 單一資產的限製為20個重複專案。 如果您為該資產新增另一個重複專案（在該集合內），請求會傳回錯誤或忽略重複專案。

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Dynamic Media不支援的網頁瀏覽器和作業系統組合 {#unsupported-browser-os}

<!-- CQDOC-19433 -->

AdobeDynamic Media不支援下列網頁瀏覽器和作業系統組合。

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1更新
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9小牛隊
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## 終止支援Secure Socket Layer 2.0和3.0以及Transport Layer Security 1.0和1.1 {#tls}

<!-- CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) -->

自2024年4月30日起，Adobe Dynamic Media將停止支援下列專案：

* SSL （安全通訊端層） 2.0
* SSL 3.0
* TLS （傳輸層安全性） 1.0和1.1
* TLS 1.2中的下列弱加密：
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

