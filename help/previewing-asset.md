---
title: 預覽資產
description: 了解如何在Adobe Dynamic Media Classic中預覽資產。
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
source-git-commit: 3185824deca4d4b3c5549bda2e47f179094110e7
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 37%

---

# 預覽資產{#previewing-an-asset}

您可以使用「預覽」來查看客戶檢視數位資產時的顯示情形。 「預覽」功能會使用指定給資產的預設檢視器。預設檢視器可在「應用程式設定」中設定。

請參閱[設定預設檢視器](application-setup.md#configuring_default_viewers)。

如果您預覽的範本資產含有參數層，可以變更參數或變更影像預設集。 因為所有變更都是以內嵌形式進行，所以您可以從相同的「預覽」視窗立即檢視結果。

另請參閱[Adobe檢視器參考程式庫範例](https://landing.adobe.com/tw/na/dynamic-media/ctir-2755/live-demos.html)。

**預覽資產:**

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」窗口的右側，選擇「**[!UICONTROL 網格視圖]**」。
   * 在「資產」窗口的右側，選擇「**[!UICONTROL 清單視圖]**」。
   * 在「資產」窗口的工具欄右側，選擇「**[!UICONTROL 詳細資訊視圖]**」。

1. 視您使用的檢視而定，執行下列其中一項操作：

   * 在「網格視圖」或「清單視圖」的「資產」窗口中，選擇單個資產，然後選擇縮圖影像附近的&#x200B;**[!UICONTROL 預覽]**。
   * 在「網格視圖」、「清單視圖」或「詳細視圖」的「資產」窗口上方的工具欄上，選擇「**[!UICONTROL 預覽]**」。

## 根據檢視器平台類型預覽資產 {#previewing-an-asset-based-on-viewer-platform-type}

您可以使用「檢視器清單」預覽資產顯示在特定檢視器平台類型 (例如 HTML5) 上的情形。視資產類型和您所選取用來預覽的相關檢視器而定，「檢視器清單」中並非提供所有平台。

您也可以使用「檢視器清單」來複製檢視器的 URL，或是檢視並複製檢視器程式碼以便內嵌到您的網頁。

對於指定的檢視器平台，「檢視器清單」視窗可讓您以視覺化方式查看哪些裝置（例如平板電腦和智慧型手機）可供檢視器使用。

**依據檢視器平台類型預覽資產:**

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」窗口的右側，選擇「**[!UICONTROL 網格視圖]**」。 在「資產」視窗中，選取單一資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**。
   * 在「資產」窗口的右側，選擇「**[!UICONTROL 清單視圖]**」。 在「資產」視窗中，選取單一資產，然後前往縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。
   * 在「資產」窗口的工具欄右側，選擇「**[!UICONTROL 詳細資訊視圖]**」。 在相同工具列上，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**。

1. （可選）在「查看器清單」窗口中，選擇列標題&#x200B;**[!UICONTROL Name]**&#x200B;或&#x200B;**[!UICONTROL Platform type]**&#x200B;以按升序或降序對列進行排序。
1. 在「查看器清單」窗口的表的「操作」列下，選擇&#x200B;**[!UICONTROL Preview]**&#x200B;以查看所選查看器和平台類型的資產如何顯示。

   關閉顯示的預覽。

1. (選擇性) 在「檢視器清單」視窗裡，位於底部之「產生複製 URL 的 URL 編碼」下拉式清單中，選取複製 URL 編碼時您要套用至資產 URL 的 URL 編碼。
1. (選擇性) 執行下列任一項作業:

   * 在「查看器清單」窗口的表的「操作」列下，為選定的查看器和平台類型選擇&#x200B;**[!UICONTROL 複製URL]**。

      選擇&#x200B;**[!UICONTROL 複製URL]**&#x200B;時，其關聯的URL會自動複製到剪貼簿。

   * 在「查看器清單」窗口的表的「操作」列下，選擇&#x200B;**[!UICONTROL Embed Code]**。

      選取&#x200B;**[!UICONTROL 內嵌程式碼]**&#x200B;時，會開啟「內嵌程式碼」視窗，供您檢視檢視器程式碼。 您無法在此視窗中編輯程式碼。您也可以將該程式碼複製到剪貼簿上，以便貼到網頁中。

      關閉顯示的預覽。

1. 在「檢視器清單」視窗的右下角，選取&#x200B;**[!UICONTROL 關閉]**&#x200B;以返回「資產」畫面。

## 根據影像預設集預覽影像資產 {#previewing-an-image-asset-based-on-its-image-preset}

您可以依據影像預設集來預覽影像資產，瞭解系統以不同大小將其動態提供給網站或是應用程式時的外觀。

「影像預設集」是預先定義之設定的集合，而這些設定可在匯出影像時，變更影像外觀的大小、影像品質、格式、解析度及其他各方面。

請參閱[設定影像預設集](setting-image-presets.md#setting_up_image_presets)。

請參閱[建立並啟用影像預設集](creating-enabling-image-presets.md#creating_and_enabling_image_presets)。

**依據影像預設集來預覽影像資產:**

1. 在左側的「資產庫」面板中，導覽至含有您要預覽之影像資產的「資產」檔案夾。
1. 執行下列任一項作業︰

   * 在「資產」窗口的右側，選擇「**[!UICONTROL 網格視圖]**」。 在「資產」視窗中，選取單一影像資產，然後在縮圖影像下方，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在「資產」窗口的右側，選擇「**[!UICONTROL 清單視圖]**」。 在「資產」窗口中，選擇單個影像資產，然後轉至縮圖影像的右側，前往&#x200B;**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**。
   * 在「資產」窗口的工具欄右側，選擇「**[!UICONTROL 詳細資訊視圖]**」。 在相同工具列上，前往「**[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**」。

1. 在「影像預設集清單」的表格中，選取您要在右側窗格內預覽之內嵌影像資產的影像預設集類型名稱。
1. （可選）在「影像預設集清單」視窗底部的「複製URL產生的URL編碼」下拉式清單中，選取複製影像資產時要套用至該URL的URL編碼。****
1. （可選）在「影像預設集清單」窗口的預覽窗格的右上角，為所選預設集類型選擇&#x200B;**[!UICONTROL 複製URL]**。

   選擇&#x200B;**[!UICONTROL 複製URL]**&#x200B;時，其關聯的URL會自動複製到剪貼簿。

1. 在「影像預設集清單」視窗的右下角，選取&#x200B;**[!UICONTROL Close]**&#x200B;以返回「資產」畫面。
