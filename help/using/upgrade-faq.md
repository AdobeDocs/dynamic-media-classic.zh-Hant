---
title: 升級常見問答集
description: 從 [!DNL Adobe Dynamic Media Classic] 案頭應用程式升級至 [!DNL Dynamic Media] Assets上的 [!DNL Adobe Experience Manager] 時，常見問題集(FAQ)。
feature: Dynamic Media Classic
role: Admin,User
exl-id: 5c2e2937-fe4f-4b64-bee8-9572ca84695b
topic: Content Management
level: Intermediate
source-git-commit: 4601442c2d51d50a2712eee7fd8e5110b43fb2a0
workflow-type: tm+mt
source-wordcount: '1564'
ht-degree: 0%

---

# 有關從[!DNL Dynamic Media Classic]升級為[!DNL Dynamic Media]的常見問題

## 一般資訊

+++**什麼是[!DNL Dynamic Media] Assets中的[!DNL Adobe Experience Manager]？**
[!DNL Dynamic Media]是[!DNL Adobe Dynamic Media Classic] Assets中[!DNL Experience Manager] （原為Scene7）功能的新一代進化。 此解決方案結合了資產管理的強大功能與多媒體遞送。 功能包括下列各項：

* 管理影像和視訊的單一使用者介面和平台。
* 創新的銷售功能。
* Adobe強大且深獲肯定的傳遞平台。
* 與[!DNL Experience Manager] Assets無縫統一。

+++

+++**升級至[!DNL Dynamic Media]的主要優點為何？**

* Collaboration和共用檔案與[!DNL Adobe Creative Cloud]應用程式同步。
* 企業級數位資產管理，具備：
   * 強大的中繼資料支援
   * 智慧型搜尋
   * Lightbox和集合
   * 版本控制
   * 供應商、合作夥伴和加盟商使用的安全資產共用
* 稽核和核准在製品資產的工作流程。
* 透過新的UI輕鬆採用和使用。
* 使用可促進轉換並豐富使用者參與度和滿意度的影像和視訊，建立可購物/互動媒體體驗。
* 結合行銷活動資產與產品資訊，以便簡化購物車的點按。
* 使用WYSIWYG Viewer Designer輕鬆建立、調整、品牌和部署互動式檢視器。
* 將最佳化的多媒體傳送至[!DNL Experience Cloud]個解決方案。
* 與[!DNL Experience Cloud]整合，以在行銷接觸點間進行進階資產分析、鎖定目標及資產重複使用。 這些接觸點包括適用於電子郵件的[!DNL Adobe Campaign]、適用於社交管道的[!DNL Adobe Social]，以及適用於回應式網頁和行動應用程式的[!DNL Experience Manager]個網站。

+++

+++**[!DNL Dynamic Media]是否使用現有的Adobe CDN （內容傳遞網路）？**
是，[!DNL Dynamic Media]使用Adobe強大的頂層傳遞網路。

* 網際網路零售1000的頂級多媒體供應商，連續九年。
* 24/7/265支援，99.95% SLA。
* 廣受肯定的基礎建設，在全球各地為800多家客戶提供服務，每月3.5 PB的流量，以及超過5億項資產的管理作業，流量逐年增加60%。

+++

+++**什麼是[!DNL Dynamic Media Classic]？ Adobe是否會變更Adobe Scene7的名稱？**
Adobe已將Adobe Scene7的名稱變更為[!DNL Dynamic Media Classic]。

+++

## 升級程式與工具

+++**誰符合升級計畫的資格？**
目前有[!DNL Dynamic Media Classic] （先前為Scene7）且也有[!DNL Experience Manager]的客戶。

+++

+++**如何開始升級程式？**
請聯絡您的Adobe客戶團隊代表或[電子郵件s7support@adobe.com](mailto:s7support@adobe.com)，主旨列為`[!DNL Dynamic Media] Upgrade Program`。

+++

+++**如何處理升級程式？**
AGS (Adobe全域服務)會處理升級，並將其視為服務專案。 Adobe僅提供資產的移轉。 客戶、AGS或合作夥伴負責所有其他升級方面和步驟。 在彙總層次，升級計畫包含下列專案：

* 布建公司/使用者帳戶。
* 將資產從[!DNL Dynamic Media Classic] （先前的Scene7）復寫到[!DNL Dynamic Media] Assets的[!DNL Experience Manager]元件(由Adobe透過自動升級工具提供)。
* 設定影像和視訊的設定。
* 修改生產流程並訓練使用者。

+++

