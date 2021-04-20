---
title: AdobeDynamic Media經典案頭應用程式——現已推出
description: 進一步瞭解Dynamic MediaClassic案頭應用程式。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
translation-type: tm+mt
source-git-commit: 8427c3ea6ca3083fd0868286e634a5569c62f7ab
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# 現已推出：AdobeDynamic Media經典案頭應用程式{#dynamic-media-classic-desktop-app}

Dynamic Media經典版使用者現在可以存取全新的案頭應用程式體驗，而不再仰賴Adobe的Flash技術。

此新應用程式現已適用於Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建議您在2020年10月1日前安裝新的AdobeDynamic Media經典案頭應用程式。 這樣做將確保在2020年12月31日淘汰AdobeFlash Player之前，您能夠順暢地轉換。 在該日期之後，您無法登入瀏覽器版本的AdobeDynamic Media經典用戶介面(在產品中標為Dynamic Media經典)。

請參閱[新Dynamic Media經典登入體驗現已推出的常見問答集。](/help/new-ui-2020.md)

## AdobeDynamic Media經典案頭應用程式的系統需求{#system-requirements-dmc-app}

AdobeDynamic Media經典案頭應用程式與下列作業系統相容：

* macOS 10.10或更新版本。
* Windows® 7或更新版本。

>[!NOTE]
>
>對於&#x200B;*minor*&#x200B;版本，不會在Dynamic MediaClassic台式機應用程式中生成升級通知。 從次要版本的修正中獲益的客戶可以升級。

## 次發行(20.21.2){#minor-release}中的修正

* Server下拉式清單20.21.1中的已知限制為空。
* 在&#x200B;**[!UICONTROL 上傳作業選項]**&#x200B;中，**[!UICONTROL Photoshop選項]**&#x200B;下方的圖層命名預設值現在為&#x200B;**[!UICONTROL Photoshop和圖層名稱]**。 PSD 檔案中的圖層以個別影像上載。
   * 先前預設的&#x200B;**[!UICONTROL 圖層名稱]**，會在影像的圖層名稱或圖層編號之後，在PSD檔案中命名影像。 如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱，則會使用圖層編號。
   * 新的預設值&#x200B;**[!UICONTROL Photoshop和圖層名稱]**&#x200B;會將影像命名為PSD檔案後面的影像，後面接著圖層名稱或圖層編號。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。
   * 鑑於Dynamic Media經典影像中的圖層影像現在有唯一的名稱，現有PSD或範本（原始PSD檔案中的共用圖層名稱）將不會更新。
* 資產的縮圖損毀。

## 最新版本(20.21.1){#latest-fixes-desktop-app}的修正

* 由於逾時而導致下列訊息的登入問題：*未經許可，可將此用戶分配給組或組。 請與管理員聯繫。*
* 檢視器預設集會與每次嘗試的密碼錯誤重複。
* 案頭應用程式由於根資料夾中有許多資產，因此無法回應。 (修正於Windows®;視需要在macOS上工作)。

## 舊版(20.20.2){#previous-version-fixes-desktop-app}的修正

* 您可透過案頭應用程式使用者介面，針對macOS和Windows®上傳的檔案數目不受限制。
* 不需要登出案頭應用程式，即可在公司間切換。
* Ctrl+V for paste操作現在可在Windows®上運作。
* 未來，當案頭應用程式發行新版本時，使用者會在案頭應用程式本身收到通知。

## 在macOS或Windows® {#installation-dmc-app}上下載並安裝最新的AdobeDynamic Media經典案頭應用程式

另請參閱:

