---
title: 升級整備
description: 當您想要在 [!DNL Adobe Experience Manager]從 [!DNL Adobe Dynamic Media Classic] 推進到 [!DNL Dynamic Media] 時，提供升級整備檢查清單。
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# 升級整備檢查清單

使用下列檢查清單協助您瞭解並準備從[!DNL Dynamic Media Classic]升級至[!DNL Dynamic Media]。

|  | 工作 | 說明 |
| :--- | :--- | --- |
| **階段1：授權** | 執行合約 | 根據流量和儲存空間，Adobe帳戶團隊會與您合作，從[!DNL Dynamic Media Classic]授權轉換，以便在[!DNL Dynamic Media]授權上續約。 |
| **階段2：準備** | 驗證功能使用情況 | 確認[!DNL Dynamic Media Classic]中使用的功能在[!DNL Dynamic Media]中可用。 請參閱[功能比較](/help/using/upgrade-feature-comparison.md)頁面。 [!DNL Dynamic Media]中尚未提供的金鑰功能包括下列專案：<br>·視覺化組態程式（影像作者、影像轉譯）。<br>·影像範本（1:1範本）。<br>· eCatalogs。<br>如果使用上述功能，升級仍可進行，並假設這些功能可透過[!DNL Dynamic Media Classic]存取。 |
|   | 識別資產 | 尋找並準備好要用於升級的資產和預設集。 |
| **階段3：環境** | 升級[!DNL Adobe Experience Manager] | [!DNL Adobe Experience Manager]的所有執行個體都必須更新至最新版本。 |
|   | 設定[!DNL Dynamic Media] | Adobe Consulting或合作夥伴會使用您的認證設定[!DNL Dynamic Media]。 |
| **階段4：升級** | 復寫資產 | 在升級程式期間，會將指定的[!DNL Dynamic Media Classic]資產復寫到Dynamic Media。 |
| **階段5：系統管理設定** | 設定使用者與許可權 | 建立使用者並授與適當的許可權。 |
|   | 設定視訊編碼設定檔 | 建立視訊編碼設定檔。 |
|   | 設定檢視器預設集 | 建立檢視器預設集。 |
|   | 設定影像預設集 | 設定影像預設集。 |
| **階段6：驗證** | 驗證 | 驗證使用案例、資產、連結和API。 |
