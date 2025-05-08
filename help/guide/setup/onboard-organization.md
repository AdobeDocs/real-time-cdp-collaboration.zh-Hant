---
title: 加入及管理組織
description: 瞭解如何在Real-Time CDP Collaboration中建立和管理組織的各個層面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 12e73a9bf64f5746748d1a8c81827c50000a6428
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 17%

---

# 加入及管理組織

{{limited-availability-release-note}}

瞭解如何將您的組織加入Real-Time CDP Collaboration並管理公司的各個層面。 本頁面概述將組織加入Adobe Real-Time CDP Collaboration的步驟，包括設定比對金鑰、偏好身分和更多選項。

![設定頁面](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## 初始組織設定

您必須先設定組織和組織詳細資訊。 導覽至左側邊欄中的&#x200B;**[!UICONTROL 設定]**，選取右上角的&#x200B;**+**&#x200B;符號，然後選取&#x200B;**[!UICONTROL 帳戶]**。

>[!TIP]
>
>設定要使用的初始帳戶後，您可以使用相同的工作流程來設定相同組織內的其他帳戶。

![選取要新增組織至Real-Time CDP Collaboration的帳戶](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

設定組織的工作流程包含下列兩個頁面：

* [設定詳細資訊](#set-up-details)
* [設定相符金鑰](#set-up-match-keys)

>[!IMPORTANT]
>
>您在組織層級選取的任何&#x200B;*相符金鑰*&#x200B;將向下滲透至廣告商與發佈商共同作業中的[專案層級](/help/guide/collaborate/manage-projects.md)。 在專案層級，您可以移除任何相符金鑰，但您&#x200B;*無法*&#x200B;新增此畫面中組織層級未選取的任何其他金鑰。

### 設定詳細資訊 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="聯絡人電子郵件"
>abstract="請提供團隊或角色型電子郵件，例如 `collaboration@yourcompany.com`。不應使用個人或個體的電子郵件地址。"

![設定組織的詳細資訊和使用案例步驟](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. 為您的公司新增&#x200B;**[!UICONTROL 組織名稱]**。
2. 新增有關您公司的&#x200B;**[!UICONTROL 描述]**。
3. 選取您的&#x200B;**[!UICONTROL 公司角色]**。 您可以選取&#x200B;**[!UICONTROL 廣告商]**&#x200B;與&#x200B;**[!UICONTROL 發佈者]**&#x200B;之間。 請閱讀[端對端工作流程檔案](/help/guide/end-to-end-workflow.md)，瞭解兩種組織角色型別之間的工作流程異同和細微差異。
4. 為您的組織選取&#x200B;**[!UICONTROL 產業]**。 某些範例包括&#x200B;**[!UICONTROL 零售業]**、**[!UICONTROL 電信業]**&#x200B;或&#x200B;**[!UICONTROL 金融服務]**。
5. 為您的組織選取&#x200B;**[!UICONTROL 地區]**。 在目前的產品版本中，**[!UICONTROL 北美洲]**&#x200B;為預設預設的預設選取範圍。
6. 為您的組織新增&#x200B;**[!UICONTROL 連絡人電子郵件]**。 這應為團隊或角色型電子郵件地址。 不應提供個人電子郵件地址。
7. 上傳貴公司的&#x200B;**[!UICONTROL 標誌]**。 目前支援SVG型別的影像。
8. 選取公司標題圖片的影像。

對您的選擇感到滿意時，請使用&#x200B;**[!UICONTROL 下一步]**&#x200B;繼續下一頁，並選取貴組織應使用的相符金鑰。

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

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="啟用比對索引鍵"
>abstract="啟動比對金鑰會根據貴組織選擇的比對金鑰而顯示。"

匹配索引鍵（例如電子郵件地址、裝置ID或客戶ID），可啟用準確且以隱私權為中心的資料同步，進而協助廣告商和發佈商共同作業，進而實現更精確的受眾目標定位和測量。

![投影片顯示Real-Time CDP Collaboration第一版的可用識別碼。](/help/assets/setup/manage-organization/available-identifiers.png)

選取您要在協調發佈者和廣告商對象成員時使用的任何比對索引鍵。 包含貴公司可使用的任何相符金鑰。 規劃未來，並選取您預計將在未來發佈商 — 廣告商行銷活動中使用的相符索引鍵。 如果您確實需要為您的組織選取其他相符金鑰，您稍後也可以在[編輯組織](#edit-organization)工作流程中執行此動作。

![符合索引鍵選取步驟。](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

最多選取五個您計畫使用的相符金鑰。 稍後，在設定連線時，您可以移除不需要的相符金鑰，但無法新增金鑰。

Real-Time CDP Collaboration中可用的相符索引鍵可以是三種型別：

* 第一方人員 ID
* 第一方裝置 ID
* 合作夥伴 ID

Real-Time CDP Collaboration第一版的可用比對索引鍵為：

* 已雜湊的電子郵件

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

準備就緒後，選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成組織設定工作流程。

## 編輯組織 {#edit-organization}

初次設定組織後，您隨時可以編輯組織的某些方面和詳細資訊。 若要編輯您的組織，請在&#x200B;**[!UICONTROL 我的組織]**&#x200B;檢視中選取&#x200B;**[!UICONTROL 編輯]**。

![已反白編輯組織控制項。](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

此時，您可以更新組織名稱、說明、標誌和組織設定檔圖片。

![組織的可編輯選項。](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

您也可以更新您在組織上線時最初選取的相符金鑰，以及與相符金鑰對應的身分最低臨界值，以便在對象重疊和其他產品區域中顯示和使用。 在&#x200B;**[!UICONTROL 相符金鑰]**&#x200B;索引標籤中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以新增任何其他所需的相符金鑰或更新身分識別臨界值。

![編輯相符金鑰](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 後續步驟

在設定組織後，您就可以[將對象](/help/guide/setup/onboard-audiences.md)匯入Real-Time CDP Collaboration。
