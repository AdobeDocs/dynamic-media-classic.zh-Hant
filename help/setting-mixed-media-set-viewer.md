---
title: 設定混合媒體集檢視器預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定混合媒體集檢視器預設集。
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 44%

---

# 設定混合媒體集檢視器預設集{#setting-up-a-mixed-media-set-viewer-preset}

混合媒體集檢視器預設集會決定主檢視器的樣式、行為和外觀。設定預設集時，必須指定您還要在混合媒體集檢視器中顯示哪些檢視器。例如，如果您在混合媒體集中包含了影像集，請為混合媒體集檢視器指定影像集檢視器預設集。

您可以選擇在混合媒體集檢視器中包含所有或部分社群功能。「內嵌」功能會增加一個連結至檢視器，可讓使用者複製在外部頁面 (如部落格、網站或社交網站) 中顯示檢視器所需的代碼。「連結」功能會提供檢視器的 URL，以便使用者可以重新連結到此檢視器。「造訪」功能會提供指定網站的連結。

1. 在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.
1. 在「檢視器預設集」頁面上，執行下列任一項作業：

   * 若要建立預設集，請選取 **[!UICONTROL 新增]**. 在「新增檢視器預設集」對話方塊中，選擇平台，然後選擇 **[!UICONTROL 混合媒體集檢視器]**，然後選取 **[!UICONTROL 新增]**.
   * 若要編輯混合媒體集檢視器預設集，請選取該預設集，然後選取 **[!UICONTROL 編輯]**.

1. 在「組態檢視器」頁面的「預設集名稱」方塊中，輸入混合媒體集檢視器預設集的名稱。
1. 指定 **[!UICONTROL 索引標籤]** 或 **[!UICONTROL 無索引標籤]**. 標籤會依照類型 (如視訊、色票和迴轉集) 來分隔項目。當您指定無定位點時，所有專案都會顯示在「預覽」視窗下的一列中。
1. 在 **[!UICONTROL 名稱]** 方塊中，輸入您要新增的檢視器名稱。

   例如，如果您要將色票集新增至混合媒體集，請輸入 `Swatch Set A`.

1. 從「檢視器」選單選擇您要檢視的資產類型，如「色票集」。
1. 從「預設集」選單中選擇所選資產類型的預設集。

   例如，如果您要新增色票集，請選擇 **[!UICONTROL 色票集1 — 色彩]**.

1. 選取 **[!UICONTROL 新增]**.

   新的檢視器預設集會顯示在清單中。

1. 針對您要增加的所有檢視器預設集重複步驟 6 - 9。
1. 若要編輯預設集清單，請執行下列任一項作業:

   * 若要從清單中刪除預設集，請選取該預設集，然後選取 **[!UICONTROL 刪除]**.
   * 若要重新排序清單中的預設集，請選取預設集，然後選取藍色 **[!UICONTROL 上]** 或 **[!UICONTROL 向下]** 箭頭。

1. 若要增加社群功能 (「內嵌」、「連結」、「造訪」) 至檢視器，請為下列任一項目指定選項:

   * **電子郵件**  — 選取 **[!UICONTROL 開啟]** 以在檢視器中啟用電子郵件按鈕。 當使用者在檢視集合時選擇電子郵件按鈕，包含集合連結的電子郵件開啟。

   * **內嵌**  — 選取 **[!UICONTROL 即時]**. 在「內嵌按鈕標籤」方框中，鍵入您要在檢視器中顯示的內嵌按鈕名稱。如有需要，請選取 **[!UICONTROL 瀏覽]** 以尋找並選取按鈕的自訂外觀。

   * **連結**  — 選取 **[!UICONTROL 即時]**. 在「連結按鈕標籤」方塊中，輸入您要在檢視器中顯示的「連結」按鈕名稱。 如有需要，請選取 **[!UICONTROL 瀏覽]** 以尋找並選取按鈕的自訂外觀。

   * **造訪**  — 選取 **[!UICONTROL 即時]**. 在「造訪按鈕標籤」方塊中，輸入您要在「造訪」按鈕的檢視器中顯示的名稱。 在「造訪 URL」方框中，輸入您要在按一下連結時開啟的網站 URL。

1. 視需要指定其他選項。若要檢視選項的說明，請選取選項旁的「資訊提示」圖示。

   當您更新和變更設定時，「預覽」頁面會顯示檢視器。

1. 選取 **[!UICONTROL 儲存]**.

>[!MORELIKETHIS]
>
>* [建立和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)

