---
title: 指定Media Portal使用者可用的匯出選項
seo-title: 指定Media Portal使用者可用的匯出選項
description: 'null'
seo-description: 瞭解如何指定Media Portal使用者可使用的匯出選項。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 指定 Media Portal 使用者可使用的匯出選項 {#specifying-export-options-available-to-media-portal-users}

如果管理員將權限給予 Media Portal 使用者，這些使用者就可以在匯出影像時予以重新格式化。例如，可以變更大小、檔案格式及影像品質。在匯出影像時予以自動重新格式化可節省時間，原因是不需要分別重新格式化影像。此外，管理員還可以建立預設集，也就是預先建立的影像格式設定選項。在匯出影像時予以重新格式化以符合公司規格時，可以使用預設集。

如果透過使用者定義的轉換匯出影像資產，或匯出原始主影像，將套用以下兩種限制:

* 適用於匯出工作的壓縮 Zip 匯出檔案的檔案大小上限為 1 GB。
* 每個匯出工作的總資產上限為 500 個。

另請參閱[從 Scene7 Publishing System 匯出資產](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system)。

**指定 Media Portal 使用者可使用的匯出選項**

1. 按一下「**設定** > **影像預設集**」。
1. 在「影像預設集」視窗中，選取下列任一選項:

   * **啟用使用者定義的轉換**：選取此選項後，使用者可從「匯出選取的資產」視窗的「大小」下拉式清單中選擇其他項目。 使用者接著可選擇度量單位，例如像素或公分，然後指定所需的寬度和高度。當使用者匯出或下載這些檔案時，影像檔案便會重新格式化。

      從「**大小**」下拉式清單中選取「**像素**」時，生成的影像寬度 x 高度不得超過 1 億像素。此大小相當于方形影像的 10,000 x 10,000 像素，或者大約為 2x3 外觀比例影像的 8,000 x 12,000 像素。如果匯出原始主影像，則不會套用此大小限制。

      如果要讓使用者下載檔案，但不要在下載時重新格式化，請取消選取此選項。

   * **啟用「匯出原稿**」可讓您匯出原始的主影像。 使用者可以在「匯出選取的資產」面板中開啟「轉換」下拉式選單，然後選擇「匯出原始檔案」，來匯出原始檔案。如果要強制使用者在匯出影像時選擇影像預設集或選擇轉換選項，請取消選取此選項。

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [為群組選擇影像預設集存取權限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

