---
title: Adobe Dynamic Media Classic平台概觀
seo-title: Adobe Dynamic Media Classic平台概觀
description: 'null'
seo-description: Dynamic Media Classic平台與工作流程程序概觀。
uuid: e7d3bfb3-1cfe-43ea-b862-ae3 b3928 c71
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ENSCENEXENDEMENDUMENT_ PK/categories/getting_ started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30 ae610 bb9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Adobe Dynamic Media Classic平台概觀{#adobe-scene-platform-overview}

Dynamic Media Classic是整合式、多媒體管理、發佈和服務環境。多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

## 工作流程程序 {#workflow-process}

主要Dynamic Media Classic工作流程步驟包括：

**上傳及管理您的資產** 將媒體資產上傳至SPS。您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。如果您安裝 Adobe Scene7 Publishing System 桌面應用程式，便可以將檔案和檔案夾從桌面拖曳至上載檔案夾，加以上載。

**建立豐富型媒體** 建立不同的資產設定，例如eCatalogs、影像集、回轉集、色票集、混合媒體集、基本範本和FXG範本。如需詳細資訊，請參閱關於多媒體。

**發佈和管理** 發佈資產至Dynamic Media Classic Saas網路，並在發佈資產時監視資產狀態、管理使用者權限並維護安全性。

**支援** 從Dynamic Media Classic SaaS網路傳送媒體至網頁、應用程式和行動裝置；媒體效能最佳化，並透過CDN快取提供。Dynamic Media Classic提供每個資產的URL。您發佈資產後，URL 便會生效。

![Dynamic Media Classic工作流程流程](/help/assets/gs_workflow.png)

## 單一主影像和單一 URL 呼叫 {#single-master-images-and-single-url-calls}

Dynamic Media Classic與其他系統根本不同，因為您可以使用Dynamic Media Classic從單一主資產和URL呼叫動態傳送媒體。

您使用Dynamic Media Classic產生的URL字串包含指示伺服器如何在傳送資產時顯示該資產的指示。例如，相同的主影像可以使用不同大小、格式、寬度、色彩和縮放檢視來傳送。透過動態媒體Classic來建立和發佈媒體資產，您可以視覺化方式設定效果。如此，您便建立了正確告知伺服器如何向應用程式呈現主資產的 URL 呼叫。

![Dynamic Media Classic可將相同的主影像傳送至不同尺寸和格式的不同媒體。](/help/assets/gs_dynamic_publishing.png)

## 內容快取 {#content-caching}

動態Media Classic動態產生的影像適合快取；在大多數情況下，它們是JPEG影像，具有識別它們的獨特URL呼叫。影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。使用任何CDN廠商實作快取機制時，只需變更伺服器名稱，指向啓用CDN的Dynamic Media Image Server。所有Dynamic Media Classic版本都包含搭售的CDN快取。