+++**升級程式需要多久的時間？**
升級程式時間會因數種因素而異，包括但不限於：資產數量和資產大小。 AGS或合作夥伴管理專案時間表。

+++

+++**如何檢查升級狀態？**
升級程式時間會因數種因素而異，包括但不限於：資產數量和資產大小。 AGS或合作夥伴管理專案時間表。

+++

+++**升級為[!DNL Dynamic Media]是否需要任何合約變更？**
升級程式時間會因數種因素而異，包括但不限於：資產數量和資產大小。 AGS或合作夥伴管理專案時間表。

+++

+++**授權成本是否有差異？**
請洽詢您的Adobe客戶團隊代表，以取得有關定價的詳細資訊。

+++

+++**是否有任何與升級程式相關的停機時間？**
不適用。 在升級程式期間，[!DNL Dynamic Media Classic]會繼續不間斷地工作。 升級完成且內容通過驗證後，所有使用者僅在[!DNL Dynamic Media] Assets的[!DNL Experience Manager]元件中工作。

+++

+++**是否需要升級整備檢查清單中的所有步驟？**
不適用。 [整備檢查清單](/help/using/upgrade-readiness.md)包含必要和選用的最佳實務步驟。

+++

+++**是否需要升級？**
不適用。 Adobe現在及未來都完全支援並維護[!DNL Dynamic Media Classic] （客戶要求的錯誤修正、安全性修正、平台擴充性及可靠性）。

當您準備好要利用[!DNL Dynamic Media]提供的新功能時，可以升級。

+++

+++**在我升級至[!DNL Dynamic Media Classic]後，是否仍可使用[!DNL Dynamic Media] （先前稱為Adobe Scene7）？**
升級為[!DNL Dynamic Media]之後，您應該只使用Dynamic Media進行影像和視訊。 您只能針對[!DNL Dynamic Media Classic]中尚未提供的功能，繼續使用[!DNL Dynamic Media]，包括下列功能：

* 視覺化設定器（影像作者、影像演算）。
* 影像範本。
* eCatalogs。

+++

+++**Adobe提供哪些工具可自動化升級程式？**
對於升級程式的初始啟動，Adobe提供的工具可以在[!DNL Dynamic Media Classic] Assets中自動將資產從[!DNL Dynamic Media]移至[!DNL Experience Manager]。

+++

+++**在我升級期間和之後，現有的[!DNL Dynamic Media Classic] URL、API整合和檢視器是否仍可繼續運作？**
是. 您可以繼續使用[!DNL Dynamic Media Classic]解決方案中的[!DNL Dynamic Media] （先前的Adobe Scene7）發佈與傳遞基礎結構。

+++

+++**我是否必須更新生產URL？**
不適用。 Adobe繼續使用[!DNL Dynamic Media Classic]解決方案中的[!DNL Dynamic Media]發佈與傳遞基礎結構。 此方法的好處是，您不必變更網頁上的任何生產URL，因此可將移轉至[!DNL Dynamic Media]的風險和工作量降至最低。

+++

+++**我是否必須重寫API整合和其他自動化指令碼？**
不適用。 Adobe繼續使用[!DNL Dynamic Media Classic]解決方案中的[!DNL Dynamic Media]發佈與傳遞基礎結構。 此外，所有資產都會復寫到[!DNL Dynamic Media Classic]。 此方法的優點在於您不需要重寫任何以API為基礎的整合或自動化指令碼，因此可將移轉至[!DNL Dynamic Media]的風險和工作量降至最低。

+++

+++**我是否需要變更或重新開發我的自訂檢視器？**
不適用。 Adobe繼續使用[!DNL Dynamic Media Classic]解決方案中的[!DNL Dynamic Media]發佈與傳遞基礎結構。 此方法的好處是，您可以繼續使用自訂的檢視器，因此將移轉至[!DNL Dynamic Media]的風險和工作量降至最低。
+++

+++**如何將我的設定（例如影像預設集、視訊編碼）移轉至[!DNL Dynamic Media]？**
預設集和其他設定必須在[!DNL Dynamic Media]內重新建立。 在服務專案中，Adobe全球服務或合作夥伴可提供協助。

+++

+++**如何設定使用者和許可權（SSO或LDAP選項）？**
必須在[!DNL Dynamic Media]內重新建立設定。 作為服務專案的一部分，AGS或Partner可提供協助。 不過，升級至[!DNL Dynamic Media]可提供SSO/LDAP整合，讓使用者管理更有效率。 此外，[!DNL Dynamic Media]還提供強大的角色和許可權來控制使用者存取權。

+++

