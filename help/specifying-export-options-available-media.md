---
title: 指定Media Portal使用者可用的匯出選項
description: 了解如何指定AdobeDynamic Media Classic中Media Portal使用者可用的匯出選項。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 66%

---

# 指定Media Portal使用者可用的匯出選項 {#specifying-export-options-available-to-media-portal-users}

如果管理員將權限給予 Media Portal 使用者，這些使用者就可以在匯出影像時予以重新格式化。例如，可以變更大小、檔案格式及影像品質。在匯出影像時予以自動重新格式化可節省時間，原因是不需要分別重新格式化影像。此外，管理員還可以建立預設集，也就是預先建立的影像格式設定選項。在匯出影像時予以重新格式化以符合公司規格時，可以使用預設集。

如果透過使用者定義的轉換匯出影像資產，或匯出原始主影像，將套用以下兩種限制:

* 適用於匯出工作的壓縮 Zip 匯出檔案的檔案大小上限為 1 GB。
* 每個匯出工作的總資產上限為 500 個。

另請參閱[從AdobeDynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc)匯出資產。

**指定 Media Portal 使用者可使用的匯出選項:**

1. 在全局導航欄上，轉到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**。
1. 在「影像預設集」視窗中，選取下列任一選項:

   * **啟用使用者定義的轉換**  — 選取此選項後，使用者可從「匯出選取的 **** 資產」視窗的「已選取資產」下拉式清單中選擇其他項目。使用者接著可選擇度量單位，例如像素或公分，然後指定所需的寬度和高度。當使用者匯出或下載這些檔案時，影像檔案便會重新格式化。

      從「**[!UICONTROL 大小]**」下拉式清單中選取「**[!UICONTROL 像素]**」時，生成的影像寬度 x 高度不得超過 1 億像素。此大小相當于方形影像的 10,000 x 10,000 像素，或者大約為 2x3 外觀比例影像的 8,000 x 12,000 像素。如果匯出原始主影像，則不會套用此大小限制。

      如果要讓使用者下載檔案，但不要在下載時重新格式化，請取消選取此選項。

   * **啟用「導出原始影像** 」 — 用於導出原始主影像。在&#x200B;**[!UICONTROL 匯出選取的資產]**&#x200B;面板中，使用者可以開啟&#x200B;**[!UICONTROL 轉換]**&#x200B;下拉式選單，並選擇&#x200B;**[!UICONTROL 匯出原始]**&#x200B;以匯出原始檔案。 如果要強制使用者選擇影像預設集或在他們匯出影像時選擇轉換選項，請取消選取此選項。

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [為群組選擇影像預設集存取權限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

