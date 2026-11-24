---
title: RMN的虛擬對象存取（對象授權） - Beta
description: 瞭解如何在Real-Time CDP Collaboration中共用虛擬對象、尋找與您共用的對象，以及管理許可權、存取持續時間和撤銷。
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 1%
---
# RMN的虛擬對象存取（對象授權） {#virtual-audience-access}

若要與連線的合作夥伴共用對象，請在[!DNL Adobe Real-Time CDP Collaboration]中使用虛擬對象存取。 對象授權可讓合作夥伴透過持續參照存取完整對象族群。 您會保留所有權，且在授予存取權時不會移動任何對象資料。

若要使用共用對象，請在詳細目錄中尋找虛擬對象。 在授予許可權內使用對象進行啟用或建立同類群組對象。 例如，零售媒體網路(RMN)可以授予廣告商存取權，以建立及啟用同類群組對象。

## 對象存取概念 {#audience-access-concepts}

若要瞭解您共用的內容以及合作夥伴如何使用對象，請檢閱下列詞語。

| 術語 | 說明 |
| --- | --- |
| 提供者 | 擁有對象並控制存取權的組織。 |
| 收件者 | 接收對象存取權的已連線合作夥伴。 |
| 授予 | 存取共用對象，包括許可的使用和存取持續時間。 |
| 虛擬對象 | 對提供者擁有之對象的持續參考，可在收件者詳細目錄中取得。 |
| 完整母體 | 共用，可授予整個對象母體的存取權。 |
| 連線範圍 | 適用於提供者和收件者之間連線的存取權，而非單一專案。 |

{style="table-layout:auto"}

若要啟用共用的對象，您需要直接啟用許可權。

虛擬對象存取適用於連線。 在專案中共用是單獨的工作流程，不會將虛擬對象新增到收件者詳細目錄。

若要透過現有的共同作業專案啟用對象，請參閱[在專案中傳送及啟用對象](/help/guide/collaborate/activate.md)。

## 先決條件 {#prerequisites}

在您授與或使用虛擬對象存取權之前，請確認您符合下列需求。

