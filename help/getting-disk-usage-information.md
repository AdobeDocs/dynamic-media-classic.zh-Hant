---
title: 取得磁碟使用量資訊
seo-title: 取得磁碟使用量資訊
description: 'null'
seo-description: 瞭解如何取得磁碟使用資訊。
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# 取得磁碟使用量資訊 {#getting-disk-usage-information}

您可使用 `disk_info` 參數擷取關於公司磁碟空間使用量的資訊，如以下範例中所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

範例回應如下所示:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查詢字串中使用以下欄位來取得磁碟使用量資訊:

| URL 參數 | 必需/可選 | 值 |
|--- |--- |--- |
| op | 必要 | disk_info |
| shared_secret | 必要 | 公司的共用密鑰 |

下面的範例代碼可取得 000Company 的磁碟資訊:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

