---
title: Adobe Dynamic Media Classic案頭應用程式——現已推出
seo-title: Adobe Dynamic Media Classic案頭應用程式——現已推出
description: 'null'
seo-description: 進一步瞭解Dynamic Media Classic案頭應用程式。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# 現已推出： Adobe Dynamic Media Classic案頭應用程式 {#dynamic-media-classic-desktop-app}

Dynamic Media Classic使用者現在可以存取新的案頭應用程式體驗，而不再依賴瀏覽器的Adobe Flash技術。

這個新應用程式現在已可用於Windows和macOS。

>[!IMPORTANT]
>
>我們建議您在2020年10月1日之前安裝新的Adobe Dynamic Media Classic案頭應用程式。 如此可確保在2020年12月31日淘汰Adobe Flash Player之前，您的轉場順暢。 在該日，您將無法再登入瀏覽器版本的Adobe Dynamic Media Classic使用者介面，在產品中標示為Dynamic Media Classic。

請參閱現已提供的 [全新Dynamic Media Classic登入體驗的常見問答集。](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic案頭應用程式的系統需求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic案頭應用程式與下列作業系統相容：
* macOS X 10.10或更新版本。
* Windows 7或更新版本。

## 下載並安裝Adobe Dynamic Media Classic案頭應用程式 {#installation-dmc-app}

1. 在您的系統上解除安裝任何舊版Dynamic Media Classic案頭應用程式。

1. 下載Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [macOS(.dmg)-下載。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows(.exe)-下載。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. 根據您下載的安裝程式，執行下列其中一項作業。

   * **對於macOS** —— 在「拖 **[!UICONTROL 放以安裝」對話方塊中，拖曳]** Adobe Dynamic Media Classic **[!UICONTROL ，並將它拖放至「應用程]** 式」 ****。

      ![在macOS上拖放安裝](/help/assets/dragondrop-install1.png)

   * 在「應用 **[!UICONTROL 程式]** 」檔案夾中，點選「Adobe Dynamic Media Classic」圖示。
   * 在對話方塊中，點選「 **[!UICONTROL 開啟]** 」以開啟Adobe Dynamic Media Classic案頭應用程式。

      ![開啟下載的應用程式](/help/assets/open-dmclassicapp1.png)

   * **針對Windows** —— 執行安裝程式二進位檔，並依照螢幕上的指示安裝案頭應用程式。

1. 當您開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Dynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 使用與您的瀏覽器認證相同的認證來登入Adobe Dynamic Media Classic。

   若要使 **[!UICONTROL 用伺服器]** ，請參閱生產環境的下列對應：

   | 瀏覽器URL | 案頭應用程式伺服器名稱 |
   |---|---|
   | https://s7sps1.scene7.com/ | 北美（北美）生產 |
   | https://s7sps3.scene7.com/ | EMEA（歐洲、中東和非洲）生產 |
   | https://s7sps5.scene7.com/ | 亞太產業 |

1. 張貼登入UI後，您會注意到熟悉的瀏覽器UI體驗。 您現在可以在案頭應用程式UI上，像平常一樣隨身攜帶日常活動。

## 使用Dynamic Media Classic案頭應用程式的視訊逐步執行

觀看使 [用Dynamic Media Classic案頭應用程式的視訊逐步執行](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) (長度： 2分36秒)。

## Dynamic Media Classic的已知限制

**_僅適用於Windows —— 可透過案頭應用程式UI上傳的檔案數目是否有限制？_**<br>&#x200B;是的，一次最多可透過案頭應用程式UI上傳150個檔案。

**_適用於Windows和macOS —— 如何在公司間切換？_**<br>&#x200B;若要在公司之間切換，請執行下列動作：
* 在Dynamic Media Classic應用程式中，從公司下拉式清單中選取新公司。
* 當快顯視窗出現時，點選「 **[!UICONTROL 確定]** 」以登出並關閉應用程式。

   ![重新啟動應用程式以使用新公司](/help/assets/dmclassic-new-company1.png)
* 重新啟動Dynamic Media Classic，然後照常登入，以便與新公司合作。

## 秘訣與訣竅

**_在Dynamic Media Classic的登陸頁面上，我無法看到「Media Cart」面板。_**<br>&#x200B;在Dynamic Media Classic中，點選「 **[!UICONTROL 設定>個人設定」]**。 在「瀏覽器」區段中，請確 **[!UICONTROL 定已選取]** 「顯示MediaPortal功能」（已勾選）。 點選「 **[!UICONTROL 儲存>關閉]**」。

**_資產的發佈狀態（綠色指標）無法正確反映。_**<br>&#x200B;在瀏覽器UI中，必須重新登入UI，才能查看資產的正確發佈狀態。 在案頭應用程式中，我們在工具列的「 **[!UICONTROL Select]** None（選取無）」按鈕右側引入了「 **[!UICONTROL Refresh]** （重新整理）」圖示。 點選「重 **[!UICONTROL 新整理]** 」圖示可查看指定頁面上所有資產的最新狀態。 不需要像瀏覽器UI一樣重新登入。

![「刷新」表徵圖](/help/assets/refresh-icon1.png)*「刷新」表徵圖*

**_我看不到在案頭應用程式中運作的批次集預設集。_**<br>&#x200B;點選「 **[!UICONTROL 上傳>工作選項>批次集預設集」]**。 確保已啟用相 **[!UICONTROL 關的批集預]** 設集。 按一 **[!UICONTROL 下「儲存並送出上傳」]**。
