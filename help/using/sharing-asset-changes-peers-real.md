---
title: 與同儕即時共用資產變更
description: 瞭解如何在Adobe Dynamic Media Classic中即時與同業共用資產變更。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# 與同儕即時共用資產變更{#sharing-asset-changes-with-peers-in-real-time}

在同一公司的多部電腦上執行多個Adobe Dynamic Media Classic復本時，所有Adobe Dynamic Media Classic使用者端的下列動作都會即時更新至所有對等使用者端：

* 編輯資產（產生器、影像編輯器等）
* 重新命名資產
* 刪除資產
* 移動資產
* 上載一或多個資產 (桌面與 FTP)
* 建立、刪除或重新命名檔案夾

在原始使用者端中進行變更後，所有登入同一公司的對等使用者端都會更新變更。 除非同級正以任何影像編輯器或建置器編輯變更中的資產，否則變更同級時不會產生通知。

登入時，系統會提示您允許或拒絕對等更新。 您可以記憶您的選擇，這樣系統只會提示您一次。若要清除您的選擇，請在「全域設定」的「同級協助網路」面板中刪除適當的網站。

如果您要變更同級已變更的資產，則系統會提示您將變更納入建置器或編輯器。如果您選擇 **[!UICONTROL 是]**，然後產生器或編輯器會捨棄對資產所做的任何變更並匯入更新的資產。 如果您選擇 **[!UICONTROL 否]**，資產在產生器或編輯器中不會變更，而您所做的任何變更會保留在該工作階段中。

儲存資產時，系統會通知您有較新的版本存在，並詢問您是否要以您進行的變更覆寫資產。
