---
title: 銳利化影像
description: 瞭解如何在Adobe Dynamic Media Classic中銳利化影像。
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '2267'
ht-degree: 38%

---

# 銳利化影像 {#sharpening-an-image}

銳利化是一種影像操作技巧，使數位影像的外框看起來更為清晰。銳利化可增加邊緣像素之間的對比，並強調深色區域與淺色區域之間的切換。銳利化可提高局部對比，顯現精緻的細節。要讓所有影像正確銳利化，並沒有嚴格的公式可循。銳利化不足會造成影像輪廓不鮮明，而過度銳利化會增加光暈、不自然感和雜訊。

Adobe Dynamic Media Classic強烈建議您對所有影像使用影像預設集。 它們可確保大小一致，而且會強制對使用影像預設集呼叫的任何影像進行銳利化。 此外，您可以輕鬆編輯和變更影像預設集的銳利化引數。 您下一次發佈時，呼叫含有該預設集的所有影像都會擁有該新值。

Adobe Dynamic Media Classic也建議為檢視器預設集新增銳利化，然後使用該預設集呼叫檢視器。 這麼做可確保檢視器內的影像清晰迷人。

不過，無論您是使用影像預設集和檢視器預設集，還是某些銳利化方法，底線是您必須銳利化影像。 否則，您的影像（和網站）可能會顯得既柔和又模糊。

>[!NOTE]
>
>「銳利化」命令會覆蓋「影像預設集」設定，包括其中的銳利化效果。影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 Adobe Dynamic Media Classic強烈建議使用影像預設集來傳送所有影像，以確保影像是以一致的大小和銳利化來傳送。 不過，變更個別影像的銳利化設定之後，「影像預設集」的銳利化設定就不再適用於該影像。它會在不含「影像預設集」銳利化設定的情況下傳送。

通常必須將影像銳利化。Adobe Dynamic Media Classic和影像伺服器提供數個銳利化選項。 請務必瞭解銳利化對影像造成的變化，以及所需的銳利化程度為何。大部分的影像都需要進行一些銳利化，不過所需的銳利化程度則取決於影像。

影像銳利化會增加像素的對比，以產生強調邊緣的效果。人們將這種加強的邊緣對比視為銳利。雖然在影像上執行銳利化濾鏡即可輕鬆改善影像，不過這樣也很容易過度銳利化影像。

將影像過度銳利化會產生光暈效果，或邊緣線條的帶狀效果。

您可以遵循最佳實務，在Adobe Dynamic Media Classic和Dynamic Media影像伺服器上最佳化影像銳利化。

另請參閱 [在Adobe Dynamic Media Classic和Dynamic Media Image Server上銳利化影像的最佳做法](/help/using/assets/s7_sharpening_images.pdf).

