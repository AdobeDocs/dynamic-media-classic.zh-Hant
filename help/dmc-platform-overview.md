---
title: Adobe Dynamic Media Classic項目概述
description: Adobe Dynamic Media Classic方案及其整個工作流程概述。
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

# Adobe Dynamic Media Classic項目概述{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是一個整合的富媒體管理、出版和服務環境。 多媒體可以傳送至所有行銷和銷售管道，包含網路、列印資料、電子郵件行銷活動、入口網站、桌上型電腦和裝置。

另請參閱 [平台概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 培訓視頻。

## 工作流程程序 {#workflow-process}

Adobe Dynamic Media Classic工作流的關鍵步驟是：

* **上載和管理您的資產**  — 將媒體資產上傳到Adobe Dynamic Media Classic。 您可以在系統上組織、瀏覽和搜尋資產。您也可以將中繼資料套用至資產。

* **建立富媒體**  — 建立不同的資產配置，如eCatalog 、影像集、旋轉集、色板集、混合媒體集、基本模板和FXG模板。

* **發佈和管理**  — 將資產發佈到Adobe Dynamic Media ClassicSaaS網路。 監視資產發佈時的狀態。 管理用戶權限並維護安全性。

* **服務**  — 將媒體從Adobe Dynamic Media ClassicSaaS網路傳輸到網頁、應用程式和移動設備；該媒體經過效能優化，並通過CDN快取提供。 Adobe Dynamic Media Classic為您提供每個資產的URL。 您發佈資產後，URL 便會生效。

![Adobe Dynamic Media Classic工作流進程](/help/assets/gs_workflow.png)

## 單個主映像和單個URL調用 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic與其他系統有根本不同，因為您可以使用Adobe Dynamic Media Classic從單個主資產和URL呼叫動態傳送媒體。

您使用Adobe Dynamic Media Classic生成的URL字串包含說明，說明在交付資產時如何顯示資產。 例如，可以以不同大小、格式、權重、顏色和縮放視圖提供相同的主影像。 作為與Adobe Dynamic Media Classic一起構建和發佈媒體資產的一部分，您可以直觀地配置效果。 在執行此操作時，您將建立URL調用，以正確指示伺服器如何向應用程式顯示主資產。

![Adobe Dynamic Media Classic可以將同一主映像以不同大小和格式傳輸到不同介質。](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic確保將一致的高質量體驗提供到任何螢幕，而不管其大小或頻寬如何。*

## 內容快取 {#content-caching}

Adobe Dynamic Media Classic動態生成的影像對快取有利；通常，它們是JPEG影像，具有標識它們的唯一URL調用。 影像會在內容傳遞網路 (CDN) 上傳送；CDN 是一種伺服器系統，會在網際網路上互相連結以更快傳送內容。影像會從全域各處的伺服器分發至電腦。使用任何CDN供應商實施快取機制時，您只需更改伺服器名稱以指向啟用CDN的Dynamic Media映像伺服器。 所有Adobe Dynamic Media Classic版本都包括捆綁的CDN快取。
