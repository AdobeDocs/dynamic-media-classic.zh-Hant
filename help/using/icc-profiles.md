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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 41%

---

# ICC 設定檔{#icc-profiles}

ICC （國際色彩聯盟）設定檔是一個檔案，說明如何正確地將影像檔案從一個色彩空間轉換到另一個色彩空間。 ICC 設定檔有助於為影像獲取正確的色彩。例如，若要正確顯示設計成要在電腦熒幕上列印的影像，您可以選擇ICC設定檔。 該設定檔將影像轉換到不同的 色域並確保色彩正確地在線上顯示。

在Adobe Dynamic Media Classic中，您可以在上傳影像時，選擇ICC設定檔將影像轉換為不同的色域。 Adobe Dynamic Media Classic預設提供所有標準Photoshop ICC設定檔。 若要在「上載」畫面中查看色彩設定檔的名稱，請選取「色彩設定檔」選單。然後選擇「自訂來源」>「目標」，並在「轉換自」和「轉換至」功能表上選擇ICC設定檔名稱。

在上傳](image-editing-options-upload.md#image-editing-options-at-upload)檢視[影像編輯選項。

除了使用預設的ICC設定檔之外，您還可以將其他ICC設定檔上傳到Adobe Dynamic Media Classic，以便用於色域轉換。 切換至「瀏覽」面板中的「詳細檢視」，以調查ICC設定檔的設定檔類別、色域型別和PCS型別。

## 上傳ICC設定檔 {#uploading-icc-profiles}

透過與上載檔案時所使用的相同技術上載 ICC 設定檔。您可以將ICC設定檔儲存在任何Adobe Dynamic Media Classic資料夾中。

檢視[上傳您的檔案](uploading-files.md#uploading_your_files)。

## 檢查ICC設定檔 {#examining-an-icc-profile}

若要檢查ICC設定檔，請在「瀏覽」面板中選取該設定檔，並在「詳細資料檢視」中顯示它。 「詳細資料檢視」提供下列有關ICC設定檔的資訊：

* **[!UICONTROL 設定檔類別]**： ICC （國際色彩聯盟）定義每個類別以涵蓋應用程式型別。 例如，輸入設定檔套用於數位相機和掃描器等裝置，輸出設定檔套用於印表機。

* **[!UICONTROL 色域型別]**：此數字是設定檔的「輸入」色域，如ICC所定義。 色域類型可定義色域的組件數目和對這些組件的解釋。例如，RGB 是具有三個組件 (紅色、綠色和藍色) 的 色域。色域類型並不定義該色域的特定色彩特性 (例如，原色的色度)。

* **[!UICONTROL PCS型別]**：此PCS型別是設定檔的「輸出」色域 — 其設定檔連線色域。 例如，色彩設定檔可以將 RGB 轉換成 PCS，然後轉換成 CMYK。

對於有助於標記色彩或影像的輸入、顯示或輸出設定檔，PCS 類型是 XYZ 或 Lab。將該設定檔解釋成在 ICC 規格中定義的相應特定色域。
