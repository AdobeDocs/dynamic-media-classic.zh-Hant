---
title: 即時與同級共用資產變更
description: 瞭解如何即時與同儕分享資產變更。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 70%

---


# 即時與同級共用資產變更{#sharing-asset-changes-with-peers-in-real-time}

在同一公司的一部或多部電腦上執行多份Dynamic Media Classic時，所有對等用戶端都會即時更新來自任何Dynamic Media Classic用戶端的下列動作：

* 編輯資產 (建置器、影像編輯器等)
* 重新命名資產
* 刪除資產
* 移動資產
* 上載一或多個資產 (桌面與 FTP)
* 建立、刪除或重新命名檔案夾

在原始用戶端中進行變更後，所有登入同一公司的對等用戶端都會隨變更而更新。 除非同級正以任何影像編輯器或建置器編輯變更中的資產，否則變更同級時不會產生通知。

當您登入時，系統會提示您允許或拒絕對等更新。 您可以記憶您的選擇，這樣系統只會提示您一次。若要清除您的選擇，請在「全域設定」的「同級協助網路」面板中刪除適當的網站。

如果您要變更同級已變更的資產，則系統會提示您將變更納入建置器或編輯器。如果您選擇「是」，則建置器或編輯器就會放棄已對資產進行的所有變更，並匯入更新的資產。如果您選擇「否」，則建置器或編輯器中的資產就不會變更，而您已進行的所有變更都會保留在該工作階段中。

儲存資產時，系統會通知您有較新的版本存在，並詢問您是否要以您進行的變更覆寫資產。
