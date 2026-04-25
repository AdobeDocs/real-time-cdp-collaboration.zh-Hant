---
title: 端對端工作流程
description: 根據您的共同作業模式，瞭解使用Real-Time CDP Collaboration的端對端工作流程。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
TQID: https://experienceleague.adobe.com/9edtg5tMbnB3BrdLrDkcHQ-AjBNOqMFGojAja3NCwCs
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1738
ht-degree: 0%

---

# 端對端工作流程

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，端對端工作流程會依您選擇的共同作業模式而有所不同。 工作流程概述設定及執行共同作業專案的相關步驟，從建立帳戶和來源受眾，到建立連線和專案。 瞭解此工作流程是有效運用平台功能達成行銷目標的關鍵。

## 快速入門

開始之前，請確定您已確實瞭解以下重要概念：

- **Collaboration模式**：這些模式定義共同作業人員如何共同作業。 共有五種不同的模式：
   - [廣告商對發佈者](./collaboration-patterns.md#advertiser-to-publisher)
   - [品牌對品牌](./collaboration-patterns.md#brand-to-brand)
   - [廣告商對資料合作夥伴](./collaboration-patterns.md#advertiser-to-data-partner)
   - [代理商對發佈商](./collaboration-patterns.md#agency-to-publisher)
   - [廣告商對機構平台](./collaboration-patterns.md#advertiser-to-agency-platform)
- **帳戶角色**：帳戶角色決定您在平台中的權能。 藍圖應與您組織的目標、品牌和目標一致。 有四個帳戶角色： [廣告商](./roles.md#advertiser)、[發佈者](./roles.md#publisher)、[機構](./roles.md#agency)和[資料夥伴](./roles.md#data-partner)。
- **使用案例**：使用案例會定義您如何善用Collaboration達成行銷目標。 有三個共同作業使用案例： [探索](./use-cases.md#discover)、[啟動](./use-cases.md#activate)以及[測量](./use-cases.md#measure)。

本指南將使用三位模擬共同作業人員來說明端對端工作流程：

- **[!UICONTROL Luma]**：運動服裝品牌。 他們是廣告商，想要透過鎖定目標的行銷活動觸及特定對象。
- **[!UICONTROL 電視管]**：數位串流提供者。 它們是提供受眾資料以供廣告商使用的發佈者。
- **[!UICONTROL 適合服飾]**：另一個運動服飾品牌。 他們為想要共同作業以分享對象資料和深入分析的第二位廣告商，藉此提升行銷成效。
- **[!UICONTROL 代理商99]**：媒體代理商。 他們可在工作區中管理多個使用者端帳戶，並與發佈者和廣告商連結。
- **[!UICONTROL DataM8]**：協力廠商資料提供者。 它們提供受眾資料供廣告商使用。
- **[!UICONTROL Holdco]**：代理商持有公司行銷與廣告服務平台，內部代理商團隊用它來管理客戶行銷活動。

## 廣告商對發佈商的工作流程 {#advertiser-to-publisher-workflow}

[!UICONTROL Luma] （一家體育零售公司）想要與數位串流供應商[!UICONTROL TV Tube]建立連線，以透過鎖定目標的行銷活動觸及特定對象。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)，而[!UICONTROL TV Tube]則以發佈者角色建立帳戶。

建立帳戶之後，[!UICONTROL Luma]和[!UICONTROL TV Tube]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 只有[!UICONTROL TV Tube]會啟用行銷活動的對象，因此他們需要[設定目的地](../setup/manage-destinations.md)。

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../connect/discover-collaborators.md)功能尋找[!UICONTROL 電視管]並起始連線要求。 在[!UICONTROL TV Tube]接受連線要求後，[!UICONTROL Luma]會設定連線設定以定義他們將如何共同作業。 [!UICONTROL TV Tube]接受連線要求，以建立兩個品牌之間的安全連結。

建立連線之後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)，以開始他們與[!UICONTROL TV Tube]的協同合作。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)使用案例來深入分析[!UICONTROL TV Tube]的對象資料。 在[!UICONTROL Luma]識別目標對象區段後，他們[啟動](../collaborate/activate.md)這些對象。

啟用對象後，[!UICONTROL TV Tube]會執行目標式行銷活動，並將資料上傳至[測量](../collaborate/measure.md)結果，以評估其行銷活動的成效。

## 品牌對品牌的工作流程 {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel]，運動服裝品牌，想要與另一個運動服裝品牌[!UICONTROL Luma]合作，以分享受眾資料與深入分析，提升行銷成效。

建立帳戶之後，[!UICONTROL Fit Apparel]和[!UICONTROL Luma]都需要[建立資料連線和來源對象](../setup/onboard-audiences.md)。 [!UICONTROL 適合的服飾]和[!UICONTROL Luma]都會啟用行銷活動的對象，因此兩者都需要[設定目的地](../setup/manage-destinations.md)。

在取得其對象後，[!UICONTROL Fit Apparel]和[!UICONTROL Luma] [在平台內建立連線](../connect/establishing-connections.md)，以安全地共用對象資料。 To do so, they must make use of the [private connection invite](../connect/establishing-connections.md#private-connection-invite) feature. [!UICONTROL Luma] shares their connect code with [!UICONTROL Fit Apparel], who then uses it to initiate a connection request. After [!UICONTROL Luma] accepts the connection request, [!UICONTROL Fit Apparel] configures the connection settings to define how they will collaborate. In the configuration, [!UICONTROL Fit Apparel] specifies that both collaborators can activate audiences for marketing campaigns. To complete the connection, [!UICONTROL Luma] accepts the request to establish a secure link between the two brands.

After the connection is established, [!UICONTROL Fit Apparel] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL Luma]. 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Fit Apparel] and [!UICONTROL Luma] can both use the [Discover](../collaborate/discover.md) use case to gain insights into each other&#39;s audience data. Once they have identified valuable audience segments, they [Activate](../collaborate/activate.md) their chosen audiences for marketing campaigns.

Finally, after executing their campaigns, both brands upload data to [Measure](../collaborate/measure.md) the results and evaluate the effectiveness of their collaboration.

## Advertiser-to-advertising platform workflow {#advertiser-to-advertising-platform-workflow}

[!UICONTROL Luma], an athletic retail company, wants to connect with [!DNL Amazon Marketing Cloud] ([!DNL AMC]) to enhance their marketing capabilities by leveraging [!DNL AMC]&#39;s identity resolution and targeting tools. Luma already has an active [!DNL Amazon Advertising] account and is approved to use [!DNL AMC].

To begin, [!UICONTROL Luma] needs to [create an account](../setup/onboard-account.md) with the advertiser role. After establishing their account, [!UICONTROL Luma] must [create a data connection and source audiences](../setup/onboard-audiences.md). Since [!UICONTROL Luma] will activate audiences for marketing campaigns, they need to [configure a destination](../setup/manage-destinations.md).

Once [!UICONTROL Luma] has their account set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) with [!DNL AMC] within the platform. [!UICONTROL Luma] uses the [discover collaborators](../connect/discover-collaborators.md) feature to find [!UICONTROL Amazon Marketing Cloud] and [initiate a connection request](../connect/advertising-platforms/amc.md). After authenticating and authorizing the connection through the [!DNL Amazon] sign-in page, the connection with [!DNL AMC] is established.

After the connection is established, [!UICONTROL Luma] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!DNL AMC]. Connection settings, including use cases, are pre-configured depending on the advertising platform. For [!DNL AMC], the available use case is [Discover](../collaborate/advertising-platforms/amc.md#discover).

[!UICONTROL Luma] leverages the [Discover](../collaborate/advertising-platforms/amc.md#discover) use case to gain insights and audience data from [!DNL AMC]. Using these insights, [!UICONTROL Luma] can optimize their marketing strategies and improve campaign effectiveness.

## Advertiser-to-data partner workflow {#advertiser-to-data-partner-workflow}

[!UICONTROL Luma], an athletic retail company, wants to collaborate with [!UICONTROL DataM8], a third-party data provider, to enrich customer profiles and improve audience targeting.

To begin, [!UICONTROL Luma] needs to [create an account](../setup/onboard-account.md) with the advertiser role, while [!UICONTROL DataM8] creates an account with the data partner role.

After establishing their accounts, both [!UICONTROL Luma] and [!UICONTROL DataM8] must [create a data connection and source audiences](../setup/onboard-audiences.md). Both collaborators may activate audiences for marketing campaigns, so they each need to [configure a destination](../setup/manage-destinations.md).

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Luma] uses the [discover collaborators](../collaborate/discover.md) feature to find [!UICONTROL DataM8] and initiate a connection request. After [!UICONTROL DataM8] accepts the connection request, [!UICONTROL Luma] configures the connection settings to define how they will collaborate. [!UICONTROL DataM8] accepts the connection request to establish a secure link between the two collaborators.

After the connection is established, [!UICONTROL Luma] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL DataM8]. During the project setup, they choose the collaboration use cases that best fit their objectives: [Discover](../collaborate/discover.md), [Activate](../collaborate/activate.md), and [Measure](../collaborate/measure.md).

