---
title: 跟踪您的積分消耗活動
description: 了解如何在即時 CDP 協作中跟踪組織的配額消耗活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: 1e8c2fdb3294111562f206ac141cfa39d5193c6c
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 追蹤您的信用沖銷活動

{{limited-availability-release-note}}

使用「我的活動&#x200B;**[!UICONTROL 」標籤]**，監視並追蹤貴組織在所有共同作業活動中的預估信用耗用量。 此功能提供在不同連線和活動中如何使用積分的詳細深入分析，可幫助您有效管理資源。

>[!IMPORTANT]
>
>信用沖銷表格會依日期進行舍入與彙總，以便進行監控。 **[!UICONTROL 我的活動]**&#x200B;儀表板中的數字代表&#x200B;*預估的*&#x200B;信用消耗。 用於計費的&#x200B;*實際*&#x200B;信用耗用已在內部系統中進行追蹤，並可應您的請求提供。 請聯絡您的Adobe代表以取得該資訊。

若要存取您的預估信用消耗活動，請瀏覽至主要導覽中的&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的活動]**&#x200B;索引標籤。

![顯示積分消耗詳細資訊的「我的活動」儀錶板](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>“ **[!UICONTROL 我的活動]** 視圖不包括有關實時協作 CDP 用戶界面不同部分中用戶作的信息。 [使用審核日誌](/help/guide/setup/audit-logs.md)功能獲取該資訊。

## 了解您的活動控制面板

活動儀表板显示組織内所有耗資作的綜合清單。 每一行代表一個不同的活動，並提供有關配額使用方式的關鍵信息：

>[!NOTE]
>
>**[!UICONTROL 對象管理]**&#x200B;活動未與另一個共同作業人員建立關聯，因此這些活動型別的&#x200B;**[!UICONTROL 連線識別碼]**&#x200B;和&#x200B;**[!UICONTROL 連線名稱]**&#x200B;欄表示&#x200B;**[!UICONTROL N/A]**&#x200B;值。

| 欄 | 說明 |
|--------|-------------|
| **[!UICONTROL 日期]** | 活動發生的日期，以YYYY/MM/DD格式顯示。 |
| **[!UICONTROL 連線ID]** | 與信用消耗活動關聯的每個連接的唯一標識符，表示為字母數位字符串。 |
| **[!UICONTROL 線上名稱]** | 與連接關聯的協作者的名稱以及消耗配額活動。 |
| **[!UICONTROL 活動]** | 執行的活動類型，例如&#x200B;**Activation - 共享**、**Activation – 傳出****或觀眾管理**。 |
| **[!UICONTROL 已使用的積分總數]** | 活動沖銷的銷退折讓總數。 |
| **[!UICONTROL 我的信用份額]** | 貴組織用於活動的積分部分。 |

{style="table-layout:auto"}

## 活動型別 {#types-of-activities}

**[!UICONTROL 活動]**&#x200B;資料行顯示不同的信用消耗作業型別。

* **[!UICONTROL 受眾管理]**：將受眾導入即時 CDP 協作時會消耗配額。 積分會根據在Real-Time CDP Collaboration中為所有對象編制索引的ID數量（以百萬為單位），以及該索引在整個計費期間的頻率（每日、每三天或每週）來使用。 閱讀更多有關匯入和管理物件](/help/guide/setup/onboard-audiences.md)的資訊[。
* **[!UICONTROL Activation - 共享]** – 積分消耗作為整個帳單期間從即時 CDP 協作激活的 ID 數量的函數。 閱讀有關在即時CDP協作中共用](/help/guide/collaborate/share.md)和[啟動受眾](/help/guide/collaborate/activate.md)的更多資訊[。
* **[!UICONTROL Activation - 出口]** – 積分消耗作為整個帳單期間從即時 CDP 協作激活的 ID 數量的函數。 閱讀有關在即時CDP協作中共用](/help/guide/collaborate/share.md)和[啟動受眾](/help/guide/collaborate/activate.md)的更多資訊[。


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
