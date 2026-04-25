---
title: 設定和管理您的帳戶
description: Learn how to configure and manage various aspects of your account in Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
TQID: https://experienceleague.adobe.com/PRmSkRSE2tQ-5t5hHKzDAGrkF6-irmZid2Akq6-PQv8
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1393
ht-degree: 14%

---

# 設定和管理您的帳戶

{{limited-availability-release-note}}

Learn how to set up your account in Real-Time CDP Collaboration to prepare for connections with other collaborators. This guide covers the initial setup of your account, including adding account details, selecting match keys, and managing your account&#39;s settings.

![The setup workspace showing a configured account.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Set up your account {#set-up-account}

When you first access Collaboration, you are prompted to set up your account. This is a one-time process that allows you to configure your account details and match keys. If this is your organization&#39;s first account, you&#39;ll be directed through the onboarding process immediately, starting with setting up your [account details](#set-up-details).

To add additional organizations, navigate to **[!UICONTROL Setup]** in the left rail and select the add icon (![Add icon.](/help/assets/icons/plus.png)) in the upper right corner. Next, select **[!UICONTROL Account]**.

![The setup workspace with the My account tab and Account option highlighted.](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### 設定詳細資訊 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="聯絡人電子郵件"
>abstract="請提供團隊或角色型電子郵件，例如 **collaboration@yourcompany.com**。 不應使用個人或個體的電子郵件地址。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="連接代碼"
>abstract="此連接代碼是您帳戶的唯一識別碼。 在 Real-Time CDP Collaboration 中會使用此代碼與其他協作者建立連線。"

To begin configuring your account, you must first set up the account details. This requires you to add the following information:

* Add an **[!UICONTROL Account name]** that clearly represents your brand.
* Add a **[!UICONTROL Description]** about your brand. This is optional, but it helps other collaborators understand your brand better.
* Select your **[!UICONTROL Role]**. You can select between **[!UICONTROL Advertiser]** and **[!UICONTROL Publisher]**. Read the [roles](/help/guide/overview/roles.md) guide to see similarities and slight differences in workflow between the two account role types.
* Select the **[!UICONTROL Industry]** for your account. Some examples include **[!UICONTROL Retail]**, **[!UICONTROL Telecommunications]**, or **[!UICONTROL Financial services]**.
* The **[!UICONTROL Region]** is automatically set based on your Adobe Experience Cloud account. 此設定隨時無法變更。
* 為您的帳戶新增&#x200B;**[!UICONTROL 連絡人電子郵件]**。 這應為團隊或角色型電子郵件地址。 不應提供個人電子郵件地址。
* 為您的帳戶上傳&#x200B;**[!UICONTROL 標誌]**。 目前支援SVG型別的影像。 這是選擇性的作法，但上傳標誌有助於在Collaboration介面中以視覺化方式呈現您的品牌
* 選取帳戶頁首圖片的影像。

>[!NOTE]
>
>雖然您可以隨時編輯這些詳細資訊，但在初始設定後，**[!UICONTROL 角色]**&#x200B;將無法編輯。 完成時，請使用&#x200B;**[!UICONTROL 下一步]**&#x200B;繼續下一頁，以選取貴組織要使用的相符金鑰。

![顯示[設定帳戶工作區]的[詳細資料]區段，並反白顯示[下一步]選項。](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### 設定比對索引鍵 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵是用於調和來自不同資料來源之客群輪廓的識別碼。 包括您的品牌可以使用的任何比對索引鍵。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="比對索引鍵"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="第一方人員 ID"
>abstract="第一方人員 ID (例如雜湊電子郵件、雜湊電話號碼或 CRM ID) 會直接與個體輪廓連線。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="第一方裝置 ID"
>abstract="第一方裝置 ID (例如 ECID 或 IP 位址) 會直接與裝置連線，這些裝置可能與數個個體共用。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支援的合作夥伴 ID"
>abstract="合作夥伴 ID 是外部合作夥伴提供之客群調和的識別碼。 合作夥伴 ID 沒有直接與個體輪廓連線。"

![支援的相符金鑰。](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>您在帳戶設定期間選取的相符金鑰將決定您連線中可用的相符金鑰。 雖然您可以在連線設定期間[移除不需要的相符金鑰](../connect/establishing-connections.md#connection-settings)，但建立連線後就無法新增相符金鑰。 請務必選取您計畫在帳戶設定期間用於未來行銷活動的&#x200B;**所有**&#x200B;相符金鑰。

比對索引鍵透過啟用準確且以隱私權為中心的資料同步，讓受眾目標定位和測量更精確，協助共同作業人員共同作業。 在帳戶設定期間選取的相符金鑰將決定哪些相符金鑰在未來的連線中可用。 當取得對象時，它們也可用來將資料連線中的欄位[對應到Collaboration中的目標欄位。](./onboard-audiences.md#map-fields)

選取您要在協調對象設定檔時使用的任何比對索引鍵。 規劃未來，並包含您可以使用的相符索引鍵，以及預測會在未來的行銷活動中使用。 如果您稍後確實需要為您的帳戶選取其他相符金鑰，您可以在[編輯帳戶](#edit-account)工作流程中進行。 但是，在初始設定後新增的任何相符索引鍵將不可用於現有連線。

#### 支援的比對索引鍵 {#supported-match-keys}

Collaboration支援三種型別的相符金鑰：第一方人員ID、第一方裝置ID和合作夥伴ID。 所有相符金鑰必須符合下列要求：

* 相符金鑰必須為&#x200B;**修剪**，**小寫**
* 雜湊比對金鑰必須為&#x200B;**SHA256-hashed**。
* 如果您提供使用大寫字元的雜湊值，Collaboration會自動將其轉換為小寫。
* 如果您的來源包含&#x200B;**純文字識別碼**，請在[資料連線設定](./manage-data-connection.md#match-keys)期間使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;選項來套用雜湊。 此選項僅適用於從Experience Platform取得受眾，雲端型來源不支援時。

##### 第一方人員 ID

第一方人員ID直接連結至個別設定檔。 目前支援的ID為：

* **[!UICONTROL 雜湊電子郵件]**
* **[!UICONTROL 雜湊電話]**
* **[!UICONTROL CRM ID]**
* **[!UICONTROL 忠誠度識別碼]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### 第一方裝置 ID

第一方裝置ID是連線至特定裝置的識別碼。 目前支援的ID為：

* **[!UICONTROL 雜湊IPv4]**：雜湊IPv4位址
* **[!UICONTROL IDFA]**： Apple iOS裝置中使用的廣告商識別碼(IDFA)
* **[!UICONTROL GAID]**： Android裝置中使用的Google廣告商ID

##### 合作夥伴 ID

合作夥伴 ID 是外部合作夥伴提供之客群調和的識別碼。 目前支援的ID為：

* **[!UICONTROL AdFixus ID]**

>[!NOTE]
>
>Adobe與[!DNL AdFixus]的整合將每個帳戶的唯一的[!UICONTROL AdFixus ID]對應到通用的Adobe編碼格式。 這些對應可用來識別共同作業人員之間的重疊。 使用&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;啟用對象時，會使用原始的ID。 Adobe編碼格式永遠不會離開Collaboration。

選取&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;時，您需要在&#x200B;**[!UICONTROL 帳戶認證]**&#x200B;區段中提供外部合作夥伴的對應ID。 此選項僅可在&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;上的&#x200B;*切換後*&#x200B;使用。 在&#x200B;**[!UICONTROL 帳戶ID]**&#x200B;欄位中輸入您的AdFixus ID，請務必仔細檢查值是否準確。

![已開啟[比對金鑰]對話方塊，並開啟[AdFixus ID]及[帳戶認證]區段。](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

選取所有需要的相符金鑰後，選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成帳戶設定工作流程。

![已顯示[設定帳戶工作區]的[比對金鑰]區段。](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 編輯帳戶 {#edit-account}

設定帳戶後，您可以隨時編輯詳細資料並比對金鑰。

### 編輯詳細資料 {#edit-details}

您可以隨時編輯帳戶的大部分詳細資料，但&#x200B;**[!UICONTROL 角色]**&#x200B;除外。 地區是根據您的Adobe Experience Cloud帳戶自動設定，且無法變更。

若要編輯您的帳戶，請在&#x200B;**[!UICONTROL 設定]**&#x200B;工作區的&#x200B;**[!UICONTROL 我的帳戶]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![反白顯示[我的帳戶]索引標籤和[編輯]選項的[設定]工作區。](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

您現在可以編輯帳戶詳細資料。 更新您要變更的任何欄位，然後選取[儲存]以確認變更。****

![編輯帳戶詳細資料對話方塊。](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### 編輯比對索引鍵 {#edit-match-keys}

您也可以更新建立帳戶時最初選取的相符金鑰。 這些比對鍵將決定可用於未來連線的比對鍵。

在&#x200B;**[!UICONTROL 比對索引鍵]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![在帳戶的「比對金鑰」區段中，以「編輯」選項醒目提示的「設定」工作區。](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

**[!UICONTROL 符合索引鍵]**&#x200B;對話方塊就會顯示。 開啟任何相符金鑰，或更新[!UICONTROL AdFixus ID的]的&#x200B;**[!UICONTROL 帳戶ID]**，然後選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以確認變更。

>[!IMPORTANT]
>
>變更您的[!UICONTROL AdFixus ID]將不會使用比對索引鍵觸發現有資料連線的[資料草圖](../glossary.md#sketches)重新整理。 您的資料草圖完成後，您的[!UICONTROL AdFixus ID]所做的任何變更都不會反映在您的[資料連線排程](./manage-data-connection.md#scheduling)設定之後的下一次對象重新整理中。 如果您在下次重新整理之前需要變更，可以刪除並重新建立資料連線。
>
>此時，將相符金鑰新增至您的帳戶後，就無法移除該金鑰。

![反白顯示[儲存]選項的[比對索引鍵]對話方塊。](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

成功對話方塊會確認已成功更新帳戶的相符金鑰。

![確認您帳戶的相符金鑰的成功對話方塊已成功更新。](/help/assets/setup/manage-account/match-key-updated-successfully.png){zoomable="yes"}

## 後續步驟

設定帳戶之後，您就可以將[來源對象](/help/guide/setup/onboard-audiences.md)放入Real-Time CDP Collaboration了。
