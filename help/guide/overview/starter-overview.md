---
title: RTCDP Collaboration入門概述
description: 瞭解Adobe Real-Time CDP Collaboration Starter如何協助您與授權合作夥伴擴展及增強以隱私權為中心的協同合作，而不需要您自己的完整Real-Time CDP授權。
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: c759496b528ed6c1e173f1ca1f1469da572c85df
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Adobe Real-Time CDP Collaboration [!DNL Starter]總覽

使用Adobe Real-Time CDP Collaboration [!DNL Starter]與授權合作夥伴共同作業以隱私權為中心的資料專案。 您不需要自己的Collaboration授權即可參與。

您的授權合作夥伴邀請您加入Collaboration，並使用其成果在廣告商對發佈商和品牌對品牌模式中，為您的聯合工作流程提供資金。 若要進一步瞭解這些模式及其運作方式，請閱讀[共同作業模式](./collaboration-patterns.md)和[端對端工作流程](./end-to-end-workflow.md)指南。

身為受邀的[!DNL Starter]使用者，您可以：

* 在[!DNL Starter]帳戶中上線及管理共同作業資料。
* Source和維護對象，以用於聯合專案。
* 深入瞭解與合作夥伴的對象重疊，以支援有效的目標定位和促銷活動測量。
* 啟用對象並與您的合作夥伴分享，以進行聯合行銷活動啟用和參與。

## 先決條件 {#prerequisites}

若要開始使用Collaboration [!DNL Starter]，請確認您的組織和授權合作夥伴位於相同地區。 您必須受到擁有Real-Time CDP Prime、Ultimate或Collaboration授權的合作夥伴的邀請。

若要啟動邀請，請提供下列資訊給您的授權合作夥伴：

* 連絡人姓名
* 聯絡人電子郵件
* 公司
* 角色（廣告商/發佈商）：廣告商
* 行業

收到並接受邀請後，貴組織必須檢閱並簽署Adobe的免費銷售訂單，才能存取Collaboration [!DNL Starter]。 如需邀請程式的詳細資訊，請參閱[邀請共同作業人員加入Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator)指南。

## 護欄 {#guardrails}

請閱讀下表以瞭解適用於您[!DNL Starter]帳戶的重要護欄。 其中包括對象來源、資料量、重新整理頻率、對象重疊和啟用功能的限制。

| 護欄 | 說明 |
|----------| ------------|
| 客群來源 | 您可以以&#x200B;**[!DNL Amazon S3]**&#x200B;作為來源，將受眾資料帶入Collaboration。 如需逐步指示，請參閱[如何設定 [!DNL Amazon S3] 對象來源](../setup/configure-aws-s3-audience-sourcing.md)。 |
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
