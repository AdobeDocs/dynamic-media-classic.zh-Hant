---
title: ICC 設定檔
seo-title: ICC 設定檔
description: 'null'
seo-description: 瞭解ICC設定檔。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC 設定檔{#icc-profiles}

ICC (國際色彩聯盟) 設定檔是描述如何正確地將影像檔案從一個 色域轉換到另一個 色域的檔案。ICC 設定檔有助於為影像獲取正確的色彩。例如，要正確地顯示用於電腦顯示器上列印的影像，可以選擇 ICC 設定檔。該設定檔將影像轉換到不同的 色域並確保色彩正確地在線上顯示。

在 Scene7 Publishing System 中，在上載影像時，可以選擇一個 ICC 設定檔以將影像轉換到不同的 色域。根據 SPS 預設，所有標準的 Photoshop ICC 設定檔都是可用的。若要在「上載」畫面中查看色彩設定檔的名稱，請選取「色彩設定檔」選單。然後選擇「自訂轉換」，再從「轉換自」和「轉換到」選單中選擇 ICC 設定檔的名稱。請參閱[上載時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload)。

除使用預設的 ICC 設定檔外，您還可以上載其他 ICC 設定檔到 SPS 上，使其可用於 色域轉換。在瀏覽面板中切換到詳細檢視，以便調查 ICC 設定檔的設定檔類別、 色域類型和 PCS 類型。

## 上載 ICC 設定檔 {#uploading-icc-profiles}

透過與上載檔案時所使用的相同技術上載 ICC 設定檔。您可以將 ICC 設定檔儲存在任何 SPS 檔案夾中。請參閱[上載檔案](uploading-files.md#uploading_your_files)。

## 檢查 ICC 設定檔 {#examining-an-icc-profile}

若要檢查 ICC 設定檔，請在瀏覽面板中選取該文件並在詳細檢視中進行顯示。詳細檢視提供有關 ICC 設定檔的以下資訊:

**描述檔類別** ICC(International Color Consortium)定義每個類別以涵蓋應用程式類型。 例如，輸入設定檔套用於數位相機和掃描器等裝置，輸出設定檔套用於印表機。

**色域類型** ：此數字是ICC所定義的描述檔的「輸入」色域。 色域類型可定義色域的組件數目和對這些組件的解釋。例如，RGB 是具有三個組件 (紅色、綠色和藍色) 的 色域。色域類型並不定義該色域的特定色彩特性 (例如，原色的色度)。

**PCS類型** ：此PCS類型是配置檔案的「輸出」顏色空間，即其配置檔案連接空間。 例如，色彩設定檔可以將 RGB 轉換成 PCS，然後轉換成 CMYK。

對於有助於標記色彩或影像的輸入、顯示或輸出設定檔，PCS 類型是 XYZ 或 Lab。將該設定檔解釋成在 ICC 規格中定義的相應特定色域。
