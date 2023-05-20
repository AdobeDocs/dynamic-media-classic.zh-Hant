---
title: 登入 Adobe Analytics
description: 瞭解如何從Adobe Dynamic Media Classic登錄Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# 登入 Adobe Analytics{#log-in-to-adobe-analytics}

在登錄以配置Adobe Analytics報告並將Adobe Analytics報告變數與Adobe Dynamic Media Classic事件匹配之前，請驗證您是Adobe Analytics的Web服務訪問組的成員。 此組中的成員可以通過Experience Cloud的Web服務API訪問指定報告套件中的所有報告，而不管在介面中設定了何種權限。 要向組添加成員，請在Adobe Analytics，轉到 **[!UICONTROL 管理工具]** > **[!UICONTROL 用戶管理]** > **[!UICONTROL 編輯組]**。

登錄時，您可以選擇輸入Experience Cloud組織ID以使用最新的視頻分析實現。 如果選擇不輸入ID，視頻報告仍然有效。 但是，它可能導致資料無法與來自Adobe Dynamic Media Classic以外的客戶端的其他資料正確整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已遷移到基於Adobe IMS的身份驗證(Identity Management系統)進行登錄，則輸入直接憑據將不起作用。

## 從Adobe Dynamic Media Classic登錄Adobe Analytics {#log-in-to-analytics-from-dmc}

首先將Dynamic Media Classic與Adobe AnalyticsOAuth整合。 Adobe AnalyticsOAuth與Dynamic Media Classic的整合通常僅為每個用戶完成一次。

1. 訪問 [Adobe Developer控制台](https://developer.adobe.com/console)。 確保您的帳戶對需要整合的組織具有管理員權限。
1. 在首頁右上角的下拉清單中，選擇相應的公司。 (下面的螢幕截圖僅供參考；您選擇的實際公司名稱可能會有所不同。)

   ![建立新項目](assets/analytics-oauth1.png)

1. 執行下列任一操作：

   * 在頁面頂部，從 **[!UICONTROL 首頁]** 頁籤 **[!UICONTROL 建立新項目]**。
   * 在頁面頂部，從 **[!UICONTROL 項目]** 頁籤。 在頁面右角附近，選擇 **[!UICONTROL 建立新項目]**。

1. 在項目頁面上，選擇 **[!UICONTROL 添加API]**。
1. 在 **[!UICONTROL 添加API]** ，選擇 **[!UICONTROL Adobe Analytics]**。
1. 在頁面右下角附近，選擇 **[!UICONTROL 下一個]**。

   ![添加API](assets/analytics-oauth2.png)

1. 在 **[!UICONTROL 配置API]** ，選擇 **[!UICONTROL 用戶身份驗證OAuth]**。
1. 在頁面右下角附近，選擇 **[!UICONTROL 下一個]**。
1. 在 **[!UICONTROL 配置API]** ，選擇 **[!UICONTROL OAUTH 2.0 Web]**。
1. 在 **[!UICONTROL 預設重定向URI]** 文本欄位中，按如所示完全輸入以下路徑：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在 **[!UICONTROL 重定向URI模式]** 文本欄位中，按如所示完全輸入以下路徑：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在頁面的右下角，選擇 **[!UICONTROL 保存已配置的API]**。
1. 在導航面板中，在Adobe Analytics頁的左側，在 **[!UICONTROL 憑據]**&#x200B;選中 **[!UICONTROL OAuth Web]**。
1. 下 **[!UICONTROL 憑據詳細資訊]**，執行以下操作：
   * 下 **[!UICONTROL 客戶端ID]**&#x200B;選中 **[!UICONTROL 複製]** 的子菜單。 您需要此值才能在Dynamic Media Classic案頭應用程式中進行後續的分析配置。
   * 下 **[!UICONTROL 客戶端密碼]**&#x200B;選中 **[!UICONTROL 檢索客戶端密鑰]** 顯示關聯值。 選擇 **[!UICONTROL 複製]** 的子菜單。 您需要此值才能在Dynamic Media Classic案頭應用程式中進行後續的Adobe Analytics配置。

## 在Adobe Dynamic Media Classic配置Adobe Analytics {#configure-analytics-in-dmc}

>[!NOTE]
>
>在Dynamic Media Classic對Adobe Analytics進行初始配置後，您唯一必須重做配置的時間是：
>
>* 分析中添加了新報告，用戶希望開始向該新報告發送資料。
>* 跟蹤伺服器在Adobe Analytics更新。
>* 報告中引入了新的跟蹤變數，您希望將Dynamic Media Classic用戶介面中的特定查看器變數連結到該新的分析變數。
>


1. 在Adobe Dynamic Media Classic案頭應用程式的右上角，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**。
1. 在左面板中，在 **[!UICONTROL 應用程式設定]**&#x200B;選中 **[!UICONTROL Adobe Analytics]**。
1. 在 **[!UICONTROL Adobe Analytics配置]** ，選擇 **[!UICONTROL Adobe Analytics登錄]**。
1. 在 **[!UICONTROL Adobe Analytics登錄]** 對話框 **[!UICONTROL 客戶端ID]** 的 **[!UICONTROL 客戶端密碼]** 欄位，貼上您以前複製的各個值。
1. 在對話框的右下角，選擇 **[!UICONTROL 登錄]** 並執行Adobe IMS(Identity Management服務)登錄。

   成功登錄後，將再次出現「Adobe Analytics登錄」對話框，並 **[!UICONTROL 公司]** 下拉清單，由您可用的公司啟動。

1. 從 **[!UICONTROL 公司]** 下拉清單，選擇一個公司。

   選擇公司後， **[!UICONTROL 套房]** 由報表套件啟動的下拉清單（可供選定公司使用）將變為可見。

1. 從 **[!UICONTROL 套房]** 下拉清單，選擇報表套件。

   >[!NOTE]
   >
   >預設情況下，用戶必須知道 **[!UICONTROL 公司]** 和 **[!UICONTROL 套房]** 下拉清單為空。 因此，用戶必須從每個清單中選擇一個值。

1. 選擇 **[!UICONTROL 確定]** 以便保存配置。

   >[!NOTE]
   >
   >的 **[!UICONTROL Adobe Analytics伺服器]** 欄位將填充建議的第三方跟蹤伺服器，當您選擇 **[!UICONTROL 確定]**。 如果使用其他跟蹤伺服器，請在此欄位中更新它以避免資料丟失。

1. 在「Adobe Analytics配置」頁的左下角，選擇 **[!UICONTROL 保存]** 以確保更新您的Adobe Analytics帳戶配置。

>[!MORELIKETHIS]
>
>* [配置Adobe Analytics報告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

