---
title: 最新Real-Time CDP Collaboration發行說明
description: 遵循Real-Time CDP Collaboration的最新發行版本
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
TQID: https://experienceleague.adobe.com/re4oFblCLiZpspWIS7D4EEYNh36EDhULEOd2-ccXH28
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 7affd3abf7a10019503825cb20d9be1ad4000603
workflow-type: tm+mt
source-wordcount: 1903
ht-degree: 3%

---

# 最新Real-Time CDP Collaboration發行說明

{{limited-availability-release-note}}

**上次更新日期**：2026年4月。

下列發行說明涵蓋Adobe Real-Time CDP Collaboration中發行的功能。 Collaboration版本會在持續傳遞模式上運作，允許大約每月發行。 這些發行說明會經常更新，請務必定期檢視。

## 2026 年 4 月 {#april-2026}

Real-Time CDP Collaboration現在提供新功能。 其中包括邀請合作夥伴的Collaboration [!DNL Starter]、從[!DNL Snowflake]和[!DNL Google Cloud Storage]擴大受眾來源、支援[!DNL Demdex ID (ECID)]作為比對索引鍵，以及兩個新的共同作業人員角色：代理和資料合作夥伴。

**新功能或更新功能**

| 功能 | 說明 |
| ------- | ----------- |
| Real-Time CDP Collaboration [!DNL Starter] | 您現在可以邀請沒有Collaboration授權的合作夥伴透過Collaboration [!DNL Starter]與您共同作業。 受邀合作夥伴可以在共用連線中取得對象、探索重疊以及啟用對象。 請參閱[Collaboration [!DNL Starter] 總覽](../overview/starter-overview.md)以開始使用。 |
| 來自[!DNL Snowflake]和[!DNL Google Cloud Storage]的自助受眾來源 | 您現在可以直接從您的[!DNL Snowflake Secure Data Share]或[!DNL Google Cloud Storage]貯體將第一方對象來源至Collaboration。 如需設定說明，請參閱下列指南： <ul><li>[設定 [!DNL Snowflake] 對象來源](../setup/configure-snowflake-audience-sourcing.md) </li><li> [設定 [!DNL Google Cloud Storage] 對象來源](../setup/configure-gcs-audience-sourcing.md) </li></ul> |
| [!DNL Demdex ID]個相符索引鍵 | [!DNL Demdex ID] (ECID)現在支援作為跨平台比對匿名Cookie型身分的比對金鑰。 它改善了對象重疊的準確性，而不需依賴已驗證的使用者資料。 如需詳細資訊，請參閱[支援的相符金鑰](../setup/onboard-account.md#supported-match-keys)。 |
| 新的共同作業人員角色 | Collaboration現在支援兩個額外的共同作業人員角色，包括&#x200B;**機構**&#x200B;和&#x200B;**資料合作夥伴**。 這些角色可擴充不同組織在平台中參與及共同作業的方式。 進一步瞭解： <ul><li>[共同作業人員帳戶角色](../overview/roles.md)</li><li>[Collaboration模式](../overview/collaboration-patterns.md)</li><li>[端對端工作流程](../overview/end-to-end-workflow.md)</li></ul> |

{style="table-layout:auto"}

## 2026年3月 {#march-2026}

您現在可以在Real-Time CDP Collaboration中產生行銷活動測量報告並管理測量資料。

**新功能或更新功能**

| 功能 | 說明 |
| ------- | ----------- |
| 測量一般可用性 | 測量報告現在通常可在Collaboration中使用。 您現在可以輸入與行銷活動關聯的行銷活動ID作為發佈者，輸入來源轉換資料作為廣告商，並產生兩種型別的報表：整體行銷活動結果的&#x200B;**行銷活動摘要**&#x200B;以及行銷活動成效深入分析的&#x200B;**歸因**。 若要開始使用，請參閱下列指南： <ul><li>[輸入行銷活動ID](../collaborate/manage-projects.md#manage-campaign-id)</li><li>[Source轉換資料](../setup/onboard-measurement-data.md)</li><li>[建立和檢視測量報告](../collaborate/measure.md)</li></ul> |
| 測量生命週期管理 | Collaboration也支援測量管理：<ul><li> 廣告商現在可以編輯或刪除測量資料連線和關聯的轉換事件，以確保準確且最新的行銷活動分析。 如需詳細資訊，請參閱[管理測量資料連線](../setup/manage-measurement-data-connection.md)和[管理轉換事件](../setup/onboard-measurement-data.md#edit-measurement-data)。</li><li>您也可以在任何共同作業專案中，直接從&#x200B;**[!UICONTROL 測量]**&#x200B;索引標籤編輯或刪除排程的測量報告。 所有使用者都可使用此功能。 如需詳細資訊，請參閱[管理測量報告指南](../collaborate/measure.md)。</li></ul> |

{style="table-layout:auto"}

## 2026 年 2 月 {#february-2026}

Real-Time CDP Collaboration現在支援直接在介面中編輯現有的連線和資料連線設定。

**新增或更新功能**

| 功能 | 說明 |
| ------- | ----------- |
| 編輯連線設定 | 連線擁有者現在可以在連線建立後更新使用案例、比對金鑰、啟用許可權和評分分割。 如需逐步指示，請參閱[編輯連線](../connect/manage-connections.md#edit-connection)。 |
| 編輯資料連線 | 直接在Collaboration中更新現有資料連線的比對索引鍵和排程設定。 如需逐步指示，請參閱[編輯資料連線](../setup/manage-data-connection.md#edit-data-connection)。 |

## 2026 年 1 月 {#january-2026}

Real-Time CDP Collaboration現在支援CSV檔案上傳作為獲取對象的新方法，以及用於增強對象比對和測量的新行動配對金鑰（IDFA和GAID）。

**新功能或更新功能**

| 功能 | 說明 |
| ------- | ----------- |
| Audience Sourcing的CSV上傳 | 直接從UI上傳CSV檔案至來源受眾至Collaboration。 適合用來為短期共同作業專案入門的第一方資料。 如需詳細資訊，請參閱[上傳對象來源指南](../setup/upload-csv-audience-sourcing.md)的CSV檔案。 |
| 行動比對金鑰支援 | Collaboration現在支援行動相符金鑰（包括IDFA和GAID），以進行對象相符和測量。 這些比對金鑰是在帳戶設定期間選取，然後可在為新連線和下游共同作業工作流程設定連線設定時使用。 如需詳細資訊，請參閱[比對金鑰設定指南](../setup/onboard-account.md#set-up-match-keys)。 |

{style="table-layout:auto"}

## 2025 年 12 月 {#december-2025}

Real-Time CDP Collaboration現在可供&#x200B;**歐洲、中東和非洲(EMEA))**&#x200B;的客戶使用。 它會自動提供給這些地區的Real-Time CDP Prime和Ultimate客戶。

## 2025 年 8 月 {#august-2025}

**加拿大**&#x200B;的客戶現在可使用Real-Time CDP Collaboration。 它會自動提供給這些地區的Real-Time CDP Prime和Ultimate客戶。

* Collaboration現在支援下列[相符金鑰](../setup/onboard-account.md#supported-match-keys)：
   * 已雜湊的電子郵件
   * 雜湊電話號碼
   * CRM ID
   * 忠誠度 ID
   * 已雜湊的 IPv4
   * AdFixus ID
* Collaboration現在提供多個相符索引鍵，讓您能夠擴大受眾規模並提高相符率。 搜尋對象、建立連線和啟用對象時，可以使用多個相符索引鍵。 若要進一步瞭解如何使用多個比對索引鍵，請閱讀[設定比對索引鍵](../setup/onboard-account.md)和[來源受眾](../setup/onboard-audiences.md#map-fields)指南。

>[!IMPORTANT]
>
>啟用使用多個相符金鑰的受眾時，如果一個（或多個）相符金鑰沒有重疊、無受眾規模或低於臨界值，則整個啟用將會失敗。 啟用之前，請確認您的對象有足夠的重疊，並符合所有相符索引鍵中1000 ID的最低臨界值。

* Adobe Experience Platform目的地現在支援使用多個相符索引鍵來啟用對象。 此外，您現在可以在設定目的地的對應時使用連結金鑰，以指定在啟用期間傳送的相符金鑰。 若要深入瞭解，請閱讀[Experience Platform目的地](../destinations/experience-platform.md#linked-keys)指南。
* 共同作業人員現在可以一次編輯多個對象。 您現在可以使用大量編輯工具，編輯多個對象的對象中繼資料、連線存取權、名稱、說明和類別。 若要深入瞭解如何編輯對象，請閱讀[管理對象](../setup/onboard-audiences.md#edit-audiences)指南。

## 2025 年 7 月 {#july-2025}

Real-time CDP Collaboration現在支援品牌對品牌共同作業。 共同作業人員現在可以建立連線，無論他們是廣告商或發佈者。 這樣可提供更具彈性的共同作業機會，並讓品牌得以運用彼此的資料和見解。 若要進一步瞭解品牌對品牌共同作業和廣告商對發佈商共同作業之間的差異，請閱讀[共同作業模式](../overview/collaboration-patterns.md)指南。

* 共同作業人員現在可以使用[私人連線邀請](../connect/establishing-connections.md#private-connection-invites)互相連線。 與共同作業人員共用您帳戶的唯一連執行緒式碼，然後共同作業人員就可以使用該程式碼直接與您連線。 這是品牌對品牌共同作業的核心功能，可讓共同作業人員建立超越廣告商探索&#x200B;**[!UICONTROL 探索共同作業人員]**&#x200B;目錄的連線。
* [自助服務目的地](../setup/manage-destinations.md)現在可供廣告商和發佈者使用。
* 現在連線中的兩個共同作業人員都可以使用對象啟用，無論他們的[帳戶角色](../overview/roles.md)為何。 在[建立連線](../connect/establishing-connections.md#configure-connection-settings)時設定對象啟用設定，可讓您指定哪些共同作業人員可以啟用對象。 若要深入瞭解對象啟用，請閱讀[啟用對象](../collaborate/activate.md)指南。
* **[!UICONTROL 啟用]**&#x200B;使用案例已重新設定為支援品牌對品牌共同作業。 專案中的「啟動&#x200B;**&#x200B;**」標籤現在會顯示已傳送給共同作業人員的對象，以及共同作業人員啟動至您目的地的對象。 若要深入瞭解，請閱讀[啟用對象](../collaborate/activate.md)指南。<br> ![啟用儀表板，其中包含傳送至的對象和啟用對象的區段。](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 現在可在專案的&#x200B;**[!UICONTROL 探索]**&#x200B;索引標籤中使用對象索引分數。 對象索引分數是評估對象與共同作業人員對象相符程度的量度。 此分數是根據基礎受眾規模和重疊來計算。 若要深入瞭解對象索引分數，請閱讀[對象索引分數](../collaborate/discover.md#audience-index-score)指南。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration現在可供&#x200B;**澳洲**&#x200B;和&#x200B;**紐西蘭**&#x200B;的客戶使用。 它會自動提供給這些地區的Real-Time CDP Prime和Ultimate客戶。
* Real-Time CDP Collaboration現在透過&#x200B;**[!UICONTROL 設定]**&#x200B;區段中的&#x200B;**[!UICONTROL 我的目的地]**&#x200B;索引標籤，提供[自助目的地](../setup/manage-destinations.md)。 目的地可讓您在第三方平台（例如廣告網路或資料管理平台）中啟用對象，以便透過各種管道觸及您的客戶。 目前僅支援Adobe Experience Platform目的地。 如果您有興趣設定不同的目的地，請聯絡您的Adobe代表。 若要深入瞭解目的地，請閱讀[目的地概觀](../destinations/overview.md)指南。
   * 目的地也新增支援，以便在[Collaboration對象入口網站](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)中檢視Adobe Experience Platform對象。
* 您現在可以在Collaboration中編輯現有資料連線的對象重新整理頻率。 目前，您可以選擇每天或每兩到六天重新整理一次對象。 若要深入瞭解如何編輯對象重新整理頻率，請參閱[管理資料連線](../setup/manage-data-connection.md#scheduling)指南。
* 現在已針對連線中選取的每個使用案例，設定共同作業人員之間的評分分割。 您可以針對每個使用案例設定不同的信用沖銷規則，以便更妥善地控制信用額的使用方式。 若要深入瞭解信用分割功能，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings)指南。 若要進一步瞭解如何使用信用額度，請閱讀[信用活動型別](../setup/my-activity.md#types-of-activities)指南。<br> ![顯示信用分割功能的連線設定畫面。](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 發佈者現在在接受廣告商的連線設定之前，可以設定廣告商名稱和ID。 發佈者可設定與其內部系統一致的名稱和ID，此名稱和ID可能與廣告商的名稱和ID不同。 若要進一步瞭解新增廣告商名稱和ID，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings.md)指南。<br> ![連線設定畫面顯示發行者設定廣告商名稱和ID。](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025 年 4 月 {#april-2025}

* 新的&#x200B;**[!UICONTROL 已處理的輸入]**&#x200B;資料行已新增至信用消耗活動表格。 此欄顯示針對每個活動處理的輸入總數（例如ID或列）。 [閱讀更多資訊](/help/guide/setup/my-activity.md#inputs-processed)。<br> ![輸入我的活動檢視中強調的處理資料行。](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 帳戶建立已新增新的連絡人電子郵件選項。 這可協助合作夥伴的共同作業人員在連線程式期間視需要與您聯絡。 [閱讀全文](../setup/onboard-account.md)。

## 2025 年 3 月 {#march-2025}

* 當[將對象](/help/guide/setup/onboard-audiences.md)來源至Collaboration時，您現在可以設定對象重新整理頻率，從&#x200B;**每隔1天到6天**，以便更妥善地管理[對象管理信用活動](/help/guide/setup/my-activity.md#types-of-activities)。 如需詳細資訊，請閱讀[管理對象](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)指南。<br> ![排程畫面，顯示更新對象成員資格的不同頻率間隔。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "排程畫面，顯示更新對象成員資格的不同頻率間隔。"){width="250" align="center" zoomable="yes"}
* 與共同作業人員建立連線時，您現在可以從預先定義的&#x200B;**使用案例**&#x200B;中進行選取。 所選的使用案例決定哪些專案區段和產品功能可供使用。 如需詳細資訊，請閱讀[管理專案](/help/guide/collaborate/manage-projects.md#project-use-cases)指南。
   * *測量*&#x200B;啟用&#x200B;**測量**&#x200B;專案區段。
   * *對象探索*&#x200B;啟用&#x200B;**探索**&#x200B;專案區段。
   * *對象啟用*&#x200B;會啟用&#x200B;**啟用**&#x200B;專案區段<br>
* 您現在可以刪除與不想再使用的共同作業人員之間的連線。 若要瞭解如何刪除連線，請閱讀[刪除連線](/help/guide/connect/establishing-connections.md#delete-connections)指南。

## 2025 年 2 月 {#february-2025}

Adobe Real-Time CDP Collaboration是專為讓廣告商和發佈商能夠探索、啟用和測量高價值受眾而不使用第三方Cookie所打造，現在美國已正式推出。

### 開始使用

1. **存取安裝程式**：系統管理員設定使用者的存取許可權。 若要進一步瞭解設定存取許可權，請閱讀[管理使用者存取權](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access)指南。
2. **連線資料來源**：要在Collaboration中使用的Source對象。 若要開始取得受眾，請閱讀[來源及管理受眾](/help/guide/setup/onboard-audiences.md)指南。
3. **建立連線**：開始與信任的廣告商或發行者共同作業。 若要深入瞭解如何建立連線，請閱讀[建立連線](/help/guide/connect/establishing-connections.md)指南。
4. **探索並啟用**：建立專案以識別要在行銷活動中啟用的有價值對象。 若要深入瞭解如何建立專案，請閱讀[管理專案](/help/guide/collaborate/manage-projects.md)指南。

### 可用性

* Adobe Real-Time CDP Collaboration目前僅開放美國客戶使用。
* Adobe Real-Time CDP Prime和Ultimate客戶可自動使用此功能

如需詳細資訊，請閱讀：

* [Collaboration概觀](/help/guide/home.md)
* [端對端工作流程](/help/guide/overview/end-to-end-workflow.md)
* [許可權總覽](/help/guide/permissions/overview.md)
