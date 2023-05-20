---
title: 銳利化影像
description: 瞭解如何在Adobe Dynamic Media Classic銳化影像。
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2278'
ht-degree: 41%

---

# 銳利化影像 {#sharpening-an-image}

銳利化是一種影像操作技巧，使數位影像的外框看起來更為清晰。銳利化可增加邊緣像素之間的對比，並強調深色區域與淺色區域之間的切換。銳利化可提高局部對比，顯現精緻的細節。要讓所有影像正確銳利化，並沒有嚴格的公式可循。銳利化不足會造成影像輪廓不鮮明，而過度銳利化會增加光暈、不自然感和雜訊。

Adobe Dynamic Media Classic強烈建議對所有影像使用「影像預設」。 它們確保大小一致，並且對使用「影像預設」調用的任何影像強制進行銳化。 此外，您可以輕鬆編輯和更改「影像預設」的銳化參數。 您下一次發佈時，呼叫含有該預設集的所有影像都會擁有該新值。

Adobe Dynamic Media Classic還建議將銳化添加到查看器預設，然後使用該預設調用查看器。 這樣可以確保觀眾中的影像清晰而吸引人。

但是，無論您是使用「影像預設」和「查看器預設」，還是使用某種替代的銳化方法，最終都必須銳化影像。 如果你不這樣做，你的影像（和網站）可能看上去很柔和模糊。

>[!NOTE]
>
>「銳利化」命令會覆蓋「影像預設集」設定，包括其中的銳利化效果。「影像預設」控制從Dynamic Media影像伺服器傳送影像的大小和格式。 Adobe Dynamic Media Classic強烈建議使用「影像預設」來傳送所有影像，以確保以均勻的大小和銳化方式傳送影像。 不過，變更個別影像的銳利化設定之後，「影像預設集」的銳利化設定就不再適用於該影像。它會在不含「影像預設集」銳利化設定的情況下傳送。

通常必須將影像銳利化。Adobe Dynamic Media Classic和影像伺服器提供了多種銳化選項。 請務必瞭解銳利化對影像造成的變化，以及所需的銳利化程度為何。大部分的影像都需要進行一些銳利化，不過所需的銳利化程度則取決於影像。

影像銳利化會增加像素的對比，以產生強調邊緣的效果。人們將這種加強的邊緣對比視為銳利。雖然在影像上執行銳利化濾鏡即可輕鬆改善影像，不過這樣也很容易過度銳利化影像。

過度銳利化影像會產生光暈效果，或使邊緣線條產生條紋。

您可以遵循一些最佳實踐來優化Adobe Dynamic Media Classic和Dynamic Media映像伺服器上的映像銳化。

請參閱 [在Adobe Dynamic Media Classic和Dynamic Media映像伺服器上銳化映像的最佳做法](/help/assets/s7_sharpening_images.pdf)。

