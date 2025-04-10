---
title: 加入及管理組織
description: 瞭解如何在Real-Time CDP Collaboration中建立和管理組織的各個層面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# 入職和管理組織

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

* [設定詳細資料](#set-up-details)
* [設定相符金鑰](#set-up-match-keys)

>[!IMPORTANT]
>
>您在組織層級選取的任何&#x200B;*相符金鑰*&#x200B;將向下滲透至廣告商與發佈商共同作業中的[專案層級](/help/guide/collaborate/manage-projects.md)。 在項目級別，您可以刪除任何匹配鍵，但&#x200B;**&#x200B;無法在此螢幕中添加未在組織級別選擇的任何其他鍵。

### 設定詳細數據 {#set-up-details}

![設定組織的詳細資訊和使用案例步驟](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. 為 **[!UICONTROL 公司添加組織名稱]** 。
2. 新增有關您公司的&#x200B;**[!UICONTROL 描述]**。
3. 選取您的&#x200B;**[!UICONTROL 公司角色]**。 您可以選取&#x200B;**[!UICONTROL 廣告商]**&#x200B;與&#x200B;**[!UICONTROL 發佈者]**&#x200B;之間。 請閱讀[端對端工作流程檔案](/help/guide/end-to-end-workflow.md)，瞭解兩種組織角色型別之間的工作流程異同和細微差異。
4. 為您的組織選取&#x200B;**[!UICONTROL 產業]**。 某些範例包括&#x200B;**[!UICONTROL 零售業]**、**[!UICONTROL 電信業]**&#x200B;或&#x200B;**[!UICONTROL 金融服務]**。
5. **[!UICONTROL 選擇組織的區域]**。在產品的當前版本中， **[!UICONTROL 北美]** 是預設的默認選擇。
6. <span class="preview"> 僅限</span>發佈商：設置發佈者組織時，您必須閱讀並確認您將被發佈者目錄中的廣告客戶發現。
   ![發佈者特定的選擇加入訊息。](/help/assets/setup/manage-organization/publisher-specific-optin-message.png){zoomable="yes"}
7. 上傳貴公司的&#x200B;**[!UICONTROL 標誌]**。 目前支援SVG型別的影像。
8. 選取公司標題圖片的影像。

對您的選擇感到滿意時，請使用&#x200B;**[!UICONTROL 下一步]**&#x200B;繼續下一頁，並選取貴組織應使用的相符金鑰。

### 設定比對索引鍵 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵是用來調解來自不同資料來源之對象中成員的識別碼。 包含貴公司可使用的任何相符金鑰。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="第一方人員ID"
>abstract="第一方人員ID （例如雜湊電子郵件地址或電話號碼）會直接連線至個別設定檔。 目前支援的ID為雜湊電子郵件和電話號碼。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="第一方裝置 ID"
>abstract="ECID 或 IP 地址等第一方 裝置 ID 直接連接到裝置，多人可共享。 IPv4 是目前唯一支持的第一方 裝置 ID。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支持的合作夥伴 ID"
>abstract="與描述檔關聯的合作夥伴ID可將觸及擴大至特定設定檔。"

匹配索引鍵（例如電子郵件地址、裝置ID或客戶ID），可啟用準確且符合隱私權規範的資料同步，進而協助廣告商和發佈商共同作業，進而實現更精確的對象定位和測量。

![投影片顯示Real-Time CDP Collaboration第一版的可用識別碼。](/help/assets/setup/manage-organization/available-identifiers.png)

選取您要在協調發佈者和廣告商對象成員時使用的任何比對索引鍵。 包括您的公司可以使用的任何匹配鍵。 計劃未來，然後選擇您預計將在將來發佈者廣告商廣告系列中使用的匹配鍵。 如果確實需要為組織選擇其他匹配鍵，也可以稍後在編輯組織](#edit-organization)工作流程中[執行此作。

![匹配鍵選擇步驟。](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

選擇最多五個您計劃使用的匹配鍵。 稍後，在設置連接時，您可以刪除不需要的匹配鍵，但不能添加新鍵。 為每個選取的符合鍵設定身分計數臨界值 （最小計數）。 在某些使用案例中，小於最小計數的相符金鑰將不會出現在身分劃分中。

Real-Time CDP Collaboration中可用的相符索引鍵可以是三種型別：

* 第一方人員ID
* 第一方裝置 ID
* 合作夥伴 ID

Real-Time CDP Collaboration第一版的可用比對索引鍵為：

* 已雜湊的電子郵件

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

準備就緒后，選擇 **[!UICONTROL 完整應用程式]** 以完成組織設置工作流程。

## 編輯組織 {#edit-organization}

初始設置組織后，您可以隨時編輯組織的某些方面和詳細資訊。 要编辑您的組織，**[!UICONTROL 請在我的組織]**&#x200B;視圖&#x200B;**[!UICONTROL 中選擇編輯]**。

![已反白編輯組織控制項。](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

此時，您可以更新組織名稱、說明、標誌和組織設定檔圖片。

![組織的可編輯選項。](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

您也可以更新您在組織上線時最初選取的相符金鑰，以及與相符金鑰對應的身分最低臨界值，以便在對象重疊和其他產品區域中顯示和使用。 在&#x200B;**[!UICONTROL 相符金鑰]**&#x200B;索引標籤中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以新增任何其他所需的相符金鑰或更新身分識別臨界值。

![編輯匹配鍵](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 後續步驟

在設定組織後，您就可以[將對象](/help/guide/setup/onboard-audiences.md)匯入Real-Time CDP Collaboration。
