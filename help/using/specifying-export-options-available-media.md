---
title: 指定Media Portal使用者可用的匯出選項
description: 瞭解如何在Adobe Dynamic Media Classic中指定Media Portal使用者可用的匯出選項。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 38%

---

# 指定Media Portal使用者可用的匯出選項 {#specifying-export-options-available-to-media-portal-users}

如果管理員將權限給予 Media Portal 使用者，這些使用者就可以在匯出影像時予以重新格式化。例如，可以變更大小、檔案格式及影像品質。在匯出影像時予以自動重新格式化可節省時間，原因是不需要分別重新格式化影像。此外，管理員還可以建立預設集，也就是預先建立的影像格式設定選項。在匯出影像時予以重新格式化以符合公司規格時，可以使用預設集。

如果您透過使用者定義的轉換來匯出影像資產，或匯出原始主要影像，則以下兩項限制適用：

* 適用於匯出工作的壓縮 Zip 匯出檔案的檔案大小上限為 1 GB。
* 每個匯出工作的總資產上限為 500 個。

另請參閱[從Adobe Dynamic Media Classic匯出資產](exporting-assets-from-dmc.md#exporting-assets-from_dmc)。

**若要指定Media Portal使用者可用的匯出選項：**

1. 在全域導覽列上，前往&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**。
1. 在「影像預設集」視窗中，選取下列任一選項:

   * **啟用使用者定義的轉換**：選取此選項時，使用者可以從[匯出選取的Assets]視窗的&#x200B;**[!UICONTROL 大小]**&#x200B;下拉式清單中選擇其他。 接著，使用者可選擇畫素或公分等度量單位，並指定所需的寬度和高度。 當使用者匯出或下載這些檔案時，影像檔案便會重新格式化。

     從&#x200B;**[!UICONTROL 大小]**&#x200B;下拉式清單中選擇&#x200B;**[!UICONTROL 畫素]**&#x200B;時，產生的影像寬度×高度不能超過100百萬畫素。 這個大小相當於方形影像的10,000×10,000畫素，或是2x3外觀比例影像的大約8,000×12,000畫素。 如果您匯出原始主要影像，則不會套用此大小限制。

     取消選取此選項，讓使用者下載檔案時不必在下載時重新格式化檔案。

   * **啟用匯出原始影像**：讓您匯出原始主要影像。 在&#x200B;**[!UICONTROL 匯出選取的Assets]**&#x200B;面板中，使用者可以開啟&#x200B;**[!UICONTROL 轉換]**&#x200B;下拉式功能表，並選擇&#x200B;**[!UICONTROL 匯出原始檔案]**&#x200B;以匯出原始檔案。 如果要強制使用者在匯出影像時選擇影像預設集或選擇轉換選項，請取消選取此選項。

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [選擇群組的影像預設集存取許可權](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
