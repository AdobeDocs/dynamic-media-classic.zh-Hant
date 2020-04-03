---
title: 管理影像集中的資訊面板內容
seo-title: 管理影像集中的資訊面板內容
description: 'null'
seo-description: 瞭解如何管理影像集中的資訊面板內容。
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 管理影像集中的資訊面板內容{#managing-info-panel-content-in-image-sets}

除了針對影像集中的滑鼠指向效果使用影像地圖文字外，您還可以使用資訊面板來增加大量滑鼠指向效果文字 (包括連結)。您也可以使用定時快取與排程內容更新來管理資訊面板。

您可以使用 Scene7 Publishing System 中的下列功能來管理資訊面板設定與資料:

* 「資訊面板設定」面板可讓您指定範本，用來顯示資訊面板文字、預設的錯誤回應以及資訊快取的時數。此外，您還可以指定是否要自動發佈影像集。
* 「資訊面板資料摘要」面板可讓您指定 CSV 檔案，其中包含您要在資訊面板滑鼠指向效果文字中顯示的文字，也可以讓您排程時間以更新資訊。
* 「匯入中繼資料」對話框可讓您匯入內含滑鼠指向效果文字資訊的 Tab 字元分隔之 TXT 檔案。針對滑鼠指向效果文字，您可以使用此 TXT 選項或含有 CSV 檔案選項的「資訊面板資料摘要」面板。

## 設定影像集的回應範本 {#set-up-a-response-template-for-image-sets}

您可以選取三個預設回應範本之一，以便在資訊面板中顯示文字。這些預設回應範本會決定您的資訊在資訊面板中如何呈現: 欄與列的數目、字型大小、字型等。您可以選取一個預設回應範本，也可以自行建立一個。

**若要設定回應範本**

1. 按兩下影像集，在詳細檢視中加以開啟。
1. Click **InfoPanel Setup** to unfold the panel.
1. 在「回應範本」下拉式清單中，執行下列任一操作:

   * 選取「預設」以使用預設回應。用於範本設計的 XML 會以暗灰色顯示在「使用者範本」文字方框中。
   * 選取「自訂」即可自行建立回應範本。在「使用者範本」文字方框中，輸入範本 XML 定義。您可以在文字方框中使用已經定義的預設範本為基礎，以作為自己的回應。

1. （可選）在「預設回應」方塊中，輸入當Dynamic Media Classic擷取影像地圖資訊時遇到錯誤時，您要顯示的文字。 例如，如果系統收到公司名稱與影像集名稱，但沒有收到滑鼠指向效果識別名稱，就會對使用者顯示此訊息。
1. 在「回應 TTL」文字欄位中輸入要在快取資料前等待的小時數。

   * 如果整天經常更新資料，請設定較低的數字。
   * 如果資料相對穩定且不需要整天經常更新，請設定較高的數字。預設為十小時。

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   支援的檔案格式包括使用 UTF-16 編碼方式的 Tab 字元分隔檔案以及使用 ASCII 編碼的 CSV 檔案。如果是 CSV 檔案，則非 ASCII 字元必須使用 HTML 編碼。

1. In the InfoPanel Setup panel, click **Publish**.

## 匯入影像集中「資訊」面板的來源內容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以針對影像集之資訊面板的來源文字，使用以 ASCII 編碼 (非 ASCII 字元必須以 HTML 編碼) 的 CSV (逗號分隔值) 檔案，或是 Tab 字元分隔檔案。Tab 字元分隔檔案必須使用 UTF-16 (Unicode) 編碼。您可以使用不同的方法來匯入不同的檔案類型。

格式化來源內容時，請記住下列準則:

* Tab 字元與逗號分隔的資料必須盡可能包含最多的欄數，以供滑鼠指向範本使用。
* 第一個項目或資料欄必須為滑鼠指向效果識別名稱 (與影像地圖 URL 的 rollover_key 值相關聯)。
* 確定識別名稱之後的每個 Tab 字元或逗號分隔項目都是您要取代回應範本的項目 (因此，第一欄會取代成 $1$，第二欄會取代成 $2$，以此類推)。

### 從外部托管位置將CSV內容匯入影像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 按兩下影像集，在詳細檢視中加以開啟。
1. Click **InfoPanel Datafeed** to unfold the panel.
1. 在外部代管的 CSV 檔案位置 (HTTP) 文字欄位中，輸入 CSV 檔案的 URL。
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   您可以選取多個更新時間。每個更新時間都會顯示在「更新時間」文字方框中。To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

