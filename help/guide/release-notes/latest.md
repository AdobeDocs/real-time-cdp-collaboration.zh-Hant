---
title: 最新Real-Time CDP Collaboration發行說明
description: 遵循Real-Time CDP Collaboration的最新發行版本
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 92e347e3258817a983d8eaed9cf2b962b3443cbc
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 3%

---

# 最新Real-Time CDP Collaboration發行說明

{{limited-availability-release-note}}

**上次更新日期**：2025年4月。

下列發行說明涵蓋Real-Time Customer Data Platform Collaboration中發行的功能。 Real-Time CDP Collaboration版本會在持續傳遞模式上運作，允許大約每月發行。 這些發行說明會經常更新，請務必定期檢視。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration現在可供&#x200B;**澳洲**&#x200B;和&#x200B;**紐西蘭**&#x200B;的客戶使用。 它會自動提供給這些地區的Real-Time CDP Prime和Ultimate客戶。
* Real-Time CDP Collaboration現在透過「設定」區段中的「我的設計」索引標籤，提供[自助式目的地](../setup/manage-destinations.md)。 目的地可讓您在第三方平台（例如廣告網路或資料管理平台）中啟用對象，以便透過各種管道觸及您的客戶。 目前僅支援Adobe Experience Platform目的地。 如果您有興趣設定不同的目的地，請聯絡您的Adobe代表。 若要深入瞭解目的地，請閱讀[目的地概觀](../destinations/overview.md)指南。

   * 目的地也新增支援，以便在[Real-Time CDP Collaboration對象入口網站](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences.)中檢視Adobe Experience Platform對象。

* 您現在可以在Real-Time CDP Collaboration中編輯現有資料連線的對象重新整理頻率。 目前，您可以選擇每天或每兩到六天重新整理一次對象。 若要深入瞭解如何編輯對象重新整理頻率，請參閱[管理資料連線](../setup/manage-data-connection.md#scheduling)指南。
* 現在已針對連線中選取的每個使用案例，設定共同作業人員之間的評分分割。 您可以針對每個使用案例設定不同的信用沖銷規則，以便更妥善地控制信用額的使用方式。 若要深入瞭解信用分割功能，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings)指南。 若要進一步瞭解如何使用信用額度，請閱讀[信用活動型別](../setup/my-activity.md#types-of-activities)指南。<br> ![顯示信用分割功能的連線設定畫面。](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 發佈者現在在接受廣告商的連線設定之前，可以設定廣告商名稱和ID。 發佈者可設定與其內部系統一致的名稱和ID，此名稱和ID可能與廣告商的名稱和ID不同。 若要進一步瞭解新增廣告商名稱和ID，請閱讀[連線設定](../connect/establishing-connections.md#connection-settings.md)指南。<br> ![連線設定畫面顯示發行者設定廣告商名稱和ID。](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025 年 4 月 {#april-2025}

* 新的&#x200B;**[!UICONTROL 已處理的輸入]**&#x200B;資料行已新增至信用消耗活動表格。 此欄顯示針對每個活動處理的輸入總數（例如ID或列）。 [閱讀更多資訊](/help/guide/setup/my-activity.md#inputs-processed)。<br> ![輸入我的活動檢視中強調的處理資料行。](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 帳戶建立已新增新的連絡人電子郵件選項。 這可協助合作夥伴的共同作業人員在連線程式期間視需要與您聯絡。 [閱讀全文](../setup/onboard-organization.md)。

## 2025 年 3 月 {#march-2025}

* 當[將對象](/help/guide/setup/onboard-audiences.md)匯入Real-Time CDP Collaboration時，您現在可以設定對象重新整理頻率，從&#x200B;**每一天到六天**，以便更妥善地管理[對象管理信用活動](/help/guide/setup/my-activity.md#types-of-activities)。 [閱讀更多資訊](/help/guide/setup/onboard-audiences.md#schedule)。<br> ![排程畫面，顯示更新對象成員資格的不同頻率間隔。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "排程畫面，顯示更新對象成員資格的不同頻率間隔。"){width="250" align="center" zoomable="yes"}
* 與共同作業人員建立連線時，您現在可以從預先定義的&#x200B;**使用案例**&#x200B;中進行選取。 所選的使用案例決定哪些專案區段和產品功能可供使用。 [閱讀全文](/help/guide/collaborate/manage-projects.md#project-use-cases)。
   * *促銷活動測量*&#x200B;啟用&#x200B;**測量**&#x200B;專案區段。
   * *對象探索*&#x200B;啟用&#x200B;**探索**&#x200B;專案區段。
   * *對象啟用*&#x200B;會啟用&#x200B;**啟用**&#x200B;專案區段<br>
* 您現在可以刪除與不想再使用的共同作業人員之間的連線。 [閱讀全文](/help/guide/connect/establishing-connections.md#delete-connections)。


## 2025年2月 — 美國客戶一般可用性 {#february-2025-ga}

Real-Time CDP Collaboration是專為讓廣告商和發佈商能夠探索、啟用和測量高價值受眾而不使用第三方Cookie所打造，現在美國已正式推出。

### 快速入門

1. **存取安裝程式**：系統管理員設定使用者的存取許可權。 [閱讀全文](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access)。
2. **連線資料來源**：匯入對象以在Real-Time CDP Collaboration中使用。 [閱讀全文](/help/guide/setup/onboard-audiences.md)。
3. **建立合作夥伴連線**：開始與信任的品牌或發行者共同作業。 [閱讀全文](/help/guide/connect/establishing-connections.md)。
4. **探索並啟動**：建立專案以識別有價值的對象區段，並在行銷活動中啟動。 [閱讀全文](/help/guide/collaborate/manage-projects.md)。

### 可用性

* Real-Time CDP Collaboration目前僅開放美國客戶使用。
* Real-Time CDP Prime和Ultimate客戶可自動使用此功能

如需詳細資訊，請閱讀：

* [Real-Time CDP Collaboration概觀](/help/guide/home.md)
* [端對端工作流程](/help/guide/end-to-end-workflow.md)
* [許可權總覽](/help/guide/permissions/overview.md)
