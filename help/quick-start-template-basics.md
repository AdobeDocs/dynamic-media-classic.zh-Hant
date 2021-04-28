---
title: '"快速入門: 基本範本"'
description: 簡介和範本入門快速入門，協助您快速上手使用。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media經典
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Quick Start: Template Basics{#quick-start-template-basics}

「範本基礎」是動態建立和可定址的分層影像檔案，例如影像編輯應用程式(例如Adobe Photoshop)中的分層檔案。 與包含圖層的靜態檔案 (如 PSD 檔案) 不同，範本可以包括參數。透過各種參數，影像的不同方面都可以定址及自訂。

範本可以包含任何數目的影像圖層和文字圖層。您可以將包含圖層（例如圖層PSD檔案）的靜態檔案轉換為範本，並在Dynamic Media經典中建立範本。 您可以使用上傳至Dynamic Media經典的字型在範本中建立文字圖層。 將文字增加到範本中之後，可以透過變更其對齊方式、字型、字型大小以及色彩來設定字型格式。

使用「參數」頁，您可以將範本的任何方面轉換為可定址的參數。 使用「參數」畫面時，可以變更要在範本中使用的分層影像或文字值。這些參數是透過 URL 字串傳遞的，因此可以透過變更任何參數，動態自訂從影像伺服器產生的回覆影像。

本快速入門的設計理念是幫助您快速設定和使用基本範本。

## 1.上傳檔案

首先請為範本上載 PSD 檔案或影像檔案。Dynamic Media經典影像除了支援PSD以外，還支援許多影像檔案格式，但是建議範本使用不失真的TIFF和PNG影像，因為它們允許透明度。

如果您使用PSD檔案來建立範本，請在上傳PSD檔案時，在&#x200B;**[!UICONTROL 上傳工作選項]**&#x200B;對話方塊中選取&#x200B;**[!UICONTROL 建立範本]**。 也請選擇「**[!UICONTROL 圖層命名]**」選項，讓Dynamic Media經典知道如何在PSD圖層上傳至Dynamic Media經典時為它們命名。

如果使用的是影像檔案，可以裁切影像，也可以上載時在影像中從剪裁路徑建立遮色片。

在「全域導覽列」上，按一下「上傳」****，將PSD檔案或其他影像檔案從您的電腦上傳至「Dynamic Media經典」的檔案夾。 請參閱[上載範本檔案](uploading-template-files.md#uploading_template_files)。

## 2.建立範本

若要從PSD檔案建立範本，請在上傳檔案時選取「建立範本」。 ****&#x200B;若要從影像建立範本，請在全域導覽列上按一下「建立&#x200B;**** > **[!UICONTROL 範本基礎]**」，輸入畫布的寬度和高度測量。 在頁面的右上角附近，選擇&#x200B;**[!UICONTROL Designer]**&#x200B;或&#x200B;**[!UICONTROL Developer]**，然後將影像拖曳至「範本」頁面。 您也可以在&#x200B;*之前選擇*&#x200B;影像，按一下&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Template Basics]**。 「範本」頁面提供下列工具：

* 增加影像圖層。若要新增圖層，請將影像拖曳至「範本」頁面。
* 增加文字圖層。按一下&#x200B;**[!UICONTROL 文本工具]**&#x200B;表徵圖。 拖曳指針，為文字圖層建立方塊；然後，使用「文字」頁面上的工具設定文字格式。
* 變更圖層大小和位置。
* 變更圖層順序。
* 將陰影和光暈效果套用於影像圖層和文字圖層。

請參閱[建立範本](creating-template.md#creating_a_template)。

## 3.建立範本參數

接下來是將圖層屬性參數化，從而確定 URL 字串中包含哪些圖層屬性。您可以透過這些參數盡可能靈活地使用範本。圖層屬性參數化之後，可以動態進行變更。

要參數化圖層，請在「模板」頁中開啟模板，然後按一下圖層名稱旁的&#x200B;**[!UICONTROL Parameters]**。 在「參數」頁面上，選取您要新增之每個參數旁的選項。 請參閱[建立範本參數](creating-template-parameters.md#creating_template_parameters)。

## 4.發佈範本

發佈範本會將範本放在Dynamic Media影像伺服器上，以便動態傳遞至您的網站或應用程式。 發佈功能也會啟動URL，將範本從Dynamic Media影像伺服器呼叫至您的網站或應用程式。

請確保發佈與範本相關的所有影像。

若要發佈範本，請將範本標示為發佈，然後在全域導覽列上按一下&#x200B;**[!UICONTROL Publish]**。 然後按一下「提交發佈」。 ****&#x200B;請參閱[發佈範本](publishing-templates.md#publishing_templates)。

## 5.將範本連結至網頁

Dynamic Media經典會建立範本的URL，並在您發佈範本至Dynamic Media影像伺服器時啟動URL。 您可以從「範本預覽」頁面複製這些URL字串。

在「瀏覽面板」中選取範本，然後按一下「預覽」以開啟「範本預覽」頁面。 ****&#x200B;選擇影像預設集以傳送範本，然後按一下「複製URL」。 ****&#x200B;從「預覽」頁面複製URL後，即可在您的網站或應用程式中使用它。 請參閱[將範本連結至網頁](linking-template-web-page.md#linking_a_template_to_a_web_page)。
