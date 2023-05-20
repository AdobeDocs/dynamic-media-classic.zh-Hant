---
title: "快速入門: 基本範本"
description: 簡介和快速入門模板基礎知識，幫助您快速在Adobe Dynamic Media Classic啟動和運行。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 28%

---

# 快速入門: 基本範本{#quick-start-template-basics}

模板基礎資訊是動態建立和可定址的分層影像檔案，如影像編輯應用程式(如Adobe Photoshop)中的分層檔案。 與包含圖層的靜態檔案 (如 PSD 檔案) 不同，範本可以包括參數。透過各種參數，影像的不同方面都可以定址及自訂。

範本可以包含任何數目的影像圖層和文字圖層。可以將包含層(如分層PSD檔案)的靜態檔案轉換為模板，並在Adobe Dynamic Media Classic建立模板。 可以使用上傳到Adobe Dynamic Media Classic的字型在模板中建立文本圖層。 將文字增加到範本中之後，可以透過變更其對齊方式、字型、字型大小以及色彩來設定字型格式。

使用「參數」(Parameters)頁，可以將模板的任何方面轉換為可定址的參數。 使用「參數」畫面時，可以變更要在範本中使用的分層影像或文字值。這些參數是透過 URL 字串傳遞的，因此可以透過變更任何參數，動態自訂從影像伺服器產生的回覆影像。

另請參閱 [模板基礎知識](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 培訓視頻。

此快速入門旨在利用模板基礎知識快速啟動和運行。

## 1。上載檔案

首先請為範本上載 PSD 檔案或影像檔案。Adobe Dynamic Media Classic除了支援PSD外，還支援許多影像檔案格式，但建議對模板使用無損TIFF和PNG影像，因為它們允許透明。

如果使用PSD檔案構建模板，請選擇 **[!UICONTROL 建立模板]** 的 **[!UICONTROL 上載作業選項]** 對話框。 另選 **[!UICONTROL 層命名]** 選項，因此Adobe Dynamic Media Classic知道在將PSD層上傳到Adobe Dynamic Media Classic時如何命名。

如果使用的是影像檔案，可以裁切影像，也可以上載時在影像中從剪裁路徑建立遮色片。

在全局導航欄上，選擇 **[!UICONTROL 上載]** 將PSD檔案或其他映像檔案從您的電腦上載到Adobe Dynamic Media Classic上的資料夾。 請參閱 [上載模板檔案](uploading-template-files.md#uploading_template_files)。

## 2.建立模板

要從PSD檔案建立模板，請選擇 **[!UICONTROL 建立模板]** 上載檔案。 要從影像建立模板，請在「全局導航」欄上，轉到 **[!UICONTROL 生成]** > **[!UICONTROL 模板基礎知識]**，輸入畫布的寬度和高度度量。 在頁面右上角附近，選擇 **[!UICONTROL 設計師]** 或 **[!UICONTROL 開發人員]**，然後將影像拖到「模板」頁。 也可以選擇影像 *先* 你去 **[!UICONTROL 生成]** > **[!UICONTROL 模板基礎知識]**。 「模板」頁提供了以下工具：

* 增加影像圖層。要添加圖層，請將影像拖到「模板」頁中。
* 增加文字圖層。選擇 **[!UICONTROL 文本工具]** 表徵圖 拖動指針為文本圖層建立框；然後使用「文本」(Text)頁面上的工具設定文本格式。
* 變更圖層大小和位置。
* 變更圖層順序。
* 將陰影和光暈效果套用於影像圖層和文字圖層。

請參閱 [建立模板](creating-template.md#creating_a_template)。

## 3.建立模板參數

接下來是將圖層屬性參數化，從而確定 URL 字串中包含哪些圖層屬性。您可以透過這些參數盡可能靈活地使用範本。圖層屬性參數化之後，可以動態進行變更。

要參數化圖層，請在「模板」頁面中開啟模板，然後選擇 **[!UICONTROL 參數]** 圖層名稱旁邊。 在「參數」(Parameters)頁面上，選擇要添加的每個參數旁邊的選項。 請參閱 [建立模板參數](creating-template-parameters.md#creating_template_parameters)。

## 4.發佈模板

發佈模板將其放在Dynamic Media映像伺服器上，以便可以動態地將其傳送到您的網站或應用程式。 發佈還激活URL，將模板從Dynamic Media映像伺服器調用到您的網站或應用程式。

請確保發佈與範本相關的所有影像。

要發佈模板，請將其標籤為發佈，並在全局導航欄上，選擇 **[!UICONTROL 發佈]**。 然後選擇 **[!UICONTROL 提交發佈]**。 請參閱 [發佈模板](publishing-templates.md#publishing_templates)。

## 5.將模板連結到網頁

Dynamic Media Classic為模板建立URL，並在將模板發佈到Dynamic Media影像伺服器時激活URL。 可以從「模板預覽」頁複製這些URL字串。

在「瀏覽面板」中選擇模板，然後選擇 **[!UICONTROL 預覽]** 開啟「模板預覽」頁。 選擇用於傳遞模板的影像預設，然後選擇 **[!UICONTROL 複製URL]**。 從「預覽」頁複製URL後，可以在網站或應用程式中使用它。 請參閱[將範本連結到網頁](linking-template-web-page.md#linking_a_template_to_a_web_page)。
