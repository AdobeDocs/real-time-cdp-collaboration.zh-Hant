---
title: 匯入和管理對象
description: 瞭解如何在Adobe Real-Time CDP Collaboration中匯入和管理對象
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 8fca38c8125cefae9fe52ecd168e3d0ff20f2936
workflow-type: tm+mt
source-wordcount: '2685'
ht-degree: 24%

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

您必須先將受眾匯入Real-Time CDP Collaboration，才能與共同作業人員共用受眾及執行重疊計算。 若要匯入對象，請依照下節中的工作流程步驟操作。

![將任何對象新增至組織之前，我的對象畫面。](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

從&#x200B;**[!UICONTROL 我的對象]**&#x200B;索引標籤，選取加號&#x200B;**+**&#x200B;符號，然後選取&#x200B;**對象**。

### 選取資料連線 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="行銷動作"
>abstract="<p>使用行銷動作來控制要從 Experience Platform 匯入哪一些客群資料到 Real-Time CDP Collaboration。<strong>資料共同作業</strong>行銷動作支援 C4、C5 和 C9 資料使用情況標籤。<strong>資料科學</strong>行銷動作支援 C9 資料使用情況標籤。</p> <p> <ul><li> 核取方塊<em>啟用</em>後，Experience Platform 中標有上述標籤的任何資料都將被排除，並且<strong>不會</strong>帶入 Real-Time CDP Collaboration 中。</li><li> 核取方塊<em>停用</em>後，可以從 Experience Platform 匯入 Real-Time CDP Collaboration 的資料沒有任何限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hant" text="資料使用標籤概觀"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="資料使用標籤字彙表"

>[!IMPORTANT]
>
>連線至您的第一個資料連線並匯入第一個對象後，您就可以選取從此現有的資料連線匯入多個對象。 在此情況下，工作流程會將您直接帶往[選取對象](#select-audience)步驟，因為其他步驟的所有先決條件資訊都會從現有連線匯入。

資料連線是資料來源，您會將受眾匯入Real-Time CDP Collaboration。 在Real-Time CDP Collaboration的第一個版本中，唯一支援的資料連線是Adobe Experience Platform。

您為資料連線設定的任何設定（例如身分對應或排程）都會套用至從此資料連線匯入的所有對象。

>[!TIP]
>
>有一個單獨的工作流程，您隨時都可以檢視及編輯在此步驟中新增的所有資料連線。 深入瞭解[管理資料連線](/help/guide/setup/manage-data-connection.md)。

![選取顯示AEP RTCDP、CSV檔案、Amazon S3和Snowflake選項的對象來源畫面。](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### 選取資料來源

在此步驟中，您將選擇對象資料的來源。 可用的來源包括：

* **Adobe Experience Platform**：選取此選項，即可從Adobe Experience Platform Real-Time CDP引進您的對象。
* **CSV檔案** （未來版本）：上傳包含您對象資料的CSV檔案，以快速且直接地擷取資料。
* **Amazon Web Services** （未來版本）：連線至您的Amazon S3儲存體，直接從S3儲存貯體匯入對象資料。
* **Snowflake** （未來版本）：使用您的Snowflake資料倉儲，順暢地提取對象資料。

#### 選取沙箱

選取&#x200B;**Adobe Experience Platform**&#x200B;做為資料來源後，您必須選取包含您將匯入之對象的沙箱。

![選取沙箱以匯入對象](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

在您選取想要的沙箱之後，選取&#x200B;**[!UICONTROL 下一步]**。

#### 治理原則和執行動作 {#governance-policy-and-enforcement-actions}

接下來，您必須確定已針對匯入的資料設定正確的行銷動作。 從Real-Time CDP匯入的資料若要用於資料共同作業，您也必須提供同意。

使用行銷動作來控制要從 Experience Platform 匯入哪一些客群資料到 Real-Time CDP Collaboration。**資料共同作業**&#x200B;行銷動作支援 C4、C5 和 C9 資料使用情況標籤。**資料科學**&#x200B;行銷動作支援 C9 資料使用情況標籤。

深入瞭解[C4、C5和C9資料使用標籤](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}。

* 核取方塊&#x200B;*啟用*&#x200B;後，Experience Platform 中標有上述標籤的任何資料都將被排除，並且&#x200B;*不會*&#x200B;帶入 Real-Time CDP Collaboration 中。
* 核取方塊&#x200B;*停用*&#x200B;後，可以從 Experience Platform 匯入 Real-Time CDP Collaboration 的資料沒有任何限制。

在Experience Platform檔案中進一步瞭解資料使用標籤：

* [資料使用標籤概觀](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [資料使用標籤字彙表](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![資料共同作業所需的行銷動作。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### 提供詳細資料

接下來，提供名稱和說明，供您日後識別此資料連線。

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### 對應欄位 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="來源欄位"
>abstract="來源欄位是來自您現有 Real-Time CDP 實施的身分識別命名空間和屬性。您可以將這些欄位對應到 Real-Time CDP Collaboration 中所定義的目標欄位。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目標欄位"
>abstract="目標欄位與您在公司上線時所選取的比對索引鍵相對應。目前，雜湊電子郵件是唯一支援的比對索引鍵。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="套用轉換"
>abstract="從來源匯入&#x200B;*非雜湊*&#x200B;欄位時，使用此選項讓 Real-Time CDP Collaboration 套用雜湊，並將純文字欄位轉換為雜湊欄位。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身分識別命名空間"
>abstract="從 Experience Platform 組織中可用的標準和自訂身分識別命名空間中，選取一個身分識別命名空間。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Experience Platform 中的標準和身分識別命名空間"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="輪廓屬性"
>abstract="從聯集結構中選取 Experience Platform 輪廓類別屬性。此視圖會顯示存在於聯集結構中，且屬於 XDM 個體輪廓類別的屬性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Experience Platform 中的聯集結構"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="目標命名空間"
>abstract="這將填寫適當的說明。"

![顯示對應到目標欄位之來源欄位的對應欄位畫面。](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

在對映欄位步驟中，您可以選取從資料連線引進之設定檔的任何身分欄位應如何對應至您在組織中選擇的相符索引鍵。

>[!TIP]
>
>您可以將多個來源欄位對應到相同的目標欄位。 例如，如果您在Experience Platform中的兩個個別欄位中有電子郵件地址，您可以將這兩個地址對應到&#x200B;**[!UICONTROL 雜湊電子郵件]**&#x200B;目標欄位，做為兩個個別的列。

>[!BEGINSHADEBOX]

**[!UICONTROL Source欄位]**&#x200B;指出在您匯入資料的來源中，身分的參照方式。

**[!UICONTROL 目標欄位]**&#x200B;指出在Real-Time CDP Collaboration中參照身分的方式。 您可以在此處選取的值對應於您在公司入門工作流程中設定的相符金鑰。

當您從來源匯入&#x200B;*非雜湊*&#x200B;欄位時，請使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;選項。 在這種情況下，Real-Time CDP Collaboration將套用雜湊並轉換欄位。 Adobe使用的雜湊演演算法是SHA256。

>[!ENDSHADEBOX]

視需要新增對應配對，並選取&#x200B;**[!UICONTROL 下一步]**&#x200B;以繼續執行下一個步驟。

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->›

### 排程 {#schedule}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="客群到期"
>abstract="有關客群到期的詳細資訊即將公佈。"

排程何時開始和結束填入及重新整理對象。 對象會籍將根據此排程重新整理。

![顯示填入對象開始和結束日期的排程畫面。](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

選取對象的重新整理頻率。 可用的選項是一至六天的重新整理頻率。

>[!IMPORTANT]
>
>調整對象更新頻率有助於管理[對象管理信用活動](/help/guide/setup/my-activity.md#types-of-activities)，這是根據對象成員資格重新整理計算所得。 這可能會造成影響，讓受眾探索報表和受眾共用及啟用的可用資料變得不那麼新鮮。

![排程畫面，顯示更新對象成員資格的不同頻率間隔。](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>在日期範圍內的結束日期之後，從此資料連線匯入的所有對象將停止重新整理。 若要更新連線，請移至[管理資料連線](/help/guide/setup/manage-data-connection.md)，並設定新的結束日期。

### 選取客群 {#select-audience}

選取對象來源後，您將選擇要包含的特定對象。 使用頁面上的搜尋和篩選選項，從您選取的資料來源尋找相關的對象。

![選取對象熒幕，顯示可用的對象清單，以及用來選取這些對象的核取方塊。](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### 審核

在最終確定對象新增之前，請檢閱所有配置和設定。 請確定所有詳細資料都正確無誤，並選取&#x200B;**[!UICONTROL 完成]**&#x200B;以完成程式。

## 檢視客群儀表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身分識別"
>abstract="根據已設定的排程，身份識別計數將在下一次資料連線重新整理後可用。初始重新整理通常發生在設定資料連線後的 24 小時內。正在進行的重新整理將遵循已設定的排程。 "

將受眾匯入Real-Time CDP Collaboration後，您可以在控制面板檢視中取得有關他們的資訊。 **[!UICONTROL 我的對象]**&#x200B;頁面中的預設檢視會顯示貴組織目前匯入Real-Time CDP Collaboration的所有對象。

![對象總覽頁面顯示廣告商匯入的所有對象](/help/assets/setup/add-manage-audiences/audiences-overview.png)

您可以檢視關於每個對象的下列相關資訊：

| 項目 | 說明 |
|----------|---------|
| **[!UICONTROL 身分]** | 表示此對象中存在的身分數量。 請注意，如果相同設定檔有兩個或多個身分，而這些身分在專案中作為相符索引鍵使用，則設定檔會在計數中顯示兩次。 |
| **[!UICONTROL 狀態]** | 指出對象是否作用中以及是否可用於專案。 「待定」狀態表示對象最近剛匯入，且對象成員尚未填入。 匯入的對象將在依照設定的排程進行下一次資料連線重新整理後填入設定檔。 初次重新整理通常發生在資料連線設定後的24小時內                                         . |
| **[!UICONTROL Source]** | 指出匯入此對象的來源。 在目前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支援的來源。 |
| **[!UICONTROL 資料連線]** | 深入展開此對象匯入來源的相關資訊。 例如，從Experience Platform來源匯入受眾時，您的組織有權存取的個別沙箱會被視為資料連線。 |
| **[!UICONTROL 連線存取]** | 定義此對象是私人或公開。 您可以在重疊報表中找到公用對象，並與共同作業人員共用。 |
| **[!UICONTROL 已建立]** | 指出此對象何時匯入Real-Time CDP Collaboration。 |
| **[!UICONTROL 上次更新時間]** | 表示上次更新此對象任何方面的日期和時間。 |

選取「管理資料連線」****以檢視及編輯您已設定的所有資料連線。
選取省略符號和**[!UICONTROL 刪除]**以移除對象。
選取省略符號和**[!UICONTROL 編輯類別]**&#x200B;以新增不同的類別標籤至對象。 在下面的[類別](/#categories)區段中取得更多資訊。
選取對象名稱，以檢查或編輯個別對象。

## 檢視個別對象 {#view-individual-audiences}

對象檢視會顯示有關對象的進一步資訊。

![檢視並檢查個別對象。](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

您可以在此畫面中檢視的量度說明如下：

| 項目 | 說明 |
|----------|---------|
| **[!UICONTROL 狀態]** | 指出對象是否作用中以及是否可用於專案。 |
| **[!UICONTROL Source]** | 指出匯入此對象的來源。 在目前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支援的來源。 |
| **[!UICONTROL 資料連線]** | 深入展開此對象匯入來源的相關資訊。 例如，從Experience Platform來源匯入受眾時，您的組織有權存取的個別沙箱會被視為資料連線。 |
| **[!UICONTROL 上次更新時間]** | 表示上次更新此對象任何方面的日期和時間。 |
| **[!UICONTROL 上次更新者]** | 表示上次更新此對象的使用者。 |
| **[!UICONTROL 已建立]** | 指出此對象何時匯入Real-Time CDP Collaboration。 |
| **[!UICONTROL 建立者：]** | 表示將受眾匯入Real-Time CDP Collaboration的使用者。 |


您可以在頁面上使用兩個其他控制項來編輯或移除對象：

* **[!UICONTROL 刪除]**：從您的詳細目錄中移除對象
* **[!UICONTROL 編輯]**：編輯對象中繼資料，如其名稱或說明。

![檢視並檢查個別對象。](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

有關對象的進一步資訊可在以下介面工具集中取得和部分編輯：

![檢視並檢查個別對象。](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [身分識別](#identities)
* [類別](#categories)
* [連線存取權](#connection-access)
* [中繼資料可見度](#metadata-visibility)

### 身分識別 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身分識別"
>abstract="取得構成這個客群的身分識別的劃分視圖，以及具有相應身分識別之輪廓的總計數。"

此區段會指出在對象中存在的設定檔數目，以及您在匯入對象時指定的任何身分。 區段也包含身分劃分，以便您分辨哪些身分構成最多受眾群體。

### 類別 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="類別"
>abstract="標記您的客群，以便於組織、篩選和檢索。您可以使用多個類別標記客群，然後可以使用這些類別標記在產品的其他方面篩選所需的客群。"

為了輕鬆進行對象組織、篩選和擷取，您可以標籤對象。 您可以標籤具有多個類別的受眾，然後在執行受眾重疊報表時，可以使用這些類別標籤在[探索](/help/guide/collaborate/discover.md)產品區域中篩選您想要的受眾。

### 連線存取權 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="連線存取權"
>abstract="<p>客群可以分為三種類型：公開、私人和自訂。</p><p> 這些客群在協作者的專案中是否可以使用，取決於連線存取權設定。您可以隨時將連線存取權從私人變更為公開，但一旦與協作者共用客群，便無法變更該設定。</p>"

選取對象是否為您私人，或在連線中是否可用和可探索。 三個可用選項包括：

* **[!UICONTROL 公開對象]**。 這些受眾可用於重疊報表，以及在與任何共同作業人員的連線中共用和啟動。
* **[!UICONTROL 私人對象]**。 這些對象&#x200B;*無法*&#x200B;用於重疊報表，以及可與任何共同作業人員共用和啟動連線。 雖然共同作業人員無法檢視或使用，但此對象的母體仍會貢獻[探索與重疊區段](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有對象]**&#x200B;檢視的總母體。 將設定變更為公用或自訂，以在與共同作業人員的連線中使用對象。
* **[!UICONTROL 自訂對象]**。 這些對象僅在重疊報表中使用，也只能在指定的連線中共用和啟動。 雖然並非所有共同作業人員都能檢視或使用，此對象的母體仍會貢獻給[探索與重疊區段](/help/guide/collaborate/discover.md)中&#x200B;**[!UICONTROL 所有對象]**&#x200B;檢視的總母體。

>[!IMPORTANT]
>
>無論存取狀態（公用、私人或自訂）為何，任何對象的母體都會貢獻至「對象探索」重疊分析檢視中的&#x200B;**[!UICONTROL 所有對象]**&#x200B;母體。<br> ![在對象探索重疊分析中，系統產生的&#x200B;**所有對象**&#x200B;對象包含具有所有連線存取狀態（公開、私人、自訂）的對象。](/help/assets/setup/add-manage-audiences/all-audiences-view.png "在**對象探索**重疊分析中，系統產生的**所有對象**對象包含具有所有連線存取狀態（公用、私用、自訂）的對象。"){width="100" zoomable="yes"}

用於合作者專案中的對象可用性會因連線存取設定而異。 您可以隨時將連線存取權從私人變更為公開，但一旦與協作者共用客群，便無法變更該設定。

### 中繼資料可見度 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="中繼資料可見度"
>abstract="<p>表示其他組織在與您的組織建立連線之前，可以看到哪些客群中繼資料資訊。 </p> <p> **身分識別計數**&#x200B;控制您的合作夥伴在探索索引標籤中檢視重疊報告時，是否可以檢視您客群的身分識別計數。**客群重疊百分比**&#x200B;控制協作者是否能夠探索其客群與您的客群之間的重疊百分比。"

>[!NOTE]
>
>如果您的共同作業人員將所有對象設為私人，則對象深入分析中的&#x200B;**[!UICONTROL 相關對象]**&#x200B;檢視將為空白。 [閱讀全文](/help/guide/collaborate/discover.md#relevant-audiences)。

指示其他組織在與您的組織連線或在不同專案檢視內之前，可以看見哪些對象中繼資料資訊。

**[!UICONTROL 顯示身分計數]**：此設定控制您的合作夥伴在[在探索索引標籤](/help/guide/collaborate/discover.md#discover-overlaps)中檢視重疊報告時，是否可以檢視您對象的身分計數。

![取消選取並選取顯示身分計數選項的並排影像。](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL 顯示對象重疊%]**：設定為True時，共同作業人員將能夠[探索其對象與屬於您的對象之間的重疊百分比](/help/guide/collaborate/discover.md#compare-audiences)。 例如，在下方的錄製中，對象`agora-advertiser-aud3`的此組態設定為true，共同作業人員可以檢視與該對象的重疊百分比。 對象`agora-advertiser-aud1`已將此設定設為false，所以共同作業人員無法檢視重疊百分比。

![兩個不同對象的對象重疊百分比。](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## 後續步驟

匯入對象後，請使用[連線](/help/guide/connect/establishing-connections.md)區段來探索要連線的發行者，並開始共同作業專案。
