---
title: 上載影像資產或向量資產
seo-title: 上載影像資產或向量資產
description: 'null'
seo-description: 瞭解如何上傳影像資產或向量資產。
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 84%

---


# 上載影像資產或向量資產{#uploading-an-image-asset-or-a-vector-asset}

您必須先要求一個共用密鑰，然後才能上載影像資產。使用此共用密鑰來擷取上載標記。然後使用上載標記來上載影像資產或向量資產。

## 要求共用密鑰 {#requesting-a-shared-secret-key}

使用 *Admin Console建立*[支援案例，以要求共用密碼金鑰。](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) 在您的支援案例中，請求共用機密金鑰。

在電子郵件中，請提供想要用於上載影像資產的公司名稱。從Dynamic Media Classic收到金鑰後，請將它儲存在本機以備日後使用。

## 擷取上載標記 {#retrieving-the-upload-token}

*上載標記*&#x200B;將確保他人不能使用相同的共用密鑰來上載資產。它確保上載合法且來自信任的來源。

上載標記是字母數字字串，只能在指定時間內使用。請使用以下 URL 代替您的共用密鑰來擷取上載標記。

* 影像
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`在此範例中，shared-secret金鑰為 `fece4b21-87ee-47fc-9b99-2e29b78b602`

* 向量
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`在此範例中，shared-secret金鑰為 `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

根據預設，上載標記在您擷取之後 5 分鐘 (300 秒) 便過期。若需要求更多時間，請在 URL 中加上 `expires`，以及您要求的時間量 (以秒鐘為單位)。例如，以下範例影像 URL 擷取有效期為 1800 秒鐘的上載標記:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

影像的成功回應如下所示:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

將上載標記儲存到本機，以用於以後要求。

您可以在查詢 URL 字串中使用以下欄位來擷取上載標記:

| URL 參數 | 必要或選擇性 | 值 |
|--- |--- |--- |
| op | 必要 | get_uploadtoken |
| shared_secret | 必要 | 正在進行上載的公司共用密鑰。 |
| expires | 選擇性 | 上載標記有效的秒數。如果不指定，則預設為 300 秒鐘。 |

**範例影像 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**範例向量 URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**允許的 HTTP 方式:** GET 和 POST

您現在可以上載影像資產。

請參閱[上載影像資產](uploading-image-asset-or-vector.md#uploading_an_image_asset)。

## 上載影像資產 {#uploading-an-image-asset}

您擷取在指定時間內有效的上載標記後，即可上載影像資產。以 multipart/form post 形式上載資產，以 URL 查詢字串形式傳送值的其餘部分，如以下範例中所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

請參閱[擷取上載標記](uploading-image-asset-or-vector.md#retrieving_the_upload_token)。

請參閱[擷取共用密鑰](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)。

您還可以透過 URL 查詢字串的形式傳送其他可選值，如以下範例所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

The `file_limit` parameter specifies the file-size limit in bytes. `file_exts` 參數指定允許上載的文件副檔名。這兩個值都是可選的。

對於允許的檔案大小限制和檔案副檔名，在應用程式中設置全域限制。如果要求中所傳送的內容是全域限制的子集，則允許這一傳送。全域限制如下所示:

| 全域限制 | 值 |
|--- |--- |
| 所有用戶端的檔案大小 | 20 MB |
| 用於上載的支援影像檔案格式 | BMP、GIF、JPG、PNG、PSD |

使用者可透過下面的 HTML 表單上載資產。表單要求使用者輸入以下資訊:

* 公司名稱.
* 上載標記.
* 檔案大小限制.
* 檔案副檔名的清單.
* 是否保留與資產相關聯的顏色配置檔案和檔案名。
* 是否使用挖空背景。 如果啟用「挖空背景」，請設定「拐角」(Corner)、「公差」(Tolerance)和「填充」(Fill)方法。 請參閱上傳時影像編 [輯選項中的挖空背景](image-editing-options-upload.md#image-editing-options-at-upload)。
* 待上載檔案的名稱

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

您可以按一下下列連結，檢視與上述表單關聯的HTML原始碼：

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

在Firefox中，在瀏覽器視窗中按一下滑鼠右鍵，然後按一下「檢視頁 **面來源」**。 代碼顯示當使用者按一下「**送出**」時執行的對應 URL 查詢字串和 POST 方式。

若要在 Internet Explorer 中檢視 XML 回應，請按一下「**檢視 > 原始檔**」。To view XML response in Firefox, click **Tools > Web Developer > Page Source**. 建議使用 Firefox 檢視 XML 回應。

下面是成功上載的範例回應:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>上載的資產 (JPG、GIF 等) 轉換為 PTIFF 格式，回應會傳送該 PTIFF 資產的直接連結。

該資產類似於任何其他的影像伺服資源；您可以對其套用處理查詢。例如，以下 URL 要求延伸到指定寬度和高度的資產。

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

以 multipart/form post 形式傳送要上載的資產，以 URL 查詢字串形式傳送值的其餘部分。您可以在 URL 查詢字串中使用以下欄位來上載資產:

| URL 參數 | 必要或選擇性 | 值 |
|--- |--- |--- |
| op | 必要 | 上載 |
| upload_token | 必要 | 與公司關聯的共用密鑰上載標記。 |
| company_name | 必要 | 執行上載的公司名稱。 |
| file_limit | 選擇性 | 資產的檔案大小限制 (以位元組為單位)。 |
| file_exts | 選擇性 | 影像資產檔案允許的副檔名清單。 |
| preserve_colorprofile | 選擇性 | 用於在將上載檔案轉換成 PTIFF 格式時保留任何內嵌的色彩設定檔。可能的值為 true 或 false。預設為 false。 |
| preserve_filename | 選擇性 | 保留所上載資產的檔案名稱。可能的值為 true 或 false。預設為 false。 |

>[!NOTE]
>
>須將待上載資產作為 multipart POST 要求中的唯一欄位傳送。

**範例 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**允許的 HTTP 方式:**

POST

### 取得影像的資產中繼資料 {#getting-asset-metadata-for-images}

您可以使用 `image_info`   擷取所上載資產的中繼資料，如以下範例中所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

成功回應的範例如下所示:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查詢字串中使用以下欄位要求有關資產的資訊:

| URL 參數 | 必要或選擇性 | 值 |
|--- |--- |--- |
| op | 必要 | image_info |
| shared_secret | 必要 | 公司的共用密鑰。 |
| image_name | 必要 | 影像的名稱。 |

**範例 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**允許的 HTTP 方式:**

GET 和 POST

## 上載向量資產 {#uploading-a-vector-asset}

您擷取在指定時間內有效的上載標記後，即可上載向量資產。以 multipart/form post 形式上載資產，以 URL 查詢字串形式傳送值的其餘部分，如以下範例中所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

請參閱[擷取上載標記](uploading-image-asset-or-vector.md#retrieving_the_upload_token)。

請參閱[擷取共用密鑰](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)。

您還可以透過 URL 查詢字串的形式傳送其他可選值，如以下範例所示:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. `file_exts` 參數指定允許上載的文件副檔名。這兩個值都是可選的。

對於允許的檔案大小限制和檔案副檔名，在應用程式中設置全域限制。如果要求中所傳送的內容是全域限制的子集，則允許這一傳送。全域限制如下所示:

| 全域限制 | 值 |
|--- |--- |
| 所有用戶端的檔案大小 | 20 MB |
| 用於上載的支援向量檔案格式 | AI、EPS、PDF (只有當 PDF 先前使用 Adobe Illustrator CS6 來開啟並儲存時) |

使用者可透過下面的 HTML 表單上載資產。表單要求使用者輸入以下資訊:

* 公司名稱.
* 上載標記.
* 檔案大小限制.
* 檔案副檔名的清單.
* 是否保留與資產相關聯的顏色配置檔案和檔案名。
* 是否使用挖空背景。 如果啟用「挖空背景」，請設定「拐角」(Corner)、「公差」(Tolerance)和「填充」(Fill)方法。 請參閱上傳時影像編 [輯選項中的挖空背景](image-editing-options-upload.md#image-editing-options-at-upload)。
* 待上載檔案的名稱

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

當您在瀏覽器視窗中按一下右鍵，然後針對圖中顯示的表單按一下「**檢視來源**」時，將顯示以下 HTML 代碼。代碼顯示當使用者按一下「**送出**」時執行的對應 URL 查詢字串和 POST 方式。

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

若要在 Internet Explorer 中檢視 XML 回應，請按一下「**檢視** > **原始檔**」。若要在 Firefox 中檢視 XML 回應，請按一下「**檢視** > **網頁原始碼**」。建議使用 Firefox 檢視 XML 回應。

下面是成功上載的範例回應:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>上載的資產 (AI、EPS、PDF 等) 轉換為 FXG 格式，回應會傳送該 FXG 資產的直接連結。

該資產類似於任何其他的網路印刷資源；您可以對其套用處理查詢。例如，下列 URL 會將 FXG 資源轉換為 500x500 png 影像。

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

以 multipart/form post 形式傳送要上載的資產，以 URL 查詢字串形式傳送值的其餘部分。您可以在 URL 查詢字串中使用以下欄位來上載資產:

| URL 參數 | 必要或選擇性 | 值 |
|--- |--- |--- |
| op | 必要 | 上載 |
| upload_token | 必要 | 與公司關聯的共用密鑰上載標記。 |
| company_name | 必要 | 執行上載的公司名稱。 |
| file_limit | 選擇性 | 資產的檔案大小限制 (以位元組為單位)。 |
| file_exts | 選擇性 | 資產檔案允許的副檔名清單。 |

>[!NOTE]
>
>須將待上載資產作為 multipart POST 要求中的唯一欄位傳送。

**範例 URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**允許的 HTTP 方式:**

POST
