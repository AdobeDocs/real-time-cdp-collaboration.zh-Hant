---
title: 設定Collaboration [!DNL Starter] 上線的管理員存取權
description: 瞭解如何使用Adobe Experience Cloud中的Admin Console設定Adobe Real-Time CDP Collaboration [!DNL Starter] 的管理員存取權。
audience: users invited to Real-Time CDP Collaboration [!DNL Starter]
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7b5aa5e2-1238-4a0b-be20-becfe6c9e0b7
source-git-commit: db4cc34592e49254163d7db54f93238146ce72a4
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 3%

---

# 設定Collaboration [!DNL Starter]上線的管理員存取權

作為您組織中第一個透過Collaboration [!DNL Starter]存取Adobe Experience Platform的使用者，您負責設定和管理您團隊的存取權。 您必須授予自己必要的管理員和使用者許可權，才能開始在Real-Time CDP Collaboration中工作。 閱讀本指南，瞭解如何在Admin Console中設定必要的存取權，以便您可以在許可權介面中管理共同作業的許可權。

## 先決條件 {#prerequisites}

在繼續之前，請確定您已：

* 已接受您的授權Collaboration合作夥伴的邀請。 如需邀請要求的詳細資訊，請參閱[Collaboration [!DNL Starter] 總覽](../overview/starter-overview.md#prerequisites)。
* 檢閱並簽署Collaboration條款與條件。
* 已收到您的Adobe歡迎電子郵件，並完成您的首次帳戶建立。

## 設定存取權 {#setup-access}

透過[!DNL Starter]工作流程建立您的Adobe帳戶時，系統會自動將系統管理員角色指派給您。 這可讓您在Admin Console中管理使用者和產品存取權。 不過，您尚未擁有管理Collaboration存取權所需的&#x200B;**[!UICONTROL 許可權]**&#x200B;存取權。

使用Admin Console授與您自己&#x200B;**產品管理員對Experience Platform的存取權**，以及&#x200B;**使用者對Experience Platform產品的存取權**，以取得&#x200B;**[!UICONTROL 許可權]**。

若要進一步瞭解Experience Cloud中的角色和產品，請閱讀[存取控制總覽](../permissions/overview.md)檔案。

>[!TIP]
>
>在本指南中，**管理員**&#x200B;會同時參照&#x200B;**系統和產品管理員**。

### 設定產品管理員存取權 {#configure-product-admin-access}

請閱讀本節，授予您管理員許可權，以開始設定Collaboration [!DNL Starter]的存取權。

#### 存取Admin Console {#access-admin-console}

若要開始，請使用您的認證登入[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。 您可以在&#x200B;**[!UICONTROL 快速存取]**&#x200B;區段中看到可用產品的清單。 選取&#x200B;**[!UICONTROL Admin Console]**。

![醒目提示Admin Console的Adobe Experience Cloud首頁。](../../assets/setup/starter/admin-access/select-admin-console.png){zoomable="yes"}

#### 存取Adobe Experience Platform產品控制面板 {#access-adobe-experience-platform}

[Admin Console](https://adminconsole.adobe.com/)工作區會在新索引標籤中開啟。 從&#x200B;**[!UICONTROL 產品和服務]**&#x200B;下的&#x200B;**[!UICONTROL 產品]**&#x200B;清單中選取&#x200B;**[!UICONTROL Adobe Experience Platform]**。

![反白顯示Adobe Experience Platform產品的Admin Console工作區。](../../assets/setup/starter/admin-access/admin-console-workspace.png){zoomable="yes"}

#### 新增產品管理員 {#add-product-admin}

在&#x200B;**[!UICONTROL Adobe Experience Platform]**&#x200B;產品儀表板中，導覽至&#x200B;**[!UICONTROL 管理員]**&#x200B;標籤。 然後選取&#x200B;**[!UICONTROL 新增管理員]**。

![Adobe Experience Platform產品儀表板，其中的「管理員」索引標籤和「新增管理員」選項已反白顯示。](../../assets/setup/starter/admin-access/add-admin.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 新增產品管理員]**&#x200B;對話方塊中輸入您的電子郵件地址或使用者名稱，然後從下拉式清單中選取正確的帳戶。 完成後，選取&#x200B;**[!UICONTROL 儲存]**。

![新增產品管理員對話方塊會顯示您帳戶的資訊，且[儲存]選項會反白顯示。](../../assets/setup/starter/admin-access/add-product-admin.png){zoomable="yes"}

您現在是產品管理員，並且可以在Admin Console中將使用者或其他管理員新增到產品中。 接著，授予您自己對Experience Platform產品的使用者存取權，以存取及執行許可權中的功能。

### 設定使用者存取權 {#configure-user-access}

若要管理Collaboration許可權，除了系統管理員存取權之外，您還必須擁有產品的&#x200B;**使用者存取權**。 使用者存取權可由系統或產品管理員設定。

>[!TIP]
>
>如果您是依照上一節的指示進行，則您應該已經在Admin Console的&#x200B;**[!UICONTROL Adobe Experience Platform]**&#x200B;產品儀表板中。 從這裡，繼續進行[將自己新增為使用者](#add-user)。

若要開始設定使用者存取權，請完成下列步驟：

1. [從Admin Console首頁](#access-admin-console)存取Adobe Experience Cloud。
2. [導覽至Adobe Experience Platform產品儀表板](#access-adobe-experience-platform)。

#### 將使用者新增至產品 {#add-user}

您現在在&#x200B;**[!UICONTROL Adobe Experience Platform]**&#x200B;產品儀表板中。 瀏覽至&#x200B;**[!UICONTROL 使用者]**&#x200B;索引標籤，然後選取&#x200B;**[!UICONTROL 新增使用者]**。

![Adobe Experience Platform產品儀表板，其中的[使用者]索引標籤和[新增使用者]選項反白顯示。](../../assets/setup/starter/admin-access/add-user.png){zoomable="yes"}

**[!UICONTROL 新增使用者至此產品]**&#x200B;對話方塊會出現，提示您輸入您的姓名、使用者群組或電子郵件地址。 填寫值，然後從下拉式清單中選取您的帳戶。

![將使用者新增至此產品對話方塊會顯示您帳戶的資訊，並反白顯示[產品]選項。](../../assets/setup/starter/admin-access/add-users-to-product.png){zoomable="yes"}

接著，在&#x200B;**[!UICONTROL 產品]**&#x200B;下選取新增圖示![新增圖示](../../assets/icons/plus.png)。

會出現一個對話方塊，其中包含可用的[產品設定檔](https://helpx.adobe.com/tw/enterprise/using/manage-product-profiles.html)清單。 選取&#x200B;**[!UICONTROL AEP-Default-All-Users]**&#x200B;和&#x200B;**[!UICONTROL 預設的生產所有存取權]**。 然後選取&#x200B;**[!UICONTROL 套用]**。

![選取產品設定檔對話方塊會顯示選取的產品設定檔，且「套用」選項會反白顯示。](../../assets/setup/starter/admin-access/select-product-profiles.png){zoomable="yes"}

最後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以完成新增使用者至產品。

![將使用者新增至此產品對話方塊，並反白顯示[儲存]選項。](../../assets/setup/starter/admin-access/save-user.png){zoomable="yes"}

取得使用者存取權後，請導覽回[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。 確認&#x200B;**[!UICONTROL 許可權]**&#x200B;和&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**&#x200B;可以在&#x200B;**[!UICONTROL 快速存取]**&#x200B;下使用。

![Adobe Experience Cloud首頁畫面顯示「快速存取」底下所列的許可權和Real-Time CDP Collaboration，並反白顯示。](../../assets/setup/starter/admin-access/permissions-collaboration-available.png){zoomable="yes"}

>[!TIP]
>
>如果&#x200B;**[!UICONTROL 許可權]**&#x200B;和&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**&#x200B;未出現在&#x200B;**[!UICONTROL 快速存取]**&#x200B;中，請嘗試登出並重新登入。

## 後續步驟 {#next-steps}

您現在同時擁有&#x200B;**管理員存取權**&#x200B;和&#x200B;**使用者存取權**&#x200B;以輸入許可權，您可在此定義角色、指派特定許可權，以及管理Collaboration功能與資源的使用者存取權。 如需逐步指示，請參閱[許可權控制指南](./starter-permission-controls.md)。
