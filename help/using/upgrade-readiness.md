---
title: 升級整備
description: 升級整備檢查清單(當您想從 [!DNL Adobe Dynamic Media Classic] 至 [!DNL Dynamic Media] 於 [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 1%

---

# 升級整備檢查清單

使用下列檢查清單來協助您瞭解並準備升級，從 [!DNL Dynamic Media Classic] 至 [!DNL Dynamic Media].

|  | 工作 | 說明 |
| :--- | :--- | --- |
| **階段1：授權** | 執行合約 | 根據流量和儲存空間，Adobe客戶團隊會與您合作，從 [!DNL Dynamic Media Classic] 於以下日期續訂的授權： [!DNL Dynamic Media] 授權。 |
| **階段2：準備** | 驗證功能使用情況 | 確認中使用的功能 [!DNL Dynamic Media Classic] 的可用位置 [!DNL Dynamic Media]. 請參閱 [功能比較](/help/using/upgrade-feature-comparison.md) 頁面。 中尚未提供重要功能 [!DNL Dynamic Media] 包含下列專案：<br>·視覺化設定器（影像作者、影像演算）。<br>·影像範本（1:1範本）。<br>· eCatalogs。<br>如果使用上述功能，升級仍可進行，並假設這些功能可透過以下方式存取： [!DNL Dynamic Media Classic]. |
|   | 識別資產 | 尋找並準備好要用於升級的資產和預設集。 |
| **階段3：環境** | 升級 [!DNL Adobe Experience Manager] | 所有執行個體 [!DNL Adobe Experience Manager] 必須更新至最新版本。 |
|   | 設定 [!DNL Dynamic Media] | Adobe諮詢或合作夥伴設定 [!DNL Dynamic Media] 連同您的認證。 |
| **第4階段：升級** | 復寫資產 | 在升級過程中，指定 [!DNL Dynamic Media Classic] 資產會復寫到Dynamic Media。 |
| **階段5：管理設定** | 設定使用者與許可權 | 建立使用者並授與適當的許可權。 |
|   | 設定視訊編碼設定檔 | 建立視訊編碼設定檔。 |
|   | 設定檢視器預設集 | 建立檢視器預設集。 |
|   | 設定影像預設集 | 設定影像預設集。 |
| **階段6：驗證** | 驗證 | 驗證使用案例、資產、連結和API。 |
