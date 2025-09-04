---
title: 最新Real-Time CDP Collaboration發行說明
description: 遵循Real-Time CDP Collaboration的最新發行版本
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 738c7bc9f3a482a1c7c92c820b364c577e61dd56
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 1%

---

# 最新Real-Time CDP Collaboration發行說明

{{limited-availability-release-note}}

**上次更新日期**：2025年8月。

下列發行說明涵蓋Adobe Real-Time CDP Collaboration中發行的功能。 Collaboration版本會在持續傳遞模式上運作，允許大約每月發行。 這些發行說明會經常更新，請務必定期檢視。

## 2025 年 8 月 {#august-2025}

* 共同作業人員現在可以一次編輯多個對象。 您現在可以使用大量編輯工具，編輯多個對象的對象中繼資料、連線存取權、名稱、說明和類別。 若要深入瞭解如何編輯對象，請閱讀[管理對象](../setup/onboard-audiences.md#edit-audiences)指南。

## 2025 年 7 月 {#july-2025}

Real-time CDP Collaboration現在支援品牌對品牌共同作業。 共同作業人員現在可以建立連線，無論他們是廣告商或發佈者。 這樣可提供更具彈性的共同作業機會，並讓品牌得以運用彼此的資料和見解。 若要進一步瞭解品牌對品牌共同作業和廣告商對發佈商共同作業之間的差異，請閱讀[共同作業模式](../overview/collaboration-patterns.md)指南。

* 共同作業人員現在可以使用[私人連線邀請](../connect/establishing-connections.md#private-connection-invites)互相連線。 與共同作業人員共用您帳戶的唯一連執行緒式碼，然後共同作業人員就可以使用該程式碼直接與您連線。 這是品牌對品牌共同作業的核心功能，可讓共同作業人員建立超越廣告商探索&#x200B;**[!UICONTROL Discover發佈者]**&#x200B;目錄的連線。
* [自助服務目的地](../setup/manage-destinations.md)現在可供廣告商和發佈者使用。
* 現在連線中的兩個共同作業人員都可以使用對象啟用，無論他們的[帳戶角色](../overview/roles.md)為何。 在[建立連線](../connect/establishing-connections.md#configure-connection-settings)時設定對象啟用設定，可讓您指定哪些共同作業人員可以啟用對象。 若要深入瞭解對象啟用，請閱讀[啟用對象](../collaborate/activate.md)指南。
* **[!UICONTROL 啟用]**&#x200B;使用案例已重新設定為支援品牌對品牌共同作業。 專案中的「啟動&#x200B;**&#x200B;**」標籤現在會顯示已傳送給共同作業人員的對象，以及共同作業人員啟動至您目的地的對象。 若要深入瞭解，請閱讀[啟用對象](../collaborate/activate.md)指南。<br> ![啟用儀表板，其中包含傳送至的對象和啟用對象的區段。](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 現在可在專案的&#x200B;**[!UICONTROL 探索]**&#x200B;索引標籤中使用對象索引分數。 對象索引分數是評估對象與共同作業人員對象相符程度的量度。 此分數是根據基礎受眾計數和重疊來計算。 若要深入瞭解對象索引分數，請閱讀[對象索引分數](../collaborate/discover.md#audience-index-score)指南。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration現在可供&#x200B;**澳洲**&#x200B;和&#x200B;**紐西蘭**&#x200B;的客戶使用。 它會自動提供給這些地區的Real-Time CDP Prime和Ultimate客戶。
* Real-Time CDP Collaboration現在透過[設定](../setup/manage-destinations.md)區段中的&#x200B;**[!UICONTROL 我的目的地]**&#x200B;索引標籤，提供&#x200B;**[!UICONTROL 自助目的地]**。 目的地可讓您在第三方平台（例如廣告網路或資料管理平台）中啟用對象，以便透過各種管道觸及您的客戶。 目前僅支援Adobe Experience Platform目的地。 如果您有興趣設定不同的目的地，請聯絡您的Adobe代表。 若要深入瞭解目的地，請閱讀[目的地概觀](../destinations/overview.md)指南。
   * 目的地也新增支援，以便在[Collaboration對象入口網站](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)中檢視Adobe Experience Platform對象。
* 您現在可以在Collaboration中編輯現有資料連線的對象重新整理頻率。 目前，您可以選擇每天或每兩到六天重新整理一次對象。 若要深入瞭解如何編輯對象重新整理頻率，請參閱[管理資料連線](../setup/manage-data-connection.md#scheduling)指南。
* 現在已針對連線中選取的每個使用案例，設定共同作業人員之間的評分分割。 您可以針對每個使用案例設定不同的信用沖銷規則，以便更妥善地控制信用額的使用方式。 若要深入瞭解信用分割功能，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings)指南。 若要進一步瞭解如何使用信用額度，請閱讀[信用活動型別](../setup/my-activity.md#types-of-activities)指南。<br> ![顯示信用分割功能的連線設定畫面。](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 發佈者現在在接受廣告商的連線設定之前，可以設定廣告商名稱和ID。 發佈者可設定與其內部系統一致的名稱和ID，此名稱和ID可能與廣告商的名稱和ID不同。 若要進一步瞭解新增廣告商名稱和ID，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings.md)指南。<br> ![連線設定畫面顯示發行者設定廣告商名稱和ID。](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025 年 4 月 {#april-2025}

* 新的&#x200B;**[!UICONTROL 已處理的輸入]**&#x200B;資料行已新增至信用消耗活動表格。 此欄顯示針對每個活動處理的輸入總數（例如ID或列）。 [閱讀更多資訊](/help/guide/setup/my-activity.md#inputs-processed)。<br> ![輸入我的活動檢視中強調的處理資料行。](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 帳戶建立已新增新的連絡人電子郵件選項。 這可協助合作夥伴的共同作業人員在連線程式期間視需要與您聯絡。 [閱讀全文](../setup/onboard-account.md)。

## 2025 年 3 月 {#march-2025}

* 當[將對象](/help/guide/setup/onboard-audiences.md)來源至Collaboration時，您現在可以設定對象重新整理頻率，從&#x200B;**每隔1天到6天**，以便更妥善地管理[對象管理信用活動](/help/guide/setup/my-activity.md#types-of-activities)。 如需詳細資訊，請閱讀[管理對象](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)指南。<br> ![排程畫面，顯示更新對象成員資格的不同頻率間隔。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "排程畫面，顯示更新對象成員資格的不同頻率間隔。"){width="250" align="center" zoomable="yes"}
* 與共同作業人員建立連線時，您現在可以從預先定義的&#x200B;**使用案例**&#x200B;中進行選取。 所選的使用案例決定哪些專案區段和產品功能可供使用。 如需詳細資訊，請閱讀[管理專案](/help/guide/collaborate/manage-projects.md#project-use-cases)指南。
   * *測量*&#x200B;啟用&#x200B;**測量**&#x200B;專案區段。
   * *對象探索*&#x200B;啟用&#x200B;**探索**&#x200B;專案區段。
   * *對象啟用*&#x200B;會啟用&#x200B;**啟用**&#x200B;專案區段<br>
* 您現在可以刪除與不想再使用的共同作業人員之間的連線。 若要瞭解如何刪除連線，請閱讀[刪除連線](/help/guide/connect/establishing-connections.md#delete-connections)指南。

## 2025 年 2 月 {#february-2025}

Adobe Real-Time CDP Collaboration是專為讓廣告商和發佈商能夠探索、啟用和測量高價值受眾而不使用第三方Cookie所打造，現在美國已正式推出。

### 快速入門

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
