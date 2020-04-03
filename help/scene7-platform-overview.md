---
title: Adobe Dynamic Media Classic平台概觀
seo-title: Adobe Dynamic Media Classic平台概觀
description: 'null'
seo-description: Dynamic Media Classic平台和工作流程程式的概觀。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Adobe Dynamic Media Classic平台概觀{#adobe-scene-platform-overview}

Dynamic Media Classic是整合的多媒體管理、發佈和服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

## 工作流程程序 {#workflow-process}

Dynamic Media Classic工作流程的主要步驟為：

* **上傳及管理您的資產**&#x200B;將媒體資產上傳至SPS。 您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。如果您安裝 Adobe Scene7 Publishing System 桌面應用程式，便可以將檔案和檔案夾從桌面拖曳至上載檔案夾，加以上載。

* **建立豐富式媒**&#x200B;體建立不同的資產設定，例如eCatalog、影像集、回轉集、色票集、混合式媒體集、基本範本和FXG範本。 如需詳細資訊，請參閱關於多媒體。

* **發佈和管理** Publish資產至Dynamic Media Classic Saas網路，並在資產發佈時監控資產狀態、管理使用者權限並維護安全性。

* **提供**&#x200B;從Dynamic Media Classic SaaS網路將媒體發佈至網頁、應用程式和行動裝置；媒體已最佳化效能，並以CDN快取傳送。 Dynamic Media Classic提供每個資產的URL。 您發佈資產後，URL 便會生效。

![Dynamic Media Classic工作流程程式](/help/assets/gs_workflow.png)

## 單一主影像和單一 URL 呼叫 {#single-master-images-and-single-url-calls}

Dynamic Media Classic與其他系統有根本不同，因為您可以使用Dynamic Media Classic從單一主資產和URL呼叫動態傳送媒體。

您使用Dynamic Media Classic產生的URL字串包含指示，告訴伺服器在傳送資產時如何顯示資產。 例如，相同的主影像可以使用不同大小、格式、寬度、色彩和縮放檢視來傳送。在使用Dynamic Media Classic建立和發佈媒體素材時，您可以視覺化設定效果。 如此，您便建立了正確告知伺服器如何向應用程式呈現主資產的 URL 呼叫。

![Dynamic Media Classic可以針對不同大小和格式的不同媒體提供相同的主影像。](/help/assets/gs_dynamic_publishing.png)

## 內容快取 {#content-caching}

Dynamic Media Classic動態產生的影像可快取；在大多數情況下，它們是具有唯一URL呼叫的JPEG影像，可識別它們。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。當使用任何CDN廠商實作快取機制時，您只需變更伺服器名稱，以指向啟用CDN的動態媒體影像伺服器。 所有Dynamic Media Classic版本都包含搭售的CDN快取。
