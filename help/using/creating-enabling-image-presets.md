---
title: 建立及啟用影像預設集
description: 瞭解如何在Adobe Dynamic Media Classic中建立和啟用影像預設集。
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 60%

---

# 建立及啟用影像預設集{#creating-and-enabling-image-presets}

使用者使用 Media Portal 匯出影像資產時，可以在「匯出選取的資產」對話框中，選擇影像預設集。「影像預設集」是預先定義之設定的集合，而這些設定可在匯出影像時，變更影像外觀的大小、影像品質、格式、解析度及其他各方面。

Media Portal 管理員可以建立影像預設集，來控制影像匯出時重新格式化的方式。使用者從Adobe Dynamic Media Classic匯出影像時，影像預設集會依貴公司的規格重新格式化影像。 使用者可匯出完全符合影像預設集規格的影像，而非自行重新格式化影像。

匯出影像資產時，會套用下列限制:

* 寬度×高度必須小於或等於每個影像100 MB。 例如，影像不能超過10 K×10 K，或是以下的任何外觀變化，例如8 K×12 K。
* 每個匯出作業的總檔案大小上限為1-GB。
* 每個匯出工作的總資產上限為 500 個。

>[!NOTE]
>
>這些限制僅適用於匯出衍生影像資產，而非主要檔案。

若要建立影像預設集，請參閱[影像預設集](application-setup.md#image_presets)。

若要讓使用者在匯出檔案時選擇影像預設集，請參閱[指定 Media Portal 使用者可使用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

若要選擇要讓群組成員使用哪些影像預設集，請參閱[為群組選擇影像預設集存取權限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。
