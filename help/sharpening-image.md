---
title: 銳利化影像
description: 了解如何在Adobe Dynamic Media Classic中銳化影像。
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

Adobe Dynamic Media Classic強烈建議您對所有影像使用影像預設集。 它們可確保大小一致，且銳利化會針對任何名為「影像預設集」的影像強制執行。 此外，您還可以輕鬆編輯和更改「影像預設集」的銳利化參數。 您下一次發佈時，呼叫含有該預設集的所有影像都會擁有該新值。

Adobe Dynamic Media Classic也建議將銳利化新增至檢視器預設集，然後使用該預設集呼叫檢視器。 這麼做可確保檢視器中的影像清晰且吸引人。

不過，無論您是使用「影像預設集」和「檢視器預設集」，還是使用某些替代的銳利化方法，底線是您必須銳利化影像。 若未這麼做，您的影像（和網站）可能會看起來柔和模糊。

>[!NOTE]
>
>「銳利化」命令會覆蓋「影像預設集」設定，包括其中的銳利化效果。影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 Adobe Dynamic Media Classic強烈建議使用「影像預設集」來傳送所有影像，以確保影像以均勻的大小和銳利化傳送。 不過，變更個別影像的銳利化設定之後，「影像預設集」的銳利化設定就不再適用於該影像。它會在不含「影像預設集」銳利化設定的情況下傳送。

通常必須將影像銳利化。Adobe Dynamic Media Classic和影像伺服器提供數個銳利化選項。 請務必瞭解銳利化對影像造成的變化，以及所需的銳利化程度為何。大部分的影像都需要進行一些銳利化，不過所需的銳利化程度則取決於影像。

影像銳利化會增加像素的對比，以產生強調邊緣的效果。人們將這種加強的邊緣對比視為銳利。雖然在影像上執行銳利化濾鏡即可輕鬆改善影像，不過這樣也很容易過度銳利化影像。

過度銳利化影像會產生光暈效果，或使邊緣線條產生條紋。

您可以遵循一些最佳實務，以最佳化Adobe Dynamic Media Classic和Dynamic Media影像伺服器上影像的銳利化。

請參閱 [銳利化Adobe Dynamic Media Classic和Dynamic Media Image Server中影像的最佳作法](/help/assets/s7_sharpening_images.pdf).

