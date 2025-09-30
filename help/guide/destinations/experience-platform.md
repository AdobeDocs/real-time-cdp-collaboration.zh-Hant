---
title: 將Adobe Experience Platform設定為目的地
description: 瞭解如何在Real-Time CDP Collaboration中設定及管理Adobe Experience Platform作為目的地。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 11%

---

# 將Adobe Experience Platform設定為目的地

{{limited-availability-release-note}}

設定此目的地以將對象從您的專案啟動至Adobe Experience Platform。 在Adobe Experience Platform中啟用對象可讓您善用平台的功能，以便在各種行銷管道中進行對象細分、分析和啟用。 若要進一步瞭解Adobe Experience Platform，請參閱[Experience Platform概觀](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/home){target="_blank"}。

>[!WARNING]
>
>目的地建立後就無法更新。 如果您需要變更任何設定，必須刪除現有目的地並建立新目的地。

## 設定目的地 {#configure-destination}

若要將Adobe Experience Platform設定為目的地，請導覽至「**[!UICONTROL 設定]**」，然後選取「**[!UICONTROL 我的目的地]**」標籤。 選取Adobe Experience Platform的&#x200B;**[!UICONTROL 設定]**。

![針對Adobe Experience Platform目的地反白顯示「我的目的地」工作區與「設定」選項。](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

**[!UICONTROL 建立目的地]**&#x200B;工作流程隨即顯示。

![為Adobe Experience Platform建立目的地工作流程。](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### 設定沙箱 {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="客群期限"
>abstract="過了此時段以後，Adobe Experience Platform 將無法再使用該客群。預設期限為 30 天，但您可以將期限設定為 1 到 30 天之間的任何值。"

首先，您必須選取將傳送對象資料的沙箱。

>[!IMPORTANT]
>
>您只能選取您的使用者有權存取的沙箱。 依預設，所有Collaboration使用者都可存取&#x200B;**Prod**&#x200B;沙箱。 若要存取其他沙箱，管理員必須將其他沙箱新增到指派給您的使用者的角色。 如需有關管理角色的詳細資訊，請參閱[管理角色](../permissions/manage-roles.md)指南。

在&#x200B;**[!UICONTROL 設定沙箱]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 沙箱]**&#x200B;下拉式清單，或輸入沙箱的名稱。

![建立目的地工作流程中反白顯示的沙箱下拉式清單。](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

或者，您可以選取&#x200B;**[!UICONTROL 瀏覽沙箱]**&#x200B;以檢視所有可用的沙箱，以及它們的&#x200B;**[!UICONTROL 型別]**、**[!UICONTROL 狀態]**&#x200B;和&#x200B;**[!UICONTROL 地區]**。 選取您要使用的沙箱，然後選取[儲存]。**&#x200B;**

接下來，設定&#x200B;**[!UICONTROL 對象有效期]**。 依預設，對象到期日設為30天。 您可以選擇將有效期設定為1到30天。 到期日後，Adobe Experience Platform中將不再提供對象。

![建立目的地工作流程中強調的「對象有效期」區段。](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### 建立啟用對應 {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="啟用比對索引鍵"
>abstract="啟用比對索引鍵根據您在建立組織時選取的比對索引鍵顯示。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_mapping"
>title="閱讀全文"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="目標命名空間"
>abstract="目標命名空間指定在 Adobe Experience Platform 中比對索引鍵將對應到的身分識別命名空間。雜湊比對索引鍵必須對應到支援雜湊值的目標命名空間。"

根據預設，為您的帳戶啟用的所有相符金鑰都會包含在啟用對應中。 如果您不想將比對索引鍵直接對應到目標名稱空間，可以使用連結索引鍵選項將其替換為不同的比對索引鍵。 如需連結金鑰的詳細資訊，請參閱下方的[區段](#linked-keys)。

#### 對應目標名稱空間 {#map-target-namespaces}

若要將每個比對索引鍵對應到目標名稱空間，請選取比對索引鍵旁邊的&#x200B;**[!UICONTROL 目標名稱空間]**&#x200B;欄位。 **[!UICONTROL 選取來源欄位]**&#x200B;對話方塊就會顯示。 在清單中尋找目標名稱空間，或搜尋特定名稱空間。 選取您要用於比對索引鍵的目標名稱空間，然後選取&#x200B;**[!UICONTROL 選取]**。

>[!IMPORTANT]
>
>雜湊比對索引鍵必須對應至支援雜湊值的目標名稱空間。 例如，**[!UICONTROL 雜湊電子郵件]**&#x200B;相符金鑰必須對應至Adobe Experience Platform中的&#x200B;**[!UICONTROL 電子郵件（SHA256，小寫）]**&#x200B;身分名稱空間。 您無法將&#x200B;**[!UICONTROL 雜湊電子郵件]**&#x200B;相符金鑰對應至&#x200B;**[!UICONTROL 電子郵件]**&#x200B;身分名稱空間，因為此名稱空間不支援雜湊值。

![選取來源欄位對話方塊中反白了選取選項……](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

對您要包含在啟動對應中的每個比對金鑰重複此程式。 如果您不想加入比對索引鍵，可以將其移除，或使用連結索引鍵選項將其取代為不同的比對索引鍵。

#### 連結索引鍵 {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="連結索引鍵"
>abstract="連結索引鍵可讓您指定在啟用期間應使用不同的比對索引鍵代替原始比對索引鍵。要啟用輪廓，它必須同時具有原始比對索引鍵和連結索引鍵的值。"

連結索引鍵可讓您指定在啟用期間應使用不同的比對索引鍵代替原始比對索引鍵。若要深入瞭解連結索引鍵的運作方式，請考量下列範例：

retailer希望將正在啟用至Experience Platform的資料傳送至其CRM系統。 retailer已啟用雜湊IP作為其帳戶的比對索引鍵，以便在啟用受眾時提高比對率。 不過，retailer的CRM系統不支援以雜湊IP作為身分名稱空間，因此他們想要在啟用對象至Experience Platform時改用CRM ID比對索引鍵。 retailer可以使用連結索引鍵選項，透過CRM ID （而非雜湊IP）啟用對象至Experience Platform。

>[!NOTE]
>
>對於要啟用的設定檔，它必須有原始比對索引鍵和連結比對索引鍵的值。 例如，如果雜湊ID連結至CRM ID，則設定檔必須同時具有雜湊ID和CRM ID的值才能啟用。 如果缺少任一值，則不會啟用設定檔。

若要使用連結的索引鍵，請切換您要用來取代的相符索引鍵旁的&#x200B;**[!UICONTROL 連結的索引鍵]**&#x200B;選項。 **[!UICONTROL 連結的索引鍵]**&#x200B;區段會出現，要求您建立對應。

![建立目的地工作流程中反白顯示的連結索引鍵選項和區段。](/help/assets/destinations/adobe-experience-platform/linked-key.png)

從下拉式選單中選取您要使用的&#x200B;**[!UICONTROL 連結索引鍵]**。 依照上述範例，retailer會選取&#x200B;**[!UICONTROL CRM ID]**&#x200B;作為連結索引鍵。

![建立目的地工作流程中反白顯示的連結索引鍵下拉式清單。](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

接下來，如果您尚未指定連結索引鍵的目標名稱空間，請務必指定。 如果您已在&#x200B;**[!UICONTROL 建立啟動對應]**&#x200B;區段中選取相符金鑰的目標名稱空間，此專案將會自動填入。 如果您尚未選取連結索引鍵的目標名稱空間，現在可以選取。

選取連結索引鍵旁的&#x200B;**[!UICONTROL 目標名稱空間]**&#x200B;欄位。 **[!UICONTROL 選取來源欄位]**&#x200B;對話方塊就會顯示。 在清單中尋找目標名稱空間，或搜尋特定名稱空間。 選取您要用於連結金鑰的目標名稱空間，然後選取&#x200B;**[!UICONTROL 選取]**。

![選取來源欄位對話方塊。](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

連結的金鑰現在已設定完畢。

>[!NOTE]
>
>每個啟用對應只能使用一個連結金鑰目標名稱空間。 例如，如果您將雜湊ID連結至CRM ID，則切換其他欄位的連結鍵選項時，也會將其連結至CRM ID。

當您完成對應所有相符金鑰時，請檢閱您的設定。 **[!UICONTROL 預覽]**&#x200B;區段提供您設定的摘要。

![建立目的地工作流程中的預覽區段。](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>目前，每個相符索引鍵都會當作個別對象啟用至Experience Platform。 例如，如果您有[!UICONTROL 雜湊電子郵件]和[!UICONTROL 雜湊電話]做為相符金鑰，則啟用對象時，將會在對象入口網站中建立兩個個別的對象。

當您對組態感到滿意時，請選取&#x200B;**[!UICONTROL 建立目的地]**。 系統會顯示一則確認訊息，指出已成功建立目的地。

## 使用Adobe Experience Platform作為目的地

一旦您將Experience Platform設定為目的地，您就可以透過專案開始[啟用對象](../collaborate/activate.md)至平台。 目前，啟用程式是由共同作業人員起始的單一步驟程式。 例如，當廣告商啟用受眾時，會傳送至發佈者預先設定的目的地(Experience Platform)。 發佈者不需要採取任何額外的步驟，即可將對象傳送至目的地。 品牌對品牌的協同合作模式也是如此。

>[!IMPORTANT]
>
>您&#x200B;**必須**&#x200B;將Experience Platform設定為目的地&#x200B;*，然後*&#x200B;您的共同作業人員才能啟用對象。 如果未設定目的地，系統會將對象傳送給您，並顯示在專案的「**[!UICONTROL 啟用]**」標籤中，但不會啟用至Experience Platform。

對象啟動後，即可在Experience Platform的[對象入口網站](#audience-portal)中使用，其來源為Real-Time CDP Collaboration。  這些對象隨後可用於行銷活動和客戶參與。

### Audience Portal {#audience-portal}

現在您已將Adobe Experience Platform設定為目的地，可以在對象入口網站中檢視啟用的對象。 Audience Portal是Adobe Experience Platform的中央樞紐，可讓您檢視和管理您的對象。 對象入口網站現在會在篩選對象時，提供Real-Time CDP Collaboration作為來源。

>[!IMPORTANT]
>
>您有責任將任何必要的資料使用標籤套用至您在Adobe Experience Platform中啟用的對象。 如需詳細資訊，請參閱[資料使用標籤](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-governance/labels/overview){target="_blank"}指南。

![在篩選選項中將Real-Time CDP Collaboration作為來源的受眾入口網站。](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

若要深入瞭解對象入口網站，請參閱[對象入口網站概觀](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"}指南。
