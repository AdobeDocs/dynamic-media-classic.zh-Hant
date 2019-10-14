---
title: '"定義可變性: 參數化與 DOM 操作"'
seo-title: '"定義可變性: 參數化與 DOM 操作"'
description: 'null'
seo-description: 瞭解如何使用參數化來定義可變性，而不是DOM操作。
uuid: dce424f2-07d8-4703-aa3a-40d2ee12f74
contentOwner: 管理員
content-type: 參考
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTENDEMAND_PK/categories/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 定義可變性: 參數化與 DOM 操作{#defining-variability-parameterization-versus-dom-manipulation}

Dynamic Media Classic提供兩種管理範本中變數內容的技巧。 透過這兩種技術，您可以在Illustrator中設計初始範本、將範本轉換為Dynamic Media Classic FXG檔案格式，然後將它上傳至SPS。 但在您對變數元素的控制程度以及使用這些元素所需的技巧方面，這兩種方法有所不同。

* **在Scene7 Publishing system中進行參數化此技巧需要在SPS的「範本發佈建立」和「預覽」畫面，或在Adobe Illustrator網路印刷增效模組中定義變數。**&#x200B;兩種方法都提供用於建立參數、指派參數值和測試結果的工具。

* **使用DOM控制**&#x200B;此技巧可讓您在XML層級上控制設計和範本。 Dynamic Media Classic FXG檔案是XML。 使用該方法，您可以直接透過設計範本的 XML DOM (顯示物件模型) 來編輯設計範本。在 Illustrator 中，使用 s7:elementID 標記變數元素，以便稍後使用 URL 命令處理這些元素。

>[!MORELIKETHIS]
>
>* [在Dynamic Media Classic中參數化範本](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM 操作](dom-manipulation.md#dom_manipulation)

