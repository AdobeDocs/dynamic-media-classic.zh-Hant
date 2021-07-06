---
title: 登入 Adobe Analytics
description: 了解如何登入Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 35%

---

# 登入 Adobe Analytics{#log-in-to-adobe-analytics}

登入以設定Adobe Analytics報表，並將Adobe Analytics報表變數與Dynamic Media Classic事件相符之前，請確認您是Adobe Analytics中「網站服務存取」群組的成員。 不論在介面中設定的權限為何，此群組的成員皆可經由 Marketing Cloud 的「網路服務 API」存取指定報告套件中的所有報告。若要在群組中增加成員，請在 Adobe Analytics 中按一下「**[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**」。

登入時，您可以選擇輸入Marketing Cloud組織ID以使用最新的視訊分析實作。 如果您選擇不輸入ID，視訊報表仍可運作。 但是，這可能會導致資料無法與來自Dynamic Media Classic外部該用戶端的其他資料正確整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已移轉至AdobeIMS型驗證(Identity Management系統)以登入，則無法輸入直接憑證。

**登入 Adobe Analytics:**

1. 在Dynamic Media Classic頁面的右上角附近，點選「**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**」。
1. 在左窗格的「**[!UICONTROL 應用程式設定]**」下，點選「**[!UICONTROL Adobe Analytics]**」。
1. 在Adobe Analytics設定頁面中，點選&#x200B;**[!UICONTROL Adobe Analytics登入]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics登入]**&#x200B;對話方塊的&#x200B;**[!UICONTROL 密碼]**&#x200B;文字欄位中，輸入您的公司名稱、Marketing Cloud組織ID（選用）、使用者名稱，以及&#x200B;*共用機密*&#x200B;金鑰。

   您可以從AnalyticsAdmin Console中擷取&#x200B;*共用機密*&#x200B;金鑰。 請參閱[如何取得使用者帳戶的API憑證](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md)。

1. 按一下&#x200B;**[!UICONTROL 「登入」]**。
1. 在&#x200B;**[!UICONTROL 報表套裝]**&#x200B;下拉式功能表中，選擇報表套裝，然後按一下&#x200B;**[!UICONTROL 確定]**。

   >[!NOTE]
   >
   >首次登入 Adobe Analytics 時，「報告套件」下拉式清單為空白。首次登入時無法選擇報告套件。首次登入後，請先登出，然後回到「Adobe Analytics」畫面。重新登入後即可選擇報告套件。

>[!MORELIKETHIS]
>
>* [設定 Adobe Analytics 報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

