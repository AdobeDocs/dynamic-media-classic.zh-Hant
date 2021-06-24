---
title: AdobeDynamic Media Classic方案概觀
description: Dynamic Media Classic計畫和工作流程程式的概觀。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: eb37440a2917094aae8f32e9337b4c187ec6c1c2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 30%

---

# AdobeDynamic Media Classic方案概觀{#adobe-scene-platform-overview}

Dynamic Media Classic是整合式多媒體管理、發佈和服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

## 工作流程程序 {#workflow-process}

Dynamic Media Classic工作流程的關鍵步驟為：

* **上傳和管理您的資產**  — 將您的媒體資產上傳至Dynamic Media Classic。您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。

* **建立豐富型媒體**  — 建立不同的資產設定，例如eCatalog、影像集、回轉集、色票集、混合型媒體集、基本範本和FXG範本。

* **發佈及管理**  — 將資產發佈至Dynamic Media Classic SaaS網路，以及監控資產發佈時的狀態、管理使用者權限，並維護安全性。

* **提供**  — 將媒體從Dynamic Media Classic SaaS網路傳送至網頁、應用程式和行動裝置；媒體已最佳化效能，並會透過CDN快取傳送。Dynamic Media Classic提供每個資產的URL。 您發佈資產後，URL 便會生效。

![Dynamic Media Classic工作流程程式](/help/assets/gs_workflow.png)

## 單一主影像和單一 URL 呼叫 {#single-master-images-and-single-url-calls}

Dynamic Media Classic與其他系統有根本不同，因為您可以使用Dynamic Media Classic，從單一主資產和URL呼叫以動態方式傳送媒體。

您透過Dynamic Media Classic產生的URL字串包含指示，告訴伺服器在傳送資產時如何顯示資產。 例如，相同的主影像可以使用不同大小、格式、寬度、色彩和縮放檢視來傳送。在使用Dynamic Media Classic建置和發佈媒體資產時，您可以透過視覺化方式設定效果。 如此，您便建立了正確告知伺服器如何向應用程式呈現主資產的 URL 呼叫。

![Dynamic Media Classic可以以不同大小和格式，將相同的主影像傳送至不同的媒體。](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic可確保將一致的品質體驗提供至任何畫面，不論其大小或頻寬為何。*

## 內容快取 {#content-caching}

Dynamic Media Classic動態產生的影像可快取；通常是具有唯一URL呼叫的JPEG影像，可識別它們。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。使用任何CDN廠商實作快取機制時，您只需變更伺服器名稱，指向啟用CDN的Dynamic Media影像伺服器。 所有Dynamic Media Classic版本都包含套裝的CDN快取。
