---
title: 加入及管理組織
description: 瞭解如何在Real-Time CDP Collaboration中建立和管理組織的各個層面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 860138b95abc4d6af94bbbf722cf498463570c1b
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 19%

---

# 加入並管理您的組織

{{limited-availability-release-note}}

瞭解如何將您的組織加入Real-Time CDP Collaboration並管理公司的各個層面。 本頁面概述將組織加入Adobe Real-Time CDP Collaboration的步驟，包括設定比對金鑰、偏好身分和更多選項。

![組織的設定工作區顯示其目前的設定。](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## 初始組織設定

您必須先設定組織和組織詳細資訊。 如果這是您的第一個組織，會立即引導您完成入門流程，從設定您的[帳戶詳細資料](#set-up-details)開始。

若要新增其他組織，請導覽至左側邊欄中的&#x200B;**[!UICONTROL 設定]**，並選取新增圖示(![新增圖示。](/help/assets/icons/plus.png))。 接著，選取&#x200B;**[!UICONTROL 帳戶]**。

![設定工作區中反白了[帳戶]選項。](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

### 設定詳細資訊 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="聯絡人電子郵件"
>abstract="請提供團隊或角色型電子郵件，例如 `collaboration@yourcompany.com`。不應使用個人或個體的電子郵件地址。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="連接代碼"
>abstract="連接代碼是您的組織的唯一識別碼。在 Real-Time CDP Collaboration 中會使用此代碼與其他組織建立連線。"

<!-- Move the above to new section for invite on this page when its created -->

若要開始建立組織，您必須先設定組織詳細資訊。 這需要您新增下列資訊：

* 為您的公司新增&#x200B;**[!UICONTROL 組織名稱]**。
* 新增有關您公司的&#x200B;**[!UICONTROL 描述]**。
* 選取您的&#x200B;**[!UICONTROL 公司角色]**。 您可以選取&#x200B;**[!UICONTROL 廣告商]**&#x200B;與&#x200B;**[!UICONTROL 發佈者]**&#x200B;之間。 請閱讀[端對端工作流程檔案](/help/guide/end-to-end-workflow.md)，瞭解兩種組織角色型別之間的工作流程異同和細微差異。
* 為您的組織選取&#x200B;**[!UICONTROL 產業]**。 某些範例包括&#x200B;**[!UICONTROL 零售業]**、**[!UICONTROL 電信業]**&#x200B;或&#x200B;**[!UICONTROL 金融服務]**。
* 為您的組織選取&#x200B;**[!UICONTROL 地區]**。 在目前的產品版本中，**[!UICONTROL 北美洲]**&#x200B;為預設預設的預設選取範圍。
* 為您的組織新增&#x200B;**[!UICONTROL 連絡人電子郵件]**。 這應為團隊或角色型電子郵件地址。 不應提供個人電子郵件地址。
* 上傳貴公司的&#x200B;**[!UICONTROL 標誌]**。 目前支援SVG型別的影像。
* 選取公司標題圖片的影像。

>[!NOTE]
>
>雖然您可以隨時編輯這些詳細資訊，但在初始設定後，**[!UICONTROL 角色]**&#x200B;和&#x200B;**[!UICONTROL 地區]**&#x200B;將無法編輯。

![顯示[詳細資料]區段的[設定組織]工作區。](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

完成時，請使用&#x200B;**[!UICONTROL 下一步]**&#x200B;繼續下一頁，以選取貴組織要使用的相符金鑰。

### 設定比對索引鍵 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵是用於調和來自不同資料來源之客群成員的識別碼。包括您的公司可以使用的任何比對索引鍵。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="第一方人員 ID"
>abstract="第一方人員 ID (例如雜湊電子郵件或電話號碼) 會直接與個體輪廓連線。目前支援的 ID 是雜湊電子郵件和電話號碼。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="第一方裝置 ID"
>abstract="第一方裝置 ID (例如 ECID 或 IP 位址) 會直接與裝置連線，這些裝置可能與數個個體共用。IPv4 是目前唯一支援的第一方裝置 ID。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支援的合作夥伴 ID"
>abstract="與輪廓關聯的合作夥伴 ID 可擴充特定輪廓的觸及範圍。"

>[!IMPORTANT]
>
>您在組織設定期間選取的相符索引鍵將決定您與其他組織建立的連線可用的相符索引鍵。 雖然您可以在連線設定期間移除相符金鑰，但您稍後無法新增相符金鑰。 在組織設定期間，請務必選取您計畫用於未來行銷活動的所有相符索引鍵。

匹配索引鍵（例如電子郵件地址、裝置ID或客戶ID），可啟用準確且以隱私權為中心的資料同步，進而協助廣告商和發佈商共同作業，進而實現更精確的受眾目標定位和測量。

![投影片顯示Real-Time CDP Collaboration第一版的可用識別碼。](/help/assets/setup/manage-organization/available-identifiers.png)

選取您要在協調發佈者和廣告商對象成員時使用的任何比對索引鍵。 包含貴公司可使用的任何相符金鑰。 規劃未來，並選取您預計將在未來發佈商 — 廣告商行銷活動中使用的相符索引鍵。 如果您確實需要為您的組織選取其他相符金鑰，您稍後也可以在[編輯組織](#edit-organization)工作流程中執行此動作。

![顯示[設定組織]工作區的[比對索引鍵]區段。](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

最多選取五個您計畫使用的相符金鑰。 稍後，在設定連線時，您可以移除不需要的相符金鑰，但無法新增金鑰。

Real-Time CDP Collaboration中可用的相符索引鍵可以是三種型別：

* 第一方人員 ID
* 第一方裝置 ID
* 合作夥伴 ID

Real-Time CDP Collaboration第一版的可用比對索引鍵為：

* 已雜湊的電子郵件

準備就緒後，選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成組織設定工作流程。

## 編輯組織 {#edit-organization}

初次設定組織後，您隨時可以編輯組織的某些方面和詳細資訊。 若要編輯您的組織，請在&#x200B;**[!UICONTROL 設定]工作區**&#x200B;的&#x200B;**[!UICONTROL 我的組織]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![反白顯示[我的組織]索引標籤和[編輯]選項的[設定]工作區。](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

您現在可以編輯組織詳細資料，但&#x200B;**[!UICONTROL 角色]**&#x200B;和&#x200B;**[!UICONTROL 地區]**&#x200B;除外。

![編輯組織詳細資料對話方塊。](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

您也可以更新您在加入組織時最初選取的相符金鑰。 在&#x200B;**[!UICONTROL 相符金鑰]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以新增任何其他所需的相符金鑰。

![在組織的「比對索引鍵」區段中，以「編輯」選項醒目提示的「設定」工作區。](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 後續步驟

在設定組織後，您就可以[將對象](/help/guide/setup/onboard-audiences.md)匯入Real-Time CDP Collaboration。
