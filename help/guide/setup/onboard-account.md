---
title: 設定和管理您的帳戶
description: 瞭解如何在Real-Time CDP Collaboration中設定和管理帳戶的各種層面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1363'
ht-degree: 14%

---

# 設定和管理您的帳戶

{{limited-availability-release-note}}

瞭解如何在Real-Time CDP Collaboration中設定您的帳戶，為與其他共同作業人員的連線做好準備。 本指南涵蓋您帳戶的初始設定，包括新增帳戶詳細資料、選取相符金鑰以及管理您的帳戶設定。

![顯示設定帳戶的安裝程式工作區。](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## 設定您的帳戶 {#set-up-account}

第一次存取Collaboration時，系統會提示您設定帳戶。 此為一次性程式，可讓您設定帳戶詳細資料和比對金鑰。 如果這是您組織的第一個帳戶，會立即引導您完成入門流程，從設定您的[帳戶詳細資料](#set-up-details)開始。

若要新增其他組織，請導覽至左側邊欄中的&#x200B;**[!UICONTROL 設定]**，並選取新增圖示(![新增圖示。](/help/assets/icons/plus.png))。 接著，選取&#x200B;**[!UICONTROL 帳戶]**。

![含有[我的帳戶]索引標籤和[帳戶]選項的設定工作區已反白顯示。](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### 設定詳細資訊 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="聯絡人電子郵件"
>abstract="請提供團隊或角色型電子郵件，例如 **collaboration@yourcompany.com**。不應使用個人或個體的電子郵件地址。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="連接代碼"
>abstract="此連接代碼是您帳戶的唯一識別碼。在 Real-Time CDP Collaboration 中會使用此代碼與其他協作者建立連線。"

若要開始設定帳戶，您必須先設定帳戶詳細資料。 這需要您新增下列資訊：

* 新增明確代表您品牌的&#x200B;**[!UICONTROL 帳戶名稱]**。
* 新增品牌的&#x200B;**[!UICONTROL 描述]**。 這是選用的功能，但可協助其他共同作業人員更清楚瞭解您的品牌。
* 選取您的&#x200B;**[!UICONTROL 角色]**。 您可以選取&#x200B;**[!UICONTROL 廣告商]**&#x200B;與&#x200B;**[!UICONTROL 發佈者]**&#x200B;之間。 閱讀[角色](/help/guide/overview/roles.md)指南，瞭解兩種帳戶角色型別之間的相似之處和工作流程細微差異。
* 為您的帳戶選取&#x200B;**[!UICONTROL 產業]**。 某些範例包括&#x200B;**[!UICONTROL 零售業]**、**[!UICONTROL 電信業]**&#x200B;或&#x200B;**[!UICONTROL 金融服務]**。
* 已根據您的Adobe Experience Cloud帳戶自動設定&#x200B;**[!UICONTROL 地區]**。 此設定隨時無法變更。
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
>abstract="比對索引鍵是用於調和來自不同資料來源之客群輪廓的識別碼。包括您的品牌可以使用的任何比對索引鍵。"

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
>abstract="第一方裝置 ID (例如 ECID 或 IP 位址) 會直接與裝置連線，這些裝置可能與數個個體共用。IPv4 是目前唯一支援的第一方裝置 ID。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支援的合作夥伴 ID"
>abstract="合作夥伴 ID 是外部合作夥伴提供之客群調和的識別碼。合作夥伴 ID 沒有直接與個體輪廓連線。"

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
* 如果您的來源包含&#x200B;**純文字識別碼**，請在&#x200B;**[!UICONTROL 資料連線設定]**&#x200B;期間使用[套用轉換](./manage-data-connection.md#match-keys)選項來套用雜湊。 此選項僅適用於從Experience Platform取得受眾，雲端型來源不支援時。

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

##### 合作夥伴 ID

合作夥伴 ID 是外部合作夥伴提供之客群調和的識別碼。目前支援的ID為：

* **[!UICONTROL Adfixus ID]**

>[!NOTE]
>
>Adobe與[!DNL Adfixus]的整合將每個帳戶的唯一的[!UICONTROL Adfixus ID]對應到常見的Adobe編碼格式。 這些對應可用來識別共同作業人員之間的重疊。 使用&#x200B;**[!UICONTROL Adfixus ID]**&#x200B;啟用對象時，會使用原始的ID。 Adobe編碼格式永遠不會離開Collaboration。

選取&#x200B;**[!UICONTROL Adfixus ID]**&#x200B;時，您需要在&#x200B;**[!UICONTROL 帳戶認證]**&#x200B;區段中提供外部合作夥伴的對應ID。 此選項只有在&#x200B;*切換* Adfixus ID **[!UICONTROL 後]**&#x200B;才能使用。 在&#x200B;**[!UICONTROL 帳戶ID]**&#x200B;欄位中輸入您的Adfixus ID，請務必仔細檢查值是否準確。

![已開啟[比對金鑰]對話方塊，並開啟[Adfixus ID]及[帳戶認證]區段。](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

選取所有需要的相符金鑰後，選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成帳戶設定工作流程。

![已顯示[設定帳戶工作區]的[比對金鑰]區段。](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 編輯帳戶 {#edit-account}

設定帳戶後，您可以隨時編輯詳細資料並比對金鑰。

### 編輯詳細資料 {#edit-details}

您可以隨時編輯帳戶的大部分詳細資料，但&#x200B;**[!UICONTROL 角色]**&#x200B;除外。 地區是根據您的Adobe Experience Cloud帳戶自動設定，且無法變更。

若要編輯您的帳戶，請在&#x200B;**[!UICONTROL 設定]**&#x200B;工作區的&#x200B;**[!UICONTROL 我的帳戶]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![反白顯示[我的帳戶]索引標籤和[編輯]選項的[設定]工作區。](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

您現在可以編輯帳戶詳細資料。 更新您要變更的任何欄位，然後選取[儲存]以確認變更。**&#x200B;**

![編輯帳戶詳細資料對話方塊。](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### 編輯比對索引鍵 {#edit-match-keys}

>[!IMPORTANT]
>
>編輯比對鍵不會影響您現有的連線。 建立連線後，您在連線設定期間選取的相符金鑰就會固定。 請務必選取您計畫在帳戶設定期間用於未來行銷活動的&#x200B;**所有**&#x200B;相符金鑰。

您也可以更新建立帳戶時最初選取的相符金鑰。 這些比對鍵將決定可用於未來連線的比對鍵。

在&#x200B;**[!UICONTROL 比對索引鍵]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![在帳戶的「比對金鑰」區段中，以「編輯」選項醒目提示的「設定」工作區。](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

**[!UICONTROL 符合索引鍵]**&#x200B;對話方塊就會顯示。 開啟或關閉任何相符金鑰，或是更新您&#x200B;**[!UICONTROL Adfixus ID的]**&#x200B;的[!UICONTROL 帳戶ID]，然後選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以確認變更。

>[!IMPORTANT]
>
>變更您的[!UICONTROL Adfixus ID]將不會使用比對索引鍵觸發現有資料連線的[資料草圖](../glossary.md#sketches)重新整理。 您的資料一旦完成草繪，在您下次根據[!UICONTROL 資料連線排程]設定重新整理對象之前，不會反映對[Adfixus ID](./manage-data-connection.md#scheduling)所做的任何變更。 如果您在下次重新整理之前需要變更，可以刪除並重新建立資料連線。

![反白顯示[儲存]選項的[比對索引鍵]對話方塊。](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

## 後續步驟

設定帳戶之後，您就可以將[來源對象](/help/guide/setup/onboard-audiences.md)放入Real-Time CDP Collaboration了。
