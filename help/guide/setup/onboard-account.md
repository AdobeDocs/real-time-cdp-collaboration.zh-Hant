---
title: 設定和管理您的帳戶
description: 瞭解如何在Real-Time CDP Collaboration中設定和管理帳戶的各種層面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 18%

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
<!-- The above will need to be updated when I update things for B2B -->
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
>abstract="比對索引鍵是用於調和來自不同資料來源之客群成員的識別碼。包括您的品牌可以使用的任何比對索引鍵。"

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
>您在帳戶設定期間選取的相符金鑰將決定您與其他共同作業人員建立的連線可用的相符金鑰。 雖然您可以在連線設定期間移除相符金鑰，但無法新增相符金鑰。 在帳戶設定期間，請務必選取您計畫用於未來促銷活動的&#x200B;**所有**&#x200B;相符金鑰。

匹配索引鍵（例如電子郵件地址、裝置ID或客戶ID），可讓共同作業人員透過啟用精確且以隱私權為中心的資料同步化來合作，進而實現更精確的對象鎖定目標和測量。

![投影片顯示Collaboration第一版的可用識別碼。](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

選取您要在協調對象設定檔時使用的任何比對索引鍵。 包含您可以使用的任何相符索引鍵。 規劃未來，並選取您預計將在未來行銷活動中使用的相符索引鍵。 如果您稍後確實需要為您的帳戶選取其他相符金鑰，您可以在[編輯帳戶](#edit-account)工作流程中進行。

最多選取五個您計畫使用的相符金鑰。 稍後，在設定連線時，您可以移除不需要的相符金鑰，但無法新增金鑰。

可用的比對索引鍵型別有三種：

* 第一方人員 ID
* 第一方裝置 ID
* 合作夥伴 ID

>[!IMPORTANT]
>
>目前唯一支援的相符金鑰是雜湊電子郵件。

準備就緒後，選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成組織設定工作流程。

![顯示[設定組織]工作區的[比對索引鍵]區段。](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 編輯帳戶 {#edit-account}

設定帳戶後，您可以隨時編輯帳戶的某些方面和詳細資訊。 若要編輯您的帳戶，請在&#x200B;**[!UICONTROL 設定]**&#x200B;工作區&#x200B;**[!UICONTROL 的]**&#x200B;我的帳戶&#x200B;**[!UICONTROL 區段中選取]編輯**。

![反白顯示[我的帳戶]索引標籤和[編輯]選項的[設定]工作區。](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

您現在可以編輯帳戶詳細資料，但&#x200B;**[!UICONTROL 角色]**&#x200B;除外。 請注意，地區是根據您的Adobe Experience Cloud帳戶自動設定，且無法隨時變更。

![編輯帳戶詳細資料對話方塊。](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

您也可以更新您在加入組織時最初選取的相符金鑰。 在&#x200B;**[!UICONTROL 相符金鑰]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以新增任何其他所需的相符金鑰。

![在帳戶的「比對金鑰」區段中，以「編輯」選項醒目提示的「設定」工作區。](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## 後續步驟

設定帳戶之後，您就可以將[來源對象](/help/guide/setup/onboard-audiences.md)放入Real-Time CDP Collaboration了。
