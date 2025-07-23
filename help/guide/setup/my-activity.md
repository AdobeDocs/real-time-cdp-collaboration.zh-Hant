---
title: 追蹤您的信用沖銷活動
description: 瞭解如何在Real-Time CDP Collaboration中追蹤貴組織的信用消耗活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 5%

---

# 追蹤您的信用沖銷活動

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90天無超額期間**：符合資格地區的客戶可享用從其地區的可用日期開始的90天無超額期間。 在此期間，客戶不會因超出其信用權益而產生超額費用。

>[!ENDSHADEBOX]

>[!IMPORTANT]
>
>信用沖銷表格會依日期進行舍入與彙總，以便進行監控。 **[!UICONTROL 我的活動]**&#x200B;儀表板中的數字代表&#x200B;*預估的*&#x200B;信用消耗。 用於計費的&#x200B;*實際*&#x200B;信用耗用已在內部系統中進行追蹤，並可應您的請求提供。 請聯絡您的Adobe代表以取得該資訊。

若要存取您的預估信用消耗活動，請瀏覽至主要導覽中的&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的活動]**&#x200B;索引標籤。

![我的活動儀表板顯示信用消耗詳細資料](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 我的活動]**&#x200B;檢視未包含使用者在Collaboration使用者介面不同部分的動作相關資訊。 使用[稽核記錄](/help/guide/setup/audit-logs.md)功能來取得該資訊。

## 瞭解您的活動儀表板 {#understand-dashboard}

活動儀表板會顯示您帳戶中所有耗用信用之作業的完整清單。 每一列代表不同的活動，並提供有關信用使用方式的主要資訊：

>[!NOTE]
>
>**[!UICONTROL 對象管理]**&#x200B;活動未與另一個共同作業人員建立關聯，因此這些活動型別的&#x200B;**[!UICONTROL 連線識別碼]**&#x200B;和&#x200B;**[!UICONTROL 連線名稱]**&#x200B;欄表示&#x200B;**[!UICONTROL -]**&#x200B;值。

| 欄 | 說明 |
|------------|--------------|
| **[!UICONTROL 日期]** | 活動發生的日期，以YYYY/MM/DD格式顯示。 |
| **[!UICONTROL 連線ID]** | 與信貸消費活動相關之每個連線的唯一識別碼，以英數字串表示。 |
| **[!UICONTROL 連線名稱]** | 與連線和信貸消費活動相關聯的共同作業人員名稱。 |
| **[!UICONTROL 活動]** | 執行的活動型別，例如&#x200B;**啟動 — 符合**、**啟動 — 輸出**&#x200B;或&#x200B;**對象管理**。 |
| 已處理&#x200B;**[!UICONTROL 個輸入]** | 為活動處理的輸入總數（例如ID或列）。 |
| **[!UICONTROL 已使用的積分總數]** | 活動沖銷的銷退折讓總數。 |
| **[!UICONTROL 我的信用份額]** | 用於活動的科目貸方部份。 |

{style="table-layout:auto"}

## 活動型別 {#types-of-activities}

**[!UICONTROL 活動]**&#x200B;資料行顯示不同的信用消耗作業型別。

* **[!UICONTROL 對象管理]**：當對象來源為Collaboration時，會使用積分。 積分會根據在Collaboration中為所有對象編制索引的ID數量（以百萬為單位）以及該索引的頻率（每日、每三天或每週）來使用。 若要深入瞭解，請參閱[來源及管理對象](/help/guide/setup/onboard-audiences.md)指南。
* **[!UICONTROL 啟用 — 符合]** — 積分會以符合併準備啟用的識別碼數目為函式使用。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 啟用 — 輸出]** — 會依據傳送至目的地的ID數量來使用積分。 此費用一律由接收對象的共同作業人員負責。 若要深入瞭解，請閱讀[啟用對象](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 測量]** — 在Collaboration中執行活動，以產生行銷活動績效報表和深入分析。 根據所有行銷活動當中活動報告的資料列數量以及產生報告的頻率 (每日、每三日或每週)，系統會消耗相應的點數。

## 管理您的信用消耗 {#manage-credit-consumption}

若要有效管理您的信用沖銷，請執行下列步驟：

1. **瞭解**&#x200B;與每個活動相關的信用耗用量。 檢查[Collaboration產品說明](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}，取得每個活動使用的積分表。
2. **定期監視**：請經常檢查您的活動儀表板，以瞭解使用模式。
3. **依連線追蹤**：使用連線名稱來識別哪些連線使用最多積分。
