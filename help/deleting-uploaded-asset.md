---
title: 刪除上載的資產
seo-title: 刪除上載的資產
description: 'null'
seo-description: 瞭解如何刪除上傳的資產。
uuid: edd2b688-c377-4be1-ba16-d2 d2 e6 f716 d
contentOwner: 管理員
content-type: 參考
products: SG_ PERIENCENCENAGER/Dynamic-Media-Scene-7
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087 eeffb
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# 刪除上載的資產{#deleting-an-uploaded-asset}

您可使用此格式的 `delete` 參數刪除資產:

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
|--- |--- |--- |
| op | 必要 | 刪除 |
| shared_secret | 必要 | 公司的共用密鑰。 |
| <ul><li>對於影像:image_name</li><li>適用於向量:fxg_name</li></ul> | 必要 | 要刪除的資產名稱。 |

**範例影像 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**範例向量 URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`