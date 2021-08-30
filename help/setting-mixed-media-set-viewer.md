---
title: 設定混合媒體集檢視器預設集
description: 了解如何在AdobeDynamic Media Classic中設定混合媒體集檢視器預設集。
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 44%

---

# 設定混合媒體集檢視器預設集{#setting-up-a-mixed-media-set-viewer-preset}

混合媒體集檢視器預設集會決定主檢視器的樣式、行為和外觀。設定預設集時，必須指定您還要在混合媒體集檢視器中顯示哪些檢視器。例如，如果您在混合媒體集中包含了影像集，請為混合媒體集檢視器指定影像集檢視器預設集。

您可以選擇在混合媒體集檢視器中包含所有或部分社群功能。「內嵌」功能會增加一個連結至檢視器，可讓使用者複製在外部頁面 (如部落格、網站或社交網站) 中顯示檢視器所需的代碼。「連結」功能會提供檢視器的 URL，以便使用者可以重新連結到此檢視器。「造訪」功能會提供指定網站的連結。

1. 在全局導航欄上，轉到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。
1. 在「查看器預設集」頁上，執行以下操作之一：

   * 要建立預設，請選擇&#x200B;**[!UICONTROL Add]**。 在「添加查看器預設集」對話框中，選擇平台，選擇&#x200B;**[!UICONTROL 混合媒體集查看器]**，然後選擇&#x200B;**[!UICONTROL 添加]**。
   * 若要編輯混合媒體集檢視器預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL Edit]**。

1. 在「配置查看器」頁面上，在「混合媒體集查看器」預設集的「預設集名稱」框中鍵入名稱。
1. 指定&#x200B;**[!UICONTROL 標籤]**&#x200B;或&#x200B;**[!UICONTROL 無標籤]**。 標籤會依照類型 (如視訊、色票和迴轉集) 來分隔項目。如果沒有指定頁簽，則所有項目都會顯示在「預覽」窗口下的行中。
1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;方塊中，輸入您要新增的檢視器名稱。

   例如，如果要將色板集添加到混合媒體集，請鍵入`Swatch Set A`。

1. 從「檢視器」選單選擇您要檢視的資產類型，如「色票集」。
1. 從「預設集」選單中選擇所選資產類型的預設集。

   例如，如果要添加色板集，請選擇&#x200B;**[!UICONTROL SwatchSet1-Colors]**。

1. 選擇&#x200B;**[!UICONTROL 添加]**。

   新的檢視器預設集會顯示在清單中。

1. 針對您要增加的所有檢視器預設集重複步驟 6 - 9。
1. 若要編輯預設集清單，請執行下列任一項作業:

   * 若要從清單中刪除預設集，請選取該預設集，然後選取&#x200B;**[!UICONTROL Delete]**。
   * 要重新排序清單中的預設集，請選擇預設集，然後選擇藍色&#x200B;**[!UICONTROL Up]**&#x200B;或&#x200B;**[!UICONTROL Down]**&#x200B;箭頭。

1. 若要增加社群功能 (「內嵌」、「連結」、「造訪」) 至檢視器，請為下列任一項目指定選項:

   * **電子郵件**  — 在檢 **** 視器中選取「啟用電子郵件」按鈕。當使用者在檢視集合時選取「電子郵件」按鈕時，會開啟包含該集合連結的電子郵件。

   * **內嵌**  — 選取「 **[!UICONTROL 即時」]**。在「內嵌按鈕標籤」方框中，鍵入您要在檢視器中顯示的內嵌按鈕名稱。如果需要，請選擇&#x200B;**[!UICONTROL Browse]**&#x200B;以查找並選擇按鈕的自定義外觀。

   * **連結**  — 選取「 **[!UICONTROL 即時」]**。在「連結按鈕標籤」方塊中，輸入您要在連結按鈕的檢視器中顯示的名稱。 如果需要，請選擇&#x200B;**[!UICONTROL Browse]**&#x200B;以查找並選擇按鈕的自定義外觀。

   * **造訪**  — 選 **[!UICONTROL 取即時]**。在「瀏覽按鈕標籤」方塊中，輸入您要在瀏覽按鈕的檢視器中顯示的名稱。 在「造訪 URL」方框中，輸入您要在按一下連結時開啟的網站 URL。

1. 視需要指定其他選項。若要查看選項的說明，請選取選項旁的「資訊提示」圖示。

   預覽頁面會在您更新和變更設定時顯示檢視器。

1. 選擇&#x200B;**[!UICONTROL 保存]**。

>[!MORELIKETHIS]
>
>* [建立和編輯查看器預設集](application-setup.md#adding_and_editing_viewer_presets)

