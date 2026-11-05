---
title: 設定及管理身分解析
description: 瞭解如何在Real-Time CDP Collaboration中設定和管理身分解析。
audience: admin, publisher, advertiser, agency
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
source-git-commit: ff233017fb78a63b2e911dc0dc94d67f2b18af04
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 2%
---
# 設定及管理身分解析

{{limited-availability-release-note}}

身分解析可協助您識別與共同作業人員共用的客戶，即使您的組織使用不同的識別碼亦然。 透過Real-Time CDP Collaboration中支援的身分提供者來設定和管理身分解析，無需為每個合作夥伴建立自訂整合。

>[!NOTE]
>
>本指南中的步驟和熒幕擷取畫面以[!DNL Epsilon Core ID]為例。 需求和可用選項可能會因您的身分提供者而異。

>[!AVAILABILITY]
>
>啟動時，只有[!DNL Epsilon Core ID]可供設定。 Epsilon核心ID身分解析僅適用於美國布建的Real-Time CDP Collaboration帳戶。

## 先決條件 {#prerequisites}

開始之前，請確定您擁有：

* **帳戶管理許可權。** 您必須擁有&#x200B;**[!UICONTROL 管理帳戶]**&#x200B;和&#x200B;**[!UICONTROL 管理Collaboration執行個體]**&#x200B;許可權。
* **至少一個對象資料連線。** 您需要現有的對象資料連線才能設定身分解析。 [視需要設定對象來源](./source-overview.md)。 不支援測量資料連線。
* **支援的相符金鑰和欄位。** 您打算用於身分解析的每個對象資料連線都必須包含身分提供者支援的欄位。 若為Epsilon Core ID，您可以使用雜湊電子郵件、雜湊電話或結合郵寄地址的名稱。

  您必須為帳戶啟用帳戶層級的比對索引鍵（例如雜湊電子郵件和雜湊電話），並對應至您的對象資料。 名稱和郵寄位址列位會在設定對象資料連線期間對應，不需要帳戶層級的啟用。

  如果使用名稱和郵寄地址，請對應每個群組中的至少一個欄位：

  * **名稱：**&#x200B;名字、姓氏或全名。
  * **郵寄地址：**&#x200B;街道地址、城市、郵遞區號、州或國家/地區。

  名稱和郵寄地址值未進行雜湊處理。 如需啟用帳戶層級比對金鑰的說明，例如雜湊電子郵件和雜湊電話，請參閱[編輯比對金鑰](./onboard-account.md#edit-match-keys)。 若要將支援的相符金鑰或名稱和郵寄位址列位對應到您的對象資料，請參閱[對應欄位](./onboard-audiences.md#map-fields)。
* **Epsilon帳號。** 請向您的Epsilon帳戶代表取得您的Epsilon帳戶號碼。

## 設定身分解析 {#configure-identity-resolution}

選取識別提供者，以開始設定識別解析。 在此[!DNL Epsilon Core ID]範例中，您會在確認前，先向提供者進行驗證、選取對象資料連線、設定日期範圍並檢閱設定。

若要開始，請在左側導覽中選取&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 身分解析]**&#x200B;標籤，以檢視可用的身分提供者。

### 選取身分提供者 {#select-identity-provider}

找出身分提供者的卡片，並檢閱其支援的區域及比對金鑰。 選取&#x200B;**[!UICONTROL 安裝程式]**&#x200B;以開始。

![包含Epsilon核心ID卡及其安裝動作的識別提供者目錄。](../../assets/setup/identity-resolution/select-an-identity-provider.png){zoomable="yes"}

在啟動設定工作流程之前，Collaboration會檢查資料連線和相容的相符索引鍵。 如果缺少需求，會出現一個對話方塊來指導流程。 請依照對話方塊中的動作操作：

* **[!UICONTROL 需要資料連線]：**&#x200B;選取&#x200B;**[!UICONTROL 設定資料連線]**&#x200B;以設定對象資料連線。 請參閱[連線來源](./source-overview.md#connect-a-source)。
* **[!UICONTROL 需要比對金鑰]：**&#x200B;選取&#x200B;**[!UICONTROL 編輯比對金鑰]**&#x200B;以啟用支援的金鑰。 請參閱[編輯相符金鑰](./onboard-account.md#edit-match-keys)。

如果兩者都遺失，資料連線對話方塊會先出現。 修正先決條件後，請返回&#x200B;**[!UICONTROL 身分解析度]**，然後再次選取&#x200B;**[!UICONTROL 安裝程式]**。

### 向您的身分提供者進行驗證 {#authenticate-with-provider}

在&#x200B;**[!UICONTROL 驗證]**&#x200B;步驟中，提供您的身分提供者所需的資訊。 對於Epsilon核心ID，請在&#x200B;**[!UICONTROL Epsilon帳號]**&#x200B;欄位中輸入您的Epsilon代表所提供的帳號。 選取&#x200B;**[!UICONTROL 「下一步」]**&#x200B;以繼續。