[!UICONTROL Luma] leverages the [Discover](../collaborate/discover.md) use case to gain insights into [!UICONTROL DataM8]&#39;s audience data. Once [!UICONTROL Luma] has identified the target audience segments, they [activate](../collaborate/activate.md) these audiences.

[!UICONTROL DataM8] can also [activate](../collaborate/activate.md) their audiences to [!UICONTROL Luma]. [!UICONTROL Luma] uses these capabilities to append third-party attributes to its customer profiles and analyze audience composition. With enriched data available directly in its CDP, [!UICONTROL Luma] can build more precise audiences and activate them to paid media destinations without moving data outside its governed environment.

## Agency-to-publisher workflow {#agency-to-publisher-workflow}

[!UICONTROL Agency99], a media agency, wants to collaborate with [!UICONTROL TV Tube], a digital streaming provider, to reach specific audiences through targeted marketing campaigns.

To begin, [!UICONTROL Agency99] needs to [create an account](../setup/onboard-account.md) with the agency role, while [!UICONTROL TV Tube] creates an account with the publisher role.

After establishing their accounts, both [!UICONTROL Agency99] and [!UICONTROL TV Tube] must [create a data connection and source audiences](../setup/onboard-audiences.md). [!UICONTROL Agency99] will set up client sub-accounts and source client data within its workspace. Only [!UICONTROL TV Tube] will activate audiences for marketing campaigns, so they need to [configure a destination](../setup/manage-destinations.md).

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Agency99] uses the [discover collaborators](../collaborate/discover.md) feature to find [!UICONTROL TV Tube] and initiate a connection request. [!UICONTROL Agency99] will do this for one or multiple clients that want to collaborate with [!UICONTROL TV Tube]. After [!UICONTROL TV Tube] accepts the connection request(s), [!UICONTROL Agency99] configures the connection settings to define how each collaboration. [!UICONTROL TV Tube] accepts the connection request(s) to establish a secure link between the two brands.

