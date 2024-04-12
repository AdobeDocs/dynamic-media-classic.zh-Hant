---
title: Adobe Dynamic Media Classic計畫總覽
description: 概述Adobe Dynamic Media Classic程式及其整個工作流程。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 17%

---

# Adobe Dynamic Media Classic計畫總覽{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是一個整合式多媒體管理、發佈和服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

另請參閱 [平台概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 訓練影片。

## 工作流程程序 {#workflow-process}

Adobe Dynamic Media Classic工作流程的關鍵步驟為：

* **上傳和管理您的資產**  — 將您的媒體資產上傳至Adobe Dynamic Media Classic。 您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。

* **建立多媒體**  — 建立資產的不同設定，例如eCatalog、影像集、迴轉集、色票集、混合媒體集、基本範本和FXG範本。

* **發佈和管理**  — 將資產發佈至Adobe Dynamic Media Classic SaaS網路。 在資產發佈時監視資產的狀態。 管理使用者許可權並維護安全性。

* **服務**  — 從Adobe Dynamic Media Classic SaaS網路傳送媒體至網頁、應用程式和行動裝置；媒體會最佳化效能，並透過CDN快取傳送。 Adobe Dynamic Media Classic會提供您每個資產的URL。 您發佈資產後，URL 便會生效。

![Adobe Dynamic Media Classic工作流程程式](/help/using/assets/gs_workflow.png)

## 單一主要影像和單一URL呼叫 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic與其他系統截然不同，因為您可以使用Adobe Dynamic Media Classic以動態方式從單一主要資產和URL呼叫傳送媒體。

您透過Adobe Dynamic Media Classic產生的URL字串包含指示，告知伺服器如何在傳送資產時顯示資產。 例如，相同的主要影像可以不同大小、格式、重量、顏色和縮放檢視提供。 使用Adobe Dynamic Media Classic建置和發佈媒體資產時，您可以透過視覺化方式設定效果。 這樣做時，您會建立URL呼叫，正確地告知伺服器如何將您的主要資產呈現給應用程式。

![Adobe Dynamic Media Classic可將相同的主要影像傳送至不同大小和格式的不同媒體。](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic可確保在任何熒幕都能提供一致的品質體驗，無論熒幕大小或頻寬為何。*

## 內容快取 {#content-caching}

Adobe Dynamic Media Classic動態產生的影像有利於快取；通常，它們是JPEG影像，具有可識別它們的唯一URL呼叫。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。使用任何CDN廠商實作快取機制時，只需將伺服器名稱變更為指向啟用CDN的Dynamic Media Image Server即可。 所有Adobe Dynamic Media Classic版本都包含套件式CDN快取。
