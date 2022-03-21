---
title: Adobe Dynamic Media Classic案頭應用 — 現已提供
description: 瞭解有關Adobe Dynamic Media Classic案頭應用程式的詳細資訊。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: f0c02d40a1a84e52b25d1c4558958af970859a07
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 1%

---

# 現在可用：Adobe Dynamic Media Classic案頭應用 {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic用戶現在可以使用一種新的案頭應用程式體驗，這種體驗不再依賴於瀏覽器中的AdobeFlash技術。

此新應用現在可用於Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建議您在2020年10月1日之前安裝新的Adobe Dynamic Media Classic案頭應用。 這樣做將確保在2020年12月31日棄用AdobeFlash Player之前進行平穩過渡。 在該日期之後，您無法登錄到瀏覽器版本的Adobe Dynamic Media Classic用戶介面，該產品中標有Adobe Dynamic Media Classic。

請參閱常見問題 [新的Adobe Dynamic Media Classic登錄體驗現已推出。](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic案頭應用的系統要求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic案頭應用與以下作業系統相容：

* macOS10.10或更高版本。

   >[!NOTE]
   >
   >Dynamic Media Classic案頭應用與macOS蒙特利一起使用時，功能正在下降。 因此，Adobe正在努力在未來幾週發佈新的案頭應用程式版本。

* Windows® 7或更高版本。

未在Adobe Dynamic Media Classic案頭應用程式內生成升級通知 *小* 版本。 從次發行版中的修復中獲益的客戶可以升級。

## 在最新版本(20.22.1)中修復 {#release-jan2022}

* 影像編輯 **[!UICONTROL 保存]** 按鈕無法正常工作。
* 在集編輯器中， **[!UICONTROL 關閉]**。 **[!UICONTROL 保存]**, **[!UICONTROL 另存為]** 在中滾動資產後，按鈕將被禁用 **[!UICONTROL 添加資產]** 的子菜單。
* **[!UICONTROL 播放]** 「視頻詳細資訊」視圖中的按鈕無效。
* 無法輸入 `d` 和 `e` 在 **[!UICONTROL 用戶名]** 和 **[!UICONTROL 密碼]** 經營macOS蒙特利時的田地。
* 已將剩餘的分析API移至2.0版。

## 20.21.3版中的修復 {#release-sept2021}

* 案頭應用上一段不活動時間後出現的資產的縮略圖已損壞。
* 案頭應用停止響應，通常在設定操作後。
* 請求模糊處理和鎖定模式在下自動啟用 **[!UICONTROL Test影像服務]**。

   請參閱 [Test安全測試服務](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service)。

* 更新了與Adobe Analytics的身份驗證機制。 與新整合相關，或者是否必須從Dynamic Media Classic案頭應用程式內更新某些分析變數。

   請參閱 [登錄Adobe Analytics](/help/log-analytics.md) 的子菜單。

## 20.21.2版中的修復 {#minor-release}

* 20.21.1中的已知限制：這樣 **[!UICONTROL 伺服器]** 登錄螢幕上的下拉清單為空。
* 在 **[!UICONTROL 上載作業選項]**，圖層命名預設值 **[!UICONTROL Photoshop選項]**，現在 **[!UICONTROL Photoshop和層名稱]**。 PSD 檔案中的圖層以個別影像上載。
   * 早期的預設值 **[!UICONTROL 層名稱]**，在PSD檔案中將影像命名為其層名或層號。 如果PSD檔案中的層名是預設的Photoshop層名，則使用層號。
   * 新預設值 **[!UICONTROL Photoshop和層名稱]**，在PSD檔案後面命名影像，後面跟圖層名稱或圖層編號。 如果 PSD 檔案中的圖層名稱為預設的 Photoshop 圖層名稱，則會使用圖層編號命名。
   * 鑑於Adobe Dynamic Media Classic的圖層影像現在具有唯一的名稱，將不會更新現有PSD或模板(原始PSD檔案中共用的圖層名稱)。
* 資產的縮略圖已損壞。

## 20.21.1版中的修復 {#latest-fixes-desktop-app}

* 由於超時而導致以下消息的登錄問題： *未經許可，可將此用戶分配給組。 請與管理員聯繫。*
* 查看器預設與每次錯誤的密碼嘗試重複。
* 由於根資料夾中的許多資產，案頭應用程式無響應。 (已在Windows®上修復；在macOS工作。)

## 20.20.2版中的修復 {#previous-version-fixes-desktop-app}

* 通過案頭應用用戶介面可以為macOS和Windows®上載的檔案數不受限制。
* 無需註銷案頭應用即可在公司之間切換。
* Ctrl+V用於貼上操作現在可在Windows®上使用。
* 將來，當案頭應用的新版本發佈時，用戶將在案頭應用本身內收到通知。

## 在macOS或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用 {#installation-dmc-app}

另請參閱:

* [下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式在Mac](#install-silent-mac-dmc-app)
* [在Windows®上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用](#install-silent-windows-dmc-app)

1. 卸載系統上所有舊版Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載Adobe Dynamic Media Classic案頭應用的最新安裝程式。

   * 最新版本(20.22.1)可從以下位置獲得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * 以前的版本(20.21.3)可在以下位置獲得：

      * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根據您下載的安裝程式執行下列操作之一。

   * **macOS**  — 在 **[!UICONTROL 拖放以安裝]** 對話框，拖動 **[!UICONTROL Adobe Dynamic Media Classic]** 然後放上 **[!UICONTROL 應用程式]**。

      ![拖放安裝到macOS](/help/assets/dragondrop-install1.png)

   * 在 **[!UICONTROL 應用程式]** 資料夾，按一下「Adobe Dynamic Media Classic」表徵圖。
   * 在對話框中，點擊 **[!UICONTROL 開啟]** 開啟Adobe Dynamic Media Classic案頭應用。

      ![開啟下載的應用](/help/assets/open-dmclassicapp1.png)

   * **窗口**  — 運行安裝程式二進位檔案，並按照螢幕說明安裝案頭應用。

1. 開啟應用程式時，將顯示新的Adobe Dynamic Media Classic登錄頁：

   ![Adobe Dynamic Media Classic登錄](/help/assets/dmclassic-login1.png)

1. 要登錄到Adobe Dynamic Media Classic案頭應用，請使用您在瀏覽器中登錄Adobe Dynamic Media Classic時使用的相同憑據。

   對於 **[!UICONTROL 伺服器]** 要使用，請參閱生產環境的以下映射：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

1. 登錄後，請注意熟悉的瀏覽器用戶介面體驗。 你可以像往常一樣在案頭應用上繼續你的日常Adobe Dynamic Media Classic活動。

## 下載和 *默* 在macOS安裝最新的Adobe Dynamic Media Classic案頭應用 {#install-silent-mac-dmc-app}

另請參閱:

* [在Mac或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用](#installation-dmc-app)
* [在Windows®上下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用](#install-silent-windows-dmc-app)

下載和 *默* 在macOS安裝最新版本的Adobe Dynamic Media Classic案頭應用：

1. 卸載系統上所有舊版Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載Adobe Dynamic Media Classic案頭應用程式macOS的最新安裝程式。

   * [macOS(.DMG) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)

1. 使用以下命令將下載的磁碟映像(.DMG)裝載到裝載點位置：

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. 將.APP檔案複製到 **[!UICONTROL 應用程式]** 使用以下命令：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. 開啟應用程式時，將顯示新的Adobe Dynamic Media Classic登錄頁：

   ![Adobe Dynamic Media Classic登錄](/help/assets/dmclassic-login1.png)

1. 要登錄到Adobe Dynamic Media Classic案頭應用，請使用您在瀏覽器中登錄Adobe Dynamic Media Classic時使用的相同憑據。

   對於 **[!UICONTROL 伺服器]** 要使用，請參閱生產環境的以下映射：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

## 下載和 *默* 在Windows®上安裝最新的Adobe Dynamic Media Classic案頭應用 {#install-silent-windows-dmc-app}

您使用的命令用於基本的MSI靜默安裝。 但是，Adobe Dynamic Media Classic案頭應用程式安裝程式是使用InstallShield建立的InstallScript MSI安裝程式。 在記錄模式下運行安裝程式時，任何用戶交互都會記錄在響應檔案中。 然後，此響應檔案將用於靜默安裝，如中所述 [在靜默模式下運行安裝。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另請參閱:

* [在Mac或Windows®上下載並安裝最新的Adobe Dynamic Media Classic案頭應用](#installation-dmc-app)
* [下載並靜默安裝最新的Adobe Dynamic Media Classic案頭應用程式在macOS](#install-silent-mac-dmc-app)

下載和 *默* 在Windows®上安裝最新版本的Adobe Dynamic Media Classic案頭應用：

1. 卸載系統上所有舊版Adobe Dynamic Media Classic案頭應用程式版本。

1. 下載Adobe Dynamic Media Classic案頭應用的最新安裝程式。

   * [Windows®(.EXE) — 下載](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 使用以下命令在記錄模式下運行安裝程式：

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安裝程式窗口中，按照安裝步驟進行安裝，以便在中記錄交互/輸入（如安裝位置） `Setup.iss` 的子菜單。

1. 複製已建立的 `Setup.iss` 檔案和 `adobe-dynamic-media-classic-20.22.1.exe` 到其他電腦。

1. 為靜默安裝運行以下命令：

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   有關命令行參數的詳細資訊，請參閱 [Setup.exe和Update.exe命令行參數。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 開啟應用程式時，將顯示新的Adobe Dynamic Media Classic登錄頁：

   ![Adobe Dynamic Media Classic登錄](/help/assets/dmclassic-login1.png)

1. 要登錄到Adobe Dynamic Media Classic案頭應用，請使用您在瀏覽器中登錄Adobe Dynamic Media Classic時使用的相同憑據。

   對於 **[!UICONTROL 伺服器]** 要使用，請參閱生產環境的以下映射：

   | 伺服器 | 瀏覽器URL |
   | --- | --- |
   | NA生產（北美） | https://s7sps1.scene7.com/ |
   | EMEA生產（歐洲、中東和非洲） | https://s7sps3.scene7.com/ |
   | APAC生產（亞太） | https://s7sps5.scene7.com/ |

## 使用Adobe Dynamic Media Classic案頭應用進行視頻瀏覽 {#dmc-app-video-walk-through}

觀看 [使用Adobe Dynamic Media Classic案頭應用進行視頻瀏覽](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (長度：2分36秒)。

## 使用案頭應用清除電腦上的映像快取和資產快取 {#clear-cache}

1. 在Adobe Dynamic Media Classic案頭應用程式右上角附近，點擊 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**。
1. 在 **[!UICONTROL 個人設定]** 的子菜單。 **[!UICONTROL 案頭]** 在標題中，執行以下任一操作：
   * 要從電腦中刪除所有AdobeDynamic Media快取的映像檔案，請點擊 **[!UICONTROL 清除映像快取]**，然後按一下 **[!UICONTROL 確定]**。
   * 要從電腦中刪除所有AdobeDynamic Media快取的資產檔案，請點擊 **[!UICONTROL 清除資產快取]**，然後按一下 **[!UICONTROL 確定]**。
1. 在頁面的右下角，點擊 **[!UICONTROL 關閉]**。

### 手動清除映像快取和資產快取

除了使用案頭應用清除映像和資產快取外，您還可以直接從檔案系統手動清除快取。

1. 根據您的作業系統，導航至以下內容：

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic的已知限20.21.1

* 的 **[!UICONTROL 伺服器]** 下拉清單在更新到Adobe Dynamic Media Classic案頭應用20.21.1後為空 — 方案：安裝並登錄到Adobe Dynamic Media Classic20.20.1或20.20.2，然後關閉應用程式。 然後你再去Adobe Dynamic Media Classic20.21.1。當您嘗試登錄時， **[!UICONTROL 伺服器]** 下拉清單 **[!UICONTROL 登錄到帳戶]** 對話框為空。 要解決這個問題，你必須 [手動清除快取](#clear-cache) （請參閱上面的步驟）。

## Adobe Dynamic Media Classic的已知限20.20.1(在20.20.2中修正)

**_僅適用於Windows® — 通過案頭應用程式UI可上載的檔案數是否有限制？_**<br>是，通過案頭應用UI一次最多可上載150個檔案。

**_適用於Windows®和macOS — 如何在公司之間切換？_**<br>要在公司之間切換，請執行以下操作：

* 在Adobe Dynamic Media Classic應用中，從公司下拉清單中選擇新公司。
* 出現彈出窗口時，點擊 **[!UICONTROL 確定]** 註銷並關閉應用。

   ![要使用新公司，請重新啟動應用](/help/assets/dmclassic-new-company1.png)

* 重新啟動Adobe Dynamic Media Classic，然後照常登錄以與新公司合作。

## 提示和技巧

**_我無法在Adobe Dynamic Media Classic的登錄頁上看到「Media Cart（媒體購物車）」面板。_**<br>在Adobe Dynamic Media Classic，點擊**[!UICONTROL 設定>個人設定&#x200B;]**。 在「瀏覽器」部分，確保**[!UICONTROL 顯示媒體門戶功能&#x200B;]**選中（已選中）。 點擊**[!UICONTROL 保存>關閉&#x200B;]**。

**_資產的發佈狀態（綠色指示器）未正確反映。_**<br>在瀏覽器用戶介面中，需要重新登錄到UI才能查看資產的正確發佈狀態。 在案頭應用中，Adobe**[!UICONTROL 刷新&#x200B;]**表徵圖**[!UICONTROL 選擇無&#x200B;]**按鈕 點擊**[!UICONTROL 刷新&#x200B;]**表徵圖，查看給定頁面上所有資產的最新狀態。 與瀏覽器UI一樣，不需要重新登錄。

![「刷新」表徵圖](/help/assets/refresh-icon1.png)
*「刷新」表徵圖*

**_我看不到在案頭應用中使用批處理集預設。_**<br>點擊**[!UICONTROL 上載>作業選項>批集預設&#x200B;]**。 確保**[!UICONTROL 批集預設&#x200B;]**的子菜單。 按一下**[!UICONTROL 保存並提交上載&#x200B;]**。