* 針對虛擬對象授權，建立與共同作業人員](/help/guide/connect/establishing-connections.md)之間的使用中[連線。
* 如果您提供對象，請確認該對象可供共用。
* 若要確認哪些動作可用，請檢閱與您共用的對象授予許可權。

**[!UICONTROL 共用對象]**&#x200B;對話方塊會顯示下列許可權。 這兩個許可權都已選取且無法編輯。

| 對象許可權 | 允許使用 |
| --- | --- |
| 直接啟用 | 對象符合啟用需求時，在沒有專案的情況下啟用共用對象至目的地。 |
| [!UICONTROL 建立新對象] | 建立受眾時，請使用共用受眾作為輸入。 |

{style="table-layout:auto"}

## 共用對象 {#share-an-audience}

若要將存取權授與連線合作夥伴給選取的對象，請授與完整母體的存取權，並設定允許的使用和持續時間。 授與存取權不會啟用對象。

首先，開啟&#x200B;**[!UICONTROL 連線]**&#x200B;工作區與收件者連線。

![連線工作區中的提供者連線概觀。](../../assets/setup/virtual-audience-access/connection-overview.png)

接著，選取「**[!UICONTROL 對象存取]**」，然後選擇您與合作夥伴共用的對象選項。

選項包含合作夥伴名稱。 在此範例中，選取&#x200B;**[!UICONTROL FrameSix Media]**。

![「對象存取」索引標籤會顯示已選取的FrameSix媒體以及「授與存取權」選項。](../../assets/setup/virtual-audience-access/grant-access.png)

然後，選取&#x200B;**[!UICONTROL 授與存取權]**&#x200B;以開啟&#x200B;**[!UICONTROL 共用對象]**&#x200B;對話方塊。

在&#x200B;**[!UICONTROL 對象]**&#x200B;中，從&#x200B;**[!UICONTROL Select對象]**&#x200B;中選擇對象，或選取&#x200B;**[!UICONTROL 瀏覽對象]**。

選取的對象會顯示在對話方塊中。 您的組織保留對象的所有權和管理。

在「共用對象」對話方塊中![Select或瀏覽對象。](../../assets/setup/virtual-audience-access/share-audiences-selection.png)

接下來，檢閱&#x200B;**[!UICONTROL 許可權]**&#x200B;中顯示的許可權。 直接啟用許可權可讓合作夥伴將虛擬對象啟用到自己的目的地。 **[!UICONTROL 建立新對象]**&#x200B;可讓合作夥伴使用虛擬對象來建立新對象。 這兩個許可權都已選取且無法編輯。

![在[共用對象]對話方塊中檢閱許可權。](../../assets/setup/virtual-audience-access/share-audiences-permission.png)

然後，從&#x200B;**[!UICONTROL 存取持續時間]**&#x200B;內的&#x200B;**[!UICONTROL 持續時間]**&#x200B;中選擇一個選項，以設定合作夥伴的存取時間。 Select **[!UICONTROL 一律]**&#x200B;無到期日存取，或指定時間限制存取的日期。

![「共用對象」對話方塊會顯示選取的對象、選取的許可權，以及「持續時間」設定為「一律」。](../../assets/setup/virtual-audience-access/share-audiences-duration.png)

最後，檢閱選取的對象、許可權和存取持續時間，然後選取&#x200B;**[!UICONTROL 授與存取權]**。

**[!UICONTROL 對象存取]**&#x200B;索引標籤會列出共用對象及其狀態、身分計數、存取持續時間、許可權和說明。

![「對象存取」索引標籤會列出兩個共用對象，其狀態為「作用中」、「一律存取」及其許可權。](../../assets/setup/virtual-audience-access/shared-audiences.png)

共用對象也會在收件者詳細目錄中顯示為虛擬參考。 您保留擁有權。 如果授權允許，收件者可以個別啟用對象。

## 尋找及使用共用對象 {#find-and-use-shared-audiences}

以收件者身分，在提供者連線的&#x200B;**[!UICONTROL 對象存取]**&#x200B;索引標籤中尋找共用對象。 使用授予許可權內的每個對象。

### 尋找共用對象 {#find-shared-audiences}

若要尋找由提供者共用的對象並檢閱其存取詳細資訊，請開啟提供者連線。 首先，開啟&#x200B;**[!UICONTROL Connect]**&#x200B;工作區與提供者連線。

接著，選取&#x200B;**[!UICONTROL 對象存取]**，然後選擇提供者所共用的對象選項。

選項包含提供者名稱。 在此範例中，從FrameSix Media ]**選取**[!UICONTROL 。

最後，檢閱共用對象及其存取詳細資訊。

![「對象存取」索引標籤會顯示由FrameSix Media共用的對象。 此表格列出其狀態、存取持續期間和許可權。](/help/assets/setup/virtual-audience-access/virtual-audience-access-shared-with-me.png)

### 建立客群 {#build-audiences}

若要從共用對象建立對象，您需要&#x200B;**[!UICONTROL 建立新對象]**&#x200B;許可權。 例如，將共用的對象與您自己的對象結合，以建立新對象。

新對象屬於您。 提供者保留來源對象的所有權。

### 啟用共用受眾 {#activate-shared-audiences}

若要直接啟用虛擬對象，請確認授與符合這些條件。

| 需求 | 條件 |
| --- | --- |
| 共用型別 | 完整母體 |
| 對象許可權 | 您具有對象的直接啟用許可權。 |
| 授予狀態 | 作用中。 存取權不限期，或在指定的日期範圍內。 |

{style="table-layout:auto"}

若要將符合資格的對象傳送到目的地，請使用&#x200B;**[!UICONTROL 啟用]**&#x200B;頁面。 您不需要專案。

如需詳細資訊，請參閱[直接啟用對象(Beta)](/help/guide/destinations/direct-audience-activation.md)。

如果對象不符合需求，您就無法選取對象來直接啟用。 Collaboration會在每次排程的啟用回合中再次檢查適用性。

## 管理對象存取權 {#manage-audience-access}

身為提供者，您可以控制存取持續的時間。 只有您可以變更授權到期日或撤銷存取權。

### 存取期間 {#access-duration}

建立授權時，請選擇存取持續時間。

| 持續時間 | 行為 |
| --- | --- |
| [!UICONTROL 一律] | 存取權沒有自動到期日。 您可以撤銷授權。 |
| 日期範圍 | 存取權會持續指定的日期範圍。 Collaboration會每小時處理過期時間。 |

{style="table-layout:auto"}

若要延長存取權，請設定未來的到期日，或將持續時間變更為無限期存取。 任一變更也會重新啟用過期的授權。

### 存取權到期 {#access-expiration}

Collaboration會每小時檢查過期授權。 當Collaboration將授權標籤為過期時，收件者會失去對受眾的虛擬存取權。

### 撤銷存取權 {#revoke-access}

若要立即移除虛擬存取權，請撤銷作用中或過期的授權。

![「撤銷存取權」對話方塊會警告協力電腦將無法存取共用的對象。 已反白顯示[撤銷存取權]選項。](/help/assets/setup/virtual-audience-access/revoke-virtual-access.png)

## 後續步驟 {#next-steps}

在您授與或接收對象存取權後，請使用下列指南來準備啟動或管理共同作業人員連線。

* [設定和管理目的地](/help/guide/destinations/manage-destinations.md)
* [管理共同作業人員連線](/help/guide/connect/manage-connections.md)