另請參閱 [銳利化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 訓練影片。

**銳利化影像:**

若要銳利化影像，請選取其滑鼠指向效果 **[!UICONTROL 編輯]** 按鈕並選擇 **[!UICONTROL 銳利化]**，或在「瀏覽」面板的「詳細資訊」檢視中開啟它，然後選取「 」 **[!UICONTROL 銳利化]**. 「銳利化編輯器」頁面隨即開啟，其中包含銳利化指令。 選擇命令，然後選取 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>銳利化影像之前，選取「套用預設集」選單，然後選擇「影像預設集」，即可查看銳利化效果。影像預設集的銳利化效果適用於您的影像。 此 **[!UICONTROL 套用預設集]** 功能表位於「銳利度編輯器」頁面的底部。

**銳利化選項**

下表顯示影像伺服器銳利化選項。

| 名稱 | URL 通訊協定 | 值 | 範例 |
| --- | --- | --- | --- |
| 簡單銳利化 | `op_sharpen` | `0` 或 `1` | `op_sharpen=1` |
| 重新取樣模式 | `resMode` | `bilin`， `bicub`， `sharp2`， `trilin`<br><br>`bilin`：選取標準的雙線性內插。 最快速的重新取樣方法；通常會出現一些鋸齒狀不自然感。<br>`bicub`：選取雙三次插值法。 比 `bilin` 需要更大量的 CPU，但是會產生較銳利的影像，且鋸齒狀不自然感較不明顯。<br><br>`sharp2`：選取修改過的Lanczos Windows®函式作為內插演演算法。 可以產生比雙立方體稍微銳利的結果，但CPU成本較高。<br><br>`trilin`: 選取已修改的三線性式內插補點，它會同時使用較高與較低解析度 (如果有的話)。建議只在必須要解決鋸齒問題時才使用，因為減少了高頻率資料，所以會降低 JPEG 大小。 | `resMode=sharp2` |
| 遮色片銳利化調整 | `op_usm` | `amount`， `radius`， `threshold`， `monochrome`<br><br>`amount`：濾鏡強度係數（實數0...5）<br><br>`radius`：濾鏡核心半徑，以畫素為單位（實數0...250） <br><br>`threshold`：濾鏡臨界值層級(int 0...255)<br><br>`monochrome`：設為 `0` 若要分別取消銳利化遮色片每個顏色元件，請將設為 `1` 以銳利化遮色片影像亮度（強度） | `op_usm=1,1,10,0` |

選取 **[!UICONTROL 銳利化]** 功能表並選擇一個選項：

* **無**  — 停用銳利化。

* **銳利化**  — 在調整檔案大小後，對檔案執行簡單的銳利化傳遞。 它類似於Adobe Photoshop中的「銳利化」濾鏡，不支援任何使用者引數。 通常您會使用此篩選器或 **[!UICONTROL 不銳利化遮色片]**，但不能同時使用兩者。 以最佳做法而言，不建議使用此方法，不過這個方法有助於補償模糊效果。(URL: `op_sharpen`)

* **不銳利化遮色片**  — 可讓您微調最終縮減取樣影像的銳利化濾鏡效果。 您可以控制效果的強度、效果的半徑（以畫素測量），以及被忽略的對比度臨界值。 此效果使用與Photoshop的「遮色片銳利化」濾鏡相同的選項。 (URL: `op_usm`)

選擇下列選項，以使用「不銳利化遮色片」微調銳利化：

* **數量**  — 控制套用至邊緣畫素的對比量。 預設是 0.0。對於高解析度的影像，您最多可以將它增加至 5.0。請將「數量」視為濾鏡飽和度的度量。此 **[!UICONTROL 數量]** Adobe Dynamic Media Classic中的設定與Adobe Photoshop中的金額設定不同。 Adobe Photoshop使用的數量範圍為1%到500%，而Adobe Dynamic Media Classic的範圍為0.0到5.0。 (5.0 約等於 Photoshop 中的 500%，0.9 類似於 90%，以此類推。)

* **半徑**  — 決定邊緣畫素周圍影響銳利化的畫素數量。 該效果會在影像的所有像素上執行，並以放射狀向所有方向輻射散開。

最佳的半徑值取決於影像大小。較低的數值只會銳利化邊緣的像素。較高的數值會銳利化較寬的像素範圍。

例如，若要針對2000 × 2000畫素影像和500 × 500畫素影像取得類似的銳利化效果，您可以在2000 × 2000畫素影像上設定兩個畫素的半徑值。 然後，在500 × 500畫素影像上設定一個畫素的半徑值（畫素較多時影像的值較大）。

* **臨界值**  — 決定套用遮色片銳利化調整濾鏡時要忽略的對比範圍。 這個選項決定銳利化的像素必須與周圍的區域有多大的差異，才會被視為邊緣像素並予以銳利化。

「臨界值」使用從0到255的值，也就是灰階影像中的亮度階數。 0=黑、128=50% 灰，而 255=白。例如，會忽略輕微變化的臨界值 12 為皮膚色調亮度，因此不會增加雜訊，同時會增加反差區域的邊緣對比，例如睫毛碰到皮膚的地方。

例如，假設您有一張某人的臉部照片。 「遮色片銳利化調整」會影響影像中對比最大的部分以及平滑皮膚本身。即使是最平滑的皮膚也會顯現亮度值的細微變化。如果您不使用臨界值，則濾鏡會在皮膚像素中強調這些細微的變化，因而建立雜訊效果 (可能是不必要的)，同時也會增加睫毛的對比，進而改善銳利度 (可能是必要的)。為了避免這個問題，請使用臨界值以告知濾鏡忽略不要大幅更改對比的像素，例如平滑皮膚。若要避免在影像中引進雜訊或後期化與肉色調，例如，嘗試使用 **[!UICONTROL 臨界值]** 值2到20。 預設 **[!UICONTROL 臨界值]** 值0會銳利化影像中的所有畫素。

* **套用到**  — 選擇 **[!UICONTROL 每種顏色]** 如果您想要個別套用銳利化至每個色彩元件，請選擇 **[!UICONTROL 亮度]** 如果要將銳利化套用至影像亮度區域。

**重新取樣**

選取 **[!UICONTROL 重新取樣]** 選單並選擇選項。 下列選項會在縮減取樣影像時予以銳利化:

* **[!UICONTROL 無]**  — 關閉重新取樣。

* **[!UICONTROL 雙線性式]**  — 最快速的重新取樣方法；會產生某些明顯的鋸齒狀不自然感。

* **[!UICONTROL 雙立方式]**  — 增加影像伺服器上的CPU使用量，但會產生較清晰的影像，且鋸齒狀不自然感較不明顯。

* **[!UICONTROL `Sharpen2`]**  — 產生的結果會比 **[!UICONTROL 雙立方式]**，但影像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 同時使用較高和較低解析度（如果有的話）；只有在別名是問題的情況下才建議使用。 這個方法會減少高頻率資料，所以能夠減少 JPEG 大小。

**銳利化和影像預設集**

您可以合併所有三種銳利化效果，以獲得最終結果。 但是，不建議使用此方法。 Adobe Dynamic Media Classic建議您將銳利化效果儲存為影像預設集的一部分。 影像預設集可讓您封裝最常使用的影像修飾元，以小文字字串建立動態調整大小的影像。 影像預設集包含檔案格式(通常是網頁的JPEG)、畫素計數和影像銳利化的值。 您不應該將URL附加至您必須用來建立特定影像大小型別的每個影像修飾元，而是要建立已命名的影像預設集，例如「縮圖」。 然後，使用適當的大小、檔案格式和銳利化選項來設定縮圖「影像預設集」。 使用影像預設集名稱呼叫影像。 影像預設集可縮短整體URL的長度。 這兩個URL會產生相同的350x350JPEG銳利化影像：

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

影像預設集可隨時更改和更新。您可以在發佈後和URL快取清除後，看到影像預設集變更的結果。

如果您針對大小類別中的每個影像都使用一個預設集，則任何公司管理員都可以更新該影像預設集的定義、重新發佈，並影響每個使用該格式的影像，而不需要更改任何網頁程式碼。最佳實踐就是在網站上根據每一種大小使用一個影像預設集。若要新增影像預設集，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設集]**. 然後選取 **[!UICONTROL 新增]** 或選取 **[!UICONTROL 編輯]** 以變更現有的預設集。 唯一的必填欄位為預設集本身的名稱。不過，最好在每個預設集中加入某種程度的銳利化。

