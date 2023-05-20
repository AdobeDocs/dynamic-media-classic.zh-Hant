---
title: "Quick 開始： Adobe Target Standard/Premium 整合"
description: 「簡介」和「快速開始以 Adobe Target Standard/Premium，以協助您使用 Adobe Target 動態媒體 Adobe Systems 的標準/特優整合技術快速啟動並執行。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# 快速開始： Adobe Target 標準/特優整合{#quick-start-target-integration}

Adobe Target標準/特優將控制權直接交給營銷人員，以便快速、持續地運行多個A/B和多變數test，衡量效率，並通過分段、目標和Automated Personalization提高線上內容的相關性。

Adobe Systems 動態媒體經典可讓您建立 Adobe Target Standard/Premium 促銷活動的選件和優惠方案集。 例如，您可以建立具有相同多媒體資產的三個變數的優惠方案集。 然後，您可以讓 Adobe Target Standard/Premium 決定哪些資產提供更好的轉換提升度。 您可以透過基本範本或各個影像建立提案和提案集。將優惠方案集推送或儲存至 Adobe Target Standard/Premium 時，如選件與 mbox 和體驗相關聯，Adobe Target Standard/Premium 可以執行促銷活動。 這些促銷活動決定了網站的哪個變體可能最適合點按進次數和轉換。

為了更好地自訂動態 Adobe Systems 動態媒體經典內容，請使用 Adobe Target Standard/Premium HTML 選件。 [如需詳細資訊，請參閱 Adobe Target Standard/Premium 產品檔 ](https://experienceleague.adobe.com/docs/target.html) 。

>[!NOTE]
>
>必須使用有效的 Adobe Target Standard/Premium 帳戶，才能 Adobe Target Standard/Premium 和 Adobe Systems 動態媒體經典。

此快速開始旨在讓您快速啟動並使用 Adobe Target Standard/Premium HTML 優惠方案集。 依照步驟 1 至 3 執行。每個步驟之後都有一個對主題標題的交叉引用，您可在其中找到更多資訊。

## 1. 在應用程式一般設定中輸入 Adobe Target 標準/Premium URL 頁面

Adobe Systems 動態媒體經典需要您的 Adobe Target Standard/Premium URL 整合 Adobe Target Standard/Premium。 將Adobe Target標準/高級URL的部分複製到（包括） `.com`，然後進入Adobe Dynamic Media Classic **[!UICONTROL 應用程式常規設定]** 的 **[!UICONTROL 伺服器]** 組， **[!UICONTROL Test目標伺服器名]** 的子菜單。 請參閱 [將Adobe Dynamic Media Classic與Adobe Target標準/高級版整合](integrating-dmc-with-target.md#integrating-dmc-with-target)。

## 2. 建立優惠方案集

使用參數化範本或影像來建立提案集。您在測試 &amp; Target 提議集頁面上建立 HTML 優惠方案集。 若要開啟此頁面，請選取您的範本或影像，然後在全域導覽列上，轉至 **[!UICONTROL 「建立]** > **[!UICONTROL 測試 > Target]** 選件」。

若要使用範本建立優惠方案，請選擇 **[!UICONTROL 「新增 &amp; 預覽]** 」。 在「新增 &amp; 預覽頁面中，變更參數值。

若要建立具有影像的優惠方案，請將影像拖曳至「頁面中的「Target 選件」集。 選取 **[!UICONTROL 預覽]** 並為影像或優惠方案集中的所有影像選擇影像預設集。

建立提案集後請將其儲存。

請參閱 [ 建立優惠方案集 ](creating-offer-set.md#creating_an_offer_set) 。

## 3. 將優惠方案集推送至 Adobe Target Standard/Premium

在「測試 &amp; Target 選件集」頁面中，選取 **[!UICONTROL 「推送]** 選件」，然後在「測試 &amp; Target 登入」對話方塊中輸入您的登入憑證。 請參閱 [向Adobe Target標準/高級版推送優惠](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
