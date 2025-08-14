---
title: Adobe Dynamic Media Classic案頭
description: 進一步瞭解現已推出的Adobe Dynamic Media Classic案頭應用程式。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# 現已推出： Adobe Dynamic Media Classic案頭應用程式 {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic使用者現在可以使用全新的案頭應用程式體驗，不必再仰賴瀏覽器的Adobe Flash技術。

此新應用程式現在可供Windows®和macOS使用。

>[!IMPORTANT]
>
>Adobe建議您在2020年10月1日前安裝新的Adobe Dynamic Media Classic案頭應用程式。 這麼做可確保Adobe Flash Player在2020年12月31日淘汰前能順利轉換。 在該日期之後，您將無法登入瀏覽器版本的Adobe Dynamic Media Classic使用者介面，該產品中標示為Adobe Dynamic Media Classic。

檢視[現在提供新Adobe Dynamic Media Classic登入的常見問題集。](/help/using/new-ui-2020.md)

## Adobe Dynamic Media Classic案頭應用程式的系統需求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic案頭應用程式與下列作業系統相容：

* macOS 10.10或更新版本。
* Windows® 7或更新版本。

如需完整系統需求，請參閱[Adobe Dynamic Media Classic案頭應用程式的系統需求](/help/using/system-requirements.md)。

未針對&#x200B;*次要*&#x200B;版本產生Adobe Dynamic Media Classic案頭應用程式中的升級通知。 受益於次要版本修正的客戶可以升級。

## 僅在最新版本(20.22.2) macOS中修正 {#release-feb2022}

