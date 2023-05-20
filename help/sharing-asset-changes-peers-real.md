---
title: 即時與同行共用資產更改
description: 瞭解如何與Adobe Dynamic Media Classic的同行即時共用資產更改。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# 即時與同行共用資產更改{#sharing-asset-changes-with-peers-in-real-time}

在同一公司的多台電腦上運行多個Adobe Dynamic Media Classic副本時，將即時更新來自任何Adobe Dynamic Media Classic客戶端的以下操作與所有對等客戶端：

* 編輯資產（生成器、影像編輯器等）
* 重新命名資產
* 刪除資產
* 移動資產
* 上載一或多個資產 (桌面與 FTP)
* 建立、刪除或重新命名檔案夾

在原始客戶端中進行更改後，所有登錄到同一公司的對等客戶端都會隨更改一起更新。 除非同級正以任何影像編輯器或建置器編輯變更中的資產，否則變更同級時不會產生通知。

登錄時，系統會提示您允許或拒絕對等更新。 您可以記憶您的選擇，這樣系統只會提示您一次。若要清除您的選擇，請在「全域設定」的「同級協助網路」面板中刪除適當的網站。

如果您要變更同級已變更的資產，則系統會提示您將變更納入建置器或編輯器。如果您選擇 **[!UICONTROL 是]**，則生成器或編輯器將放棄對資產所做的任何更改，並導入更新的資產。 如果您選擇 **[!UICONTROL 否]**，該資產在生成器或編輯器中保持不變，並且您所做的任何更改都將保留在該會話中。

儲存資產時，系統會通知您有較新的版本存在，並詢問您是否要以您進行的變更覆寫資產。