另請參閱 [銳利化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 訓練影片。

**銳利化影像:**

要銳化影像，請選擇其變換 **[!UICONTROL 編輯]** 按鈕並選擇 **[!UICONTROL 銳利化]**，或在「詳細資訊檢視」的「瀏覽面板」中開啟它，然後選取 **[!UICONTROL 銳利化]**. 「銳利度編輯器」頁面隨即開啟，其中包含銳利化命令。 選擇命令，然後選擇 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>銳利化影像之前，選取「套用預設集」選單，然後選擇「影像預設集」，即可查看銳利化效果。「影像預設集」的銳利化效果適合您的影像。 此 **[!UICONTROL 套用預設集]** 菜單位於「銳度編輯器」頁的底部。

**銳利化選項**

下表顯示影像伺服器銳利化選項。

| 名稱 | URL 通訊協定 | 值 | 範例 |
| --- | --- | --- | --- |
| 簡單銳利化 | `op_sharpen` | `0` 或 `1` | `op_sharpen=1` |
| 重新取樣模式 | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`:選擇標準雙線性插值。 最快重採樣方法；有些鋸齒偽影經常會引起注意。<br>`bicub`:選擇雙三次插值。 比 bilin 需要更大量的 CPU，但是會產生較銳利的影像，且鋸齒狀不自然感較不明顯。<br><br>`sharp2`:選擇修改的Lanczos Windows®函式作為插值算法。 CPU成本較高，產生的結果會比雙立方體稍銳。<br><br>`trilin`: 選取已修改的三線性式內插補點，它會同時使用較高與較低解析度 (如果有的話)。建議只在必須要解決鋸齒問題時才使用，因為減少了高頻率資料，所以會降低 JPEG 大小。 | `resMode=sharp2` |
| 遮色片銳利化調整 | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`:過濾器強度因子（實數0..5）<br><br>`radius`:以像素為單位篩選內核半徑（實數0...250） <br><br>`threshold`:篩選閾值級別(int 0...255)<br><br>`monochrome`:設為 `0` 要單獨對每個顏色元件進行銳利化遮色，請將設定為 `1` 不銳利化遮色片影像亮度（強度） | `op_usm=1,1,10,0` |

選取 **[!UICONTROL 銳利化]** ，然後選擇選項：

* **無**  — 停用銳利化。

* **銳利化**  — 調整檔案大小後，在檔案上運行簡單銳利化刀路。 它類似於Adobe Photoshop中的「銳利化」篩選器，不支援任何使用者參數。 通常，您會使用此篩選器或 **[!UICONTROL 不銳利化遮色片]**，但不能兩者兼而有之。 以最佳做法而言，不建議使用此方法，不過這個方法有助於補償模糊效果。(URL: `op_sharpen`)

* **不銳利化遮色片**  — 可讓您微調最終縮減取樣影像的銳利化濾鏡效果。 您可以控制效果的強度、效果半徑（以像素計量），以及忽略的對比度臨界值。 此效果使用的選項與 Photoshop的「遮色片銳利化」濾鏡相同。(URL: `op_usm`)

選擇以下選項，以便使用「銳利化遮色片」來微調銳利化：

* **金額**  — 控制套用至邊緣像素的對比度量。 預設是 0.0。對於高解析度的影像，您最多可以將它增加至 5.0。請將「數量」視為濾鏡飽和度的度量。此 **[!UICONTROL 金額]** 在Adobe Dynamic Media Classic中的設定與在Adobe Photoshop中的「金額」設定不同。 Adobe Photoshop使用的量範圍為1%至500%，而Adobe Dynamic Media Classic則從0.0調整為5.0。 (5.0 約等於 Photoshop 中的 500%，0.9 類似於 90%，以此類推。)

* **半徑**  — 決定影響銳利化的邊緣像素周圍的像素數。 該效果會在影像的所有像素上執行，並以放射狀向所有方向輻射散開。

最佳的半徑值取決於影像大小。較低的數值只會銳利化邊緣的像素。較高的數值會銳利化較寬的像素範圍。

例如，若要獲得類似於2000 x 2000像素影像和500 x 500像素影像的銳利化效果，您可以在2000 x 2000像素影像上設定兩個像素的半徑值。 然後，將 500 x 500 像素影像的半徑值設為 1 個像素 (較多像素的影像要用較大的值)。

* **臨界值**  — 決定套用遮色片銳利化濾鏡時要忽略的對比度範圍。 這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。

閾值使用0到255的值，該值是灰度影像中的亮度步驟數。 0=黑、128=50% 灰，而 255=白。例如，會忽略輕微變化的臨界值 12 為皮膚色調亮度，因此不會增加雜訊，同時會增加反差區域的邊緣對比，例如睫毛碰到皮膚的地方。

舉例來說，假設您有一張某人臉部的相片。「遮色片銳利化調整」會影響影像中對比最大的部分以及平滑皮膚本身。即使是最平滑的皮膚也會顯現亮度值的細微變化。如果您不使用臨界值，則濾鏡會在皮膚像素中強調這些細微的變化，因而建立雜訊效果 (可能是不必要的)，同時也會增加睫毛的對比，進而改善銳利度 (可能是必要的)。為了避免這個問題，請使用臨界值以告知濾鏡忽略不要大幅更改對比的像素，例如平滑皮膚。為了避免在含有肉色色調的影像中引入雜訊或後驗，例如嘗試嘗試使用 **[!UICONTROL 臨界值]** 值2到20。 預設 **[!UICONTROL 臨界值]** 值0會銳化影像中的所有像素。

* **套用至**  — 選擇 **[!UICONTROL 每種顏色]** 如果要分別將銳利化應用於每個顏色元件；選擇 **[!UICONTROL 亮度]** 如果要將銳利化套用至影像亮度區域。

**重新取樣**

選取 **[!UICONTROL 重新取樣]** ，然後選擇選項。 下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL 無]**  — 關閉重新採樣。

* **[!UICONTROL 雙線性]**  — 最快的重採樣方法；一些鋸齒偽影是可以注意到的。

* **[!UICONTROL 雙比克]**  — 增加影像伺服器上的CPU使用量，但生成更清晰的影像，並且出現較少明顯的鋸齒偽影。

* **[!UICONTROL 銳利化2]**  — 產生的結果比 **[!UICONTROL 雙比克]**，但映像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 如果可用，則使用更高和更低的解析度；僅當出現鋸齒時才建議使用。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

**銳利化和影像預設集**

