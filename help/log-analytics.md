---
title: 登入 Adobe Analytics
description: 了解如何從AdobeDynamic Media Classic登入Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 9ae252ab0e62696360c7ee487f9b26d722c603a1
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 1%

---

# 登入 Adobe Analytics{#log-in-to-adobe-analytics}

登入以設定Adobe Analytics報表，並比對Adobe Analytics報表變數以AdobeDynamic Media Classic事件之前，請確認您是Adobe Analytics中「網站服務存取」群組的成員。 不論介面中設定的權限為何，此群組中的成員都可透過Experience Cloud的網站服務API存取指定報表套裝中的所有報表。 若要將成員新增至群組，請在Adobe Analytics中前往&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**。

登入時，您可以選擇輸入Experience Cloud組織ID以使用最新的視訊分析實作。 如果您選擇不輸入ID，視訊報表仍可運作。 但是，這可能會導致資料無法與該用戶端的其他資料從外部AdobeDynamic Media Classic正確整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已移轉至Adobe IMS型驗證(Identity Management系統)登入，則無法輸入直接憑證。

**若要從AdobeDynamic Media Classic登入Adobe Analytics:**

首先，整合Dynamic Media Classic與Adobe Analytics OAuth。 Adobe Analytics OAuth與Dynamic Media Classic的整合通常只對每位使用者執行一次。

1. 訪問[Adobe開發人員控制台](https://developer.adobe.com/console)。 確認您的帳戶擁有需要整合之組織的管理員權限。
1. 在首頁的右上角附近，從下拉式清單中選取適當的公司。 (下方螢幕截圖僅供參考；您選擇的實際公司名稱可能有所不同)。

   ![建立新專案](assets/analytics-oauth1.png)

1. 執行下列任一操作：

   * 在頁面頂部，從&#x200B;**[!UICONTROL Home]**&#x200B;頁簽中，選擇&#x200B;**[!UICONTROL 建立新項目]**。
   * 在頁面頂端，從&#x200B;**[!UICONTROL Projects]**&#x200B;標籤。 在頁面的右角附近，選擇&#x200B;**[!UICONTROL 建立新項目]**。

1. 在專案的頁面上，選取&#x200B;**[!UICONTROL 新增API]**。
1. 在&#x200B;**[!UICONTROL 新增API]**&#x200B;頁面上，選取&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在頁面的右下角附近，選擇&#x200B;**[!UICONTROL Next]**。

   ![新增API](assets/analytics-oauth2.png)

1. 在&#x200B;**[!UICONTROL 設定API]**&#x200B;頁面上，選取&#x200B;**[!UICONTROL 使用者驗證OAuth]**。
1. 在頁面的右下角附近，選擇&#x200B;**[!UICONTROL Next]**。
1. 在&#x200B;**[!UICONTROL 設定API]**&#x200B;頁面上，選取&#x200B;**[!UICONTROL OAUTH 2.0 Web]**。
1. 在&#x200B;**[!UICONTROL 預設重定向URI]**&#x200B;文本欄位中，準確輸入以下路徑，如所示：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在&#x200B;**[!UICONTROL 重定向URI模式]**&#x200B;文本欄位中，準確輸入以下路徑，如所示：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在頁面的右下角，選取「**[!UICONTROL 儲存已設定的API]**」。
1. 在導覽面板中，在Adobe Analytics頁面左側的&#x200B;**[!UICONTROL Credentials]**&#x200B;下，選取&#x200B;**[!UICONTROL OAuth Web]**。
1. 在&#x200B;**[!UICONTROL 憑據詳細資訊]**&#x200B;下，執行以下操作：
   * 在&#x200B;**[!UICONTROL 客戶端ID]**&#x200B;下，選擇&#x200B;**[!UICONTROL 複製]**&#x200B;以複製值。 您需要此值，才能在後續的Dynamic Media Classic案頭應用程式中設定後續的Analytics。
   * 在「**[!UICONTROL 客戶機密碼]**」下，選擇「**[!UICONTROL 檢索客戶機密碼]**」以顯示關聯值。 選擇&#x200B;**[!UICONTROL 複製]**&#x200B;以複製值。 在後續的Dynamic Media Classic案頭應用程式中，您需要此值才能完成後續的Adobe Analytics設定。

**在Dynamic Media Classic案頭應用程式中設定Adobe Analytics**

>[!NOTE]
>
>在Dynamic Media Classic中初始設定Adobe Analytics後，您只有在下列情況下才能重做設定：
>
>* Analytics中會新增一個報表，且使用者想要開始傳送資料至該新報表。
>* 追蹤伺服器已在Adobe Analytics中更新。
>* 報表中推出了新的追蹤變數，而您想要將Dynamic Media Classic使用者介面中的特定檢視器變數連結至該新的Analytics變數。

>


1. 在AdobeDynamic Media Classic案頭應用程式的右上角附近，轉至&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**。
1. 在左側面板的&#x200B;**[!UICONTROL Application Setup]**&#x200B;下，選擇&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics設定]**&#x200B;頁面上，選取&#x200B;**[!UICONTROL Adobe Analytics登入]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics登入]**&#x200B;對話方塊中，在&#x200B;**[!UICONTROL CLIENT ID]**&#x200B;欄位和&#x200B;**[!UICONTROL CLIENT SECRET]**&#x200B;欄位中，貼上您先前複製的個別值。
1. 在對話方塊的右下角，選取「登入」並執行您的Adobe IMS(Identity Management服務)登入。

   成功登入時，「Adobe Analytics登入」對話方塊會再次顯示，同時顯示&#x200B;**[!UICONTROL COMPANYS]**&#x200B;下拉式清單，由您可用的公司啟動。

1. 從&#x200B;**[!UICONTROL 公司]**&#x200B;下拉式清單中，選擇公司。

   選取公司後，由所選公司可用的報表套裝啟動的&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉式清單就會顯示。

1. 從&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉式清單中，選擇報表套裝。

   >[!NOTE]
   >
   >依預設，使用者必須注意以下事實： **[!UICONTROL COMPANIES]**&#x200B;和&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉式清單均空白。 因此，使用者必須從每個清單中選取值。—>

1. 選擇&#x200B;**[!UICONTROL OK]**&#x200B;以便保存配置。
1. 在「Adobe Analytics設定」頁面的左下角，選取&#x200B;**[!UICONTROL Save]** ，以確保Adobe Analytics帳戶設定已更新。

>[!MORELIKETHIS]
>
>* [設定Adobe Analytics報表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

