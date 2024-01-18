---
title: 管理影像集中的資訊面板內容
description: 瞭解如何管理Adobe Dynamic Media Classic影像集中的資訊面板內容。
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 51%

---

# 管理影像集中的資訊面板內容{#managing-info-panel-content-in-image-sets}

除了針對影像集中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用定時快取與排程內容更新來管理資訊面板。

您可以使用Adobe Dynamic Media Classic中的下列功能來管理資訊面板設定和資料：

* 「資訊面板設定」面板可讓您指定範本，用來顯示資訊面板文字、預設的錯誤回應以及資訊快取的時數。此外，您還可以指定是否要自動發佈影像集。
* 「資訊面板」資料摘要面板可讓您指定CSV檔案，其中包含您要顯示在資訊面板滑鼠指向效果文字中的文字，以及更新資訊的排程時間。
* 「匯入中繼資料」對話框可讓您匯入內含滑鼠指向效果文字資訊的 Tab 字元分隔之 TXT 檔案。您可以針對滑鼠指向效果文字，使用此TXT選項或具有CSV檔案選項的「資訊面板」資料摘要面板。

## 設定影像集的回應範本 {#set-up-a-response-template-for-image-sets}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取一個預設回應範本，也可以自行建立一個。

**若要設定影像集的回應範本：**

1. 按兩下「影像集」，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]**.
1. 在「回應範本」下拉式清單中，執行下列任一操作:

   * 若要使用預設回應，請選取 **[!UICONTROL 預設]**. 用於範本設計的 XML 會以暗灰色顯示在「使用者範本」文字方框中。
   * 若要建立您自己的回應範本，請選取 **[!UICONTROL 自訂]**. 在「使用者範本」文字方框中，輸入範本 XML 定義。您可以在文字方框中使用已經定義的預設範本為基礎，以作為自己的回應。

1. （選擇性）在「預設回應」方塊中，輸入您要在Adobe Dynamic Media Classic擷取影像地圖資訊時發生錯誤，顯示的文字。 例如，如果系統收到公司名稱與影像集名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」文字欄位中輸入要在快取資料前等待的小時數。

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要整天經常更新，請設定較高的數字。預設為十小時。

1. 選取 **[!UICONTROL 上傳]** 若要根據rollover_key值將資訊面板內容上傳至s7info。
1. 在「S7Info上傳」對話方塊中，瀏覽至您要使用的檔案，然後選取 **[!UICONTROL 上傳]**.

   支援的檔案格式為使用UTF-16編碼的TAB分隔檔案和使用ASCII編碼的CSV檔案。 如果是 CSV 檔案，則非 ASCII 字元必須使用 HTML 編碼。

1. 在「資訊面板設定」面板中，選取 **[!UICONTROL 發佈]**.

## 匯入影像集中資訊面板的來源內容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以針對影像集之資訊面板的來源文字，使用以 ASCII 編碼 (非 ASCII 字元必須以 HTML 編碼) 的 CSV (逗號分隔值) 檔案，或是 Tab 字元分隔檔案。Tab 字元分隔檔案必須使用 UTF-16 (Unicode) 編碼。您可以使用不同的方法來匯入不同的檔案類型。

格式化來源內容時，請記住下列準則:

* 以定位字元和逗號分隔的資料可包含變換範本所需任意數目的欄。
* 資料的第一個專案或欄是滑鼠指向效果識別碼（與影像地圖URL中的rollover_key值相關聯）。
* 請確定識別碼之後的每個定位字元或逗號分隔專案都是您要取代至回應範本的專案。 因此，第一欄會替換為$1$，第二欄會替換為$2$，以此類推。

### 從外部託管位置將CSV內容匯入影像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 連按兩下「影像集」，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板資料摘要]**.
1. 在外部代管的 CSV 檔案位置 (HTTP) 文字欄位中，輸入 CSV 檔案的 URL。
1. （選擇性）在「排程更新」欄位中，指定更新內容的時間，然後選取 **[!UICONTROL 新增]**.

   您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」文字方框中。若要移除排定的時間，請選取該時間，然後選取 **[!UICONTROL 刪除]**.

1. （選用）選取 **[!UICONTROL 執行更新]** 以立即更新內容。