另請參閱 [銳化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 培訓視頻。

**銳利化影像:**

要銳化影像，請選擇其滾動影像 **[!UICONTROL 編輯]** 按鈕 **[!UICONTROL 銳化]**，或在「詳細資訊視圖」的「瀏覽面板」中開啟它，然後選擇 **[!UICONTROL 銳化]**。 「銳度編輯器」(Sharency Editor)頁面隨即開啟，其中帶有銳化命令。 選擇命令，然後選擇 **[!UICONTROL 保存]**。

>[!NOTE]
>
>銳利化影像之前，選取「套用預設集」選單，然後選擇「影像預設集」，即可查看銳利化效果。「影像預設」的銳化效果適合影像。 的 **[!UICONTROL 應用預設]** 菜單開啟它。

**銳化選項**

下表顯示影像伺服器銳利化選項。

| 名稱 | URL 通訊協定 | 值 | 範例 |
| --- | --- | --- | --- |
| 簡單銳利化 | `op_sharpen` | `0` 或 `1` | `op_sharpen=1` |
| 重新取樣模式 | `resMode` | `bilin`。 `bicub`。 `sharp2`。 `trilin`<br><br>`bilin`:選擇標準雙線性插值。 快速重採樣方法；一些鋸齒偽像通常是可以察覺的。<br>`bicub`:選擇雙三次插值。 比 bilin 需要更大量的 CPU，但是會產生較銳利的影像，且鋸齒狀不自然感較不明顯。<br><br>`sharp2`:選擇修改的Lanczos Windows®函式作為插值算法。 在CPU成本較高的情況下，結果比雙立方的結果更清晰。<br><br>`trilin`: 選取已修改的三線性式內插補點，它會同時使用較高與較低解析度 (如果有的話)。建議只在必須要解決鋸齒問題時才使用，因為減少了高頻率資料，所以會降低 JPEG 大小。 | `resMode=sharp2` |
| 遮色片銳利化調整 | `op_usm` | `amount`。 `radius`。 `threshold`。 `monochrome`<br><br>`amount`:過濾器強度因子（實數0..5）<br><br>`radius`:篩選內核半徑（以像素為單位）（實數0..250） <br><br>`threshold`:篩選器閾值級別(int 0...255)<br><br>`monochrome`:設定為 `0` 分別取消對每個顏色分量進行銳化，設定為 `1` 到非銳化蒙版影像亮度（強度） | `op_usm=1,1,10,0` |

選擇 **[!UICONTROL 銳化]** 菜單，然後選擇一個選項：

* **無**  — 禁用銳化。

* **銳化**  — 調整檔案大小後，對檔案運行簡單銳化通道。 它類似於Adobe Photoshop的「銳化」濾鏡，並支援任何用戶參數。 通常，您會使用此篩選器或 **[!UICONTROL 非銳化蒙版]**&#x200B;但不是兩者。 以最佳做法而言，不建議使用此方法，不過這個方法有助於補償模糊效果。(URL: `op_sharpen`)

* **非銳化蒙版**  — 用於對最終的下採樣影像微調銳化濾鏡效果。 可以控制效果強度、效果半徑（以像素計量）以及忽略的對比度閾值。 此效果會使用與 Photoshop 之「遮色片銳利化調整」濾鏡相同的選項。(URL: `op_usm`)

選擇以下選項，以便可以使用「非銳化蒙版」微調銳化：

* **金額**  — 控制應用於邊緣像素的對比度量。 預設是 0.0。對於高解析度的影像，您最多可以將它增加至 5.0。請將「數量」視為濾鏡飽和度的度量。的 **[!UICONTROL 金額]** 在Adobe Dynamic Media Classic的設定與在Adobe Photoshop的「金額」設定不同。 Adobe Photoshop使用1%至500%的比例，而Adobe Dynamic Media Classic則從0.0到5.0。 (5.0 約等於 Photoshop 中的 500%，0.9 類似於 90%，以此類推。)

* **半徑**  — 確定影響銳化的邊緣像素周圍的像素數。 該效果會在影像的所有像素上執行，並以放射狀向所有方向輻射散開。

最佳的半徑值取決於影像大小。較低的數值只會銳利化邊緣的像素。較高的數值會銳利化較寬的像素範圍。

例如，要對2000 x 2000像素影像和500 x 500像素影像獲得類似的銳化效果，可以在2000 x 2000像素影像上設定兩個像素的半徑值。 然後，將 500 x 500 像素影像的半徑值設為 1 個像素 (較多像素的影像要用較大的值)。

* **閾值**  — 確定應用非銳化蒙版濾鏡時要忽略的對比度範圍。 這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。

閾值使用0到255之間的值，即灰度影像中的亮度階數。 0=黑、128=50% 灰，而 255=白。例如，會忽略輕微變化的臨界值 12 為皮膚色調亮度，因此不會增加雜訊，同時會增加反差區域的邊緣對比，例如睫毛碰到皮膚的地方。

舉例來說，假設您有一張某人臉部的相片。「遮色片銳利化調整」會影響影像中對比最大的部分以及平滑皮膚本身。即使是最平滑的皮膚也會顯現亮度值的細微變化。如果您不使用臨界值，則濾鏡會在皮膚像素中強調這些細微的變化，因而建立雜訊效果 (可能是不必要的)，同時也會增加睫毛的對比，進而改善銳利度 (可能是必要的)。為了避免這個問題，請使用臨界值以告知濾鏡忽略不要大幅更改對比的像素，例如平滑皮膚。為避免使用肉色色調引入雜訊或色調後驗，例如嘗試使用 **[!UICONTROL 閾值]** 值2到20 預設 **[!UICONTROL 閾值]** 值0將銳化影像中的所有像素。

* **應用於**  — 選擇 **[!UICONTROL 每種顏色]** 要將銳化分別應用於每個顏色分量；選擇 **[!UICONTROL 亮度]** 的子菜單。

**重新取樣**

選擇 **[!UICONTROL 重採樣]** 的子菜單。 下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL 無]**  — 關閉重新取樣。

* **[!UICONTROL 雙線性]**  — 最快的重採樣方法；有些鋸齒偽影是可以察覺的。

* **[!UICONTROL 雙立方]**  — 提高影像伺服器上的CPU使用率，但生成更清晰的影像，並減少明顯的鋸齒偽像。

* **[!UICONTROL 銳化2]**  — 結果比 **[!UICONTROL 雙立方]**，但映像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 如果可用，則使用較高和較低解析度；僅在出現混淆時建議。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

