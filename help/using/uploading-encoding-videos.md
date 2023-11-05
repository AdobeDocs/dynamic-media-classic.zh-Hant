---
title: 上傳並編碼視訊
description: 瞭解如何在Adobe Dynamic Media Classic中上傳視訊並進行編碼。
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '3951'
ht-degree: 49%

---

# 上傳並編碼視訊{#uploading-and-encoding-videos}

若要建立單一視訊或自我調整視訊集以傳送至網頁或行動裝置，您必須先將主要視訊檔案上傳至Adobe Dynamic Media Classic。 Adobe Dynamic Media Classic會將視訊編碼為MP4格式，並會以下列檔案格式發佈視訊：

* **MP4** - Adobe Dynamic Media Classic建議將MP4作為慣用的視訊檔案格式。 使用 MP4 檔案可進行以下動作:

   * 桌面的 HTTP 動態串流。
   * HTTP即時資料流(Apple的資料流通訊協定)。
   * 漸進式視訊傳送至Android™、BlackBerry®和Windows®行動裝置

  Adobe Dynamic Media Classic提供兩種上傳視訊檔案的工作流程：

* **預先編碼的視訊**  — 您直接將MP4檔案上傳至Adobe Dynamic Media Classic。 在此工作流程中，上載時不會將檔案編碼。檔案在準備傳送到桌面和行動裝置時會進行預先編碼。

