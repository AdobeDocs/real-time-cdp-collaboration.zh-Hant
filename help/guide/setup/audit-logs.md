---
title: 稽核記錄
description: 瞭解如何使用Real-Time CDP Collaboration中的稽核記錄功能來追蹤使用者活動和變更。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# 稽核記錄

{{limited-availability-release-note}}

為了提高系統中所執行活動的透明度和可見度，您可以在Adobe Experience Platform中以稽核記錄的形式稽核各種服務和功能的使用者活動。 這些記錄形成了稽核軌跡，可以幫助對Adobe Real-Time CDP Collaboration中的問題進行疑難排解，並幫助您的企業有效地遵守公司資料管理政策和監管要求。

基本上，稽核記錄會告知&#x200B;*誰*&#x200B;執行了&#x200B;*什麼*&#x200B;動作，以及&#x200B;*何時*。 記錄中記錄的每個動作都包含中繼資料，其指出動作型別、日期和時間、執行動作之使用者的電子郵件ID，以及與動作型別相關的其他屬性。

使用Collaboration中的稽核記錄功能，追蹤平台內的使用者活動和變更。 此功能已與Experience Platform稽核服務整合，且此功能的UI位於Experience Platform中。

![稽核記錄功能的高階概觀畫面。](/help/assets/setup/audit-logs/audit-logs-overview.png)

如需稽核記錄的完整資訊，請瀏覽[Experience Platform稽核記錄檔案](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}。

## 存取稽核記錄

您可以透過兩種方式存取稽核記錄，如下節所述。 這兩個選項都會顯示稽核記錄清單，這些記錄會擷取在Collaboration內執行的各種活動。

### 從Collaboration使用者介面存取稽核記錄

1. 導覽至Collaboration中&#x200B;**[!UICONTROL 設定]**&#x200B;工作區中的&#x200B;**[!UICONTROL 我的活動]**&#x200B;索引標籤。
2. 選取頁面頂端文字中的Experience Platform連結。

![從Collaboration的[我的活動]索引標籤存取稽核記錄。](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### 直接在Experience Platform使用者介面中存取稽核記錄

1. 導覽至[Experience Platform](https://platform.adobe.com/)，然後從左側功能表選取&#x200B;**[!UICONTROL 稽核]**&#x200B;區段。 如果您無法檢視稽核記錄，請聯絡貴組織的系統管理員以取得必要的許可權。

![從Experience Platform存取稽核記錄。](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## 檢視及使用稽核記錄

若要檢視稽核記錄：

1. 導覽至Experience Platform中的&#x200B;**[!UICONTROL 稽核]**&#x200B;區段。
2. 使用[篩選器](#filter-audit-logs)，根據您的條件縮小記錄檔的範圍。
3. 選取記錄專案以檢視詳細資訊，包括時間戳記、請求ID、資源詳細資訊和動作狀態。

![詳細的稽核記錄](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### 擷取的活動

稽核記錄會擷取有關使用者活動的詳細資訊，包括：

* **時間戳記**：以月/日/年/小時:minute上午/下午(AM/PM)格式執行動作的確切日期和時間。
* **資產名稱**：執行動作的資源名稱。
* **類別**：執行動作的資源型別。
* **動作**：執行的特定動作，例如建立或刪除。
* **使用者**：執行動作之使用者的電子郵件地址。

這些記錄會建立Collaboration執行個體中所有活動的完整追蹤，這對資料控管和法規遵循非常有用。 深入瞭解[如何在UI](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui)中管理稽核記錄。

### 篩選稽核記錄 {#filter-audit-logs}

稽核記錄UI提供數個篩選器，協助您搜尋特定記錄：

* **類別**：執行動作的資源型別，例如Collaboration執行個體或Collaboration連線邀請。
* **動作**：執行的動作型別。 可用動作取決於選取的類別。 例如，Collaboration例項的動作包括建立、更新和刪除。
* **要求識別碼**：要求的唯一識別碼。
* **使用者**：執行動作之使用者的電子郵件地址。
* **狀態**：動作的狀態，例如允許或拒絕。
* **日期範圍**：您要檢視其記錄檔的日期範圍。

深入瞭解[篩選稽核記錄](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs)。

## 優點

稽核記錄為使用Collaboration的組織提供幾個優點：

* **資料控管**：使用稽核記錄檔來確保平台內的所有活動都受到追蹤且可稽核。
* **法規遵循**：此功能提供使用者活動的追蹤，以符合法規要求。
* **疑難排解**：稽核記錄提供使用者動作的詳細記錄，以協助識別及解決問題。

## 類別和動作參考

下表提供Real-Time CDP Collaboration所有類別和動作的參考資料。

![Real-Time CDP Collaboration稽核記錄中醒目提示的可用類別。](/help/assets/setup/audit-logs/available-categories.png)

| 類別 | 動作 | 說明 |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration執行個體]** | 建立、更新、刪除 | 管理帳戶，包括建立、更新和刪除帳戶。 若要瞭解更多資訊，請閱讀[設定您的帳戶](/help/guide/setup/onboard-account.md)指南。 |
| **[!UICONTROL Collaboration連線邀請]** | 建立、更新、刪除、核准、拒絕 | 管理連線邀請，包括建立、更新、刪除、核准和拒絕邀請。 如需詳細資訊，請參閱[建立連線](/help/guide/connect/establishing-connections.md)指南。 |
| **[!UICONTROL Collaboration連線]** | 建立、更新、刪除、核准、拒絕、請求核准 | 管理連線，包括建立、更新、刪除、核准、拒絕和要求核准連線。 |
| **[!UICONTROL Collaboration資料連線]** | 建立、更新、刪除 | 管理您來源及管理對象的資料連線，包括建立、更新和刪除資料連線。 如需詳細資訊，請參閱[管理資料連線](/help/guide/setup/manage-data-connection.md)指南。 |
| **[!UICONTROL Collaboration資料實體]** | 建立、更新、刪除 | 管理Collaboration的資料實體，包括建立、更新和刪除資料實體。 此內容中的資料實體是指對象。 如需詳細資訊，請參閱[來源及管理對象](/help/guide/setup/onboard-audiences.md)指南。 |
| **[!UICONTROL Collaboration專案]** | 建立、更新、刪除 | 在Collaboration中管理專案，包括建立、更新和刪除專案。 如需詳細資訊，請參閱[管理專案](/help/guide/collaborate/manage-projects.md)指南。 |
| **[!UICONTROL Collaboration模組]** | 建立、更新、刪除 | 管理專案中的不同模組，包括在UI中建立、更新和刪除各種模組。 例如，[啟用對象](/help/guide/collaborate/activate.md)的功能。 |

{style="table-layout:auto"}

運用稽核記錄功能，您可以維護Collaboration中所有活動的清楚詳細記錄，以確保透明度和問責制。
