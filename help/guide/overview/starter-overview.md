---
title: RTCDP Collaboration Starter Overview
description: Learn how Adobe Real-Time CDP Collaboration Starter helps you to expand and enhance privacy-centric collaboration with a licensed partner without requiring your own full Real-Time CDP license.
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: 3d29985d88e6370b4a0e8cd3d56358e85bb91e06
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Adobe Real-Time CDP Collaboration [!DNL Starter] Overview

Use Adobe Real-Time CDP Collaboration [!DNL Starter] to collaborate with a licensed partner on privacy-centric data projects. You do not need your own Collaboration license to participate.

Your licensed partner invites you into Collaboration and uses their credits to fund your joint workflows, across both advertiser-to-publisher and brand-to-brand patterns. To learn more about these patterns and how they work, read the [collaboration patterns](./collaboration-patterns.md) and [end-to-end workflow](./end-to-end-workflow.md) guides.

As an invited [!DNL Starter] user, you can:

* Onboard and manage collaboration data in a [!DNL Starter] account.
* Source and maintain audiences for use in joint projects.
* Gain insights into audience overlaps with your partner to support effective targeting and campaign measurement.
* Activate audiences and share them back to your partner for joint campaign activation and engagement.

## 先決條件 {#prerequisites}

To get started with Collaboration [!DNL Starter], ensure that both your organization and your licensed partner are located in the same region. You must be invited by a partner who holds a Real-Time CDP Prime, Ultimate, or Collaboration license.

To initiate the invitation, provide the following information to your licensed partner:

* Contact name
* 聯絡人電子郵件
* 公司
* Role (Advertiser/Publisher): Advertiser
* 行業

After you receive and accept the invitation, your organization must review and sign a no-cost Sales Order with Adobe to access Collaboration [!DNL Starter]. For more details on the invitation process, see the [inviting a collaborator to Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator-to-starter) guide.

## 護欄 {#guardrails}

Read the following table to understand the key guardrails that apply to your [!DNL Starter] account. These include limits on audience sourcing, data volume, refresh frequency, audience overlaps and activation capabilities.

| Guardrail | 說明 |
|----------| ------------|
| 客群來源 | You can bring audience data into Collaboration with **[!DNL Amazon S3]** as your source. For step-by-step instructions, see [how to configure [!DNL Amazon S3] for audience sourcing](../setup/configure-aws-s3-audience-sourcing.md). |
| 客群 | 您的[!DNL Starter]帳戶最多可享有：<ul><li>來自[!DNL AWS S3]貯體的10個對象</li><li>身分總計5,000萬（根據對象資料中的列數計算）</li><li>每個對象1次重新整理（每6天）</li></ul> |
| 對象重疊和深入分析 | 您的對象執行對象重疊和深入分析的頻率沒有使用限制。 瞭解如何[探索重疊並比較對象](../collaborate/discover.md)。 |
| 啟用 | 身為[!DNL Starter]使用者，您只能與邀請您的合作夥伴啟用及共用對象。 無法設定外部平台的目的地。 深入瞭解[啟用您的對象](../collaborate/activate.md)。 |

{style="table-layout:auto"}

## 快速入門 {#getting-started}

在您[接受您的邀請並同意條款後](../connect/establishing-connections.md#accept-invitation-sign-terms)，請使用您的認證登入[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。 您必須先將適當的存取權和角色授予您的帳戶，您才能使用Collaboration。

使用此工作流程來設定您的[!DNL Starter]帳戶，並開始與您的合作夥伴共同作業。

### 設定管理員存取權 {#setup-admin-access}

首先，使用&#x200B;**管理員存取權**&#x200B;工作區來授予您必要的存取權。 這可確保您同時擁有Experience Platform產品的管理許可權和使用者存取權。 如需設定初始存取許可權的詳細步驟，請參閱[管理員存取指示](../setup/starter-admin-access.md)。

完成後，您應該會在[Experience Platform](https://experience.adobe.com/){target="_blank"}首頁的&#x200B;**[!UICONTROL 快速存取]**&#x200B;區段中，看到&#x200B;**[!UICONTROL 許可權]**、**[!UICONTROL Adobe Experience Cloud]**&#x200B;和&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。

![產品管理員存取設定後，Adobe Experience Cloud工作區會顯示許可權、Experience Platform和Real-Time CDP Collaboration。](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

如需有關存取角色和不同Adobe Experience Cloud產品的詳細資訊，請閱讀[存取控制總覽](../permissions/overview.md)。

### 設定許可權 {#configure-permissions}

現在您擁有管理員許可權，可以將角色和許可權指派給您自己和組織中的其他使用者。 您必須先執行此步驟，才能存取Real-Time CDP Collaboration或允許其他人使用。 如需詳細指示，請參閱[如何設定許可權](../setup/starter-permission-controls.md)。 如需Collaboration中不同角色和許可權的詳細資訊，請參閱[管理角色](../permissions/manage-roles.md)檔案。

指派角色和許可權後，請確認您可以存取Collaboration。 導覽至[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}，並在&#x200B;**[!UICONTROL 快速存取]**&#x200B;區段內選取&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。 這會開啟&#x200B;**[!UICONTROL Adobe Real-Time CDP Collaboration]**&#x200B;工作區，您可在此開始使用Collaboration功能。

### 設定連線 {#set-up-connections}

接下來，請遵循下列指南中的步驟，以設定連線並開始與合作夥伴合作：

* [設定您的Collaboration帳戶](../setup/onboard-account.md)
* [與邀請的共同作業人員建立連線](../connect/overview.md)
* [建立新專案並開始與合作夥伴合作](../collaborate/overview.md)

### 瞭解信用使用情況 {#understand-credit-usage}

所有Collaboration [!DNL Starter]活動都使用積分。 但是，身為受邀使用者，您不需要購買或管理這些積分。 邀請您的共同作業人員涵蓋與活動相關的所有信用使用情況。 若要深入瞭解，請參閱Collaboration [!DNL Starter][&#128279;](../setup/starter-credit-usage.md)檔案中的信用使用量和消耗量。

## 後續步驟 {#next-steps}

您現在已經完成初始設定，並將您的組織設定為安全共同作業。 接下來，探索下列資源，以瞭解Collaboration中的對象來源和不同的專案使用案例：

* [Source和管理對象](../setup/onboard-audiences.md)
* [專案使用案例](../collaborate/overview.md#project-use-cases)：
   * [探索重疊並比較對象](../collaborate/discover.md)
   * [啟用客群](../collaborate/activate.md)
   * [測量行銷活動績效](../collaborate/measure.md)
