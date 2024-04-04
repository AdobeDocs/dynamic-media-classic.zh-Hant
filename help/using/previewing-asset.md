---
title: 預覽資產
description: 瞭解如何在Adobe Dynamic Media Classic中預覽資產。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 19%

---

# 預覽資產{#previewing-an-asset}

您可以使用預覽來檢視客戶檢視時數位資產的顯示方式。 「預覽」功能會使用指定給資產的預設檢視器。預設檢視器可在「應用程式設定」中設定。

另請參閱 [設定預設檢視器](application-setup.md#configuring_default_viewers).

如果您使用引數圖層預覽範本資產，可以變更引數或變更影像預設集。 因為所有變更都是以內嵌形式進行，所以您可以從相同的「預覽」視窗立即檢視結果。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**若要預覽資產：**

1. 在左側的「資產庫」面板中，導覽至包含您要預覽之資產的資產資料夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 格點檢視]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 清單檢視]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**.

1. 根據您使用的檢視，執行下列任一項作業：

   * 在「網格檢視」或「清單檢視」的「資產」視窗中，選取單一資產，然後選取 **[!UICONTROL 預覽]** 靠近縮圖影像。
   * 在「網格檢視」、「清單檢視」或「詳細資料檢視」的「資產」視窗上方的工具列上，選取「 」 **[!UICONTROL 預覽]**.

## 根據檢視器平台型別預覽資產 {#previewing-an-asset-based-on-viewer-platform-type}

您可以使用「檢視器清單」預覽資產顯示在特定檢視器平台類型 (例如 HTML5) 上的情形。視資產類型和您所選取用來預覽的相關檢視器而定，「檢視器清單」中並非提供所有平台。

您也可以使用「檢視器清單」來複製檢視器的URL，或檢視並複製檢視器程式碼以內嵌在您的網頁中。

對於指定的檢視器平台，「檢視器清單」視窗可讓您以視覺化方式檢視哪些裝置（例如平板電腦和智慧型手機）可供檢視器使用。

**若要根據檢視器平台型別預覽資產：**

1. 在左側的「資產庫」面板中，導覽至包含您要預覽之資產的資產資料夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一資產，然後在縮圖影像下方，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

1. （選擇性）在「檢視器清單」視窗中，選取欄標題 **[!UICONTROL 名稱]** 或 **[!UICONTROL 平台型別]** 以遞增或遞減順序排序欄。
1. 在「檢視器清單」視窗中，選取表格的「動作」欄下 **[!UICONTROL 預覽]** 以檢視所選檢視器和平台型別的資產顯示方式。

   關閉顯示的預覽。

1. （選擇性）在「檢視器清單」視窗中，在底部的「產生複製URL的URL編碼」下拉式清單中，選取要在複製資產時套用至資產URL的URL編碼。
1. (選擇性) 執行下列任一項作業:

   * 在「檢視器清單」視窗中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]** 適用於選取的檢視器和平台型別。

     當您選取 **[!UICONTROL 複製URL]**，其相關聯的URL會自動複製到剪貼簿。

   * 在「檢視器清單」視窗中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

     當您選取 **[!UICONTROL 內嵌程式碼]**，會開啟內嵌程式碼視窗，供您檢閱檢視器程式碼。 您無法在此視窗中編輯程式碼。您也可以將該程式碼複製到剪貼簿上，以便貼到網頁中。

     關閉顯示的預覽。

1. 在「檢視器清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。

## 根據影像預設集預覽影像資產 {#previewing-an-image-asset-based-on-its-image-preset}

您可以依據影像預設集來預覽影像資產，瞭解系統以不同大小將其動態提供給網站或是應用程式時的外觀。

「影像預設集」是預先定義的設定集合，在匯出影像時，會變更影像的大小、影像品質、格式、解析度及其他外觀方面。

另請參閱 [設定影像預設集](setting-image-presets.md#setting_up_image_presets).

另請參閱 [建立及啟用影像預設集](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**若要根據影像預設集預覽影像資產：**

1. 在左側的「資產庫」面板中，導覽至包含您要預覽之影像資產的資產資料夾。
1. 執行下列任一項作業︰

   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一影像資產，然後前往縮圖影像右側 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗的工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.

1. 在「影像預設集清單」的表格中，選取您要在右側窗格內預覽之內嵌影像資產的影像預設集類型名稱。
1. （選擇性）在「影像預設集清單」視窗的 **[!UICONTROL 產生復本URL所使用的URL編碼]** 從底部的下拉式清單中，選取URL編碼，以在複製影像資產時套用至其URL。
1. （選擇性）在「影像預設集清單」視窗的預覽窗格右上角區域中，選取 **[!UICONTROL 複製URL]** 選取的預設集型別。

   當您選取 **[!UICONTROL 複製URL]**，其相關聯的URL會自動複製到剪貼簿。

1. 在「影像預設集清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。
