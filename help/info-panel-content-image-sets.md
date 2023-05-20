---
title: 管理影像集中的資訊面板內容
description: 瞭解如何管理Adobe Dynamic Media Classic影像集中的資訊面板內容。
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 51%

---

# 管理影像集中的資訊面板內容{#managing-info-panel-content-in-image-sets}

除了針對影像集中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用定時快取與排程內容更新來管理資訊面板。

可以使用Adobe Dynamic Media Classic的以下功能管理InfoPanel設定和資料：

* 「資訊面板設定」面板可讓您指定範本，用來顯示資訊面板文字、預設的錯誤回應以及資訊快取的時數。此外，您還可以指定是否要自動發佈影像集。
* 使用「資訊面板資料源」面板，可以指定包含要顯示在「資訊」面板滾動更新文本中的文本的CSV檔案，並指定更新資訊的時間。
* 「匯入中繼資料」對話框可讓您匯入內含滑鼠指向效果文字資訊的 Tab 字元分隔之 TXT 檔案。可以將此TXT選項或「資訊面板」資料饋送面板與滾動影像文本的CSV檔案選項一起使用。

## 設定映像集的響應模板 {#set-up-a-response-template-for-image-sets}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取一個預設回應範本，也可以自行建立一個。

**要設定映像集的響應模板：**

1. 按兩下「影像集」，以在「詳細資訊視圖」中開啟。
1. 選擇 **[!UICONTROL InfoPanel安裝]**。
1. 在「回應範本」下拉式清單中，執行下列任一操作:

   * 要使用預設響應，請選擇 **[!UICONTROL 預設]**。 用於範本設計的 XML 會以暗灰色顯示在「使用者範本」文字方框中。
   * 要建立您自己的響應模板，請選擇 **[!UICONTROL 自定義]**。 在「使用者範本」文字方框中，輸入範本 XML 定義。您可以在文字方框中使用已經定義的預設範本為基礎，以作為自己的回應。

1. （可選）在「預設響應」框中，鍵入在Adobe Dynamic Media Classic檢索影像映射資訊時遇到錯誤時要顯示的文本。 例如，如果系統收到公司名稱與影像集名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」文字欄位中輸入要在快取資料前等待的小時數。

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要整天經常更新，請設定較高的數字。預設為十小時。

1. 選擇 **[!UICONTROL 上載]** 將資訊面板內容基於roudper_key值上載到s7info。
1. 在「S7Info上載」對話框中，瀏覽到要使用的檔案，然後選擇 **[!UICONTROL 上載]**。

   支援的檔案格式是TAB分隔的UTF-16編碼檔案和ASCII編碼CSV檔案。 如果是 CSV 檔案，則非 ASCII 字元必須使用 HTML 編碼。

1. 在「資訊面板設定」面板中，選擇 **[!UICONTROL 發佈]**。

## 導入影像集中「資訊」面板的源內容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以針對影像集之資訊面板的來源文字，使用以 ASCII 編碼 (非 ASCII 字元必須以 HTML 編碼) 的 CSV (逗號分隔值) 檔案，或是 Tab 字元分隔檔案。Tab 字元分隔檔案必須使用 UTF-16 (Unicode) 編碼。您可以使用不同的方法來匯入不同的檔案類型。

格式化來源內容時，請記住下列準則:

* 制表符和逗號分隔的資料可以包含滾動更新模板所需的列數。
* 第一項或第一列資料是滾動更新標識符（與來自影像映射URL的roulder_key值關聯）。
* 確保標識符後的每個制表符或逗號分隔項是要替換到響應模板中的項。因此，第一列被替換為$1$ ，第二列被替換為$2$，依此類推)。

### 從外部托管位置將CSV內容導入映像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 按兩下「影像集」(Image Set)，以在「詳細視圖」(Detail View)中開啟。
1. 選擇 **[!UICONTROL InfoPanel資料源]**。
1. 在外部代管的 CSV 檔案位置 (HTTP) 文字欄位中，輸入 CSV 檔案的 URL。
1. （可選）在「計畫更新」欄位中，指定更新內容的時間，然後選擇 **[!UICONTROL 添加]**。

   您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」文字方框中。要刪除計畫時間，請選擇它，然後選擇 **[!UICONTROL 刪除]**。

1. （可選）選擇 **[!UICONTROL 運行更新]** 以立即更新內容。