+++**我仍然可以使用FTP來批次/大量上傳資產嗎？**
是. 您不需要修改現有的擷取工作流程，可以繼續排程FTP式上傳。

+++

+++**哪些資源可用來訓練新使用者？**
培訓可透過ADLS (Adobe數位學習服務)提供。 [!DNL Dynamic Media]功能包含在2個課程中：管理和傳遞數位Assets以及自訂數位Assets。

+++

+++**是否[!DNL Dynamic Media]適用於所有地理位置？**
是. Adobe在北美、歐洲和亞太地區擁有資料中心。

+++

+++**[!DNL Dynamic Media Classic]要以獨立產品形式存在多久？**
Adobe現在及未來都完全支援並維護[!DNL Dynamic Media Classic] （客戶要求的錯誤修正、安全性修正、平台擴充性及可靠性）。

+++

+++**[!DNL Dynamic Media]隨附多少儲存空間？**
Dynamic Media隨附60 GB的儲存空間。 您可以以250GB的區塊購買額外的儲存空間。 檢查您的合約詳細資料，以便取得目前的儲存配額。

+++

+++**使用哪個量度來測量[!DNL Dynamic Media]使用量？**
每月頁面檢視次數(PVM)。 「頁面檢視」是指對網際網路網站之電子郵件或網頁的單一檢視。 此外也包含應用程式畫面檢視、應用程式畫面狀態、行動網頁和社交網路頁面。 發生頁面檢視：

* 每次載入或重新整理網頁時
* 載入應用程式時
* 內容轉譯時
* 透過已開啟或已檢視的電子郵件顯示

+++

+++**個人化媒體何時可搭配[!DNL Dynamic Media]使用？**
Adobe正積極地將「個人化媒體」功能新增到[!DNL Dynamic Media]。 即將提供更多關於發行時機的資訊。

+++

+++**在升級期間如何驗證資產？ 我是否需要執行手動驗證？**
Adobe會對所有移至[!DNL Dynamic Media]的資產執行自動驗證。 建議使用[!DNL Dynamic Media]支援的主要網站、頁面和體驗的一般手動驗證。

+++

+++**是否有[!DNL Dynamic Media]的SLA？**
是. 如需詳細資訊，請聯絡您的Adobe客戶團隊代表。

+++

+++**我可以搭配[!DNL Dynamic Media]使用自己的CDN （內容傳遞網路）嗎？**
是. 您可以使用自己的CDN搭配[!DNL Dynamic Media]。

+++

+++**[!DNL Dynamic Media]是否有我需要的功能以便升級？ [!DNL Dynamic Media] Assets上的[!DNL Experience Manager]有哪些可用功能？**
請參閱[功能比較](/help/using/upgrade-feature-comparison.md)頁面，瞭解更多資訊。

+++

+++**哪些功能仍只在[!DNL Dynamic Media Classic]中可用？ 我還可以升級嗎？**
需要下列專案的客戶可以繼續存取[!DNL Dynamic Media Classic]支援的功能：

* 視覺化設定器（影像作者、影像演算）。
* 影像範本。
* eCatalogs。

另請參閱[功能比較](/help/using/upgrade-feature-comparison.md)頁面，您可在此瞭解更多資訊。

+++

+++**[!DNL Dynamic Media Classic] Media Portal解決方案發生什麼事？**
[!DNL Experience Manager] Brand Portal是[!DNL Dynamic Media Classic] Media Portal的替代產品。

+++

## 諮詢服務

+++**我可以自行完成升級程式嗎？**
不適用。 與您的Adobe代表和AGS合作，設定升級範圍。

+++

+++**服務專案是什麼樣子？**
Adobe會與您合作來規劃專案。 Adobe負責布建和設定帳戶、複製資產、測試和驗證。

客戶主要負責變更管理，包括培訓使用者、編輯生產流程以及推出新功能。

+++

## 支援與訓練

+++**我要如何取得支援？**
24/7/365客戶服務支援。 [連絡技術支援](https://experienceleague.adobe.com/zh-hant?support-solution=General#support)。

電話： 1-800-898-9743 （美國） | +44 (0)20 35641782 （英國） | +81-3-6743-9632 （日本）

+++

+++**我可以在何處進一步瞭解付費訓練選項？**
請參閱[Adobe數位學習服務](https://learning.adobe.com)。

若要進行自訂或個人訓練，請聯絡您的Adobe客戶團隊代表。

+++

## 其他資源

+++**我可以在何處進一步瞭解[!DNL Dynamic Media]及其功能？**
檢視[[!DNL Dynamic Media] 微網站](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/solutions.html)以進一步瞭解[!DNL Dynamic Media]。

+++
