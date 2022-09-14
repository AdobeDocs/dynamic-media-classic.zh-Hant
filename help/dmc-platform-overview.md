---
title: Adobe Dynamic Media Classic方案概觀
description: 概述Adobe Dynamic Media Classic計畫及其整個工作流程程式。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 17%

---

# Adobe Dynamic Media Classic方案概觀{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是整合式多媒體管理、發佈和服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

另請參閱 [平台概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 訓練影片。

## 工作流程程序 {#workflow-process}

Adobe Dynamic Media Classic工作流程的關鍵步驟為：

* **上傳和管理您的資產**  — 上傳您的媒體資產至Adobe Dynamic Media Classic。 您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。

* **建立多媒體**  — 為資產建立不同的設定，例如eCatalog、影像集、回轉集、色票集、混合媒體集、基本範本和FXG範本。

* **發佈與管理**  — 將資產發佈至Adobe Dynamic Media Classic SaaS網路。 在資產發佈時監控其狀態。 管理使用者權限並維護安全性。

* **提供**  — 將媒體從Adobe Dynamic Media Classic SaaS網路傳送至網頁、應用程式和行動裝置；媒體已最佳化效能，並會透過CDN快取傳送。 Adobe Dynamic Media Classic提供每個資產的URL。 您發佈資產後，URL 便會生效。

![Adobe Dynamic Media Classic工作流程程式](/help/assets/gs_workflow.png)

## 單一主要影像和單一URL呼叫 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic與其他系統有根本不同，因為您可以使用Adobe Dynamic Media Classic從單一主要資產和URL呼叫以動態方式傳送媒體。

您透過Adobe Dynamic Media Classic產生的URL字串包含指示，告訴伺服器在傳送資產時如何顯示資產。 例如，相同的主影像可以以不同的大小、格式、粗細、顏色和縮放視圖來傳送。 透過Adobe Dynamic Media Classic建立和發佈媒體資產時，您可以透過視覺化方式設定效果。 如此一來，您就能建立URL呼叫，正確告知伺服器如何將主要資產呈現給應用程式。

![Adobe Dynamic Media Classic可以以不同大小和格式，將相同的主影像傳送至不同的媒體。](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic可確保將一致的品質體驗提供至任何畫面，不論其大小或頻寬為何。*

## 內容快取 {#content-caching}

Adobe Dynamic Media Classic動態產生的影像有利於快取；通常是JPEG影像，其URL呼叫不重複，可識別影像。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。使用任何CDN廠商實作快取機制時，您只需變更伺服器名稱，指向啟用CDN的Dynamic Media影像伺服器。 所有Adobe Dynamic Media Classic版本都包含套件式CDN快取。