![顯示Epsilon帳號欄位的驗證步驟。](../../assets/setup/identity-resolution/authenticate.png){zoomable="yes"}

### 選取資料連線 {#select-data-connections}

接著，選擇您要用於身分解析的對象資料連線。 這會決定要將哪些受眾資料用於比對您的客戶身分與身分提供者。 身分解析會自動使用每個所選連線中對應的支援識別碼。
接著，選擇您要用於身分解析的對象資料連線。 選取的連線會決定哪些對象資料和對應的欄位可用於身分解析。

身分解析會套用至每個選取的資料連線中的所有對象，包括稍後新增的任何對象。 您目前無法選取個別對象。

如果未列出您想要的連線，[請先設定對象資料連線](./source-overview.md)，然後再繼續。

在&#x200B;**[!UICONTROL 資料來源]**&#x200B;底下，選取您要包含在&#x200B;**[!UICONTROL 對象來源]**&#x200B;中的每個連線核取方塊。 您必須至少選取一個連線。 選取&#x200B;**[!UICONTROL 「下一步」]**&#x200B;以繼續。

![顯示已選取和未選取資料連線的對象來源卡片。](../../assets/setup/identity-resolution/source-selection.png){zoomable="yes"}

### 設定身分解析排程 {#set-schedule}

選擇開始和結束日期，以定義Adobe重新整理合作夥伴ID的期間。 重新整理頻率是由選取的對象資料連線所決定，因此您無法針對身分解析設定個別的重新整理頻率。

在&#x200B;**[!UICONTROL 排程]**&#x200B;步驟中，選取&#x200B;**[!UICONTROL 日期範圍]**&#x200B;下的行事曆控制項，然後選擇您的日期。 選取&#x200B;**[!UICONTROL 「下一步」]**&#x200B;以繼續。

![使用Epsilon核心ID識別解析的日期範圍排程步驟。](../../assets/setup/identity-resolution/schedule-identity-resolution-job.png){zoomable="yes"}

### 檢閱並確認設定 {#review-and-confirm}

在&#x200B;**[!UICONTROL 檢閱]**&#x200B;步驟中，檢查您的驗證詳細資料、選取的對象資料連線和排程。 若要進行變更，請選取相關區段旁的&#x200B;**[!UICONTROL 編輯]**。

安裝後無法編輯設定。 若要稍後進行變更，您必須將其刪除並重新設定。 在您滿意您的選擇後，請選取&#x200B;**[!UICONTROL 確認並排程]**。

![檢閱步驟，顯示驗證、資料來源及排程摘要。](../../assets/setup/identity-resolution/review-and-confirm.png){zoomable="yes"}

確認對話方塊表示已成功設定身分解析。

<!-- [Question: Does the first identity resolution run happen immediately after setup, or at the next scheduled audience data connection refresh?] -->

## 管理身分解析 {#manage-identity-resolution}

確認您的設定後，您會自動返回&#x200B;**[!UICONTROL 身分解析]**&#x200B;標籤，您可以在其中檢視或刪除您的設定。

### 檢視設定詳細資料 {#view-configuration-details}

若要檢閱您的設定，請選取您設定的身分提供者卡片上的&#x200B;**[!UICONTROL 檢視詳細資料]**。

檢閱驗證詳細資料、選取的對象資料連線和日期範圍。 您還可以檢視組態詳細資訊中顯示的相符金鑰，以及組態狀態以及建立和更新資訊。

![身分解析設定詳細資訊，顯示狀態、比對金鑰、排程和相關聯的對象連線。](../../assets/setup/identity-resolution/view-connection-details.png){zoomable="yes"}

### 變更現有設定 {#edit-configuration}

設定後，您無法編輯核心ID設定。 若要變更Epsilon帳號、選取的資料連線或日期範圍，請[刪除組態](#delete-configuration)，然後再次完成[安裝工作流程](#configure-identity-resolution)。

<!-- Question: Do other providers have the same limitation? -->

### 刪除身分解析設定 {#delete-configuration}

若要刪除設定，請瀏覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 身分解析]**，並在您設定的身分提供者卡上選取&#x200B;**[!UICONTROL 刪除]**。 檢閱確認對話方塊，然後選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以進行確認。

如果您想要再次使用此身分提供者，您需要[設定新的組態](#configure-identity-resolution)。

<!-- [UNVERIFIED: Does deletion affect previously resolved identifiers, future processing, or both? Confirm before publication.] -->

## 疑難排解設定問題 {#troubleshoot}

如果因為缺少資料連線或比對金鑰而無法開始安裝，請依照[選取識別提供者](#select-identity-provider)下的指示進行。

對於Epsilon核心ID，請檢查下列專案：

* **在您的地區無法使用：** Epsilon核心ID僅適用於在美國布建的Collaboration帳戶。
* **Epsilon帳號無法使用：**&#x200B;請連絡您的Epsilon代表以取得您的帳號。
