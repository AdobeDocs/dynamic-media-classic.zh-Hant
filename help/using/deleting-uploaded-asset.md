---
title: 刪除已上傳的點陣影像資產
description: 瞭解如何刪除Adobe Dynamic Media Classic中已上傳的資產。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 34%

---

# 刪除已上傳的資產{#deleting-an-uploaded-asset}

您可以使用 `delete` 要刪除資產的引數：

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

下面是刪除影像資產時的回應範例:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查詢字串中使用以下欄位來刪除資產:

| URL 參數 | 必需/可選 | 值 |
| --- | --- | --- |
| `op` | 必要 | 刪除 |
| `shared_secret` | 必要 | 公司的共用機密金鑰。 |
| `image_name` | 必要 | 要刪除的資產名稱。 |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>自2023年5月1日起，Dynamic Media中的UGC資產最多可在上傳日期起的60天內使用。 60天後，資產將會移除。

>[!NOTE]
>
>Adobe Dynamic Media Classic已於2021年9月30日停止支援新的或現有的UGC向量影像資產。

**範例影像 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
