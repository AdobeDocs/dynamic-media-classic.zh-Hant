---
title: ICC （國際色彩聯盟）設定檔
description: 瞭解Adobe Dynamic Media Classic中的ICC設定檔。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5cf4a3f436cd6dd46ee68daeb0ef798402ae311a
workflow-type: tm+mt
source-wordcount: 527
ht-degree: 29%

---

# ICC 設定檔{#icc-profiles}

ICC （國際色彩聯盟）設定檔是一個檔案，說明如何正確地將影像檔案從一個色彩空間轉換到另一個色彩空間。 ICC 設定檔有助於為影像獲取正確的色彩。 例如，要正確地顯示用於電腦顯示器上列印的影像，可以選擇 ICC 設定檔。 該設定檔將影像轉換到不同的 色域並確保色彩正確地在線上顯示。

在Adobe Dynamic Media Classic中，您可以在上傳影像時，選擇ICC設定檔將影像轉換為不同的色域。 Adobe Dynamic Media Classic預設提供所有標準Adobe Photoshop ICC設定檔。 若要在「上載」畫面中查看色彩設定檔的名稱，請選取「色彩設定檔」選單。 然後按一下&#x200B;**自訂從** > **到**，並在&#x200B;**轉換自**&#x200B;和&#x200B;**轉換成**&#x200B;功能表上選擇ICC設定檔名稱。

在上傳](image-editing-options-upload.md#image-editing-options-at-upload)檢視[影像編輯選項。

除了使用預設的ICC設定檔之外，您還可以將其他ICC設定檔上傳到Adobe Dynamic Media Classic，以便用於色域轉換。 若要調查ICC設定檔的設定檔類別、色域型別和PCS型別，請切換至「瀏覽」面板中的「詳細資料檢視」。

總而言之，ICC設定檔的關鍵點如下：

* ICC設定檔可為影像檔案啟用不同色彩空間之間的正確色彩轉換。
* Adobe Dynamic Media Classic整合了所有標準Adobe Photoshop ICC設定檔，以實現強大的影像轉換。
* 自訂ICC設定檔可為進階色域轉換需求增加彈性。
* 在「詳細資料檢視」中檢視「設定檔類別」和「PCS型別」等詳細資料可協助您管理ICC設定。
* 上傳ICC設定檔非常簡單，而且可確保在[!DNL Adobe Dynamic Media Classic]中的資料夾之間存取。


## 上傳ICC設定檔 {#uploading-icc-profiles}

使用您用來上傳檔案的相同方法來上傳ICC設定檔。 您可以將ICC設定檔儲存在任何Adobe Dynamic Media Classic資料夾中。

檢視[上傳您的檔案](uploading-files.md#uploading_your_files)。

## 檢查ICC設定檔 {#examining-an-icc-profile}

若要檢查ICC設定檔，請在「瀏覽」面板中選取該設定檔，並在「詳細資料檢視」中顯示它。 「詳細資料檢視」提供下列有關ICC設定檔的資訊：

* **[!UICONTROL 設定檔類別]**： ICC定義每個類別以涵蓋應用程式型別。 例如，輸入設定檔適用於數位相機與掃描器等裝置。 輸出設定檔適用於印表機。

* **[!UICONTROL 色域型別]**：此值是設定檔的「輸入」色域，如ICC所定義。 色域類型可定義色域的組件數目和對這些組件的解釋。 例如，RGB 是具有三個組件 (紅色、綠色和藍色) 的 色域。 色域類型並不定義該色域的特定色彩特性 (例如，原色的色度)。

* **[!UICONTROL PCS型別]**：此PCS型別是設定檔的「輸出」色域 — 設定檔連線色域。 例如，色彩設定檔可以將 RGB 轉換成 PCS，然後轉換成 CMYK。

對於用於標籤顏色或影像的輸入、顯示或輸出設定檔，PCS型別是XYZ或Lab。 將該設定檔解釋成在 ICC 規格中定義的相應特定色域。
