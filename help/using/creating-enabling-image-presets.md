---
title: 建立及啟用影像預設集
description: 瞭解如何在Adobe Dynamic Media Classic中建立和啟用影像預設集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:41:19.856Z'
TQID: 'https://experienceleague.adobe.com/AlYkBI41GganXzy28kbNN9DXU1Pd4mVCwJKCdwmnN4M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: da232d1762d4bb21788ab094ea56d715a58c27d2
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 46%

---

# 建立及啟用影像預設集{#creating-and-enabling-image-presets}

使用者使用 Media Portal 匯出影像資產時，可以在「匯出選取的資產」對話框中，選擇影像預設集。 影像預設集是預先定義設定的集合。 這些設定可變更匯出影像時的尺寸、影像品質、格式、解析度及其他外觀方面。

Media Portal 管理員可以建立影像預設集，來控制影像匯出時重新格式化的方式。 使用者從Adobe Dynamic Media Classic匯出影像時，影像預設集會依貴公司的規格重新格式化影像。 使用者不會手動重新格式化影像，而是將其匯出為影像預設集的精確規格。

匯出影像資產時，會套用下列限制:

* 寬度×高度必須小於或等於每個影像100 MB。 例如，影像不能超過10 K×10 K，或是以下的任何外觀變化，例如8 K×12 K。
* 每個匯出工作的總檔案大小上限為 1 GB。
* 每個匯出工作的總資產上限為 500 個。

>[!NOTE]
>
>這些限制僅適用於匯出衍生影像資產，而非主要檔案。

若要建立影像預設集，請參閱[影像預設集](application-setup.md#image_presets)。

若要讓使用者在匯出檔案時選擇影像預設集，請參閱[指定 Media Portal 使用者可使用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

若要選擇要讓群組成員使用哪些影像預設集，請參閱[為群組選擇影像預設集存取權限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。
