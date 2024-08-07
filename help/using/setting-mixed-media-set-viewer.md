---
title: 設定混合媒體集檢視器預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定混合媒體集檢視器預設集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 20%

---

# 設定混合媒體集檢視器預設集{#setting-up-a-mixed-media-set-viewer-preset}

混合媒體集檢視器預設集會決定主檢視器的樣式、行為和外觀。設定預設集時，必須指定您還要在混合媒體集檢視器中顯示哪些檢視器。例如，如果您已在混合媒體集中加入影像集，請為混合媒體集檢視器指定影像集檢視器預設集。

您可以選擇在混合媒體集檢視器中包含所有或部分社群功能。內嵌功能會新增檢視器的連結，讓使用者複製在外部頁面（例如部落格、網站或社交網站）中顯示檢視器所需的程式碼。 「連結」功能會提供檢視器的 URL，以便使用者可以重新連結到此檢視器。「瀏覽」功能會提供您指定網站的連結。

1. 在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**。
1. 在「檢視器預設集」頁面上，執行下列任一項作業：

   * 若要建立預設集，請選取&#x200B;**[!UICONTROL 新增]**。 在「新增檢視器預設集」對話方塊中，選擇平台。 然後按一下&#x200B;**[!UICONTROL 混合媒體集檢視器]** > **[!UICONTROL 新增]**。
   * 若要編輯混合媒體集檢視器預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL 編輯]**。

1. 在「組態檢視器」頁面的「預設集名稱」方塊中，輸入「混合媒體集檢視器預設集」的名稱。
1. 指定&#x200B;**[!UICONTROL 標籤]**&#x200B;或&#x200B;**[!UICONTROL 無標籤]**。 索引標籤會依型別來分隔專案，例如視訊、色票和迴轉集。 未指定標籤時，所有專案都會顯示在「預覽」視窗下的一列中。
1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;方塊中，輸入您要新增的檢視器名稱。

   例如，如果您要將色票集新增至混合媒體集，請輸入`Swatch Set A`。

1. 在「檢視器」功能表中，選取您要檢視的資產型別，例如「色票集」。
1. 從「預設集」選單中，選取所選資產型別的預設集。

   例如，如果您要新增色票集，請選取&#x200B;**[!UICONTROL 色票集1 — 顏色]**。

1. 選取&#x200B;**[!UICONTROL 新增]**。

   新的檢視器預設集會顯示在清單中。

1. 對您要新增的所有檢視器預設集重複步驟6:9。
1. 若要編輯預設集清單，請執行下列任一項作業:

   * 若要從清單中刪除預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL 刪除]**。
   * 若要重新排序清單中的預設集，請選取預設集，然後選取藍色的&#x200B;**[!UICONTROL 向上]**&#x200B;或&#x200B;**[!UICONTROL 向下]**&#x200B;箭頭。

1. 若要增加社群功能 (「內嵌」、「連結」、「造訪」) 至檢視器，請為下列任一項目指定選項:

   * **電子郵件**：選取&#x200B;**[!UICONTROL 開啟]**&#x200B;以在檢視器中啟用電子郵件按鈕。 當使用者在檢視集合時選擇電子郵件按鈕，會開啟包含集合連結的電子郵件。

   * **內嵌**：選取&#x200B;**[!UICONTROL 即時]**。 在「內嵌按鈕標籤」方框中，鍵入您要在檢視器中顯示的內嵌按鈕名稱。如果需要，請選取&#x200B;**[!UICONTROL 瀏覽]**&#x200B;以尋找並選取按鈕的自訂外觀。

   * **連結**：選取&#x200B;**[!UICONTROL 即時]**。 在「連結按鈕標籤」方塊中，輸入您要在「連結」按鈕的檢視器中顯示的名稱。 如果需要，請選取&#x200B;**[!UICONTROL 瀏覽]**&#x200B;以尋找並選取按鈕的自訂外觀。

   * **造訪**：選取&#x200B;**[!UICONTROL 即時]**。 在「造訪按鈕標籤」方塊中，輸入您要在「造訪」按鈕的檢視器中顯示的名稱。 在「瀏覽URL」方塊中，輸入您要在選取連結時開啟之網站的URL。

1. 視需要指定其他選項。若要檢視選項的說明，請選取選項旁的「資訊提示」圖示。

   當您更新和變更設定時，「預覽」頁面會顯示檢視器。

1. 選取&#x200B;**[!UICONTROL 儲存]**。

>[!MORELIKETHIS]
>
>* [建立和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)
