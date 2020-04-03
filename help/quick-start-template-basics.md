---
title: '"快速入門: 基本範本"'
seo-title: '"快速入門: 基本範本"'
description: 'null'
seo-description: 簡介和範本入門快速入門，協助您快速上手使用。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template Basics{#quick-start-template-basics}

「範本基礎」是動態建立和可定址的圖層影像檔，例如Adobe Photoshop等影像編輯應用程式中的圖層檔案。 與包含圖層的靜態檔案 (如 PSD 檔案) 不同，範本可以包括參數。透過各種參數，影像的不同方面都可以定址及自訂。

>[!NOTE]
>
>您也可以使用「範本發佈」和Adobe Illustrator和Adobe InDesign的檔案，從版面設計建立範本。 請參閱[範本發佈](quick-start-template-publishing.md)。

範本可以包含任何數目的影像圖層和文字圖層。您可以將包含圖層（例如圖層PSD檔案）的靜態檔案轉換為範本，並在Dynamic Media Classic中建立範本。 可以使用上載到 SPS 中的字型在範本中建立文字圖層。將文字增加到範本中之後，可以透過變更其對齊方式、字型、字型大小以及色彩來設定字型格式。

透過「參數」畫面，可以將範本的任何方面轉換為可定址的參數。使用「參數」畫面時，可以變更要在範本中使用的分層影像或文字值。這些參數是透過 URL 字串傳遞的，因此可以透過變更任何參數，動態自訂從影像伺服器產生的回覆影像。

**快速入門**

本快速入門的設計理念是幫助您快速設定和使用基本範本。

**1. 上載檔案**

首先請為範本上載 PSD 檔案或影像檔案。除了PSD外，Dynamic Media Classic還支援許多影像檔案格式，但範本建議使用不失真的TIFF和PNG影像，因為它們允許透明度。

如果建置範本時使用的是 PSD 檔案，請在上載 PSD 檔案時，從「上載工作選項」對話框中選取「建立範本」選項。也選擇「圖層命名」選項，告訴Dynamic Media Classic如何在PSD圖層上傳至Scene7 Publishing System時命名。

如果使用的是影像檔案，可以裁切影像，也可以上載時在影像中從剪裁路徑建立遮色片。

在全域導覽列上選取「上載」按鈕，將 PSD 檔案或其他影像檔案從電腦上載到 SPS 上的檔案夾中。請參閱[上載範本檔案](uploading-template-files.md#uploading_template_files)。

**2. 建立範本**

若要從 PSD 檔案建立範本，請在上載檔案時選取「建立範本」選項。若要從影像建立範本，請選擇「建置 > 基本範本」，輸入畫布的寬度和高度度量值，選取「設計師」或「開發人員」，並將影像拖曳到「範本」畫面上。也可以先選取影像，然後再選取「建置 > 基本範本」。「範本」畫面提供了以下工具:

* 增加影像圖層。若要增加圖層，請將影像拖曳到「範本」畫面中。
* 增加文字圖層。選取文字工具 並拖曳來繪製文字圖層方框；然後使用「文字」畫面上的工具來設定文字格式。
* 變更圖層大小和位置。
* 變更圖層順序。
* 將陰影和光暈效果套用於影像圖層和文字圖層。

請參閱[建立範本](creating-template.md#creating_a_template)。

**3. 建立範本參數**

接下來是將圖層屬性參數化，從而確定 URL 字串中包含哪些圖層屬性。您可以透過這些參數盡可能靈活地使用範本。圖層屬性參數化之後，可以動態進行變更。

若要參數化圖層，請在「範本」畫面中開啟範本，並選取圖層名稱旁邊的「參數」按鈕。在「參數」畫面上，選取要增加的各個參數旁邊的選項。請參閱[建立範本參數](creating-template-parameters.md#creating_template_parameters)。

**4. 發佈範本**

發佈範本時，範本會放在動態媒體影像伺服器上，以便動態傳遞至您的網站或應用程式。 發佈功能也會啟動URL，將範本從動態媒體影像伺服器呼叫至您的網站或應用程式。

請確保發佈與範本相關的所有影像。

若要發佈範本，請將其標記為發佈，接著在全域導覽列上選取「發佈」按鈕。然後選取「開始發佈」按鈕。請參閱[發佈範本](publishing-templates.md#publishing_templates)。

**5. 將範本連結至網頁**

Dynamic Media Classic會建立範本的URL，並在您發佈範本至動態媒體影像伺服器時啟動URL。 可以從「範本預覽」畫面複製這些 URL 字串。

在瀏覽面板中選取範本，然後按一下「預覽」按鈕，開啟「範本預覽」畫面。然後選取「影像預設集」來傳送範本，並選取「複製 URL」按鈕。從「預覽」畫面複製 URL 之後，就可以將它用於網站或應用程式。請參閱[將範本連結至網頁](linking-template-web-page.md#linking_a_template_to_a_web_page)。
