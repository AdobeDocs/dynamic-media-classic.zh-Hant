---
title: 上傳點陣化影像資產
description: 瞭解如何將點陣影像資產上傳至Adobe Dynamic Media Classic
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 67%

---

# 上傳點陣化影像資產 {#uploading-an-image-asset-or-a-vector-asset}

您必須先要求一個共用密鑰，然後才能上載影像資產。使用此共用密鑰來擷取上載標記。然後使用上傳Token來上傳點陣影像資產。

>[!IMPORTANT]
>
>自2023年5月1日起，Dynamic Media中的UGC資產最多可在上傳日期後60天內使用。 60天後，資產將會移除。

>[!NOTE]
>
>Adobe Dynamic Media Classic已於2021年9月30日終止支援新的或現有的UGC向量資產。

## 要求共用秘密金鑰 {#requesting-a-shared-secret-key}

請求 *共用秘密金鑰* 作者： [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，要求共用秘密金鑰。

在電子郵件中，請提供想要用於上載影像資產的公司名稱。從Adobe Dynamic Media Classic收到金鑰後，請儲存於本機以供日後使用。

## 擷取上傳權杖 {#retrieving-the-upload-token}

*上載標記*&#x200B;將確保他人不能使用相同的共用密鑰來上載資產。它確保上載合法且來自信任的來源。

上載標記是字母數字字串，只能在指定時間內使用。使用下列URL取代您的共用秘密金鑰，以便擷取上傳權杖。

* 點陣影像
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`在此範例中，共用秘密金鑰為 `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

根據預設，上載標記在您擷取之後 5 分鐘 (300 秒) 便過期。若需要求更多時間，請在 URL 中加上 `expires`，以及您要求的時間量 (以秒鐘為單位)。例如，以下範例影像 URL 擷取有效期為 1800 秒鐘的上載標記:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

影像的成功回應如下所示：

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
| --- | --- | --- |
| op | 必要 | get_uploadtoken |
| shared_secret | 必要 | 正在進行上載的公司共用密鑰。 |
| expires | 選擇性 | 上載標記有效的秒數。如果不指定，則預設為 300 秒鐘。 |

**點陣影像URL範例：**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**允許的HTTP方法：**
`GET` 和 `POST`

您現在可以上載影像資產。

另請參閱 [上傳影像資產](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## 上傳點陣化影像資產 {#uploading-an-image-asset}

您擷取在指定時間內有效的上載標記後，即可上載影像資產。以 multipart/form post 形式上載資產，以 URL 查詢字串形式傳送值的其餘部分，如以下範例中所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

此 `upload_token` 和 `company_name` 欄位為必填欄位。

另請參閱 [擷取上傳權杖](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

另請參閱 [擷取共用秘密金鑰](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

您還可以透過 URL 查詢字串的形式傳送其他可選值，如以下範例所示:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

此 `file_limit` parameter指定檔案大小限制（位元組）。 `file_exts` 參數指定允許上載的文件副檔名。這兩個值都是可選的。

對於允許的檔案大小限制和檔案副檔名，在應用程式中設置全域限制。如果要求中所傳送的內容是全域限制的子集，則允許這一傳送。全域限制如下所示:

| 全域限制 | 值 |
| --- | --- |
| 所有用戶端的檔案大小 | 20 MB |
| 用於上載的支援影像檔案格式 | BMP、GIF、JPG、PNG、PSD，TIFF |

使用者可透過下面的 HTML 表單上載資產。表單要求使用者輸入以下資訊:

* 公司名稱.
* 上載標記.
* 檔案大小限制.
* 檔案副檔名的清單.
* 是否要保留與資產相關聯的色彩設定檔和檔案名稱。
* 是否要使用去底色背景。 如果您啟用「去底色背景」，請設定「轉角」、「公差」和「填色」方法。
請參閱中的去底色背景 [上傳時影像微調選項](image-editing-options-upload.md#image-editing-options-at-upload).
* 待上載檔案的名稱.

您可以選取「 」，檢視與上述表單相關聯的HTML原始碼 [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

在Firefox中，在瀏覽器視窗中按一下滑鼠右鍵，然後選取 **[!UICONTROL 檢視頁面來源]**. 代碼顯示當使用者按一下「**[!UICONTROL 送出]**」時執行的對應 URL 查詢字串和 POST 方式。

若要在Internet Explorer中檢視XML回應，請前往 **[!UICONTROL 檢視]** > **[!UICONTROL 來源]**. 若要在Firefox中檢視XML回應，請前往 **[!UICONTROL 工具]** > **[!UICONTROL 瀏覽器工具]** > **[!UICONTROL Web開發人員工具]**. 建議使用 Firefox 檢視 XML 回應。

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
| --- | --- | --- |
| `op` | 必要 | 上載 |
| `upload_token` | 必要 | 與公司關聯的共用密鑰上載標記。 |
| `company_name` | 必要 | 執行上載的公司名稱。 |
| `file_limit` | 選擇性 | 資產的檔案大小限制 (以位元組為單位)。 |
| `file_exts` | 選擇性 | 影像資產檔案允許的副檔名清單。 |
| `preserve_colorprofile` | 選擇性 | 用於在將上載檔案轉換成 PTIFF 格式時保留任何內嵌的色彩設定檔。可能的值為 true 或 false。預設為 false。 |
| `preserve_filename` | 選擇性 | 保留所上載資產的檔案名稱。可能的值為 true 或 false。預設為 false。 |

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

成功回應的範例如下所示：

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
| --- | --- | --- |
| `op` | 必要 | image_info |
| `shared_secret` | 必要 | 公司的共用密鑰。 |
| `image_name` | 必要 | 影像的名稱。 |

**範例 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**允許的 HTTP 方式:**

GET 和 POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->