---
title: 客群概觀
description: 瞭解Real-Time CDP Collaboration中的對象，包括這些對象的來源。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 160bd29d89d1ce828476d68e917e0271d0852eb6
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 5%

---

# 客群概觀

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，受眾是您帶入Collaboration的使用者或客戶群組。 取得來源後，您可以使用對象來探索與共同作業人員的重疊、啟用對象，以及評估行銷活動績效。 您可以根據對象資料的存放位置，從多種來源型別取得對象，包括Adobe Experience Platform、雲端儲存和共用系統以及檔案上傳工作流程。

## 您可以對受眾執行的操作 {#audiences-in-collaboration}

將受眾來源至Collaboration後，受支援的共同作業工作流程即可使用該受眾。

在Collaboration中使用對象來：

* 比較您的對象與共同作業人員對象
* 識別重疊和商機
* 啟用客群
* 衡量結果和行銷活動績效
* 管理對象可見度和相關設定

## 對象如何融入Collaboration {#conceptual-diagram}

>[!NOTE]
>
> 下圖提供來源對象如何融入Collaboration及如何用於專案的高層級檢視。

```text
Source → Data connection → Audience → Project
                                         │
                          ┌──────────────┼──────────────┐
                          ▼              ▼              ▼
                      Discover       Activate       Measure
                                         │
                                         ▼
                                    Destination
```

## 核心概念 {#core-concepts}

以下概念說明與對象來源和共同作業工作流程相關的主要物件。

**Source**\
對象資料的來源系統或位置，例如Adobe Experience Platform、雲端儲存位置或檔案上傳。

**資料連線**\
Collaboration用來從來源存取對象資料的已設定連線。 資料連線包括來源特定的設定細節，例如驗證、欄位對應和排程。

**客群**\
來源為Collaboration且可用於專案的一組使用者或客戶。

**Connection**\
您的組織與另一個組織之間的共同作業關係。

**專案**\
共同作業人員針對支援的使用案例（例如探索、啟用和測量）一起使用對象的工作區。

**目標**\
傳送已啟動對象的外部平台或系統。

**相符金鑰**
Collaboration用來比對資料集和共同作業人員之間記錄的識別碼。 比對索引鍵支援工作流程，例如對象重疊、啟用和測量。

## 對象生命週期 {#audience-lifecycle}

在Collaboration中，您會透過資料連線來取得對象、在&#x200B;**[!UICONTROL 設定]**&#x200B;中管理對象，並在受支援使用案例的專案中使用對象。

1. **Source對象**：透過資料連線將對象資料帶入Collaboration。
2. **管理對象**：檢閱和管理對象詳細資料、可見度和相關設定。
3. **在專案中使用對象**：在支援的使用案例中使用專案中的來源對象，包括&#x200B;**Discover**、**Activate**&#x200B;和&#x200B;**Measure**。

並非每個對象都用於每個使用案例。 例如，可以在未啟動的情況下將對象來源並用於&#x200B;**Discover**，或者可以在未傳送至目的地的&#x200B;**Measure**&#x200B;工作流程中使用對象。

如需來源及管理對象的詳細資訊，請參閱[Source及管理對象](./onboard-audiences.md)。 如需有關管理資料連線的資訊，請參閱[管理資料連線](./manage-data-connection.md)。

## 對象來源 {#supported-sources}

Collaboration支援多種對象來源型別。 您選擇的來源會決定設定流程、先決條件、驗證需求、資料格式、欄位對應、重新整理行為，以及將對象帶入Collaboration的可用設定選項。

* Adobe Experience Platform
* 雲端儲存空間，包括Amazon S3、Google雲端儲存空間和Azure儲存空間
* 資料共用服務，包括Snowflake和Databricks Delta Share
* Adobe Audience Manager
* CSV檔案上傳

如需支援的來源和特定來源設定步驟清單，請參閱[來源概觀](./source-overview.md#available-sources)。

## 對象由哪些部分組成 {#match-keys}

RTCDP Collaboration中的受眾是由相符索引鍵所組成。 根據您的帳戶設定，支援的相符金鑰可包含&#x200B;**人員ID**、**裝置ID**&#x200B;和&#x200B;**合作夥伴ID**。 比對金鑰支援工作流程，例如&#x200B;**對象重疊**、**啟用**&#x200B;和&#x200B;**測量**。

若要深入瞭解，請參閱[設定比對索引鍵](../setup/onboard-account.md#set-up-match-keys)和[管理資料連線](../setup/manage-data-connection.md#match-keys)

## 在專案中使用對象 {#audiences-in-projects}

專案提供與另一個組織合作的前後關聯。 在專案中，您可以將受眾用於支援的共同作業使用案例：

* **探索**：比較對象並檢閱重疊深入分析。 檢視[探索對象重疊](../collaborate/discover.md)。
* **啟用**：啟用選取的對象以供行銷活動使用。 啟動是從專案工作區的[!UICONTROL 啟動]索引標籤啟動，並將對象傳送到連線的設定目的地。 請參閱[啟用對象](../collaborate/activate.md)。
* **量值**：檢閱與專案相關的行銷活動傳遞和轉換報告。 請參閱[測量效能](../collaborate/measure.md)。

如需建立和管理專案的詳細資訊，請參閱[建立和管理專案](../collaborate/manage-projects.md)。 如需設定目的地的相關資訊，請參閱[目的地概觀](../destinations/overview.md)。

## 後續步驟 {#next-steps}

* [檢閱可用的對象來源](./source-overview.md)
* [Source和管理對象](./onboard-audiences.md)
* [建立和管理專案](../collaborate/manage-projects.md)
* [探索對象重疊](../collaborate/discover.md)
* [啟用客群](../collaborate/activate.md)
* [測量績效](../collaborate/measure.md)
* [目的地概觀](../destinations/overview.md)
