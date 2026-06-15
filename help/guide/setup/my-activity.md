---
title: 追蹤您的點數耗用活動
description: 瞭解如何在Real-Time CDP Collaboration中檢視您組織的「信用公事包」及追蹤信用沖銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
TQID: https://experienceleague.adobe.com/hDvkKFUCBYvsX8wntcYFrL6qZTxOo5CZOWAbxNwk7mw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 681f4af47a58a2ce66b25b09d793d0b5b127df39
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 4%

---

# 追蹤您的點數耗用活動 {#track-credit-consumption-activity}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_my_activity"
>title="閱讀全文"
>abstract=""

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90天無超額期間**：符合資格地區的客戶可享用從其地區的可用日期開始的90天無超額期間。 在此期間，客戶不會因超出其信用權益而產生超額費用。

>[!ENDSHADEBOX]

若要存取您的信用公事包與信用消費活動，請瀏覽至主要導覽中的&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的活動]**&#x200B;標籤。

![「我的活動」標籤顯示「信用公事包」，其中包含已布建的信用額度、已沖銷的信用額度、可用的信用額度，以及信用沖銷活動表格。](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 我的活動]**&#x200B;檢視不包含來自Real-Time CDP Collaboration介面其他區域的使用者動作。 使用[稽核記錄](/help/guide/setup/audit-logs.md)功能來取得該資訊。

## 瞭解我的活動檢視 {#understand-dashboard}

使用&#x200B;**[!UICONTROL 我的活動]**&#x200B;檢視來監視您的信用使用情況，並檢閱使用信用額的活動。 此檢視表包含「信用公事包」和活動表格。

「銷退折讓公事包」會顯示您布建的銷退折讓、已沖銷的銷退折讓及可用的銷退折讓。

| 量度 | 說明 |
|---------|-------------|
| **[!UICONTROL 已布建的積分]** | 為您的帳戶布建的信用數。 |
| **[!UICONTROL 已使用的積分]** | 截至最近一次每日重新整理為止，您的帳戶所消耗的積分數。 |
| **[!UICONTROL 可用積分]** | 您的帳戶可用的銷退折讓數，從已布建的銷退折讓減去已沖銷的銷退折讓計算。 |

{style="table-layout:auto"}

作業表格會依日期、作業型態、處理的輸入及使用的銷退折讓列出每日銷退折讓衝減記錄：

>[!NOTE]
>
>**[!UICONTROL 對象管理]**&#x200B;活動未與另一個共同作業人員建立關聯，因此這些活動型別的&#x200B;**[!UICONTROL 連線識別碼]**&#x200B;和&#x200B;**[!UICONTROL 連線名稱]**&#x200B;欄顯示&#x200B;**[!UICONTROL -]**&#x200B;值。

| 欄 | 說明 |
|------------|--------------|
| **[!UICONTROL 日期]** | 活動發生的日期，以YYYY/MM/DD格式顯示。 |
| **[!UICONTROL 連線ID]** | 與信貸消費活動相關之每個連線的唯一識別碼，以英數字串表示。 |
| **[!UICONTROL 連線名稱]** | 與連線和信貸消費活動相關聯的共同作業人員名稱。 |
| **[!UICONTROL 活動]** | 執行的活動型別，例如&#x200B;**[!UICONTROL 啟動 — 對象存取（一次）]**、**[!UICONTROL 啟動 — 對象存取（循環）]**、**[!UICONTROL 啟動 — 對象輸出（一次）]**、**[!UICONTROL 啟動 — 對象輸出（循環）]**&#x200B;或&#x200B;**[!UICONTROL 對象管理]**。 |
| 已處理&#x200B;**[!UICONTROL 個輸入]** | 為活動處理的輸入總數（例如ID或列）。 |
| **[!UICONTROL 已使用的積分總數]** | 活動沖銷的積分總計。 |
| **[!UICONTROL 我的信用份額]** | 用於活動的科目貸方部份。 |

{style="table-layout:auto"}

## 活動型別 {#types-of-activities}

**[!UICONTROL 活動]**&#x200B;資料行顯示不同的信用消耗作業型別。

* **[!UICONTROL 對象管理]**：當對象來源為Collaboration時，會使用積分。 積分會根據在Collaboration中編制所有受眾索引ID的數量以及該索引的頻率來使用，例如每日、每三天或每週。 若要深入瞭解，請參閱[來源及管理對象](/help/guide/setup/onboard-audiences.md)指南。
* **[!UICONTROL 啟用 — 對象存取（一次）]**：對象存取透過啟用工作流程處理一次時，就會使用積分。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 啟用 — 對象存取（週期性）]**：當對象存取是透過啟用工作流程以週期性排程進行處理時，會使用積分。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 啟用 — 對象輸出（一次）]**：當對象輸出到目的地的程式通過啟用工作流程處理一次時，就會使用積分。 此活動的費用由接收對象的共同作業人員支付。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 啟用 — 對象輸出（週期性）]**：當對象輸出到目的地的處理是透過啟用工作流程按照週期排程時，會使用積分。 此活動的費用由接收對象的共同作業人員支付。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 測量]**：當您在Collaboration中產生行銷活動績效報表和深入分析時，會使用積分。 銷退折讓是根據所有行銷活動的行銷活動報告列數和報告頻率，例如每日、每三天或每週。

## 管理您的信用消耗 {#manage-credit-consumption}

若要有效管理您的信用沖銷，請執行下列步驟：

1. **瞭解**&#x200B;與每個活動相關的信用耗用量。 檢查[Collaboration產品說明](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}，取得每個活動使用的積分表。
2. **定期監視使用狀況**：檢閱您可用的學分和活動表格，以瞭解跨對象管理、對象存取、對象輸出和測量活動的使用模式。
3. **依連線追蹤**：使用連線名稱來識別哪些連線使用最多積分。
