---
title: 檢視 Adobe Analytics 報告以測試整合
seo-title: 檢視 Adobe Analytics 報告以測試整合
description: 'null'
seo-description: 瞭解如何透過檢視Adobe Analytics報表來測試整合。
uuid: 937375e0-6dea-4ba-a2 b0-4f3 e461 c9 ee
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
geptopics: SG_ ScenesEvenONDEMENT_ PKK/categories/adobe_ analytics_ tooling_ kit
discoiquuid: 1ddc89ff-d2 e9-42eb-a442-aa6 b9871 c991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 檢視 Adobe Analytics 報告以測試整合{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中建立必要變數後，將它們連結至Dynamic Media Classic事件並完成必要的實施步驟後，您應該測試設定。您可以測試並確認 Adobe Analytics 本身正在擷取資料。如果設定在此有效，則不需再執行其他步驟。假設您遵循上述步驟，並將動態媒體Classic事件資料連結至一或多個自訂流量變數，請依照此工作流程在Adobe Analytics中測試您的資料。

**檢視 Adobe Analytics 報告以測試整合**

1. 從您的帳戶啓動Dynamic Media Classic檢視器，尤其是廣播量度，以便擷取您要擷取的量度，並與它互動以建立一些事件資料。

   例如，如果要測量影像集內最常用的替代檢視，請預設影像集，並按一下不同的縮圖影像。

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   例如，若要存取範例帳戶中的 LoadAsset 屬性，則適當的選單選項為「自訂流量 &gt; 自訂流量 1-10 &gt; LoadAsset」。如果您有超過十個自訂屬性，可能還會看到其他選單選項。

1. 檢視 Adobe Analytics 產生的圖表請注意，這通常只是單一度量的資料。如果您也想知道此資料關聯的資產(例如，觀看哪些視訊至50%，或某組影像中的哪個影像最受歡迎)，請記得擷取此事件的資產資料。

>[!NOTE]
>
>所有動態媒體Classic檢視器資料都在「自訂流量」報表或Adobe Analytics的「自訂轉換」報表中顯示和報告。

如需詳細資訊，請參閱 [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)。
