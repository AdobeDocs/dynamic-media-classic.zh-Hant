---
title: 設定混合媒體集查看器預設
description: 瞭解如何在Adobe Dynamic Media Classic設定混合媒體集查看器預設。
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

# 設定混合媒體集查看器預設{#setting-up-a-mixed-media-set-viewer-preset}

混合媒體集檢視器預設集會決定主檢視器的樣式、行為和外觀。設定預設集時，必須指定您還要在混合媒體集檢視器中顯示哪些檢視器。例如，如果您在混合媒體集中包含了影像集，請為混合媒體集檢視器指定影像集檢視器預設集。

您可以選擇在混合媒體集檢視器中包含所有或部分社群功能。「內嵌」功能會增加一個連結至檢視器，可讓使用者複製在外部頁面 (如部落格、網站或社交網站) 中顯示檢視器所需的代碼。「連結」功能會提供檢視器的 URL，以便使用者可以重新連結到此檢視器。「造訪」功能會提供指定網站的連結。

1. 在全局導航欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 查看器預設]**。
1. 在「查看器預設」頁面上，執行下列操作之一：

   * 要建立預設，請選擇 **[!UICONTROL 添加]**。 在「添加查看器預設」對話框中，選擇平台，選擇 **[!UICONTROL 混合媒體集查看器]**，然後選擇 **[!UICONTROL 添加]**。
   * 要編輯「混合媒體集查看器」預設，請選擇該預設，然後選擇 **[!UICONTROL 編輯]**。

1. 在「配置查看器」頁面上，在「預設名稱」框中為「混合媒體集查看器」預設鍵入名稱。
1. 指定 **[!UICONTROL 頁籤]** 或 **[!UICONTROL 無頁籤]**。 標籤會依照類型 (如視訊、色票和迴轉集) 來分隔項目。如果未指定任何制表符，則所有項目都會顯示在「預覽」窗口下的一行中。
1. 在 **[!UICONTROL 名稱]** 框中，鍵入要添加的查看器的名稱。

   例如，如果要將色板集添加到混合媒體集，請鍵入 `Swatch Set A`。

1. 從「檢視器」選單選擇您要檢視的資產類型，如「色票集」。
1. 從「預設集」選單中選擇所選資產類型的預設集。

   例如，如果要添加色板集，請選擇 **[!UICONTROL 色板集1 — 顏色]**。

1. 選擇 **[!UICONTROL 添加]**。

   新的檢視器預設集會顯示在清單中。

1. 針對您要增加的所有檢視器預設集重複步驟 6 - 9。
1. 若要編輯預設集清單，請執行下列任一項作業:

   * 要從清單中刪除預設，請選擇該預設，然後選擇 **[!UICONTROL 刪除]**。
   * 要重新排序清單中的預設，請選擇預設，然後選擇藍色 **[!UICONTROL 上]** 或 **[!UICONTROL 向下]** 。

1. 若要增加社群功能 (「內嵌」、「連結」、「造訪」) 至檢視器，請為下列任一項目指定選項:

   * **電子郵件**  — 選擇 **[!UICONTROL 開]** 按鈕。 當用戶在查看集時選擇「電子郵件」按鈕時，將開啟包含到集的連結的電子郵件。

   * **嵌入**  — 選擇 **[!UICONTROL 實況]**。 在「內嵌按鈕標籤」方框中，鍵入您要在檢視器中顯示的內嵌按鈕名稱。如果需要，請選擇 **[!UICONTROL 瀏覽]** 查找並選擇按鈕的自定義外觀。

   * **連結**  — 選擇 **[!UICONTROL 實況]**。 在「連結按鈕標籤」框中，鍵入要在「連結」按鈕的查看器中顯示的名稱。 如果需要，請選擇 **[!UICONTROL 瀏覽]** 查找並選擇按鈕的自定義外觀。

   * **訪問**  — 選擇 **[!UICONTROL 實況]**。 在「訪問按鈕標籤」框中，鍵入要在查看器中顯示的「訪問」按鈕的名稱。 在「造訪 URL」方框中，輸入您要在按一下連結時開啟的網站 URL。

1. 視需要指定其他選項。要查看選項的說明，請選擇選項旁邊的「資訊提示」表徵圖。

   在更新和更改設定時，「預覽」(Preview)頁面將顯示查看器。

1. 選擇 **[!UICONTROL 保存]**。

>[!MORELIKETHIS]
>
>* [建立和編輯查看器預設](application-setup.md#adding_and_editing_viewer_presets)

