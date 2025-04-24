---
title: 追蹤您的信用沖銷活動
description: 瞭解如何在Real-Time CDP Collaboration中追蹤貴組織的信用消耗活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: a69d4405c47824c8afabc84782dc9f8a9d70763a
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 追蹤您的信用沖銷活動

{{limited-availability-release-note}}

使用「我的活動&#x200B;**[!UICONTROL 」標籤]**，監視並追蹤貴組織在所有共同作業活動中的預估信用耗用量。 此功能提供在不同連線和活動中如何使用積分的詳細深入分析，可幫助您有效管理資源。

>[!IMPORTANT]
>
>信用沖銷表格會依日期進行舍入與彙總，以便進行監控。 **[!UICONTROL 我的活動]**&#x200B;儀表板中的數字代表&#x200B;*預估的*&#x200B;信用消耗。 用於計費的&#x200B;*實際*&#x200B;信用耗用已在內部系統中進行追蹤，並可應您的請求提供。 請聯絡您的Adobe代表以取得該資訊。

若要存取您的預估信用消耗活動，請瀏覽至主要導覽中的&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的活動]**&#x200B;索引標籤。

![我的活動儀表板顯示信用消耗詳細資料](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 我的活動]**&#x200B;檢視未包含在Real-Time Collaboration CDP使用者介面不同部分中的使用者動作相關資訊。 使用[稽核記錄](/help/guide/setup/audit-logs.md)功能來取得該資訊。

## 瞭解您的活動儀表板 {#understand-dashboard}

活動儀表板會顯示貴組織內所有銷退折讓作業的完整清單。 每一列代表不同的活動，並提供有關信用使用方式的主要資訊：

>[!NOTE]
>
>**[!UICONTROL 對象管理]**&#x200B;活動未與另一個共同作業人員建立關聯，因此這些活動型別的&#x200B;**[!UICONTROL 連線識別碼]**&#x200B;和&#x200B;**[!UICONTROL 連線名稱]**&#x200B;欄表示&#x200B;**[!UICONTROL N/A]**&#x200B;值。

| 欄 | 說明 |
|------------|--------------|
| **[!UICONTROL 日期]** | 活動發生的日期，以YYYY/MM/DD格式顯示。 |
| **[!UICONTROL 連線ID]** | 與信貸消費活動相關之每個連線的唯一識別碼，以英數字串表示。 |
| **[!UICONTROL 連線名稱]** | 與連線和信貸消費活動相關聯的共同作業人員名稱。 |
| **[!UICONTROL 活動]** | 執行的活動型別，例如&#x200B;**啟動 — 共用**、**啟動 — 輸出**&#x200B;或&#x200B;**對象管理**。 |
| 已處理&#x200B;**[!UICONTROL 個輸入]** | 為活動處理的輸入總數（例如ID或列），以百萬為測量單位。 這可協助您瞭解活動的成本，方法是將其與您的CPM （每千成本）建立關聯，以計算粗略成本。 |
| **[!UICONTROL 已使用的積分總數]** | 活動沖銷的銷退折讓總數。 |
| **[!UICONTROL 我的信用份額]** | 貴組織用於活動的積分部分。 |

{style="table-layout:auto"}

## 活動型別 {#types-of-activities}

**[!UICONTROL 活動]**&#x200B;資料行顯示不同的信用消耗作業型別。

* **[!UICONTROL 對象管理]**：將對象匯入Real-Time CDP Collaboration時會使用積分。 積分會根據在Real-Time CDP Collaboration中為所有對象編制索引的ID數量（以百萬為單位），以及該索引在整個計費期間的頻率（每日、每三天或每週）來使用。 深入瞭解[匯入及管理對象](/help/guide/setup/onboard-audiences.md)。
* **[!UICONTROL 啟用 — 共用]** — 在整個帳單期間，積分會根據從Real-Time CDP Collaboration啟用的識別碼數目來使用。 深入瞭解Real-Time CDP Collaboration中的[共用](/help/guide/collaborate/share.md)和[啟用對象](/help/guide/collaborate/activate.md)。
* **[!UICONTROL 啟用 — 輸出]** — 在整個帳單期間，積分會根據從Real-Time CDP Collaboration啟用的ID數量來使用。 深入瞭解Real-Time CDP Collaboration中的[共用](/help/guide/collaborate/share.md)和[啟用對象](/help/guide/collaborate/activate.md)。
* **[!UICONTROL 對象重疊]** — 使用資料草圖分析對象重疊時會使用積分。 資料草圖是受眾資料的簡化摘要，可協助判斷兩個受眾的相似程度，同時維護資料隱私權。 在探索標籤](/help/guide/collaborate/discover.md)中閱讀有關[對象重疊的詳細資訊。
* **[!UICONTROL 對象測量]** — 在Real-Time CDP Collaboration中執行活動，以產生行銷活動績效報表和深入分析。 銷退折讓是根據所有行銷活動的行銷活動報告列數和報告頻率（每日、每三天或每週）。


<!--

**[!UICONTROL Audience Overlaps]** – Credits are consumed as a function of the number of matched IDs across 2 or more shared audiences throughout the billing period. Read more about [audience overlaps in the discover tab](/help/guide/collaborate/discover.md).

Collaboration Measurement – Credits are consumed as a function of the number of rows existing in campaign reports across all campaigns, and the frequency of that reporting (daily, every three days, or weekly).

-->


## 管理您的信用消耗 {#manage-credit-consumption}

若要有效管理您的信用沖銷，請執行下列步驟：

1. **瞭解**&#x200B;與每個活動相關聯的信用消耗。 檢查[Real-Time CDP Collaboration產品說明](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}，取得每個活動使用的共同作業信用額表。
2. **定期監視**：請經常檢查您的活動儀表板，以瞭解使用模式。
3. **依連線追蹤**：使用連線名稱，識別哪些合作關係消耗的點數最多。

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
