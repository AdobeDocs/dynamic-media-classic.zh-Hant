---
title: 登入 Adobe Analytics
description: 了解如何從Adobe Dynamic Media Classic登入Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 8111895ac527b92b152382ea80b7b383659f00a9
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# 登入 Adobe Analytics{#log-in-to-adobe-analytics}

登入以設定Adobe Analytics報表，並將Adobe Analytics報表變數與Adobe Dynamic Media Classic事件相符之前，請確認您是Adobe Analytics中「網站服務存取」群組的成員。 不論介面中設定的權限為何，此群組中的成員都可透過Experience Cloud的網站服務API存取指定報表套裝中的所有報表。 要向組添加成員，請在Adobe Analytics中，轉到 **[!UICONTROL 管理工具]** > **[!UICONTROL 使用者管理]** > **[!UICONTROL 編輯群組]**.

登入時，您可以選擇輸入Experience Cloud組織ID以使用最新的視訊分析實作。 如果您選擇不輸入ID，視訊報表仍可運作。 但是，這可能會導致資料無法正確與來自Adobe Dynamic Media Classic以外之該用戶端的其他資料整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已移轉至Adobe IMS型驗證(Identity Management系統)登入，則無法輸入直接憑證。

## 從Adobe Dynamic Media Classic登入Adobe Analytics {#log-in-to-analytics-from-dmc}

首先，整合Dynamic Media Classic與Adobe Analytics OAuth。 Adobe Analytics OAuth與Dynamic Media Classic的整合通常只對每位使用者執行一次。

1. 存取 [Adobe開發人員控制台](https://developer.adobe.com/console). 確認您的帳戶擁有需要整合之組織的管理員權限。
1. 在首頁的右上角附近，從下拉式清單中選取適當的公司。 (下方螢幕截圖僅供參考；您選擇的實際公司名稱可能有所不同)。

   ![建立新專案](assets/analytics-oauth1.png)

1. 執行下列任一操作：

   * 在頁面頂端，從 **[!UICONTROL 首頁]** 索引標籤，選取 **[!UICONTROL 建立新專案]**.
   * 在頁面頂端，從 **[!UICONTROL 專案]** 標籤。 在頁面的右角附近，選取 **[!UICONTROL 建立新專案]**.

1. 在專案的頁面上，選取 **[!UICONTROL 新增API]**.
1. 在 **[!UICONTROL 新增API]** 頁面，選取 **[!UICONTROL Adobe Analytics]**.
1. 在頁面的右下角附近，選取 **[!UICONTROL 下一個]**.

   ![新增API](assets/analytics-oauth2.png)

1. 在 **[!UICONTROL 設定API]** 頁面，選取 **[!UICONTROL 使用者驗證OAuth]**.
1. 在頁面的右下角附近，選取 **[!UICONTROL 下一個]**.
1. 在 **[!UICONTROL 設定API]** 頁面，選取 **[!UICONTROL OAUTH 2.0網頁版]**.
1. 在 **[!UICONTROL 預設重定向URI]** 文本欄位，請按照所示輸入以下路徑：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在 **[!UICONTROL 重定向URI模式]** 文本欄位，請按照所示輸入以下路徑：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在頁面的右下角，選取 **[!UICONTROL 儲存已設定的API]**.
1. 在導覽面板中，Adobe Analytics頁面左側的 **[!UICONTROL 憑證]**，選取 **[!UICONTROL OAuth Web]**.
1. 在 **[!UICONTROL 憑據詳細資訊]**，請執行下列動作：
   * 在 **[!UICONTROL 用戶端ID]**，選取 **[!UICONTROL 複製]** 來複製值。 您需要此值，才能在後續的Dynamic Media Classic案頭應用程式中進行後續的Analytics設定。
   * 在 **[!UICONTROL 用戶端密碼]**，選取 **[!UICONTROL 擷取用戶端密碼]** 以顯示相關值。 選擇 **[!UICONTROL 複製]** 來複製值。 您需要此值才能執行後續Dynamic Media Classic案頭應用程式中的Adobe Analytics設定。

## 在Adobe Dynamic Media Classic中設定Adobe Analytics {#configure-analytics-in-dmc}

>[!NOTE]
>
>在Dynamic Media Classic中初始設定Adobe Analytics後，您唯一必須重做設定的時間如下：
>
>* Analytics中會新增一個報表，且使用者想要開始傳送資料至該新報表。
>* 追蹤伺服器已在Adobe Analytics中更新。
>* 報表中推出了新的追蹤變數，而您想要將Dynamic Media Classic使用者介面中的特定檢視器變數連結至該新的Analytics變數。

>


1. 在Adobe Dynamic Media Classic案頭應用程式的右上角附近，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**.
1. 在左側面板中，位於 **[!UICONTROL 應用程式設定]**，選取 **[!UICONTROL Adobe Analytics]**.
1. 在 **[!UICONTROL Adobe Analytics設定]** 頁面，選取 **[!UICONTROL Adobe Analytics登入]**.
1. 在 **[!UICONTROL Adobe Analytics登入]** 對話框， **[!UICONTROL 用戶端ID]** 欄位和 **[!UICONTROL 用戶端密碼]** 欄位，貼上您先前複製的個別值。
1. 在對話方塊的右下角，選取「登入」並執行您的Adobe IMS(Identity Management服務)登入。

   成功登入時，Adobe Analytics登入對話方塊會再次顯示，同時顯示 **[!UICONTROL 公司]** 下拉式清單，由您可用的公司啟動。

1. 從 **[!UICONTROL 公司]** 下拉式清單，選擇公司。

   選取公司後， **[!UICONTROL 套裝]** 下拉式清單（由所選公司可用的報表套裝啟動）會顯示。

1. 從 **[!UICONTROL 套裝]** 下拉式清單中，選擇報表套裝。

   >[!NOTE]
   >
   >依預設，使用者必須了解以下事實： **[!UICONTROL 公司]** 和 **[!UICONTROL 套裝]** 下拉清單為空。 因此，使用者必須從每個清單中選取值。

1. 選擇 **[!UICONTROL 確定]** 以便儲存設定。

   >[!NOTE]
   >
   >此 **[!UICONTROL Adobe Analytics伺服器]** 欄位會填入建議的第三方追蹤伺服器，當您選取 **[!UICONTROL 確定]**. 如果您使用不同的追蹤伺服器，請在此欄位中更新它，以避免資料遺失。

1. 在Adobe Analytics設定頁面的左下角，選取 **[!UICONTROL 儲存]** 以確保更新Adobe Analytics帳戶設定。

>[!MORELIKETHIS]
>
>* [設定Adobe Analytics報表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

