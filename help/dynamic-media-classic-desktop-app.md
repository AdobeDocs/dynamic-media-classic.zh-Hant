---
title: AdobeDynamic Media Classic案頭應用程式 — 現已推出
description: 進一步了解AdobeDynamic Media Classic案頭應用程式。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: e3c2dcaa245e486ada62edd554db5a39d495483e
workflow-type: tm+mt
source-wordcount: '1870'
ht-degree: 1%

---

# 現已推出：AdobeDynamic Media Classic案頭應用程式 {#dynamic-media-classic-desktop-app}

AdobeDynamic Media Classic使用者現在可以存取新的案頭應用程式體驗，不再仰賴瀏覽器的AdobeFlash技術。

此新應用程式現已可用於Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建議您在2020年10月1日前安裝新的AdobeDynamic Media Classic案頭應用程式。 這麼做可確保在2020年12月31日汰除AdobeFlash Player之前，有順暢的轉換。 在當天以後，您無法登入AdobeDynamic Media Classic使用者介面的瀏覽器版本，在產品中標示為AdobeDynamic Media Classic。

請參閱[新AdobeDynamic Media Classic登入體驗現已推出的常見問題集。](/help/new-ui-2020.md)

## AdobeDynamic Media Classic案頭應用程式的系統需求 {#system-requirements-dmc-app}

AdobeDynamic Media Classic案頭應用程式與下列作業系統相容：

* macOS 10.10或更新版本。
* Windows® 7或更高版本。

>[!NOTE]
>
>未針對&#x200B;*次要*&#x200B;版本產生AdobeDynamic Media Classic案頭應用程式內的升級通知。 從次要版本的修正中受益的客戶可升級。

## 次要版本中的修正(20.21.2) {#minor-release}

* 已知的20.21.1伺服器下拉式清單為空。
* 在&#x200B;**[!UICONTROL 上傳工作選項]**&#x200B;中，**[!UICONTROL Photoshop選項]**&#x200B;下的層命名預設值現在為&#x200B;**[!UICONTROL Photoshop和層名稱]**。 PSD 檔案中的圖層以個別影像上載。
   * 先前預設的&#x200B;**[!UICONTROL 圖層名稱]**，在影像的圖層名稱或PSD檔案中的圖層編號後命名。 如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱，則使用圖層號。
   * 新的預設值&#x200B;**[!UICONTROL Photoshop和圖層名稱]**&#x200B;會在PSD檔案後面命名影像，後面跟圖層名稱或圖層編號。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。
   * 由於AdobeDynamic Media Classic中的圖層影像現在具有唯一名稱，因此不會更新現有PSD或範本（原始PSD檔案中的共用圖層名稱）。
* 資產縮圖損毀。

## 最新版本的修正(20.21.1) {#latest-fixes-desktop-app}

* 因逾時而出現登入問題，導致下列訊息：*此用戶可被分配給組或組，但無權。 聯繫管理員。*
* 檢視器預設集會與每次錯誤的密碼嘗試重複。
* 案頭應用程式因根資料夾中的許多資產而停止回應。 (在Windows®上修正；在macOS上視需要運作。)

## 舊版修正(20.20.2) {#previous-version-fixes-desktop-app}

* 不限於您可透過macOS和Windows®案頭應用程式使用者介面上傳的檔案數。
* 無需登出案頭應用程式，即可在公司之間切換。
* Ctrl+V組合鍵現在可在Windows®上運作。
* 日後當發行新版案頭應用程式時，使用者將會在案頭應用程式本身收到通知。

## 在macOS或Windows®上下載並安裝最新的AdobeDynamic Media Classic案頭應用程式 {#installation-dmc-app}

另請參閱:

