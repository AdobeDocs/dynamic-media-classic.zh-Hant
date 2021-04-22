---
title: AdobeDynamic Media經典平台概觀
description: Dynamic Media經典平台與工作流程流程的概觀。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media經典
role: Administrator,Business Practitioner
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 31%

---

# AdobeDynamic Media經典平台概觀{#adobe-scene-platform-overview}

Dynamic Media經典是整合的豐富式媒體管理、出版與服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

## 工作流程程序 {#workflow-process}

關鍵的Dynamic Media經典工作流程步驟包括：

* **上傳及管理您的資產** -將您的媒體資產上傳至Dynamic Media經典。您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。

* **建立豐富式媒體** -建立不同的資產設定，例如eCatalog、影像集、回轉集、色票集、混合式媒體集、基本範本和FXG範本。

* **發佈和管理** -將資產發佈到Dynamic MediaClassic SaaS網路，並在資產發佈時監控資產狀態、管理用戶權限並維護安全。

* **服務** -將媒體從Dynamic MediaClassic SaaS網路傳送至網頁、應用程式和行動裝置；媒體已最佳化效能，並以CDN快取傳送。Dynamic Media經典為您提供每個資產的URL。 您發佈資產後，URL 便會生效。

![Dynamic Media經典工作流程程式](/help/assets/gs_workflow.png)

## 單一主影像和單一 URL 呼叫 {#single-master-images-and-single-url-calls}

Dynamic Media經典與其他系統有本質的不同，因為您可以使用Dynamic Media經典從單一主資產和URL呼叫動態傳送媒體。

您使用Dynamic MediaClassic產生的URL字串包含指示，告訴伺服器在傳送資產時如何顯示資產。 例如，相同的主影像可以使用不同大小、格式、寬度、色彩和縮放檢視來傳送。在使用Dynamic Media經典建立和發佈媒體素材時，您可以視覺化設定效果。 如此，您便建立了正確告知伺服器如何向應用程式呈現主資產的 URL 呼叫。

![Dynamic Media經典可以針對不同尺寸和格式的不同媒體提供相同的主影像。](/help/assets/gs_dynamic_publishing.png)

## 內容快取 {#content-caching}

Dynamic Media經典動態產生的影像對快取友好；通常是具有唯一URL呼叫的JPEG影像，可識別它們。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。當使用任何CDN廠商實作快取機制時，您只需變更伺服器名稱，以指向啟用CDN的Dynamic Media影像伺服器。 所有Dynamic MediaClassic版本都包含搭售的CDN快取。