* macOS Montery：檔案上傳頁面在後續上傳時凍結。<!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新版本(20.22.1)中的修正 {#release-jan2022}

* 編輯影像時，**[!UICONTROL 儲存]**&#x200B;按鈕無法運作。
* 在「設定」編輯器中，捲動「**[!UICONTROL 新增Assets]**」面板中的資產後，**[!UICONTROL 關閉]**、**[!UICONTROL 儲存]**&#x200B;和&#x200B;**[!UICONTROL 另存新檔]**&#x200B;按鈕會停用。
* 視訊詳細資料檢視中的&#x200B;**[!UICONTROL 播放]**&#x200B;按鈕無法運作。
* 執行macOS Monterey時，無法在`d`使用者名稱`e`和&#x200B;**[!UICONTROL 密碼]**&#x200B;欄位中輸入&#x200B;**[!UICONTROL 和]**。
* 將其餘的Analytics API移至2.0版。

## 20.21.3版中的修正 {#release-sept2021}

* 在案頭應用程式上閒置一段時間後，資產的縮圖遭到破壞。
* 案頭應用程式通常會在「設定」作業後停止回應。
* 在&#x200B;**[!UICONTROL 測試影像伺服]**&#x200B;下自動啟用要求模糊化和鎖定模式。

  請參閱[安全測試服務](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service)。

* 更新Adobe Analytics的驗證機制。 與新的整合或是必須從Dynamic Media Classic案頭應用程式中更新某些Analytics變數相關。

  如需更新步驟，請參閱[登入Adobe Analytics](/help/using/log-analytics.md)。

## 20.21.2版中的修正 {#minor-release}

* 20.21.1中的已知限制：登入畫面上的&#x200B;**[!UICONTROL 伺服器]**&#x200B;下拉式清單是空的。
* 在&#x200B;**[!UICONTROL 上載工作選項]**&#x200B;中，**[!UICONTROL Photoshop選項]**&#x200B;下的預設圖層名稱值為&#x200B;**[!UICONTROL Photoshop和圖層名稱]**。 PSD檔案中的圖層會以個別影像上傳。
   * **[!UICONTROL 圖層名稱]**&#x200B;的早期預設值，在PSD檔案中以圖層名稱或圖層編號命名。 如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱，則會使用圖層編號。
   * 新預設值&#x200B;**[!UICONTROL Photoshop和圖層名稱]**&#x200B;會在PSD檔案後面加上圖層名稱或圖層編號來命名影像。 如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱，則會使用圖層編號。
   * 鑑於Adobe Dynamic Media Classic中的圖層影像現在具有唯一名稱，將不會更新現有的PSD或範本(哪些會共用原始PSD檔案中的圖層名稱)。
* 資產的縮圖損毀。

## 20.21.1版中的修正 {#latest-fixes-desktop-app}

* 由於逾時而導致下列訊息的登入問題： *此使用者可能會指派給沒有許可權的群組或群組。 請連絡您的系統管理員。*
* 檢視器預設集會與每個錯誤的密碼嘗試重複。
* 由於根資料夾中有許多資產，案頭應用程式變得無回應。 (在Windows®上修正；視需要在macOS上運作。)

## 20.20.2版中的修正 {#previous-version-fixes-desktop-app}

* 對於macOS和Windows®，您可透過案頭應用程式使用者介面上傳的檔案數沒有限制。
* 不需登出案頭應用程式，即可在各公司間切換。
* Ctrl+V貼上操作現在可在Windows®上運作。
* 未來，當案頭應用程式發佈新版本時，使用者會在案頭應用程式中收到通知。

## 在macOS或Windows上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式® {#installation-dmc-app}

另請參閱：

* [在Mac上下載並以無訊息方式安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)
* [在Windows上下載並自動安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

1. 在您的系統上解除安裝任何較舊的Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * 最新版本可從下列網址取得：

      * [macOS (.DMG)：下載](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE)：下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 先前版本可在以下位置使用：

      * [macOS (.DMG)：下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE)：下載](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根據您下載的安裝程式，執行下列任一項作業。

   * **macOS** — 在&#x200B;**[!UICONTROL 拖放以安裝]**&#x200B;對話方塊中，拖曳&#x200B;**[!UICONTROL Adobe Dynamic Media Classic]**&#x200B;並將其放置到&#x200B;**[!UICONTROL 應用程式]**&#x200B;上。

     ![拖放安裝至macOS](/help/using/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL 應用程式]**&#x200B;資料夾中，點選Adobe Dynamic Media Classic圖示。
   * 在對話方塊中，點選&#x200B;**[!UICONTROL 開啟]**&#x200B;以開啟Adobe Dynamic Media Classic案頭應用程式。

     ![開啟下載的應用程式](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** — 執行安裝程式二進位檔，然後依照熒幕上的指示安裝案頭應用程式。

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/using/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用您在瀏覽器中登入Adobe Dynamic Media Classic的相同憑證。

   若要讓&#x200B;**[!UICONTROL 伺服器]**&#x200B;使用，請參閱下列生產環境的對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

1. 登入後，請注意熟悉的瀏覽器使用者介面體驗。 您可以照常在案頭應用程式上繼續進行日常Adobe Dynamic Media Classic活動。

## 在macOS上下載並&#x200B;*無訊息地*&#x200B;安裝最新的Adobe Dynamic Media Classic案頭應用程式 {#install-silent-mac-dmc-app}

另請參閱：

* [在Mac或Windows上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式](#installation-dmc-app)
* [在Windows上下載並自動安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

若要在macOS上下載並&#x200B;*無訊息地*&#x200B;安裝最新版的Adobe Dynamic Media Classic案頭應用程式：

1. 在您的系統上解除安裝任何較舊的Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載適用於macOS的Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [macOS (.DMG)：下載](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 使用下列命令將下載的磁碟映像(.DMG)掛載到掛載點位置：

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令將.APP檔案複製到&#x200B;**[!UICONTROL 應用程式]**：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/using/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用您在瀏覽器中登入Adobe Dynamic Media Classic的相同憑證。

   若要讓&#x200B;**[!UICONTROL 伺服器]**&#x200B;使用，請參閱下列生產環境的對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

## 在Windows®上下載並&#x200B;*自動安裝*&#x200B;最新的Adobe Dynamic Media Classic案頭應用程式 {#install-silent-windows-dmc-app}

您使用的指令用於基本的MSI無訊息安裝。 不過，Adobe Dynamic Media Classic案頭應用程式安裝程式是使用InstallShield建立的InstallScript MSI安裝程式。 當您以記錄模式執行安裝程式時，任何使用者互動都會記錄在回應檔案中。 然後此回應檔案會用於無訊息安裝，如[以無訊息模式執行安裝](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm)中所述。

另請參閱：

* [在Mac或Windows上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式](#installation-dmc-app)

* [在macOS上下載並以無訊息方式安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)

若要在Windows®上下載並&#x200B;*自動安裝*&#x200B;最新版本的Adobe Dynamic Media Classic案頭應用程式：

1. 在您的系統上解除安裝任何較舊的Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [Windows® (.EXE)：下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 使用下列命令以記錄模式執行安裝程式：

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安裝程式視窗中，依照安裝步驟進行，以便在`Setup.iss`檔案中記錄互動/輸入，例如安裝位置。

1. 將已建立的`Setup.iss`檔案和`adobe-dynamic-media-classic-20.22.1.exe`複製到其他電腦。

1. 針對無訊息安裝執行以下命令：

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   有關命令列引數的詳細資訊，請參閱[Setup.exe和Update.exe命令列引數](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters)。

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/using/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用您在瀏覽器中登入Adobe Dynamic Media Classic的相同憑證。

   若要讓&#x200B;**[!UICONTROL 伺服器]**&#x200B;使用，請參閱下列生產環境的對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

## 使用Adobe Dynamic Media Classic案頭應用程式的影片逐步解說 {#dmc-app-video-walk-through}

觀看[使用Adobe Dynamic Media Classic案頭應用程式的逐步說明影片](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) （長度： 2分36秒）。

## 使用案頭應用程式清除電腦上的影像快取和資產快取 {#clear-cache}

1. 在Adobe Dynamic Media Classic案頭應用程式右上角附近，點選&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 在「**[!UICONTROL 個人設定]**」頁面的「**[!UICONTROL 案頭]**」標題下，執行下列任一動作：
   * 若要從您的電腦移除所有Adobe Dynamic Media快取的影像檔案，請點選&#x200B;**[!UICONTROL 清除影像快取]**，然後點選&#x200B;**[!UICONTROL 確定]**。
   * 若要從您的電腦移除所有Adobe Dynamic Media快取的資產檔案，請點選&#x200B;**[!UICONTROL 清除資產快取]**，然後點選&#x200B;**[!UICONTROL 確定]**。
1. 在頁面的右下角，點選&#x200B;**[!UICONTROL 關閉]**。

### 手動清除影像快取和資產快取

除了使用案頭應用程式清除影像和資產快取以外，您也可以直接從檔案系統手動清除快取。

1. 根據您的作業系統，瀏覽至下列專案：

   * macOS： `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®： `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1的已知限制

* 更新至Adobe Dynamic Media Classic案頭應用程式20.21.1後，**[!UICONTROL 伺服器]**&#x200B;下拉式清單為空白：案例：您安裝並登入Adobe Dynamic Media Classic 20.20.1或20.20.2，然後關閉應用程式。 接著您更新至Adobe Dynamic Media Classic 20.21.1。當您嘗試登入時，**[!UICONTROL 登入您的帳戶]**&#x200B;對話方塊中的&#x200B;**[!UICONTROL 伺服器]**&#x200B;下拉式清單是空的。 若要解決此問題，您必須[手動清除快取](#clear-cache) （請參閱上述步驟）。

## Adobe Dynamic Media Classic 20.20.1的已知限制（已在20.20.2中修正）

**_僅適用於Windows® — 可透過案頭應用程式UI上傳的檔案數量是否有限制？_**<br>是，使用案頭應用程式UI一次最多可上傳150個檔案。

**_套用至Windows®和macOS — 如何在公司之間切換？_**<br>若要切換公司，請執行下列動作：

* 在Adobe Dynamic Media Classic應用程式中，從公司下拉式清單中選取新公司。
* 當快顯視窗出現時，點選&#x200B;**[!UICONTROL 確定]**&#x200B;以登出並關閉應用程式。

  ![若要使用新公司，請重新啟動應用程式](/help/using/assets/dmclassic-new-company1.png)

* 重新啟動Adobe Dynamic Media Classic，然後照常登入以與新公司合作。

## 提示與秘訣

**_我在Adobe Dynamic Media Classic的登陸頁面上無法看到媒體購物車面板。_**<br>在Adobe Dynamic Media Classic中，點選**[!UICONTROL 設定>個人設定&#x200B;]**。 在瀏覽器區段中，確定已選取**[!UICONTROL 顯示MediaPortal功能&#x200B;]**（已核取）。 點選**[!UICONTROL 儲存>關閉&#x200B;]**。

**_無法正確反映資產的發佈狀態（綠色指標）。_**<br>在瀏覽器使用者介面中，必須重新登入UI才能檢視資產的正確發佈狀態。 在案頭應用程式中，Adobe在工具列的**[!UICONTROL 不選&#x200B;]**按鈕右側引入了**[!UICONTROL 重新整理&#x200B;]**圖示。 點選**[!UICONTROL 重新整理&#x200B;]**圖示以檢視指定頁面上所有資產的最新狀態。 使用瀏覽器UI無需重新登入。

![重新整理圖示](/help/using/assets/refresh-icon1.png)
*重新整理圖示*

**_我看不到批次集預設集在案頭應用程式中運作。_**<br>點選**[!UICONTROL 上傳>工作選項>批次集預設集&#x200B;]**。 請確定已啟用相關的**[!UICONTROL 批次集預設集&#x200B;]**。 按一下**[!UICONTROL 儲存並提交上傳&#x200B;]**。