**銳化和影像預設**

您可以合併所有三種銳化效果，以獲得最終結果。 但是，不建議使用此方法。 Adobe Dynamic Media Classic建議將銳化效果保存為「影像預設」的一部分。 「影像預設」允許您將最常用的影像修飾符打包，以在小文本字串中建立動態調整大小的影像。 「影像預設」包含檔案格式(通常為webJPEG)、像素數和影像銳化的值。 不要將URL附加到必須用於建立特定類型影像大小的每個影像修飾符，而是建立命名的影像預設，如「縮略圖」。 然後，使用適當的大小、檔案格式和銳化選項配置縮略圖「影像預設」。 使用「影像預設」名稱調用影像。 「影像預設」可縮短整個URL的長度。 這兩個URL生成的350x350JPEG影像與銳化影像相同：

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

影像預設集可隨時更改和更新。在發佈後和清除URL的快取後，您會看到更改為「影像預設」的結果。

如果您針對大小類別中的每個影像都使用一個預設集，則任何公司管理員都可以更新該影像預設集的定義、重新發佈，並影響每個使用該格式的影像，而不需要更改任何網頁程式碼。最佳實踐就是在網站上根據每一種大小使用一個影像預設集。要添加影像預設，請在「全局導航」欄上，轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設]**。 然後，選擇 **[!UICONTROL 添加]** 或 **[!UICONTROL 編輯]** 更改現有預設。 唯一的必填欄位為預設集本身的名稱。但是，最好在每個預設中都包含一些銳化級別。

**JPG 品質**

「JPG 品質」選項可控制 JPG 壓縮層級:

* **JPG質量**  — 如果要控制壓縮級別和色度下採樣，請選擇此選項。

* **滑塊**  — 確定JPG壓縮級別。 這個設定會同時影響檔案大小與影像品質。JPG質量等級為1-100。

* **啟用JPG色度下採樣**  — 由於眼睛對高頻顏色資訊的敏感度低於高頻亮度，JPEG影像將影像資訊分為亮度和顏色分量。 壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣可將資料量減少三分之一或二分之一，而且幾乎不會影響肉眼能感知的品質。縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。

**設定公司範圍的銳化選項**

如果未使用影像預設集或要使用 URL 字串通過特定的影像伺服器銳利化通訊協定，則縮減取樣時，影像不會銳利化。但是，如果出現這種缺少銳化的情況，則可以設定預設銳化值，然後任何影像都始終具有一些銳化。

要設定公司的預設銳化選項，請轉到 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 映像伺服器]**。 如果將「預設重採樣模式」(Default Resacking Mode)設定為 **[!UICONTROL 夏普2]**，在下採樣時，它總是會銳化影像。

**將銳化添加到查看器預設**

除非您將銳利化影像修飾元增加至預設集，否則小型的初始載入影像可能會看起來柔化，因為該影像是經過縮減取樣以符合檢視器視窗，而未進行銳利化。

查看器預設（如影像預設）允許您將許多選項集中到一個位置，包括外觀選項和查看器選項（如包括「打印」按鈕或控制縮放動畫的速度）。 「查看器預設」與「影像預設」在同一部分，位於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 查看器預設]**。

請參閱 [查看器預設](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 培訓視頻。

「修飾元」選項則位於所有「eCatalog」、「迴轉」與「自訂縮放檢視器預設集」的「Core 設定」區段下。將 URL 銳利化命令增加至「修飾元」方框後，每次呼叫含有該檢視器預設集的檢視器時，您都可以增加銳利化。

要調用查看器預設，請使用 `config=` 的子菜單。 下面是使用查看器預設(`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

此處的預設集會銳利化並更改預設的檢視器外觀。

**建立特定於映像的覆蓋**

最後一個 (最不建議的) 銳利化方法是以逐一影像為基礎來建立銳利化覆蓋。此方法用其自己的特定值覆蓋影像預設中的銳化。 但是，此方法也會覆蓋任何大小的所有其他銳化方法。 如果某些影像的解析度不夠高，且影像預設集中的值對於這些小型影像而言太高時，最適合使用此方法。在這種情況下，可能需要對每個影像銳化一些。

在Adobe Dynamic Media Classic，選擇任意影像，轉到「細節視圖」（通過按兩下或按） **[!UICONTROL 詳細資訊視圖]** )，然後選擇 **[!UICONTROL 銳化]**。 更改任何參數，然後選擇 **[!UICONTROL 保存]**。 此過程會通知影像伺服器使用這些銳化參數，而不是您在URL中調用的任何命令，如銳化修飾符或影像預設。 確保發佈以查看更改是否生效。