After the connection is established, [!UICONTROL Agency99] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL TV Tube] in each client sub-account. During the project setup, they choose the collaboration use cases that best fit their objectives: [Discover](../collaborate/discover.md), [Activate](../collaborate/activate.md), and [Measure](../collaborate/measure.md).

[!UICONTROL Agency99] leverages the [Discover](../collaborate/discover.md) use case to gain insights into [!UICONTROL TV Tube]&#39;s audience data. Once [!UICONTROL Agency99] has identified the target audience segments, they [activate](../collaborate/activate.md) these audiences.

After activating the audiences, [!UICONTROL TV Tube] runs targeted marketing campaigns and uploads data to [measure](../collaborate/measure.md) the results to evaluate the effectiveness of their campaign.

## Advertiser-to-agency platform workflow {#advertiser-to-agency-platform-workflow}

[!UICONTROL Luma], an athletic retail company, wants to collaborate with [!UICONTROL Holdco], an agency platform, to share data and receive paid media insights.

To begin, [!UICONTROL Luma] needs to [create an account](../setup/onboard-account.md) with the advertiser role, while [!UICONTROL Holdco] creates an account with the agency role. 

After establishing their accounts, both [!UICONTROL Luma] and [!UICONTROL Holdco] must [create a data connection and source audiences](../setup/onboard-audiences.md). Both collaborators may activate audiences for marketing campaigns, so they each need to [configure a destination](../setup/manage-destinations.md). 

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Luma] uses the [discover collaborators](../collaborate/discover.md) feature to find [!UICONTROL Holdco] and initiate a connection request. After [!UICONTROL Holdco] accepts the connection request, [!UICONTROL Luma] configures the connection settings to define how they will collaborate.

[!UICONTROL Holdco] accepts the connection request to establish a secure link between the two collaborators.

After the connection is established, [!UICONTROL Luma] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL Holdco]. During the project setup, they choose the collaboration use cases that best fit their objectives: [Discover](../collaborate/discover.md), [Activate](../collaborate/activate.md), and [Measure](../collaborate/measure.md).

[!UICONTROL Luma] leverages the [Discover](../collaborate/discover.md) use case to gain insights into [!UICONTROL Holdco]&#39;s audience data. Once [!UICONTROL Luma] has identified the target audience segments, they [activate](../collaborate/activate.md) these audiences.

[!UICONTROL Holdco] can also [activate](../collaborate/activate.md) their audiences to [!UICONTROL Luma]. [!UICONTROL Luma] uses these capabilities to receive paid media insights from agency-run campaigns for insights, CDP profile appends and owned media orchestration.
