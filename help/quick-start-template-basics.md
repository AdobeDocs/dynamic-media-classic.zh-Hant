---
title: '"快速入門: 基本範本"'
description: 簡介和範本基礎快速入門可協助您在Adobe Dynamic Media Classic中快速上手並執行。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 28%

---

# 快速入門: 基本範本{#quick-start-template-basics}

「範本基本須知」是動態建立和可定址的分層影像檔案，例如影像編輯應用程式(如Adobe Photoshop)中的分層檔案。 與包含圖層的靜態檔案 (如 PSD 檔案) 不同，範本可以包括參數。透過各種參數，影像的不同方面都可以定址及自訂。

範本可以包含任何數目的影像圖層和文字圖層。您可以將包含圖層的靜態檔案(如分層PSD檔案)轉換為範本，並在Adobe Dynamic Media Classic中建立範本。 您可以使用上傳至Adobe Dynamic Media Classic的字型，在範本中建立文字層。 將文字增加到範本中之後，可以透過變更其對齊方式、字型、字型大小以及色彩來設定字型格式。

使用「參數」頁，您可以將範本的任何方面轉換為可定址的參數。 使用「參數」畫面時，可以變更要在範本中使用的分層影像或文字值。這些參數是透過 URL 字串傳遞的，因此可以透過變更任何參數，動態自訂從影像伺服器產生的回覆影像。

另請參閱[範本基本知識](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)訓練影片。

此快速入門旨在讓您透過範本基本知識快速上手並執行。

## 1.上傳檔案

首先請為範本上載 PSD 檔案或影像檔案。Adobe Dynamic Media Classic除了支援PSD外，還支援許多影像檔案格式，但建議範本使用無損TIFF和PNG影像，因為它們允許透明。

如果您使用PSD檔案來建立模板，請在上傳PSD檔案時，在&#x200B;**[!UICONTROL 上傳作業選項]**&#x200B;對話方塊上選擇&#x200B;**[!UICONTROL 建立範本]**。 也選擇&#x200B;**[!UICONTROL 「圖層命名」]**&#x200B;選項，讓Adobe Dynamic Media Classic知道在PSD圖層上傳至Adobe Dynamic Media Classic時如何為其命名。

如果使用的是影像檔案，可以裁切影像，也可以上載時在影像中從剪裁路徑建立遮色片。

在全局導航欄上，選擇&#x200B;**[!UICONTROL Upload]**&#x200B;以將PSD檔案或其他影像檔案從您的電腦上載到Adobe Dynamic Media Classic上的資料夾。 請參閱[上傳範本檔案](uploading-template-files.md#uploading_template_files)。

## 2.建立範本

要從PSD檔案建立模板，請在上載檔案時選擇&#x200B;**[!UICONTROL 建立模板]**。 若要從影像建立範本，請在全域導覽列上前往&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Template Basics]**，輸入畫布的寬度和高度測量。 在頁面的右上角附近，選擇&#x200B;**[!UICONTROL Designer]**&#x200B;或&#x200B;**[!UICONTROL Developer]**，然後將影像拖曳至「範本」頁面。 您也可以在&#x200B;*之前選取影像*，前往&#x200B;**[!UICONTROL Build]** > **[!UICONTROL 範本基礎]**。 「模板」頁提供以下工具：

* 增加影像圖層。若要新增圖層，請將影像拖曳至「範本」頁面。
* 增加文字圖層。選取&#x200B;**[!UICONTROL 文字工具]**&#x200B;圖示。 拖曳指標以建立文字層的方塊；然後使用「文本」(Text)頁面上的工具設定文本格式。
* 變更圖層大小和位置。
* 變更圖層順序。
* 將陰影和光暈效果套用於影像圖層和文字圖層。

請參閱[建立範本](creating-template.md#creating_a_template)。

## 3.建立範本參數

接下來是將圖層屬性參數化，從而確定 URL 字串中包含哪些圖層屬性。您可以透過這些參數盡可能靈活地使用範本。圖層屬性參數化之後，可以動態進行變更。

要參數化圖層，請在「模板」頁中開啟模板，然後選擇圖層名稱旁的&#x200B;**[!UICONTROL 參數]**。 在「參數」頁面上，選取您要新增之每個參數旁的選項。 請參閱[建立範本參數](creating-template-parameters.md#creating_template_parameters)。

## 4.發佈範本

發佈範本後，範本會放置在Dynamic Media影像伺服器上，以便動態傳遞至您的網站或應用程式。 發佈也會啟用URL，從Dynamic Media影像伺服器呼叫範本至您的網站或應用程式。

請確保發佈與範本相關的所有影像。

若要發佈範本，請將其標示為發佈，然後在全域導覽列上，選取&#x200B;**[!UICONTROL Publish]**。 然後選擇&#x200B;**[!UICONTROL 提交發佈]**。 請參閱[發佈範本](publishing-templates.md#publishing_templates)。

## 5.將模板連結到網頁

Dynamic Media Classic會為範本建立URL，並在您將範本發佈至Dynamic Media影像伺服器時啟用URL。 您可以從「範本預覽」頁面複製這些URL字串。

在「瀏覽」面板中選擇模板，然後選擇&#x200B;**[!UICONTROL Preview]**&#x200B;以開啟「模板預覽」頁。 選擇用於傳遞模板的影像預設集，然後選擇&#x200B;**[!UICONTROL 複製URL]**。 從「預覽」頁面複製URL後，即可在您的網站或應用程式中使用它。 請參閱[將範本連結到網頁](linking-template-web-page.md#linking_a_template_to_a_web_page)。
