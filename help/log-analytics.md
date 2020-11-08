---
title: 登入 Adobe Analytics
seo-title: 登入 Adobe Analytics
description: 'null'
seo-description: 瞭解如何登入Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 36%

---


# 登入 Adobe Analytics{#log-in-to-adobe-analytics}

在您登入以設定Adobe Analytics報表並將Adobe Analytics報表變數與Dynamic Media Classic事件相符之前，請確認您已新增為Adobe Analytics中「網站服務存取」群組的成員。 不論在介面中設定的權限為何，此群組的成員皆可經由 Marketing Cloud 的「網路服務 API」存取指定報告套件中的所有報告。若要在群組中增加成員，請在 Adobe Analytics 中按一下「**管理工具** > **使用者管理** > **編輯群組**」。

當您登入時，可以選擇輸入Marketing Cloud組織ID以使用最新的視訊分析實作。 如果您選擇不輸入ID，視訊報表仍然有效。 但是，這會導致資料無法與來自Dynamic Media Classic外部該用戶端的其他資料正確整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已移轉至Adobe IMS型驗證（身分管理系統）進行登入，則無法輸入直接認證。

**登入 Adobe Analytics**

1. 在「Dynamic Media Classic」（動態媒體經典）頁面的右上角附近，點選「 **[!UICONTROL 設定>應用程式設定」]**。
1. In the left pane, under **[!UICONTROL Application Setup]**, tap **[!UICONTROL Adobe Analytics]**.
1. In the Adobe Analytics Configuration page, tap **[!UICONTROL Adobe Analytics Login]**.
1. 在「 **[!UICONTROL Adobe Analytics登入]** 」對話方塊中，在「密碼」文字欄位中輸入您的公司名稱、Marketing Cloud組織ID（可選）、使用者名稱 *和共用的機密金鑰***** 。

   您可以從「分析管 *理員* 」控制台擷取共用的機密金鑰。 請參 [閱如何取得使用者帳戶的API認證](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html)。

1. 按一下&#x200B;**[!UICONTROL 「登入」]**。
1. 在「報 **[!UICONTROL 表套裝]** 」下拉式功能表中，選擇報表套裝，然後按一下「 **[!UICONTROL 確定」]**。

   >[!NOTE]
   >
   >首次登入 Adobe Analytics 時，「報告套件」下拉式清單為空白。首次登入時無法選擇報告套件。首次登入後，請先登出，然後回到「Adobe Analytics」畫面。重新登入後即可選擇報告套件。

>[!MORELIKETHIS]
>
>* [設定 Adobe Analytics 報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

