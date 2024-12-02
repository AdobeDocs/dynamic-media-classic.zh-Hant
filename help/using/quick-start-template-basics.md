---
title: '快速入門: 基本範本'
description: 範本基本概念的簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速上手並執行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# 快速入門: 基本範本{#quick-start-template-basics}

範本基本概念是動態建立且可定址的分層影像檔案，例如Adobe Photoshop等影像編輯應用程式中的分層檔案。 與包含圖層的靜態檔案 (如 PSD 檔案) 不同，範本可以包括參數。透過各種參數，影像的不同方面都可以定址及自訂。

範本可以包含任何數目的影像圖層和文字圖層。您可以將包含圖層的靜態檔案(例如圖層PSD檔案)轉換為範本，並在Adobe Dynamic Media Classic中建立範本。 您可以使用上傳至Adobe Dynamic Media Classic的字型，在範本中建立文字圖層。 將文字新增至範本後，您可以變更文字齊行、字型、字型大小及顏色來格式化文字。

您可以在「引數」頁面將範本的任何方面轉換為可定址引數。 這樣做時，您可以變更要使用哪個圖層影像，或要在範本中使用的文字值。 引數會與URL字串一併傳遞，可讓您變更任何引數，以便動態自訂從影像伺服器產生的回覆影像。

另請觀看[基本範本](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)訓練影片。

本快速入門旨在協助您快速啟動並運用範本基本知識。

## 1.上傳檔案

首先請為範本上載 PSD 檔案或影像檔案。除了PSD之外，Adobe Dynamic Media Classic還支援許多影像檔案格式，但建議範本使用不失真TIFF和PNG影像，因為它們允許透明度。

如果您使用PSD檔案來建置範本，請在您上傳PSD檔案時選取&#x200B;**[!UICONTROL 上傳工作選項]**&#x200B;對話方塊中的&#x200B;**[!UICONTROL 建立範本]**。 同時選擇&#x200B;**[!UICONTROL 圖層命名]**&#x200B;選項，讓Adobe Dynamic Media Classic知道如何將PSD圖層上傳至Adobe Dynamic Media Classic時為其命名。

如果您使用影像檔案，您可以裁切影像，也可以在上傳影像時，從影像中的剪裁路徑建立遮色片。

在全域導覽列上，選取&#x200B;**[!UICONTROL 上傳]**，將PSD檔案或其他影像檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。 請參閱[上傳範本檔案](uploading-template-files.md#uploading_template_files)。

## 2.建立範本

若要從PSD檔案建立範本，請在上傳檔案時選取&#x200B;**[!UICONTROL 建立範本]**。 若要從影像建立範本，請在全域導覽列上，前往&#x200B;**[!UICONTROL 建置]** > **[!UICONTROL 範本基本知識]**，輸入畫布的寬度和高度測量。 在頁面的右上角附近，選取&#x200B;**[!UICONTROL Designer]**&#x200B;或&#x200B;**[!UICONTROL Developer]**，然後將影像拖曳至[範本]頁面。 您也可以在&#x200B;*之前選取影像，並移至&#x200B;**[!UICONTROL 建置]**>**[!UICONTROL 基本範本]**。*「範本」頁面提供下列工具：

* 增加影像圖層。若要新增圖層，請將影像拖曳至「範本」頁面。
* 增加文字圖層。選取&#x200B;**[!UICONTROL 文字工具]**&#x200B;圖示。 拖曳指標以建立文字圖層的方塊；然後使用「文字」頁面上的工具來格式化文字。
* 變更圖層大小和位置。
* 變更圖層順序。
* 將陰影和光暈效果套用於影像圖層和文字圖層。

請參閱[建立範本](creating-template.md#creating_a_template)。

## 3.建立範本引數

接下來是將圖層屬性參數化，從而確定 URL 字串中包含哪些圖層屬性。您可以透過這些參數盡可能靈活地使用範本。圖層屬性參數化之後，可以動態進行變更。

若要將圖層引數化，請在[範本]頁面中開啟範本，然後選取圖層名稱旁的&#x200B;**[!UICONTROL 引數]**。 在「引數」頁面上，選取您想要新增的每個引數旁的選項。 請參閱[建立範本引數](creating-template-parameters.md#creating_template_parameters)。

## 4. Publish範本

發佈範本時會將其置於Dynamic Media影像伺服器上，以便動態傳送至您的網站或應用程式。 發佈也會啟用URL，以將範本從Dynamic Media影像伺服器呼叫至您的網站或應用程式。

請確保發佈與範本相關的所有影像。

若要發佈範本，請將其標籤為發佈，並在全域導覽列上選取&#x200B;**[!UICONTROL Publish]**。 然後選取&#x200B;**[!UICONTROL 提交Publish]**。 請參閱[Publish範本](publishing-templates.md#publishing_templates)。

## 5.將範本連結至網頁

Dynamic Media Classic會為範本建立URL，並在您將範本發佈至Dynamic Media影像伺服器時啟用URL。 您可以從「範本預覽」頁面複製這些URL字串。

在[瀏覽]面板中選取您的範本，然後選取[**[!UICONTROL 預覽]**]以開啟[範本預覽]頁面。 選擇影像預設集以傳遞您的範本，然後按一下「**[!UICONTROL 複製URL]**」按鈕。 從「預覽」頁面複製URL後，即可在您的網站或應用程式中使用。 請參閱[將範本連結至網頁](linking-template-web-page.md#linking_a_template_to_a_web_page)。