* [在Mac上下載並靜默安裝最新AdobeDynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)
* [在Windows®上下載並靜默安裝最新AdobeDynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

1. 在您的系統上解除安裝任何舊版AdobeDynamic Media Classic案頭應用程式版本。

1. 下載AdobeDynamic Media Classic案頭應用程式的最新安裝程式。

   * 最新版本(20.21.2)可於下列位置取得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 舊版(20.21.1)可在下列位置取得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根據您下載的安裝程式執行下列其中一項操作。

   * **macOS**  — 在拖放至 **[!UICONTROL 安裝對話方]** 塊中，拖曳AdobeDynamic Media **[!UICONTROL Classic,]** 並將其拖放至應用 **[!UICONTROL 程式]**。

      ![在macOS上拖放安裝](/help/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL Applications]**&#x200B;資料夾中，點選「AdobeDynamic Media Classic」圖示。
   * 在對話方塊中，點選&#x200B;**[!UICONTROL 開啟]**&#x200B;以開啟AdobeDynamic Media Classic案頭應用程式。

      ![開啟下載的應用程式](/help/assets/open-dmclassicapp1.png)

   * **Windows**  — 執行安裝程式二進位檔，並依照螢幕上指示安裝案頭應用程式。

1. 開啟應用程式時，會顯示新的AdobeDynamic Media Classic登入頁面：

   ![AdobeDynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入AdobeDynamic Media Classic案頭應用程式，請使用與您用來在瀏覽器中登入AdobeDynamic Media Classic的相同憑證。

   若要使用&#x200B;**[!UICONTROL 伺服器]**，請參閱生產環境的下列對應：

   | 瀏覽器URL | 案頭應用伺服器名稱 |
   | --- | --- |
   | https://s7sps1.scene7.com/ | NA（北美）生產 |
   | https://s7sps3.scene7.com/ | 歐洲、中東和非洲(EMEA)生產 |
   | https://s7sps5.scene7.com/ | APAC（亞太）生產 |

1. 登入後，請注意熟悉的瀏覽器使用者介面體驗。 您可以照常在案頭應用程式上AdobeDynamic Media Classic活動，繼續日復一日。

## 下載並&#x200B;*silent*&#x200B;在macOS上安裝最新AdobeDynamic Media Classic案頭應用程式 {#install-silent-mac-dmc-app}

另請參閱:

* [在Mac或Windows®上下載並安裝最新的AdobeDynamic Media Classic案頭應用程式](#installation-dmc-app)
* [在Windows®上下載並靜默安裝最新AdobeDynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

若要下載並&#x200B;*silent*&#x200B;在macOS上安裝最新版的AdobeDynamic Media Classic案頭應用程式：

1. 在您的系統上解除安裝任何舊版AdobeDynamic Media Classic案頭應用程式版本。

1. 下載AdobemacOS專用Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 使用以下命令將下載的磁碟映像(.DMG)裝載到安裝點位置：

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令將.APP檔案複製到&#x200B;**[!UICONTROL Applications]**:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. 開啟應用程式時，會顯示新的AdobeDynamic Media Classic登入頁面：

   ![AdobeDynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入AdobeDynamic Media Classic案頭應用程式，請使用與您用來在瀏覽器中登入AdobeDynamic Media Classic的相同憑證。

   若要使用&#x200B;**[!UICONTROL 伺服器]**，請參閱生產環境的下列對應：

   | 瀏覽器URL | 案頭應用伺服器名稱 |
   | --- | --- |
   | https://s7sps1.scene7.com/ | NA（北美）生產 |
   | https://s7sps3.scene7.com/ | 歐洲、中東和非洲(EMEA)生產 |
   | https://s7sps5.scene7.com/ | APAC（亞太）生產 |

## 下載並&#x200B;*silent*&#x200B;在Windows®上安裝最新的AdobeDynamic Media Classic案頭應用程式 {#install-silent-windows-dmc-app}

您使用的命令用於基本MSI靜默安裝。 但是，AdobeDynamic Media Classic案頭應用程式安裝程式是使用InstallShield建立的InstallScript MSI安裝程式。 以記錄模式運行安裝程式時，任何用戶交互都記錄在響應檔案中。 然後，此響應檔案將用於靜默安裝，如[在靜默模式下運行安裝中所述。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另請參閱:

* [在Mac或Windows®上下載並安裝最新的AdobeDynamic Media Classic案頭應用程式](#installation-dmc-app)
* [在macOS上下載並靜默安裝最新AdobeDynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)

要下載並&#x200B;*silent*&#x200B;在Windows®上安裝最新版的AdobeDynamic Media Classic案頭應用：

1. 在您的系統上解除安裝任何舊版AdobeDynamic Media Classic案頭應用程式版本。

1. 下載AdobeDynamic Media Classic案頭應用程式的最新安裝程式。

   * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 使用以下命令在記錄模式下運行安裝程式：

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. 在GUI安裝程式窗口中，按照步驟進行安裝，以便交互/輸入（如安裝位置）記錄在`Setup.iss`檔案中。

1. 將建立的`Setup.iss`檔案和`adobe-dynamic-media-classic-20.21.2.exe`複製到其他電腦。

1. 運行以下命令以進行靜默安裝：

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   有關命令行參數的詳細資訊，請訪問[Setup.exe和Update.exe命令行參數。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 開啟應用程式時，會顯示新的AdobeDynamic Media Classic登入頁面：

   ![AdobeDynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入AdobeDynamic Media Classic案頭應用程式，請使用與您用來在瀏覽器中登入AdobeDynamic Media Classic的相同憑證。

   若要使用&#x200B;**[!UICONTROL 伺服器]**，請參閱生產環境的下列對應：

   | 瀏覽器URL | 案頭應用伺服器名稱 |
   | --- | --- |
   | https://s7sps1.scene7.com/ | NA（北美）生產 |
   | https://s7sps3.scene7.com/ | 歐洲、中東和非洲(EMEA)生產 |
   | https://s7sps5.scene7.com/ | APAC（亞太）生產 |


## 使用AdobeDynamic Media Classic案頭應用程式的影片逐步說明 {#dmc-app-video-walk-through}

使用AdobeDynamic Media Classic案頭應用程式](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media)觀看[影片逐步說明(長度：2分36秒)。

## 使用案頭應用程式清除電腦上的影像快取和資產快取 {#clear-cache}

1. 在Adobe的Dynamic Media Classic案頭應用程式中，在右上角附近，點選&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**。
1. 在&#x200B;**[!UICONTROL Personal Setup]**&#x200B;頁的&#x200B;**[!UICONTROL Desktop]**&#x200B;標題下，執行下列任一操作：
   * 若要從電腦移除所有AdobeDynamic Media快取影像檔案，請點選&#x200B;**[!UICONTROL 清除影像快取]**，然後點選&#x200B;**[!UICONTROL 確定]**。
   * 若要從電腦移除所有AdobeDynamic Media快取資產檔案，請點選&#x200B;**[!UICONTROL 清除資產快取]**，然後點選&#x200B;**[!UICONTROL 確定]**。
1. 在頁面的右下角，點選&#x200B;**[!UICONTROL 關閉]**。

### 手動清除影像快取和資產快取

除了使用案頭應用程式清除影像和資產快取外，您也可以直接從檔案系統手動清除快取。

1. 根據您的作業系統，導覽至下列項目：

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## AdobeDynamic Media Classic的已知限制20.21.1

* **[!UICONTROL Server]**&#x200B;下拉式清單在更新至AdobeDynamic Media Classic案頭應用程式20.21.1後為空 — 案例：安裝並登入AdobeDynamic Media Classic 20.20.1或20.20.2，然後關閉應用程式。 然後更新為AdobeDynamic Media Classic 20.21.1。嘗試登錄時，**[!UICONTROL 登錄帳戶]**&#x200B;對話框中的&#x200B;**[!UICONTROL 伺服器]**&#x200B;下拉清單為空。 若要解決此問題，您必須[手動清除快取](#clear-cache)（請參閱上述步驟）。

## AdobeDynamic Media Classic 20.20.1的已知限制(已在20.20.2中修正)

**_僅適用於Windows® — 是否對可通過案頭應用程式UI上載的檔案數有限制？_**<br>是的，一次最多可透過案頭應用程式UI上傳150個檔案。

**_適用於Windows®和macOS — 如何在公司之間切換？_**<br>要在公司之間切換，請執行以下操作：

* 在AdobeDynamic Media Classic應用程式中，從公司下拉式清單中選取新公司。
* 出現快顯視窗時，點選&#x200B;**[!UICONTROL 確定]**&#x200B;以登出並關閉應用程式。

   ![若要使用新公司，請重新啟動應用程式](/help/assets/dmclassic-new-company1.png)

* 重新啟動AdobeDynamic Media Classic，然後照常登入以與新公司合作。

## 提示與秘訣

**_我在Adobe Dynamic Media Classic的登陸頁面上看不到「媒體購物車」面板。_**<br>在AdobeDynamic Media Classic中，點**[!UICONTROL 選「設定>個人設定」]**。在「瀏覽器」區段中，確認已選取**[!UICONTROL 顯示MediaPortal功能&#x200B;]**（已勾選）。 點選**[!UICONTROL 儲存>關閉&#x200B;]**。

**_資產的發佈狀態（綠色指標）未正確反映。_**<br>在瀏覽器使用者介面中，必須重新登入UI，才能查看資產的正確發佈狀態。在案頭應用程式中，Adobe已在工具列的**[!UICONTROL 選取無&#x200B;]**按鈕右側導入**[!UICONTROL 重新整理&#x200B;]**圖示。 點選**[!UICONTROL 重新整理&#x200B;]**圖示，即可查看指定頁面上所有資產的最新狀態。 瀏覽器UI不需要重新登入。

![刷新表](/help/assets/refresh-icon1.png)
*徵圖刷新表徵圖*

**_我看不到批集預設集在案頭應用程式中工作。_**<br>點選**[!UICONTROL 「上傳>工作選項>批次集預設集」]**。確保已啟用相關的**[!UICONTROL 批集預設集&#x200B;]**。 按一下「**[!UICONTROL 儲存並提交上傳&#x200B;]**」。