您可以合併所有這三種銳利化效果，以取得最終結果。 不過，不建議使用此方法。 Adobe Dynamic Media Classic建議您將銳利化效果儲存為影像預設集的一部分。 影像預設集可讓您封裝最常使用的影像修飾元，以在小文字字串中建立動態調整大小的影像。 「影像預設集」包含檔案格式(通常是網頁JPEG)、像素計數和影像銳利化的值。 您不必使用每個影像修飾元來附加URL以建立特定類型的影像大小，而是建立命名的「影像預設集」，例如「縮圖」。 然後，使用適當的大小、檔案格式和銳利化選項來配置縮圖影像預設集。 使用「影像預設集」名稱呼叫影像。 影像預設集會縮短整體URL的長度。 這兩個URL會以銳利化方式產生相同的350x350JPEG影像：

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

影像預設集可隨時更改和更新。您會在發佈後和URL的快取清除後，看到影像預設集變更的結果。

如果您針對大小類別中的每個影像都使用一個預設集，則任何公司管理員都可以更新該影像預設集的定義、重新發佈，並影響每個使用該格式的影像，而不需要更改任何網頁程式碼。最佳實踐就是在網站上根據每一種大小使用一個影像預設集。若要新增影像預設集，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設集]**. 然後，選取 **[!UICONTROL 新增]** 或選取 **[!UICONTROL 編輯]** 來更改現有預設集。 唯一的必填欄位為預設集本身的名稱。不過，最好在每個預設集中加入一些銳利化等級。

**JPG 品質**

「JPG 品質」選項可控制 JPG 壓縮層級:

* **JPG品質**  — 如果要控制壓縮級別和色度縮減採樣，請選擇此選項。

* **滑桿**  — 決定JPG壓縮級別。 這個設定會同時影響檔案大小與影像品質。JPG質量等級為1-100。

* **啟用JPG色度縮減取樣**  — 由於眼睛對高頻顏色資訊的敏感度比高頻亮度低，JPEG影像將影像資訊分為亮度和顏色分量。 壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣可將資料量減少三分之一或二分之一，而且幾乎不會影響肉眼能感知的品質。縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。

**設定公司範圍的銳利化選項**

如果未使用影像預設集或要使用 URL 字串通過特定的影像伺服器銳利化通訊協定，則縮減取樣時，影像不會銳利化。不過，如果出現此缺少銳利化，您可以設定預設銳利化值，則任何影像一律會有某些銳利化。

若要設定公司的預設銳利化選項，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]**. 如果將「預設重採樣模式」設定為 **[!UICONTROL Sharp2]**，則會在縮減取樣時銳化影像。

**將銳利化新增至檢視器預設集**

除非您將銳利化影像修飾元增加至預設集，否則小型的初始載入影像可能會看起來柔化，因為該影像是經過縮減取樣以符合檢視器視窗，而未進行銳利化。

查看器預設集（如「影像預設集」）可讓您將許多選項集中到一個位置，包括選擇外觀和查看器選項（如包括「打印」按鈕或控制縮放動畫的速度）。 檢視器預設集位於與影像預設集相同的區段，位於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 檢視器預設集]**.

請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

「修飾元」選項則位於所有「eCatalog」、「迴轉」與「自訂縮放檢視器預設集」的「Core 設定」區段下。將 URL 銳利化命令增加至「修飾元」方框後，每次呼叫含有該檢視器預設集的檢視器時，您都可以增加銳利化。

若要呼叫檢視器預設集，請使用 `config=` 命令。 以下是使用檢視器預設集(`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

此處的預設集會銳利化並更改預設的檢視器外觀。

**建立影像特定覆寫**

最後一個 (最不建議的) 銳利化方法是以逐一影像為基礎來建立銳利化覆蓋。此方法會以自己的特定值覆寫影像預設集中的銳利化。 不過，此方法也會覆寫任何大小的所有其他銳利化方法。 如果某些影像的解析度不夠高，且影像預設集中的值對於這些小型影像而言太高時，最適合使用此方法。在這種情況下，可能需要個別影像銳利化部分。

在Adobe Dynamic Media Classic中，選取任何影像，前往「詳細資料檢視」(按兩下或按 **[!UICONTROL 詳細資料檢視]** ) **[!UICONTROL 銳利化]**. 變更任何參數，然後選取 **[!UICONTROL 儲存]**. 此程式會告訴影像伺服器使用這些銳利化參數，而非您在URL中呼叫的任何命令，例如銳利化修飾元或影像預設集。 請務必發佈，以確認變更生效。