* [在Mac上下載並無訊息安裝最新的AdobeDynamic Media經典案頭應用程式](#install-silent-mac-dmc-app)
* [在Windows®上下載並無訊息安裝最新的AdobeDynamic Media經典案頭應用程式](#install-silent-windows-dmc-app)

1. 在您的系統上解除安裝任何舊版Dynamic Media經典案頭應用程式。

1. 下載AdobeDynamic Media經典案頭應用程式的最新安裝程式。

   * 最新版本(20.21.2)可從以下網址取得：

      * [macOS(.DMG)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows®(.EXE)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 舊版(20.21.1)可從以下網址取得：

      * [macOS(.DMG)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows®(.EXE)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根據您下載的安裝程式，執行下列其中一項作業。

   * **對於macOS** -在「拖放至 **[!UICONTROL 安裝」對話]** 方塊中，拖曳 **[!UICONTROL AdobeDynamic Media]** 類別並拖放至應用 **[!UICONTROL 程式]**。

      ![在macOS上拖放安裝](/help/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL Applications]**&#x200B;資料夾中，點選AdobeDynamic Media經典圖示。
   * 在對話方塊中，點選&#x200B;**[!UICONTROL Open]**&#x200B;以開啟AdobeDynamic Media經典案頭應用程式。

      ![開啟下載的應用程式](/help/assets/open-dmclassicapp1.png)

   * **針對Windows**  —— 執行安裝程式二進位檔，並依照螢幕上的指示安裝案頭應用程式。

1. 當您開啟應用程式時，會顯示新的Adobe「Dynamic Media傳統登入」頁面：

   ![Dynamic Media經典登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe的Dynamic Media經典案頭應用程式，請使用與您在瀏覽器中登入Dynamic Media經典的相同認證。

   要使用&#x200B;**[!UICONTROL Server]**，請參見生產環境的以下映射：

   | 瀏覽器URL | 案頭應用程式伺服器名稱 |
   |---|---|
   | https://s7sps1.scene7.com/ | 北美（北美）生產 |
   | https://s7sps3.scene7.com/ | EMEA（歐洲、中東和非洲）生產 |
   | https://s7sps5.scene7.com/ | 亞太產業 |

1. 登入後，請注意熟悉的瀏覽器使用者介面體驗。 您可以像平常一樣，在案頭應用程式上繼續日常的Dynamic Media經典活動。

## 下載並&#x200B;*silent*&#x200B;在macOS {#install-silent-mac-dmc-app}上安裝最新的AdobeDynamic Media經典案頭應用程式

另請參閱:

* [在Mac或Windows®上下載並安裝最新的AdobeDynamic Media經典案頭應用程式](#installation-dmc-app)
* [在Windows®上下載並無訊息安裝最新的AdobeDynamic Media經典案頭應用程式](#install-silent-windows-dmc-app)

若要下載並&#x200B;*silent*&#x200B;在macOS上安裝最新版的AdobeDynamic Media經典案頭應用程式：

1. 在您的系統上解除安裝任何舊版Dynamic Media經典案頭應用程式。

1. 下載AdobemacOS專用Dynamic Media經典案頭應用程式的最新安裝程式。

   * [macOS(.DMG)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 使用以下命令將下載的磁碟映像(.DMG)裝載到裝載點位置：

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令將。APP檔案複製到&#x200B;**[!UICONTROL Applications]**:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. 當您開啟應用程式時，會顯示新的Adobe「Dynamic Media傳統登入」頁面：

   ![Dynamic Media經典登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe的Dynamic Media經典案頭應用程式，請使用與您在瀏覽器中登入Dynamic Media經典的相同認證。

   要使用&#x200B;**[!UICONTROL Server]**，請參見生產環境的以下映射：

   | 瀏覽器URL | 案頭應用程式伺服器名稱 |
   |---|---|
   | https://s7sps1.scene7.com/ | 北美（北美）生產 |
   | https://s7sps3.scene7.com/ | EMEA（歐洲、中東和非洲）生產 |
   | https://s7sps5.scene7.com/ | 亞太產業 |

## 下載並&#x200B;*silent*&#x200B;在Windows® {#install-silent-windows-dmc-app}上安裝最新的AdobeDynamic Media經典案頭應用程式

您使用的命令是用於基本MSI無訊息安裝。 不過，Dynamic Media傳統案頭應用程式安裝程式是使用InstallShield建立的InstallScript MSI安裝程式。 當您以記錄模式執行安裝程式時，任何使用者互動都會記錄在回應檔案中。 然後，此響應檔案將用於靜默安裝，如[在靜默模式下運行安裝中所述。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另請參閱:

* [在Mac或Windows®上下載並安裝最新的AdobeDynamic Media經典案頭應用程式](#installation-dmc-app)
* [在macOS上下載並無訊息安裝最新的AdobeDynamic Media經典案頭應用程式](#install-silent-mac-dmc-app)

要下載並&#x200B;*silent*&#x200B;在Windows®上安裝最新版的AdobeDynamic Media經典案頭應用程式：

1. 在您的系統上解除安裝任何舊版Dynamic Media經典案頭應用程式。

1. 下載AdobeDynamic Media經典案頭應用程式的最新安裝程式。

   * [Windows®(.EXE)-下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 使用下列命令，以記錄模式執行安裝程式：

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. 在GUI安裝程式窗口中，按照安裝步驟進行安裝，使交互／輸入（如安裝位置）記錄在`Setup.iss`檔案中。

1. 將已建立的`Setup.iss`檔案和`adobe-dynamic-media-classic-20.21.2.exe`複製到其他電腦。

1. 對靜默安裝運行以下命令：

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   有關命令行參數的詳細資訊，請參閱[Setup.exe和Update.exe命令行參數。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 當您開啟應用程式時，會顯示新的Adobe「Dynamic Media傳統登入」頁面：

   ![Dynamic Media經典登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe的Dynamic Media經典案頭應用程式，請使用與您在瀏覽器中登入Dynamic Media經典的相同認證。

   要使用&#x200B;**[!UICONTROL Server]**，請參見生產環境的以下映射：

   | 瀏覽器URL | 案頭應用程式伺服器名稱 |
   |---|---|
   | https://s7sps1.scene7.com/ | 北美（北美）生產 |
   | https://s7sps3.scene7.com/ | EMEA（歐洲、中東和非洲）生產 |
   | https://s7sps5.scene7.com/ | 亞太產業 |


## 使用Dynamic Media經典案頭應用程式{#dmc-app-video-walk-through}的視訊逐步執行

觀看使用Dynamic Media經典案頭應用程式的[視訊逐步瀏覽(長度：2分36秒)。](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media)

## 使用案頭應用程式{#clear-cache}清除電腦上的影像快取和資產快取

1. 在靠近右上角的Dynamic Media經典案頭應用程式中，點選「Setup **[!UICONTROL >**[!UICONTROL  Personal Setup ]**」。]**
1. 在&#x200B;**[!UICONTROL 個人設定]**&#x200B;頁面的&#x200B;**[!UICONTROL Desktop]**&#x200B;標題下，執行下列任一操作：
   * 若要從您的電腦移除所有Adobe的Dynamic Media快取影像檔，請點選「清除影像快取」，然後點選「確定」。********
   * 若要從您的電腦移除所有Adobe的Dynamic Media快取資產檔案，請點選「清除資產快取」，然後點選「確定」。********
1. 在頁面的右下角，點選&#x200B;**[!UICONTROL Close]**。

### 手動清除影像快取和資產快取

除了使用案頭應用程式清除影像和資產快取外，您也可以直接從檔案系統手動清除快取。

1. 根據您的作業系統，導覽至下列：

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Dynamic Media經典版20.21.1的已知限制

* **[!UICONTROL Server]**&#x200B;下拉式清單在更新至Dynamic Media傳統案頭應用程式20.21.1後為空——藍本：您可以安裝並登入Dynamic MediaClassic 20.20.1或20.20.2，然後關閉應用程式。 然後更新為Dynamic Media經典20.21.1。當您嘗試登入時，**[!UICONTROL 登入帳戶]**&#x200B;對話方塊中的&#x200B;**[!UICONTROL Server]**&#x200B;下拉式清單是空的。 要解決此問題，您必須[手動清除快取](#clear-cache)（請參閱上述步驟）。

## Dynamic MediaClassic 20.20.1的已知限制（已修正於20.20.2）

**_僅適用於Windows® —— 可透過案頭應用程式UI上傳的檔案數目是否有限制？_**<br>是的，一次最多可透過案頭應用程式UI上傳150個檔案。

**_適用於Windows®和macOS —— 如何在公司間切換？_**<br>若要在公司之間切換，請執行下列動作：

* 在Dynamic Media經典應用程式中，從公司下拉式清單中選取新公司。
* 出現快顯視窗時，點選&#x200B;**[!UICONTROL OK]**&#x200B;以登出並關閉應用程式。

   ![若要使用新公司，請重新啟動應用程式](/help/assets/dmclassic-new-company1.png)

* 重新啟動Dynamic Media經典，然後照常登入，與新公司合作。

## 秘訣與訣竅

**_我無法在Dynamic Media經典網站的登陸頁面上看到媒體購物車面板。_**<br>在「Dynamic Media經典」中，**[!UICONTROL 點選「設定>個人設定」]**。在「瀏覽器」區段中，請確定已選取**[!UICONTROL 「顯示MediaPortal功能&#x200B;]**」（已勾選）。 點選**[!UICONTROL 儲存>關閉&#x200B;]**。

**_資產的發佈狀態（綠色指標）無法正確反映。_**<br>在瀏覽器使用者介面中，必須重新登入UI，才能查看資產的正確發佈狀態。在案頭應用程式中，Adobe在**[!UICONTROL 選擇無&#x200B;]**按鈕右側的工具列中，引入了**[!UICONTROL Refresh ]**圖示。 點選**[!UICONTROL 重新整理&#x200B;]**圖示，查看指定頁面上所有資產的最新狀態。 不需要像瀏覽器UI一樣重新登入。

![「刷新」](/help/assets/refresh-icon1.png)
*表徵圖「刷新」表徵圖*

**_我看不到在案頭應用程式中運作的批次集預設集。_**<br>點選「**[!UICONTROL 上傳>工作選項>批次集預設集」]**。確保已啟用相關的**[!UICONTROL 批集預設集&#x200B;]**。 按一下「儲存並送出上傳」**[!UICONTROL 。]**
