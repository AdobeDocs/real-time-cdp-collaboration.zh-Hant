---
title: 連線概觀
description: 瞭解Real-Time CDP Collaboration中的連線。
audience: publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 419dde94-fee2-4dc1-b25d-cf79b7e57ec0
TQID: https://experienceleague.adobe.com/ZF3bqoR0XRv2G7abRULz1ElRgk5xLCZySHylrqzPqg0
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 803
ht-degree: 2%

---

# 連線概觀

{{limited-availability-release-note}}

共同作業人員必須建立連線，才能共同處理行銷活動。 此連線可讓他們啟用對象、建立專案，以及執行行銷活動績效報表。

系統會根據您選擇的共同作業模式來建立連線。 Collaboration支援三種關鍵共同作業模式：廣告商對發佈商、品牌對品牌，以及廣告商對廣告平台。 若要深入瞭解這些模式，請參閱[共同作業模式](/help/guide/overview/collaboration-patterns.md)指南。

若要瞭解如何建立連線，請閱讀以下與您的共同作業模式對應的章節：

- [廣告商與發佈商的連線](#advertiser-to-publisher-connection)
- [品牌對品牌連線](#brand-to-brand-connection)
- [廣告商與廣告平台連線](#advertiser-to-advertising-platform-connection)

## 廣告商與發佈商的連線 {#advertiser-to-publisher-connection}

![廣告商 — 發佈商連線程式的高階圖表。](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

在廣告商對發佈者模式中，廣告商會透過&#x200B;**[!UICONTROL Discover publishers]**&#x200B;工作區發現他們想要使用的發佈者，並傳送連線邀請。 發佈者接著會稽核並接受邀請，允許廣告商提出連線設定。 發佈者接受連線設定後，連線就會建立，兩個共同作業人員就可以開始一起處理專案。

### 高層級概觀

若要在廣告商與發佈商之間建立連線，需執行下列步驟：

1. [探索發行者](./discover-collaborators.md)：廣告商會識別可與其合作的潛在發行者。
2. [傳送邀請](./establishing-connections.md#send-invite)：廣告商傳送連線邀請給選取的發行者。
3. [接受邀請](./establishing-connections.md#accept-invite)：發行者稽核並接受邀請。
4. [設定連線設定](./establishing-connections.md#configure-connection-settings)：廣告商會設定連線設定，並將設定傳送給發佈者進行稽核。
5. [確認連線設定](./establishing-connections.md#review-connection-settings)：發行者檢閱連線設定，然後接受或拒絕連線設定。 如果接受，則會建立連線。 若遭拒絕，發佈者可針對產品外部的修訂提供意見回饋。 然後廣告商可以修訂設定並重新傳送以進行稽核。

接受連線設定後，連線即建立，共同作業人員已準備好[建立專案](/help/guide/collaborate/manage-projects.md#create-project)以開始共同作業行銷活動。

## 品牌對品牌連線 {#brand-to-brand-connection}

![品牌對品牌連線程式的高階圖表。](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>術語&#x200B;**品牌**&#x200B;是用來指代Collaboration以外的公司或品牌。 術語&#x200B;**共同作業人員**&#x200B;是指任何可以在Collaboration中建立連線的帳戶，無論其是否為廣告商或發佈者。

在品牌對品牌模式中，在產品外部溝通的兩個品牌，可以使用[私人連線邀請](#private-connection-invite)直接在Collaboration中連線。 品牌可以是廣告商或發佈者。 對於不符合傳統廣告商 — 發佈商模式的品牌（例如兩個廣告商或兩個發佈商），此模式特別實用。

共同作業人員若要開始，會傳送私人連線邀請給其他共同作業人員。 收件者會檢閱邀請並接受邀請，允許擁有者提出連線設定。 一旦收件者接受連線設定，連線就會建立，而且共同作業人員可以開始一起處理專案。

### 高層級概觀

>[!TIP]
>
>討論連線程式時，**所有者**&#x200B;和&#x200B;**收件者**&#x200B;之間會有區別。 擁有者是透過傳送邀請來啟動連線的共同作業人員，而收件者是接收及檢閱邀請的共同作業人員。

兩個品牌之間的連線程式涉及幾個步驟。 在連線程式開始之前，必須滿足幾個先決條件：

1. 兩個品牌在產品外部溝通，討論可能的連線。
1. 品牌[在Collaboration中建立帳戶](/help/guide/setup/onboard-account.md) （如果尚未建立），請務必選取適當的角色型別（廣告商或發佈商）。

滿足先決條件後，即可開始連線程式。 下列步驟概述此程式：

1. [傳送私人連線邀請](./establishing-connections.md#private-connection-invite)：一個共同作業人員傳送私人連線邀請給另一個共同作業人員。
2. [接受私人連線邀請](./establishing-connections.md#accept-invite)：收件者檢閱並接受私人連線邀請。
3. [設定連線設定](./establishing-connections.md#configure-connection-settings)：擁有者設定連線設定，並將設定傳送給收件者進行檢閱和接受。
4. [確認連線設定](./establishing-connections.md#review-connection-settings)：收件者會檢閱連線設定，然後接受或拒絕連線設定。

接受連線設定後，連線即建立，共同作業人員已準備好[建立專案](/help/guide/collaborate/manage-projects.md#create-project)以開始共同作業行銷活動。

## 廣告商與廣告平台連線 {#advertiser-to-advertising-platform-connection}

廣告商與廣告平台連線程式可讓廣告商與協力廠商廣告平台(例如Amazon Marketing Cloud (AMC))連線，以增強其行銷功能。

### 高層級概觀

廣告商與廣告平台之間的連線程式包含數個步驟。 在連線程式開始之前，請確定您有使用中帳戶（使用廣告平台）且已核准使用其服務。 下列步驟概述連線程式：

1. [探索廣告平台](./discover-collaborators.md)：廣告商會識別可共同作業的潛在廣告平台。
2. [連線到Advertising平台](./advertising-platforms/overview.md#advertising-platforms-overview)：廣告商透過選取要連線的廣告平台來啟動連線程式，並依照提示驗證及授權連線。