**JPG 品質**

「JPG 品質」選項可控制 JPG 壓縮層級:

* **JPG品質**  — 如果要控制壓縮等級和色度縮減取樣，請選取此選項。

* **滑桿**  — 決定JPG壓縮等級。 這個設定會同時影響檔案大小與影像品質。JPG品質比例為1-100。

* **啟用JPG色度縮減取樣**  — 由於眼睛對高頻色彩資訊的敏感性低於高頻明度，JPEG影像會將影像資訊分成明度和色彩元件。 壓縮 JPEG 影像時，明度組件會保留完整解析度，而色彩組件則會透過平均像素群組來縮減取樣。縮減取樣將資料量減少一半或三分之一，幾乎不影響感知品質。 縮減取樣不適用於灰階影像。這個技巧可減少適用於高對比度影像的壓縮量 (例如含有覆蓋文字的影像)。

**設定全公司的銳利化選項**

如果未使用影像預設集或要使用 URL 字串通過特定的影像伺服器銳利化通訊協定，則縮減取樣時，影像不會銳利化。不過，如果發生這種缺乏銳利化的情況，您可以設定預設銳利化值，然後任何影像就會一律有一些銳利化。

若要設定貴公司的預設銳利化選項，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]**. 如果您將「預設重新取樣模式」設定為 **[!UICONTROL `Sharp2`]**&#x200B;時，縮減取樣一律會銳利化影像。

**新增銳利化至檢視器預設集**

除非您將銳利化影像修飾元增加至預設集，否則小型的初始載入影像可能會看起來柔化，因為該影像是經過縮減取樣以符合檢視器視窗，而未進行銳利化。

檢視器預設集（如影像預設集）可讓您將許多選項集中到一個位置，包括外觀和檢視器選項（例如包括「列印」按鈕或控制縮放動畫的速度）。 檢視器預設集位於與影像預設集相同的區段中，位於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 檢視器預設集]**.

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

「修飾元」選項則位於所有「eCatalog」、「迴轉」與「自訂縮放檢視器預設集」的「Core 設定」區段下。將 URL 銳利化命令增加至「修飾元」方框後，每次呼叫含有該檢視器預設集的檢視器時，您都可以增加銳利化。

若要呼叫檢視器預設集，請使用 `config=` 命令於檢視器URL上。 以下是呼叫含有檢視器預設集（鞋子）的影像集的範例`FantasticoZoom2022`)：

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

此處的預設集會銳利化並更改預設的檢視器外觀。

**建立影像專用覆寫**

最後一個 (最不建議的) 銳利化方法是以逐一影像為基礎來建立銳利化覆蓋。此方法會以影像預設集自己的特定值覆寫銳利化。 不過，此方法也會以任何大小覆寫所有其他銳利化方法。 如果某些影像的解析度不夠高，且影像預設集中的值對於這些小型影像而言太高時，最適合使用此方法。在此情況下，可能需要針對個別影像進行某些銳利化。

在Adobe Dynamic Media Classic中，選取任何影像，前往「詳細資料檢視」（按兩下或按） **[!UICONTROL 詳細資料檢視]** 按鈕)，然後選取 **[!UICONTROL 銳利化]**. 變更任何引數，然後選取 **[!UICONTROL 儲存]**. 此程式會告知影像伺服器使用這些銳利化引數，而非您在URL中呼叫的任何命令，例如銳利化修飾元或影像預設集。 請確定您已發佈，變更才會生效。