* **主要來源影片**  — 上傳主要來源視訊檔案，並在上傳時將這些檔案編碼為MP4檔案。 已編碼的視訊在「瀏覽」面板中會標示為「視訊」。 Adobe Dynamic Media Classic支援多種格式的視訊檔案編碼。

   * 請確定您想要編碼的主要來源視訊檔案是否受支援。

     請參閱[編碼支援的視訊檔案類型](uploading-encoding-videos.md#supported-video-file-types-for-encoding)。

   * 選擇視訊編碼預設集。

     請參閱[編碼視訊檔案的視訊預設集](application-setup.md#video-presets-for-encoding-video-files)。

     請參閱[視訊編碼的最佳實踐](uploading-encoding-videos.md#best-practices-for-video-encoding)。

Adobe Dynamic Media Classic也會產生視訊縮圖。 您可以深入瞭解視訊縮圖、如何取得其 URL，以及修改海報框架。

另請參閱 [使用視訊縮圖](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**上載和編碼視訊:**

執行下列任一項作業.

*如果您的視訊已編碼*

1. 在全域導覽列上，選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面中，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在上傳頁面上，在 **[!UICONTROL 選取要上載的檔案]** 面板，選取 **[!UICONTROL 瀏覽]**，導覽至MP4視訊檔案，然後選取 **[!UICONTROL 開啟]**.
1. 在 **[!UICONTROL 選擇檔案夾目的地]** 面板，選取上傳檔案的資料夾。
1. 在上傳頁面上，確認 **[!UICONTROL 上傳後發佈]** 已勾選。
1. 選取 **[!UICONTROL 提交上傳]**.

*如果您想要使用Adobe Dynamic Media Classic對視訊進行編碼*

1. 在全域導覽列上，選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面中，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在 **[!UICONTROL 選取要上傳的檔案]** 面板，選取 **[!UICONTROL 瀏覽]**，導覽至主要來源視訊檔案，然後選取「 」 **[!UICONTROL 開啟]**.
1. 在 **[!UICONTROL 選擇檔案夾目的地]** 面板，選取上傳檔案的資料夾。
1. 在頁面的右下角，選取 **[!UICONTROL 工作選項]**，
1. 在「上載工作選項」對話方塊中，展開 **[!UICONTROL EVideo選項]**，然後執行下列任一項作業：

   * 最佳實務是選取 **[!UICONTROL 自我調整視訊編碼]**. 請參閱[最適化視訊 (預設)](application-setup.md#adaptive-video-default)。
   * 選擇性. 如果您想使用個別編碼設定，請展開 **[!UICONTROL 單一編碼預設集]**，然後選取您要用於案頭、行動裝置和平板電腦的編碼選項。
請參閱[桌上型電腦視訊編碼預設集](application-setup.md#desktop-video-encoding-presets)、[行動裝置視訊編碼預設集](application-setup.md#mobile-video-encoding-presets)、[平板電腦視訊編碼預設集](application-setup.md#tablet-video-encoding-presets)。
1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在上傳頁面上，確認 **[!UICONTROL 上傳後發佈]** 已勾選。
1. 在上傳頁面的右下角，選取「 」 **[!UICONTROL 提交上傳]**.

*如果您想要將先前上載的視訊檔案重新編碼*

1. 在Adobe Dynamic Media Classic的「瀏覽」面板中，導覽至視訊並加以選取。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]**.
1. 在「重新處理資產」對話方塊中，展開 **[!UICONTROL EVideo選項]**，然後執行下列任一項作業：
   * 最佳做法是使用以下方法。選取「**最適化視訊**」。請參閱[最適化視訊 (預設)](application-setup.md#adaptive-video-default)。
   * 選擇性. 如果您想使用個別編碼設定，請展開 **[!UICONTROL 單一編碼預設集]**，然後選取您要用於案頭、行動裝置和平板電腦的編碼選項。
請參閱[桌上型電腦視訊編碼預設集](application-setup.md#desktop-video-encoding-presets)、[行動裝置視訊編碼預設集](application-setup.md#mobile-video-encoding-presets)、[平板電腦視訊編碼預設集](application-setup.md#tablet-video-encoding-presets)。
1. 在「重新處理資產」對話方塊中，選取 **[!UICONTROL 提交]**.

當您使用自我調整視訊編碼預設集或使用多個單一編碼預設集時，結果會是自動建立含有多個視訊編碼自我調整視訊集。 您也可以選取個別視訊，手動建立最適化視訊集。

當您自動或手動產生最適化視訊集，只會建立 MP4 和 M4V 檔案類型。

## 編碼支援的視訊檔案類型 {#supported-video-file-types-for-encoding}

下表列出在上載檔案時可以編碼為 MP4 或 OGV 格式的視訊檔案類型 (具有允許的視訊編碼器)。此表格列出了檔案格式和轉碼器:

* **視訊檔案格式**  — 視訊檔案格式與ZIP檔案類似，可決定檔案在視訊檔案中的包含方式。 視訊檔案通常包含多個軌道:一個視訊軌道 (沒有音訊) 和一或多個音訊軌道 (沒有視訊)。這些軌道相互關聯並且同步。視訊檔案格式決定了這些不同資料軌道和中繼資料的組織方式。

* **視訊轉碼器**  — 視訊轉碼器說明視訊編碼的演演算法。 視訊播放器根據其轉碼器對視訊進行解碼，然後在畫面顯示一系列影像或影格。轉碼器將視訊檔案儲存為播放視訊所需的資訊量降至最低。只會儲存一個影格和下一個影格之間差異的相關資訊，而不儲存每個單獨影格的相關資訊。由於大部分的視訊在不同影格之間幾乎不會變化，因此轉碼器允許較高的壓縮率，導致檔案大小較小。

  | 視訊檔案格式 | 視訊轉碼器 |
  | --- | --- |
  | 3GP | H.263、H.264 |
  | AVI | DivX、DV |
  | M2P | MPEG-2 PS |
  | M2T | MPEG-2 TS |
  | M2TS | MPEG-2 TS |
  | M2V | MPEG-2 ES |
  | M4V | H.264 |
  | MOV | DV、DVCPro 50、H.261、H.263、H.264、Sorenson Video 1 |
  | MP4 | H.264/MPEG-4 AVC |
  | MPEG | MPEG-2 SS |
  | MPG | MPEG-2 SS |
  | MTS | MPEG-2 |
  | ProRes | APCN、APCS、APCO、APCH、AP4H |
  | TS | DVCPro 50 |
  | VOB | MPEG-2 |
  | WMV/ASF | VC-1、Windows® Media Video 7、Windows® Media Video 8 |

  >[!NOTE]
  >
  >如果您上載並嘗試編碼視訊檔案，但因檔案包含不相容的編碼器或檔案容器而被拒絕，「工作」畫面會發出警告。如需詳細資訊，請參閱 [檢查工作檔案](checking-job-files.md).

## 視訊編碼最佳實踐 {#best-practices-for-video-encoding}

以下是在Adobe Dynamic Media Classic中編碼來源視訊檔案的最佳實務提示。

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### 來源視訊檔案 {#source-video-files}

您編碼視訊檔案時，使用可實現的最高品質來源視訊檔案。請避免使用先前編碼的視訊檔案，因為這些檔案已壓縮，再次編碼會導致視訊品質變差。

下表說明編碼來源視訊檔案時，其建議的大小、外觀比例和最低位元速率等資訊：

| 大小 | 外觀比例 | 最小位元速率 |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 4500 kbps (適用於大部分視訊) |
| 1280 X 720 | 16:9 | 3000 - 6000 kbps (依據視訊中的動作量而定) |
| 1920 X 1080 | 16:9 | 6000 - 8000 kbps (依據視訊中的動作量而定) |

### 取得檔案的中繼資料 {#obtaining-a-file-s-metadata}

您可以在Adobe Dynamic Media Classic中檢視檔案的中繼資料、使用視訊編輯工具或使用專為取得中繼資料而設計的應用程式，藉此取得檔案的中繼資料。 以下是使用MediaInfo （協力廠商應用程式）來取得視訊檔案中繼資料的指示：

1. 移至此網頁： [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. 選取和下載圖形介面版本的安裝程式，並按安裝指示操作。
1. 安裝之後，請以滑鼠右鍵按一下視訊檔案(僅限Windows®)並選取MediaInfo，或開啟MediaInfo並將視訊檔案拖曳到應用程式中。 您會看到與視訊檔案相關的所有中繼資料，其中包括其寬度、高度和 fps。

### 外觀比例 {#aspect-ratio}

當您選擇或建立主要視訊檔案的視訊編碼預設集時，請確定預設集具有與主要視訊檔案相同的外觀比例。 *外觀比例*&#x200B;是視訊寬度相對於視訊高度的比例。

若要判斷視訊檔案的外觀比例，請取得檔案的中繼資料，並注意檔案的寬度和高度(請參閱 [取得檔案的中繼資料](uploading-encoding-videos.md#obtaining_a_file_s_metadata))。 然後，使用以下公式來確定外觀比例:

寬度/高度 = 外觀比例

下表描述了如何將公式結果轉換為常用外觀比例選項:

| 公式結果 | 外觀比例 |
| --- | --- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

例如，1440寬度×1080高度的視訊的外觀比例為1440/1080，即1.33。在這種情況下，您可以選擇外觀比例為4:3的視訊編碼預設集來編碼視訊檔案。

### 資料速率 {#data-rate}

*資料速率* (也稱為&#x200B;*位元速率*) 是用於編碼以組成一秒鐘視訊播放的資料量。資料速率以千位元/秒鐘 (Kbps) 為度量單位。

>[!NOTE]
>
>因為所有轉碼器使用有損壓縮，所以資料速率是決定視訊品質的最重要因素。使用有損壓縮時，將視訊檔案壓縮的越多，品質下降的越多。因此，所有其他特性 (解析度、影格速率和轉碼器) 不變時，資料速率越低，壓縮檔案的品質越低。

選擇視訊編碼預設集時，請記得考慮目標使用者的連線速度。 選擇資料速率為該速度 80% 的預設集。例如，如果目標使用者的連線速度是1000 Kbps，則最佳預設集是視訊資料速率為800 Kbps的預設集。

下面表格描述了標準連線速度的資料速率。

| 速度 (Kbps) | 連線類型 |
| --- | --- |
| 256 | 撥號連線。 |
| 800 | 標準行動裝置連線。對於此連線，將資料速率設定在範圍為 400 至最大值 800 內，以呈現 3G 體驗。 |
| 2000 | 標準頻寬桌面連線。針對此連線，將資料速率目標設定在800至2000 Kbps範圍內，大部分目標平均為1200至1500 Kbps。 |
| 5000 | 標準高速頻寬連線。不建議在此上限範圍內編碼，因為大部分消費者無法使用此速度的視訊傳送。 |

### 解析度 {#resolution}

*解析度* 說明視訊檔案的高度和寬度（畫素）。 大部分的來源視訊都是以高解析度儲存(例如1920 × 1080)。 為了串流目的，來源視訊會壓縮成較小的解析度(640 × 480或更小)。

解析度和資料速率是決定視訊品質的兩個不可分割因素。為獲得相同的視訊品質，視訊檔案的像素數 (解析度越高) 越高，資料速率必須越高。例如，請考慮320 × 240解析度和640 × 480解析度視訊檔案中每幀的畫素數：

| 解析度 | 每影格像素數 |
| --- | --- |
| 320 × 240 | 76,800 |
| 640 × 480 | 307,200 |

640×480檔案的每個影格有四倍多的畫素。 若要讓這兩個範例解析度達到相同的資料速率，您可以對640 × 480檔案套用四倍的壓縮，這會降低視訊的品質。 因此，250 Kbps的視訊資料速率可以以320 × 240的解析度呈現高品質的視覺效果，但無法以640 × 480的解析度呈現。

>[!NOTE]
>
>一般而言，您使用的資料速率越高，視訊顯示效果就越好，而且您使用的解析度越高，您必須維持的檢視品質資料速率就越高（相較於解析度較低的情況）。

因為解析度和資料速率是關聯的，在編碼視訊時您有兩個選擇:

* 選擇資料速率，然後以您選擇之資料速率顯示的最佳解析度編碼。
* 選擇一個解析度，然後在您所選解析度下，以呈現高品質視訊所需的資料速率進行編碼。

當您選擇（或建立）主要視訊檔案的視訊編碼預設集時，請使用此表格來鎖定正確的解析度：

| 解析度 | 高度 (像素) | 畫面大小 |
| --- | --- | --- |
| 240p | 240 | 微型畫面 |
| 300p | 300 | 通常適用於行動裝置的小型熒幕 |
| 360p | 360 | 小型畫面 |
| 480p | 480 | 中型畫面 |
| 720p | 720 | 大型畫面 |
| 1080p | 1080 | 高畫質大型畫面 |

### Fps (每秒鐘影格數) {#fps-frames-per-second}

在美國和日本，大部分視訊以 29.97 影格/秒鐘 (fps) 拍攝；在歐洲，大部分視訊以 25 fps 拍攝。電影以 24 fps 拍攝。

選擇符合主要視訊檔案fps速率的視訊編碼預設集。 例如，如果您的主要視訊是25 fps，請選擇具有25 fps的編碼預設集。 依預設，所有自訂編碼都會使用主要視訊檔案的FP。 因此，在建立視訊編碼預設集時，您不需要明確指定 fps 設定。

### 視訊編碼尺寸 {#video-encoding-dimensions}

為獲得最佳效果，請選取將來源視訊整個乘上所有編碼視訊的編碼尺寸。

若要計算出這個比例，請將來源寬度除以編碼的寬度，以得出寬度比例。接著，將來源高度除以編碼的高度，以得出高度比例。

如果求得的比例為整數，表示視訊的縮放的比例為最佳比例。如果求得的比例不是整數，會因為在畫面上留下剩餘的像素人為因素，而影響到視訊品質。當視訊含有文字時，這種影響最明顯。

例如，假設您的來源視訊是1920 × 1080。 下表中的三種編碼的視訊，均提供可用的最佳編碼設定。

| 視訊類型 | 寬度×高度 | 寬度比例 | 高度比例 |
| --- | --- | --- | --- |
| 來源 | 1920 × 1080 | 1 | 1 |
| 編碼 | 960 × 540 | 2 | 2 |
| 編碼 | 640 × 360 | 3 | 3 |
| 編碼 | 480 × 270 | 4 | 4 |

### 編碼視訊檔案格式 {#encoded-video-file-format}

Adobe Dynamic Media Classic建議使用MP4 H.264視訊編碼預設集。 因為 MP4 檔案使用 H.264 視訊轉碼器，所以會提供高畫質視訊，但是會壓縮檔案大小。

## 使用視訊編碼預設集 {#working-with-video-encoding-presets}

使用視訊製作裝置和視訊編輯軟體建立的主要視訊檔案通常太大，且格式不正確，無法傳送到線上目的地。 若要將数位視訊轉換為適用於在不同畫面上播放的適當格式和規格，您可以將視訊檔案&#x200B;*轉碼* (此過程也稱為&#x200B;*編碼*)。在編碼過程中，會將視訊壓縮為小而有效的檔案大小，適合傳送到網路和行動裝置。

另請參閱 [上傳並編碼視訊](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic提供您預先定義的視訊編碼預設集資料庫，這些預設集可反映目前最常用的編碼設定。 這些編碼預設集已針對在目標畫面播放進行了最佳化。此外，管理員還可以建立自己的視訊編碼預設集，以便自訂視訊的大小和對終端使用者播放的品質。所有視訊編碼預設集(不論是來自Adobe Dynamic Media Classic的現成可用或自訂的)都會以MP4檔案格式輸出視訊。

在「視訊預設集」畫面上，管理員可以設定和管理視訊編碼。他們可以執行下列作業: 

* 啟用和停用視訊編碼預設集。
* 建立視訊編碼預設集。
* 編輯視訊編碼預設集。
* 刪除視訊預設集。

上傳至Adobe Dynamic Media Classic或在Adobe Dynamic Media Classic中編碼的任何視訊都會視為「視訊」。 換句話說，此資產類別表示您可傳送視訊以供桌上型電腦、行動裝置或兩者播放。例如，您可以在Adobe Dynamic Media Classic中預覽這些型別的影片。 您也可以產生 URL (使用「複製 URL」功能) 和可內嵌的程式碼 (使用「內嵌程式碼」功能)，以用於視訊播放器、網站等處。

另請參閱 [在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

另請參閱 [將視訊檢視器內嵌在網頁上](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

對於您在Adobe Dynamic Media Classic中上傳和編碼的視訊資產，視訊會以下列檔案格式傳送：

**MP4 H.264** 將MP4檔案用於下列專案：

* 桌面的 HTTP 動態串流。
* HLS (HTTP即時資料流、Apple的資料流通訊協定)。
* 漸進式視訊傳送至Android™、BlackBerry®和Windows®行動裝置。

任何其他視訊格式及轉碼器會視為「主要視訊」。 此資產類別表示視訊屬於來源視訊檔案，且無法用來傳送以供桌面或行動裝置播放。例如，您無法在Adobe Dynamic Media Classic中預覽這些型別的影片。 您無法產生複製URL或內嵌程式碼以用於視訊播放器、網站等。

### 篩選視訊編碼預設集清單 {#filtering-the-list-of-video-encoding-presets}

「視訊預設集」頁面和「自我調整視訊預設集」頁面包含一個表格，其中列出作用中狀態、預設集名稱、預期的播放裝置、視訊大小和每個視訊預設集的資料速率。

您可以選擇依「兩者」、「作用中」或「非作用中」篩選清單、查看所有視訊預設集，或將清單縮減成作用中或非作用中的預設集，藉此精簡清單。

您也可以根據播放裝置選項進行篩選，將清單縮減成用於在所有裝置、桌上型電腦、行動裝置或平板電腦上播放視訊的視訊預設集。

**篩選視訊編碼預設集的清單:**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 最適化視訊預設集]** 或 **[!UICONTROL 單一編碼預設集]**.

   「自我調整視訊預設集」和「單一編碼預設集」頁面包含一個表格，其中列出「作用中」狀態、預設集名稱、預期的播放裝置、視訊維度和每個視訊預設集的資料速率。

1. 在稱為「視訊預設集」的「單一編碼預設集」頁面中，使用「視訊預設集」工具列上的兩個下拉式清單，依「作用中狀態」和「播放裝置」精簡表格中的預設集清單。

   * 首先，在較窄的下拉式清單中選擇「**[!UICONTROL 兩者]**」以查看所有視訊預設集，或選擇「**[!UICONTROL 作用中]**」或「**[!UICONTROL 非作用中]**」將清單縮減成作用中或非作用中的預設集。
   * 接著，在較寬的下拉式清單中選擇播放裝置選項，將清單縮減成用於在桌上型電腦上播放視訊，或用於在行動裝置或平板電腦上播放視訊的視訊預設集。

### 啟用或停用視訊編碼預設集 {#activating-or-deactivating-video-encoding-presets}

已啟用的視訊預設集會顯示在「上載工作選項」對話框中。當使用者在上傳過程中上傳視訊檔案時，會出現此對話方塊。 他們可以從所有已啟用的編碼預設集中選擇。

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 進行以下一項操作:

   * 選取 **[!UICONTROL 最適化視訊預設集]**.
   * 選取 **[!UICONTROL 單一編碼預設集]**.

1. 進行以下一項操作:

   * 若要啟用視訊預設集，請在預設集頁面的「作用中」欄底下，選取預設集名稱旁的方框。
   * 若要停用視訊預設集，請取消選取您要使其非使用中的視訊預設集旁的方塊。

     >[!NOTE]
     >
     >非作用中視訊預設集不會出現在「上載工作選項」對話框中。

1. 在頁面的右下角，選取 **[!UICONTROL 關閉]**.

### 新增或編輯視訊編碼預設集 {#adding-or-editing-a-video-encoding-preset}

您可以建立自己的自訂、單一編碼視訊預設集，並將其新增至「視訊預設集」表格。 您也可以變更Adobe Dynamic Media Classic隨附的任何預先定義單一編碼視訊預設集，前提是您以新名稱儲存編輯的預設集。

Adobe Dynamic Media Classic已設定目標資料速率、解析度高度和解析度寬度的最大限制，以確保適當的播放體驗。 如果您超過以下限制，就會出現警告訊息: 

* 電腦播放的限製為： （寬度/16） &#42; (Height/16) &lt; 8192。
* 行動播放的限製為： （寬度/16） &#42; （高度/16） &lt; 660；目標資料速率&lt; 4000。
* 平板電腦播放的限製為：（寬度/16） &#42; (Height/16) &lt; 3600。

**增加或編輯視訊編碼預設集:**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 選取 **[!UICONTROL 單一編碼預設集]**.
1. 在「視訊預設集」頁面中，執行下列任一項作業: 

   * 在「視訊預設集」工具列上，選取 **[!UICONTROL 新增]** 以便新增視訊預設集。
   * 選取視訊預設集。在工具列中，選取 **[!UICONTROL 編輯]**.

     您無法編輯Adobe Dynamic Media Classic預先定義的預設集；您只能透過選擇 **[!UICONTROL 另存為]**.

1. 在「增加視訊預設集」頁面或「編輯視訊預設集」頁面上，設定您想要的視訊預設集選項。

   請參閱[視訊編碼的最佳實踐](uploading-encoding-videos.md#best-practices-for-video-encoding)中的建議設定。

   | 視訊預設集選項 | 說明 |
   | --- | --- |
   | 預設集名稱 | 輸入視訊預設集的描述性名稱。您輸入的名稱會顯示在供使用者選擇轉碼選項的「上載工作選項」對話框中。 |
   | 說明 | 描述視訊預設集。當您將指標移到「上載工作選項」對話方塊中的預設集名稱上時，您輸入的內容會顯示為工具提示，使用者可在其中選擇轉碼選項。 |
   | 播放裝置 | 選擇要用來播放視訊的裝置。選項包括電腦（桌上型電腦）、行動裝置(iPhone、iPad、Android™)或平板電腦(僅限iPad)。 此設定會自動確定在編碼期間使用的適當視訊和音訊轉碼器。 |
   | 目標資料速率 | 輸入目標終端使用者的網際網路平均連線速度 (kbps)。您可以輸入速率，或拖曳滑桿進行輸入。使用者連線速度光譜會列出寬頻、DSL、行動裝置和撥接上網的常見速度。此設定會自動確定合併的視訊和音訊資料速率。也就是構成一秒鐘視訊播放所編碼的資料量。資料速率越高，所得到視訊的品質就越高。但是，如果資料速率太高，會導致檔案非常大並造成低頻寬使用者的觀看體驗不佳。最好是在高資料速率和低資料速率之間找到一個平衡點。旨在建立優質播放體驗，頻寬較低的使用者也能享受該體驗。 |
   | 外觀比例 | 外觀比例是視訊寬度相對於視訊高度的比例。以下所列的前兩個外觀比例經常用於水平顯示視訊:<ul><li> 4:3 - 幾乎適用於所有的標準畫質電視廣播內容。</li><li>16:9 — 用於高畫質電視(HDTV)的幾乎所有寬熒幕內容和電影。</li><li>自動縮放 — （預設）單一編碼預設集，可與任何外觀比例搭配使用，建立傳送至行動裝置、平板電腦和案頭的視訊。 使用此預設集編碼而上載的來源視訊，會設定成固定的高度。不過，寬度會自動調整比例，以保留視訊的外觀比例（寬高比）。</li><li>自訂 - 當您想要定義非標準的視訊大小時會使用。</li><li>您選擇的外觀比例會決定「解析度大小」的寬度和高度設定；寬度和高度值會自動縮放為適當的外觀比例。</li></ul> |
   | 解析度大小 | 解析度大小（以寬度的畫素數乘以高度的畫素數表示）決定大小。 以像素為單位輸入寬度和高度值，或拖曳滑桿來輸入這些值。解析度範圍列出了標準解析度大小。寬度和高度值會自動符合您選取的外觀比例。 例如，如果您選取 4:3 作為外觀比例，並且為寬度輸入 400，則會自動為高度輸入 300。如果您對「外觀比例」設定選取「自動縮放」，「解析度大小」的「寬度」值會自動設為「自動」。選取 **[!UICONTROL 預覽]** 因此您可以開啟瀏覽器視窗，並在其中檢視您的解決方案選擇。 |
   | 編碼檔案字尾 | 輸入字尾。該字尾會附加到產生的編碼視訊檔案。您可以在名稱中輸入連字符號和底線；不允許使用空格和特殊字元。 |
   | 其他設定 | Adobe Dynamic Media Classic會根據最佳實務編碼准則，自動決定所有其他編碼設定。 |

1. 進行以下一項操作:

   * 選取 **[!UICONTROL 儲存]** 如果您新增或編輯視訊預設集。
   * 選取 **[!UICONTROL 另存為]** 如果您是從現有預設集開始增加視訊預設集。

### 刪除視訊編碼預設集 {#deleting-a-video-encoding-preset}

管理員可以刪除自訂視訊預設集。Adobe Dynamic Media Classic隨附的視訊預設集無法刪除。

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 選取 **[!UICONTROL 單一編碼預設集]**.
1. 在「視訊預設集」頁面中，選取表格中您不再想要或需要的視訊預設集。
1. 在「視訊預設集」工具列上，選取 **[!UICONTROL 刪除]**.
1. 在「刪除預設集」對話方塊中，選取 **[!UICONTROL 刪除]**.

>[!MORELIKETHIS]
>
>* [快速入門：Adobe Dynamic Media Classic中的影片](quick-start-video.md#quick-start-video)
>* [上傳並編碼視訊](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [使用視訊檢視器預設集](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片
