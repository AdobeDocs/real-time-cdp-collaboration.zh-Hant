---
title: 匯入和管理對象
description: 瞭解如何在Adobe Real-Time CDP Collaboration中匯入和管理對象
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '2961'
ht-degree: 18%

---

# 匯入和管理對象

{{limited-availability-release-note}}

受眾是根據各種屬性劃分的特定使用者或客戶群組。 這些功能可讓廣告商和發佈商在針對性行銷和個人化體驗上共同作業，以進行更有效率的廣告行銷活動。

使用此頁面作為切入點，瞭解您可以檢視的所有與對象相關的量度，以及將對象匯入Adobe Real-Time CDP Collaboration的工作流程步驟。

>[!TIP]
>
>使用此畫面中的資訊來取得有關您的對象的所有所需資訊，以及[探索和重疊畫面](/help/guide/collaborate/discover.md)來取得有關哪些對象最適合不同行銷活動型別的深入分析（與發佈者詳細目錄相比）。

>[!BEGINSHADEBOX]

您可在此檔案頁面上找到以下內容：

* [將受眾匯入Real-Time CDP Collaboration](#import-audiences)
* [檢視客群儀表板](#view-audiences-dashboard)
* [檢視個別對象](#view-individual-audiences)

>[!ENDSHADEBOX]

## 將受眾匯入Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>若要匯入對象，必須將您的使用者指派給包含兩個設定檔管理許可權的角色：檢視設定檔和檢視區段。 如需指派必要許可權的相關資訊，請參閱[對象匯入](../permissions/overview.md#audience-importation)指南。

您必須先將受眾匯入Real-Time CDP Collaboration，才能透過共同作業人員啟用受眾及執行重疊計算。 若要匯入對象，請依照下節中的工作流程步驟操作。

從&#x200B;**[!UICONTROL 步驟]**&#x200B;工作區內的&#x200B;**[!UICONTROL 我的對象]**&#x200B;索引標籤中，選取新增圖示(![新增圖示。](/help/assets/icons/plus.png))或&#x200B;**[!UICONTROL 新增]選項**，然後選取&#x200B;**對象**。

![我的受眾工作區，其中的[新增]選項和[受眾]選項已反白顯示。](/help/assets/setup/add-manage-audiences/add-audiences.png)

### 選取資料連線 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="行銷動作"
>abstract="<p>使用行銷動作來控制要從 Experience Platform 匯入哪一些客群資料到 Real-Time CDP Collaboration。<strong>資料共同作業</strong>行銷動作支援 C4、C5 和 C9 資料使用情況標籤。<strong>資料科學</strong>行銷動作支援 C9 資料使用情況標籤。</p> <p> <ul><li> 核取方塊<em>啟用</em>後，Experience Platform 中標有上述標籤的任何資料都將被排除，並且<strong>不會</strong>帶入 Real-Time CDP Collaboration 中。</li><li> 核取方塊<em>停用</em>後，可以從 Experience Platform 匯入 Real-Time CDP Collaboration 的資料沒有任何限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hant" text="資料使用標籤概觀"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=zh-Hant" text="資料使用標籤字彙表"

>[!IMPORTANT]
>
>在建立至您的第一個資料連線並匯入第一個對象後，您就可以從現有的資料連線匯入多個對象。 新增其他對象時，您將會從[選取對象](#select-audience)步驟開始，因為其他步驟的所有先決條件資訊都會從現有連線匯入。

資料連線是資料來源，您會將受眾匯入Real-Time CDP Collaboration。 目前唯一支援的資料連線是Adobe Experience Platform。

您為資料連線設定的任何設定（例如排程）都會套用至從此資料連線匯入的所有對象。

>[!TIP]
>
>有一個單獨的工作流程，您可以在其中檢視和編輯資料連線。 如需詳細資訊，請參閱[管理資料連線](/help/guide/setup/manage-data-connection.md)指南。

若要開始新增您的資料連線，請選取&#x200B;**[!UICONTROL 新增新的資料連線]**，然後選取&#x200B;**[!UICONTROL 下一步]**。

![反白顯示[新增資料連線]選項的[新增對象]工作區。](/help/assets/setup/add-manage-audiences/add-data-connection.png)

#### 選取資料來源

接下來，您將選擇資料連線的來源。 可用的來源包括：

* **Adobe Experience Platform**：選取此選項，即可從Adobe Experience Platform Real-Time CDP引進您的對象。
* **CSV檔案** （未來版本）：上傳包含您對象資料的CSV檔案，以快速且直接地擷取資料。
* **Amazon Web Services** （未來版本）：連線至您的Amazon S3儲存體，直接從S3儲存貯體匯入對象資料。
* **Snowflake** （未來版本）：使用您的Snowflake資料倉儲，順暢地提取對象資料。

選取您的資料來源，然後選取&#x200B;**[!UICONTROL 下一步]**。

![反白顯示Adobe Experience Platform選項的「新增對象」工作區。](/help/assets/setup/add-manage-audiences/select-data-connection-source.png)

#### 選取沙箱

選取您的資料來源後，您必須選取包含您將匯入之對象的沙箱。 從可用沙箱清單中選取沙箱，然後選取&#x200B;**[!UICONTROL 下一步]**

![已選取沙箱的「新增對象」工作區。](/help/assets/setup/add-manage-audiences/select-sandbox.png)

#### 治理原則和執行動作 {#governance-policy-and-enforcement-actions}

接下來，您必須確定已針對匯入的資料設定正確的行銷動作。 從Real-Time CDP匯入的資料若要用於資料共同作業，您也必須提供同意。

使用行銷動作來控制要從 Experience Platform 匯入哪一些客群資料到 Real-Time CDP Collaboration。**資料共同作業**&#x200B;行銷動作支援 C4、C5 和 C9 資料使用情況標籤。**資料科學**&#x200B;行銷動作支援 C9 資料使用情況標籤。

深入瞭解[C4、C5和C9資料使用標籤](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}。

* 核取方塊&#x200B;*啟用*&#x200B;後，Experience Platform 中標有上述標籤的任何資料都將被排除，並且&#x200B;*不會*&#x200B;帶入 Real-Time CDP Collaboration 中。
* 核取方塊&#x200B;*停用*&#x200B;後，可以從 Experience Platform 匯入 Real-Time CDP Collaboration 的資料沒有任何限制。

在Experience Platform檔案中進一步瞭解資料使用標籤：

* [資料使用標籤概觀](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [資料使用標籤字彙表](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-governance/labels/reference){target="_blank"}

此外，您也會想要選取同意規則，以套用至匯入至Real-Time CDP Collaboration的資料。

![在治理原則與強制動作區段新增對象工作區。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

選取行銷動作和同意規則後，選取&#x200B;**[!UICONTROL 下一步]**&#x200B;以繼續執行下一個步驟。 將會出現確認對話方塊，要求您接受條款。 選取核取方塊，然後選取&#x200B;**[!UICONTROL 確定]**&#x200B;確認。

![以核取方塊和[確定]選項標示的[治理原則與強制執行]動作對話方塊。](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png)

### 提供詳細資料

接下來，為您的資料連線提供名稱和說明。 此資訊可協助您稍後識別資料連線。

![新增對象工作區可選擇提供名稱和說明。](/help/assets/setup/add-manage-audiences/data-connection-details.png)

### 對應欄位 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="來源欄位"
>abstract="來源欄位是來自您現有 Real-Time CDP 實施的身分識別命名空間和屬性。您可以將這些欄位對應到 Real-Time CDP Collaboration 中所定義的目標欄位。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目標欄位"
>abstract="目前，雜湊電子郵件是唯一支援的比對索引鍵。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="套用轉換"
>abstract="從來源匯入&#x200B;*非雜湊*&#x200B;欄位時，使用此選項讓 Real-Time CDP Collaboration 套用雜湊，並將純文字欄位轉換為雜湊欄位。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身分識別命名空間"
>abstract="從 Experience Platform 組織中可用的標準和自訂身分識別命名空間中，選取一個身分識別命名空間。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=zh-Hant#standard" text="Experience Platform 中的標準和身分識別命名空間"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="輪廓屬性"
>abstract="從聯集結構中選取 Experience Platform 輪廓類別屬性。此視圖會顯示存在於聯集結構中，且屬於 XDM 個體輪廓類別的屬性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html?lang=zh-Hant" text="Experience Platform 中的聯集結構"

接下來，您將選取來源欄位，以對應至Real-Time CDP Collaboration中的目標欄位。

![新增對象工作區，可選擇將來源欄位對應至目標欄位。](/help/assets/setup/add-manage-audiences/add-map-fields.png)

>[!TIP]
>
>您可以將多個來源欄位對應到相同的目標欄位。 例如，如果您在Experience Platform中的兩個個別欄位中有電子郵件地址，您可以將這兩個地址對應到&#x200B;**[!UICONTROL 雜湊電子郵件]**&#x200B;目標欄位，做為兩個個別的列。

>[!BEGINSHADEBOX]

**[!UICONTROL Source欄位]**&#x200B;是來自您現有Real-Time CDP實作的身分識別名稱空間和屬性。 這些是身分如何存在於您匯入資料的來源中。 Source欄位會對應至Real-Time CDP Collaboration中定義的目標欄位。

**[!UICONTROL 目標欄位]**&#x200B;指出在Real-Time CDP Collaboration中參照身分的方式。 目前，雜湊電子郵件是唯一支援的比對索引鍵。

當您從來源匯入&#x200B;*非雜湊*&#x200B;欄位時，請使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;選項。 在這種情況下，Real-Time CDP Collaboration將套用雜湊並轉換欄位。 Adobe使用的雜湊演演算法是SHA256。

>[!ENDSHADEBOX]

選取目標欄位旁邊的空白來源欄位。 **[!UICONTROL 選取來源欄位]**&#x200B;對話方塊將會出現。 在&#x200B;**[!UICONTROL 身分識別名稱空間]**&#x200B;和&#x200B;**[!UICONTROL 設定檔屬性]**&#x200B;選項之間選取，以尋找所需的來源欄位，然後從清單中選取來源欄位，使用搜尋選項來尋找所需的欄位。

![顯示電子郵件選項的[選取來源欄位]對話方塊。](/help/assets/setup/add-manage-audiences/select-source-field.png)

若要處理多個電子郵件欄位，請使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;來對應非雜湊電子郵件來源欄位。

![將電子郵件來源欄位對應到目標欄位的「新增對象」工作區中，已針對其中一個欄位開啟「套用」轉換。](/help/assets/setup/add-manage-audiences/apply-transformation.png)

視需要繼續新增對應配對，然後選取&#x200B;**[!UICONTROL 下一步]**。

### 排程 {#schedule}

接下來，排程何時開始和結束填入對象。 對象將根據此排程重新整理。

![顯示排程選項的新增對象工作區。](/help/assets/setup/add-manage-audiences/audience-scheduling.png)

>[!IMPORTANT]
>
>調整對象更新頻率有助於管理[對象管理信用活動](/help/guide/setup/my-activity.md#types-of-activities)，這是根據對象重新整理計算所得。 選取較高的頻率可能會影響資料的時效性，而資料可用於對象探索報表和對象啟動。

從&#x200B;**[!UICONTROL 頻率]**&#x200B;下拉式清單中選取對象重新整理的頻率。

![開啟[頻率]下拉式清單的[新增對象]排程工作區。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png)

接著，選取&#x200B;**[!UICONTROL 日期範圍]**。 開始日期是對象開始填入設定檔的日期，結束日期是對象停止重新整理的日期。

![顯示[日期範圍]選項的[新增對象]排程工作區。](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png)

>[!IMPORTANT]
>
>在日期範圍內的結束日期之後，從此資料連線匯入的所有對象將停止重新整理。 若要更新連線，請移至[管理資料連線](/help/guide/setup/manage-data-connection.md)，並設定新的結束日期。

### 選取客群 {#select-audience}

選取對象來源後，您將選擇要包含的特定對象。 使用搜尋和篩選選項，從您的資料來源尋找相關的對象。 選取您需要的對象，然後選取&#x200B;**[!UICONTROL 下一步]**。

![具有可用對象清單的新增對象工作區。](/help/assets/setup/add-manage-audiences/select-audience.png)

### 審核

在最終確定對象新增之前，請檢閱所有配置和設定。 請確定所有詳細資料均正確無誤，然後選取[完成] **&#x200B;**&#x200B;以完成資料連線的建立。

![顯示所有選取組態的新增對象工作區。](/help/assets/setup/add-manage-audiences/review-connection.png)

## 檢視客群儀表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身分識別"
>abstract="根據已設定的排程，身份識別計數將在下一次資料連線重新整理後可用。初始重新整理通常發生在設定資料連線後的 24 小時內。正在進行的重新整理將遵循已設定的排程。 "

將對象匯入Real-Time CDP Collaboration後，**[!UICONTROL 我的對象]**&#x200B;工作區會顯示您的組織目前匯入Real-Time CDP Collaboration的所有對象。


每個受眾都包含下列資訊的概觀：

| 項目 | 說明 |
|----------|---------|
| **[!UICONTROL 身分]** | 表示此對象中存在的身分數量。 請注意，如果相同設定檔有兩個或多個身分，而這些身分在專案中作為相符索引鍵使用，則設定檔會在計數中顯示兩次。 |
| **[!UICONTROL 狀態]** | 指出對象是否作用中以及是否可用於專案。 **[!UICONTROL 擱置中]**&#x200B;狀態表示對象最近剛匯入，且對象成員尚未填入。 匯入的對象會在初次重新整理後填入設定檔，這通常發生在資料連線設定後的24小時內。 |
| **[!UICONTROL Source]** | 指出從中匯入對象的來源。 在目前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支援的來源。 |
| **[!UICONTROL 資料連線]** | 受眾來源的資料連線。 您可以選取名稱以檢視資料連線。 |
| **[!UICONTROL 連線存取]** | 定義對象是私人或公開。 可在重疊報表中找到的公開對象，並可於專案中啟動。 |
| **[!UICONTROL 已建立]** | 指出將對象匯入Real-Time CDP Collaboration的時間。 |
| **[!UICONTROL 上次更新時間]** | 表示上次更新對象任何層面的日期和時間。 |

![「我的對象」工作區顯示所有已匯入的對象。](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

若要對對象執行快速動作，請選取對象名稱旁的省略符號&#x200B;**...**。 提供下列選項：

* **[!UICONTROL 編輯類別]**&#x200B;可讓您將不同的類別標籤新增至對象。 如需詳細資訊，請參閱下方的[類別](#categories)區段。
* **[!UICONTROL 刪除]**&#x200B;將會從資料連線中刪除對象。

![我的對象工作區中會開啟省略符號功能表，並反白顯示[編輯類別]和[刪除]選項。](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png)

## 檢視個別對象 {#view-individual-audiences}

若要檢視詳細資訊並編輯個別對象的設定，請從&#x200B;**[!UICONTROL 我的對象]**&#x200B;工作區中選取對象。 對象工作區會顯示所選對象的詳細資訊，包括其詳細資料、身分、類別、連線存取和中繼資料視覺效果設定。

### 客群詳細資料

系統會為每個個別對象顯示下列資訊：

| 項目 | 說明 |
|----------|---------|
| **[!UICONTROL 狀態]** | 指出對象是否作用中以及是否可用於專案。 |
| **[!UICONTROL Source]** | 指出從中匯入對象的來源。 在目前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支援的來源。 |
| **[!UICONTROL 資料連線]** | 受眾來源的資料連線。 |
| **[!UICONTROL 上次更新時間]** | 表示上次更新對象的日期和時間。 |
| **[!UICONTROL 上次更新者]** | 表示上次更新對象的使用者。 |
| **[!UICONTROL 已建立]** | 指出將對象匯入Real-Time CDP Collaboration的時間。 |
| **[!UICONTROL 建立者：]** | 表示將受眾匯入Real-Time CDP Collaboration的使用者。 |

![個別對象的工作區。](/help/assets/setup/add-manage-audiences/audience-details.png)

此外，受眾工作區中有以下控制項：

* **[!UICONTROL 刪除]**：從您的資料連線移除對象。
* **[!UICONTROL 編輯]**：編輯對象的名稱或描述。

![個別對象的工作區中，醒目提示「編輯與刪除」選項。](/help/assets/setup/add-manage-audiences/audience-details-edit-delete.png)

接下來，您可以在對象的工作區中更新下列區段：

* [身分識別](#identities)
* [類別](#categories)
* [連線存取權](#connection-access)
* [中繼資料可見度](#metadata-visibility)

### 身分識別 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身分識別"
>abstract="組成此對象的身分的劃分檢視，以及包含個別身分的設定檔總數。"

**[!UICONTROL 身分]**&#x200B;區段會指出在匯入對象時，具有您選取之任何身分的對象中呈現的個人檔案數。 區段也包含身分劃分，以便您分辨哪些身分構成最多受眾群體。

![個別對象工作區的「身分」區段。](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

### 類別 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="類別"
>abstract="標記您的客群，以便於組織、篩選和檢索。您可以使用多個類別標記客群，然後可以使用這些類別標記在產品的其他方面篩選所需的客群。"

為了輕鬆進行對象組織、篩選和擷取，您可以標籤對象。 您可以標籤具有多個類別的受眾，然後在執行受眾重疊報表時，可以使用這些類別標籤在[探索](/help/guide/collaborate/discover.md)產品區域中篩選您想要的受眾。

若要新增類別，請選取&#x200B;**[!UICONTROL 類別]**&#x200B;區段中的&#x200B;**[!UICONTROL 編輯]**&#x200B;選項。

![個別對象工作區的「類別」區段。](/help/assets/setup/add-manage-audiences/audience-details-categories.png)

**[!UICONTROL 類別]**&#x200B;對話方塊將會顯示，允許您選取要新增至對象的類別。 若要選取個別類別，請選取類別名稱旁的核取方塊。

![顯示具有可用類別的[類別]對話方塊。](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png)

### 連線存取權 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="連線存取權"
>abstract="<p>客群可以分為三種類型：公開、私人和自訂。</p><p> 這些客群在協作者的專案中是否可以使用，取決於連線存取權設定。您一律可以將連線存取權從私人變更為公開，但一旦對象透過共同作業人員啟用，您就無法再變更該設定。</p>"

和共同作業人員一起使用的專案中，對象的可用性會因連線存取設定而異。 在&#x200B;**[!UICONTROL 連線存取]**&#x200B;區段中，您可以選取對象應為私人，或是連線中可用且可探索。

若要更新對象的連線存取權，請在&#x200B;**[!UICONTROL 連線存取權]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;選項。

![個別對象工作區的「連線存取」區段。](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png)

出現&#x200B;**[!UICONTROL 連線存取]**&#x200B;對話方塊，其中包含三個可用的連線存取選項：

* **[!UICONTROL 私人對象]**。 這些對象&#x200B;*無法*&#x200B;用於重疊報表中，或用於與任何共同作業人員的連線中啟動。 雖然共同作業人員無法檢視或使用對象，但對象母體仍會貢獻[比較對象區段](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有對象]**&#x200B;檢視的總母體。 將設定變更為公用或自訂，以在與共同作業人員的連線中使用對象。
* **[!UICONTROL 公開對象]**。 這些對象可用於重疊報表，以及在與任何共同作業人員的連線中啟動。
* **[!UICONTROL 自訂對象]**。 這些對象只能在重疊報表中使用，也只能在指定的連線中啟動。 雖然共同作業人員無法檢視或使用對象，但對象母體仍會貢獻[比較對象區段](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有對象]**&#x200B;檢視的總母體。

選取想要的連線存取選項，然後選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以套用變更。

![顯示具有可用選項的[連線存取]對話方塊。](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

>[!IMPORTANT]
>
>無論存取狀態（公用、私人或自訂）為何，任何對象的母體都會貢獻至專案內&#x200B;**[!UICONTROL 比較對象]**&#x200B;區段中的&#x200B;**[!UICONTROL 所有對象]**&#x200B;母體。<br>

用於合作者專案中的對象可用性會因連線存取設定而異。 您一律可以將連線存取權從私人變更為公用，但一旦啟用對象，您就無法再改回該設定。

### 中繼資料可見度 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="中繼資料可見度"
>abstract="<p>指出其他組織在連線至您的組織之前，可以看見對象的中繼資料。 </p> <p> **身分識別計數**&#x200B;控制您的合作夥伴在探索索引標籤中檢視重疊報告時，是否可以檢視您客群的身分識別計數。**客群重疊百分比**&#x200B;控制協作者是否能夠探索其客群與您的客群之間的重疊百分比。"

>[!NOTE]
>
>如果您的共同作業人員將所有對象設為私人，專案的&#x200B;**[!UICONTROL 探索]**&#x200B;工作區中的&#x200B;**[!UICONTROL 相關對象]**&#x200B;區段將為空白。 如需詳細資訊，請閱讀[探索](/help/guide/collaborate/discover.md#relevant-audiences)。 指南。

中繼資料可見性表示在其他組織連線至您的組織之前，或在不同專案檢視中，對象的中繼資料是否可見。 若要更新對象的中繼資料可見度，請在&#x200B;**[!UICONTROL 中繼資料可見度]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**&#x200B;選項。

![個別對象工作區的「中繼資料可見度」區段。](/help/assets/setup/add-manage-audiences/audience-details-metadata.png)

**[!UICONTROL 中繼資料可見性]**&#x200B;對話方塊會出現，可讓您設定對象的可見性設定。 您可以為每個對象設定兩個中繼資料可見性設定：

**[!UICONTROL 顯示身分計數]**：此設定控制您的共同作業人員是否可以在專案中[在探索索引標籤](/help/guide/collaborate/discover.md#discover-overlaps)中檢視重疊報告時，檢視您對象的身分計數。

**[!UICONTROL 顯示對象重疊%]**：設定為True時，共同作業人員將能夠[探索其對象與您的對象之間的重疊百分比](/help/guide/collaborate/discover.md#compare-audiences)。

![顯示具有可用選項的中繼資料可見性對話方塊。](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

## 後續步驟

匯入對象後，是時候探索與[連線](/help/guide/connect/establishing-connections.md)的發行者並開始共同作業專案了。
