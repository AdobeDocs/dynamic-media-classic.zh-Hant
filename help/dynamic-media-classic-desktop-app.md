---
title: Adobe Dynamic Media Classic案頭應用程式 — 現已推出
description: 深入了解Adobe Dynamic Media Classic案頭應用程式。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: a575c698fec3f85e537ad07f5948e7e65912ca52
workflow-type: tm+mt
source-wordcount: '2002'
ht-degree: 1%

---

# 現已推出：Adobe Dynamic Media Classic案頭應用程式 {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic使用者現在可以存取新的案頭應用程式體驗，不再仰賴瀏覽器的AdobeFlash技術。

此新應用程式現已可用於Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建議您在2020年10月1日前安裝新的Adobe Dynamic Media Classic案頭應用程式。 這麼做可確保在2020年12月31日汰除AdobeFlash Player之前，有順暢的轉換。 在當天以後，您將無法登入瀏覽器版本的Adobe Dynamic Media Classic使用者介面，產品中標示為Adobe Dynamic Media Classic。

請參閱的常見問題集 [全新Adobe Dynamic Media Classic登入體驗現已推出。](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic案頭應用程式的系統需求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic案頭應用程式與下列作業系統相容：

* macOS 10.10或更新版本。
* Windows® 7或更高版本。

>[!NOTE]
>
>系統不會為產生Adobe Dynamic Media Classic案頭應用程式內的升級通知 *次要* 版本。 從次要版本的修正中受益的客戶可升級。

## 最新版本的修正(20.22.1) {#release-jan2022}

影像編輯 **[!UICONTROL 儲存]** 按鈕無法正常工作。

* 影像編輯 **[!UICONTROL 儲存]** 按鈕無法正常工作。
* 在「設定」編輯器中， **[!UICONTROL 關閉]**, **[!UICONTROL 儲存]**，和 **[!UICONTROL 另存新檔]** 在中捲動資產後，按鈕會變為停用 **[!UICONTROL 新增資產]** 中。
* **[!UICONTROL 播放]** 按鈕無法運作。
* 無法輸入 `d` 和 `e` in **[!UICONTROL 使用者名稱]** 和 **[!UICONTROL 密碼]** 運行macOS蒙特利時的欄位。
* 將剩餘的Analytics API移至2.0版。

## 版本修正(20.21.3) {#release-sept2021}

* 案頭應用程式閒置一段時間後，所看到資產的縮圖損毀。
* 案頭應用程式通常會在設定操作後停止回應。
* 請求模糊化和鎖定模式會在 **[!UICONTROL 測試影像提供]**.

   請參閱 [測試安全測試服務](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* 更新Adobe Analytics的驗證機制。 與新整合相關，或某些Analytics變數必須從Dynamic Media Classic案頭應用程式內更新。

   請參閱 [登入Adobe Analytics](/help/log-analytics.md) ，了解更新的步驟。

## 20.21.2版中的修正 {#minor-release}

* 20.21.1中的已知限制：the **[!UICONTROL 伺服器]** 登入畫面上的下拉式清單為空。
* 在 **[!UICONTROL 上傳作業選項]**，圖層命名預設值位於 **[!UICONTROL Photoshop選項]**，現在 **[!UICONTROL Photoshop和圖層名稱]**. PSD 檔案中的圖層以個別影像上載。
   * 先前的 **[!UICONTROL 圖層名稱]**，在影像的圖層名稱或圖層編號後，將其命名為PSD檔案。 如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱，則使用圖層編號。
   * 的新預設值 **[!UICONTROL Photoshop和圖層名稱]**，在PSD檔案後面加上圖層名稱或圖層號。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。
   * 鑑於Adobe Dynamic Media Classic中的圖層影像現在具有唯一名稱，現有PSD或範本將不會更新(原始PSD檔案中的共用圖層名稱)。
* 資產縮圖損毀。

## 20.21.1版中的修正 {#latest-fixes-desktop-app}

* 因逾時而出現登入問題，導致下列訊息： *此用戶可以被指派給組或組，但無需權限。 請聯絡您的管理員。*
* 檢視器預設集會與每次錯誤的密碼嘗試重複。
* 案頭應用程式因根資料夾中的許多資產而停止回應。 (在Windows®上修正；視需要在macOS上工作。)

## 20.20.2版中的修正 {#previous-version-fixes-desktop-app}

* 不限於可透過macOS和Windows®案頭應用程式使用者介面上傳的檔案數。
* 無需登出案頭應用程式，即可在公司之間切換。
* Ctrl+V組合鍵現在可在Windows®上運作。
* 日後當發行新版案頭應用程式時，使用者將會在案頭應用程式本身收到通知。

## 在macOS或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式 {#installation-dmc-app}

另請參閱:

* [在Mac上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)
* [在Windows®上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

1. 在您的系統上解除安裝任何舊版Adobe Dynamic Media Classic案頭應用程式。

1. 下載Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * 最新版本(20.22.1)可於下列位置取得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * 舊版(20.21.3)可在下列位置取得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根據您下載的安裝程式執行下列其中一項操作。

   * **macOS**  — 在 **[!UICONTROL 拖放以安裝]** 對話框，拖動 **[!UICONTROL Adobe Dynamic Media Classic]** 放上 **[!UICONTROL 應用程式]**.

      ![在macOS上拖放安裝](/help/assets/dragondrop-install1.png)

   * 在 **[!UICONTROL 應用程式]** 資料夾，點選Adobe Dynamic Media Classic圖示。
   * 在對話方塊中，點選 **[!UICONTROL 開啟]** 開啟Adobe Dynamic Media Classic案頭應用程式。

      ![開啟下載的應用程式](/help/assets/open-dmclassicapp1.png)

   * **Windows**  — 運行安裝程式二進位，並按照螢幕上的說明安裝案頭應用。

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用與您在瀏覽器中登入Adobe Dynamic Media Classic時所使用的相同憑證。

   若 **[!UICONTROL 伺服器]** 若要使用，請參閱生產環境的下列對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太地區） | https://s7sps5.scene7.com/ |

1. 登入後，請注意熟悉的瀏覽器使用者介面體驗。 您可以照常在案頭應用程式上繼續進行Adobe Dynamic Media Classic活動。

## 下載和 *靜默* 在macOS上安裝最新的Adobe Dynamic Media Classic案頭應用程式 {#install-silent-mac-dmc-app}

另請參閱:

* [在Mac或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式](#installation-dmc-app)
* [在Windows®上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-windows-dmc-app)

若要下載和 *靜默* 在macOS上安裝最新版的Adobe Dynamic Media Classic案頭應用程式：

1. 在您的系統上解除安裝任何舊版Adobe Dynamic Media Classic案頭應用程式。

1. 下載適用於macOS的Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)

1. 使用以下命令將下載的磁碟映像(.DMG)裝載到安裝點位置：

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. 將.APP檔案複製到 **[!UICONTROL 應用程式]** 使用下列命令：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用與您在瀏覽器中登入Adobe Dynamic Media Classic時所使用的相同憑證。

   若 **[!UICONTROL 伺服器]** 若要使用，請參閱生產環境的下列對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太地區） | https://s7sps5.scene7.com/ |

## 下載和 *靜默* 在Windows®上安裝最新的Adobe Dynamic Media Classic案頭應用程式 {#install-silent-windows-dmc-app}

您使用的命令用於基本MSI靜默安裝。 但是，Adobe Dynamic Media Classic案頭應用程式安裝程式是使用InstallShield建立的InstallScript MSI安裝程式。 以記錄模式運行安裝程式時，任何用戶交互都記錄在響應檔案中。 然後，此響應檔案將用於靜默安裝，如 [以靜默模式運行安裝。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另請參閱:

* [在Mac或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用程式](#installation-dmc-app)
* [在macOS上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式](#install-silent-mac-dmc-app)

若要下載和 *靜默* 在Windows®上安裝最新版Adobe Dynamic Media Classic案頭應用程式：

1. 在您的系統上解除安裝任何舊版Adobe Dynamic Media Classic案頭應用程式。

1. 下載Adobe Dynamic Media Classic案頭應用程式的最新安裝程式。

   * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 使用以下命令在記錄模式下運行安裝程式：

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安裝程式窗口中，按照步驟進行安裝，以便交互/輸入（如安裝位置）記錄在 `Setup.iss` 檔案。

1. 複製已建立的 `Setup.iss` 檔案和 `adobe-dynamic-media-classic-20.22.1.exe` 到其他電腦。

1. 運行以下命令以進行靜默安裝：

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   有關命令行參數的詳細資訊，請參見 [Setup.exe和Update.exe命令行參數。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 開啟應用程式時，會顯示新的Adobe Dynamic Media Classic登入頁面：

   ![Adobe Dynamic Media Classic登入](/help/assets/dmclassic-login1.png)

1. 若要登入Adobe Dynamic Media Classic案頭應用程式，請使用與您在瀏覽器中登入Adobe Dynamic Media Classic時所使用的相同憑證。

   若 **[!UICONTROL 伺服器]** 若要使用，請參閱生產環境的下列對應：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太地區） | https://s7sps5.scene7.com/ |

## 使用Adobe Dynamic Media Classic案頭應用程式的影片逐步說明 {#dmc-app-video-walk-through}

觀看 [使用Adobe Dynamic Media Classic案頭應用程式的影片逐步說明](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (長度：2分36秒)。

## 使用案頭應用程式清除電腦上的影像快取和資產快取 {#clear-cache}

1. 在Adobe Dynamic Media Classic案頭應用程式右上角附近，點選 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 在 **[!UICONTROL 個人設定]** 頁面下方 **[!UICONTROL 案頭]** 標題，執行下列任一操作：
   * 若要從電腦移除所有AdobeDynamic Media快取影像檔案，請點選 **[!UICONTROL 清除影像快取]**，然後點選 **[!UICONTROL 確定]**.
   * 若要從電腦移除所有AdobeDynamic Media快取資產檔案，請點選 **[!UICONTROL 清除資產快取]**，然後點選 **[!UICONTROL 確定]**.
1. 在頁面的右下角，點選 **[!UICONTROL 關閉]**.

### 手動清除影像快取和資產快取

除了使用案頭應用程式清除影像和資產快取外，您也可以直接從檔案系統手動清除快取。

1. 根據您的作業系統，導覽至下列項目：

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic的已知限制20.21.1

* 此 **[!UICONTROL 伺服器]** 更新至Adobe Dynamic Media Classic案頭應用程式後，下拉式清單為空20.21.1 — 案例：安裝並登入Adobe Dynamic Media Classic 20.20.1或20.20.2，然後關閉應用程式。 然後更新為Adobe Dynamic Media Classic 20.21.1。嘗試登錄時， **[!UICONTROL 伺服器]** 下拉式清單 **[!UICONTROL 登入您的帳戶]** 對話框為空。 若要解決此問題，您必須 [手動清除快取](#clear-cache) （請參閱上述步驟）。

## Adobe Dynamic Media Classic 20.20.1的已知限制(20.20.2中修正)

**_僅適用於Windows® — 是否對可通過案頭應用程式UI上載的檔案數有限制？_**<br>是的，一次最多可透過案頭應用程式UI上傳150個檔案。

**_適用於Windows®和macOS — 如何在公司之間切換？_**<br>要在公司之間切換，請執行以下操作：

* 在Adobe Dynamic Media Classic應用程式中，從公司下拉式清單中選取新公司。
* 出現快顯視窗時，點選 **[!UICONTROL 確定]** 登出並關閉應用程式。

   ![若要使用新公司，請重新啟動應用程式](/help/assets/dmclassic-new-company1.png)

* 重新啟動Adobe Dynamic Media Classic，然後照常登入以與新公司合作。

## 提示與秘訣

**_我在Adobe Dynamic Media Classic的登陸頁面上看不到「媒體購物車」面板。_**<br>在Adobe Dynamic Media Classic中，點選**[!UICONTROL 設定>個人設定&#x200B;]**. 在「瀏覽器」區段中，確定**[!UICONTROL 顯示MediaPortal功能&#x200B;]**已選取（已勾選）。 點選**[!UICONTROL 儲存>關閉&#x200B;]**.

**_資產的發佈狀態（綠色指標）未正確反映。_**<br>在瀏覽器使用者介面中，必須重新登入UI，才能查看資產的正確發佈狀態。 在案頭應用程式中，Adobe已導入**[!UICONTROL 重新整理&#x200B;]**圖示**[!UICONTROL 選擇無&#x200B;]**按鈕。 點選**[!UICONTROL 重新整理&#x200B;]**圖示來查看指定頁面上所有資產的最新狀態。 瀏覽器UI不需要重新登入。

![重新整理圖示](/help/assets/refresh-icon1.png)
*重新整理圖示*

**_我看不到批集預設集在案頭應用程式中工作。_**<br>點選**[!UICONTROL 上傳>作業選項>批集預設集&#x200B;]**. 確保**[!UICONTROL 批集預設集&#x200B;]**啟用。 按一下**[!UICONTROL 儲存並提交上傳&#x200B;]**.
