---
title: 稽核記錄
description: 瞭解如何使用Real-Time CDP Collaboration中的稽核記錄功能來追蹤使用者活動和變更。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# 稽核記錄

{{limited-availability-release-note}}

為了提高系統中所執行活動的透明度和可見度，您可以在Adobe Real-Time Customer Data Platform (CDP)中以稽核記錄的形式稽核各種服務和功能的使用者活動。 這些記錄形成了稽核軌跡，可以幫助對Real-Time CDP Collaboration中的問題進行疑難排解，並幫助您的企業有效地遵守公司資料管理政策和監管要求。

基本上，稽核記錄會告知&#x200B;*誰*&#x200B;執行了&#x200B;*什麼*&#x200B;動作，以及&#x200B;*何時*。 記錄中記錄的每個動作都包含中繼資料，其指出動作型別、日期和時間、執行動作之使用者的電子郵件ID，以及與動作型別相關的其他屬性。

使用Real-Time CDP Collaboration中的稽核記錄功能，追蹤平台內的使用者活動和變更。 此功能已與Adobe Experience Platform稽核服務整合，且此功能的UI位於Experience Platform中。

![稽核記錄功能的高階概觀畫面](/help/assets/setup/audit-logs/audit-logs-overview.png)

如需稽核記錄的完整資訊，請瀏覽[Adobe Experience Platform稽核記錄檔案](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}。

## 存取稽核記錄

您可以透過兩種方式存取稽核記錄，如下節所述。 這兩個選項都會顯示稽核記錄清單，這些記錄會擷取在Real-Time CDP Collaboration UI內執行的各種活動

### 從Real-Time CDP Collaboration使用者介面存取稽核記錄

1. 導覽至Real-Time CDP Collaboration UI中的&#x200B;**[!UICONTROL 我的活動]**&#x200B;索引標籤。
2. 選取頁面頂端UI文字中的Experience Platform連結。

![從Real-Time CDP Collaboration UI存取稽核記錄](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### 直接在Experience Platform使用者介面中存取稽核記錄

1. 導覽至Adobe Experience Platform UI，然後從左側功能表選取&#x200B;**[!UICONTROL 稽核]**&#x200B;區段。 如果您無法檢視稽核記錄，請聯絡貴組織的系統管理員以取得必要的許可權。

![從Experience Platform UI存取稽核記錄](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## 檢視及使用稽核記錄

若要檢視稽核記錄：

1. 導覽至Adobe Experience Platform UI中的&#x200B;**[!UICONTROL 稽核]**&#x200B;區段。
2. 根據您的條件，使用篩選器縮小記錄範圍。
3. 選取記錄專案以檢視詳細資訊，包括時間戳記、請求ID、資源詳細資訊和動作狀態。

![詳細的稽核記錄](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### 擷取的活動

稽核記錄會擷取有關使用者活動的詳細資訊，包括：

* **使用者ID**：執行動作之使用者的識別碼。
* **動作**：執行的動作型別（例如，建立、更新、刪除）。
* **資源**：已修改或已建立的資源。
* **時間戳記**：執行動作的時間。

這些記錄會建立Real-Time CDP Collaboration執行個體中所有活動的完整追蹤，這對資料控管和法規遵循非常有用。 深入瞭解[如何在UI](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui)中管理稽核記錄。

### 篩選稽核記錄

稽核記錄UI提供數個篩選器，協助您搜尋特定記錄：

* **類別**：參考資源型別（例如：共同作業執行個體、連線、專案）。
* **動作**：執行的動作型別（例如：建立、刪除、更新）。
* **要求識別碼**：要求的唯一識別碼。
* **使用者電子郵件**：執行動作之使用者的電子郵件地址。
* **狀態**：動作的狀態（例如：允許、拒絕）。
* **日期範圍**：您要檢視其記錄檔的日期範圍。

深入瞭解[篩選稽核記錄](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs)。

### 用法範例

當您在Experience Platform UI中執行動作（例如管理對象、擴充連線邀請、建立專案等）時，稽核記錄會在Real-Time CDP Collaboration稽核UI中產生並顯示。 例如，會擷取建立或更新專案部分的作業，如下所示：

![建立和更新專案部分時產生的稽核記錄範例。](/help/assets/setup/audit-logs/create-project-audits.png)

## 優點

瞭解使用稽核記錄的優點：

* **資料控管**：使用稽核記錄檔來確保平台內的所有活動都受到追蹤且可稽核。
* **法規遵循**：此功能提供使用者活動的追蹤，以符合法規要求。
* **疑難排解**：稽核記錄提供使用者動作的詳細記錄，以協助識別及解決問題。

## 類別和動作參考

下表提供Real-Time CDP Collaboration所有類別和動作的參考資料。

![Real-Time CDP Collaboration稽核記錄中醒目提示的可用類別。](/help/assets/setup/audit-logs/available-categories.png)

| 類別 | 動作 | 說明 |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration執行個體]** | 建立、更新、刪除 | 管理組織帳戶，包括建立、更新和刪除組織。 深入瞭解[設定組織](/help/guide/setup/onboard-organization.md)。 |
| **[!UICONTROL Collaboration連線邀請]** | 建立、更新、刪除、核准、拒絕 | 管理連線邀請，包括建立、更新、刪除、核准和拒絕邀請。 深入瞭解[連線邀請](/help/guide/connect/establishing-connections.md)。 |
| **[!UICONTROL Collaboration連線]** | 建立、更新、刪除、核准、拒絕、請求核准 | 管理共同作業連線，包括建立、更新、刪除、核准、拒絕和請求連線的核准。 |
| **[!UICONTROL Collaboration資料連線]** | 建立、更新、刪除 | 管理共同作業的資料連線以匯入和管理對象，包括建立、更新和刪除資料連線。 深入瞭解[管理資料連線](/help/guide/setup/manage-data-connection.md)。 |
| **[!UICONTROL Collaboration資料實體]** | 建立、更新、刪除 | 管理資料實體以進行共同作業，包括建立、更新和刪除資料實體。 此內容中的資料實體是指對象。 深入瞭解[匯入及管理對象](/help/guide/setup/onboard-audiences.md)。 |
| **[!UICONTROL Collaboration專案]** | 建立、更新、刪除 | 在共同作業內管理專案，包括建立、更新和刪除專案。 深入瞭解[管理專案](/help/guide/collaborate/manage-projects.md)。 |
| **[!UICONTROL Collaboration模組]** | 建立、更新、刪除 | 在共同作業專案中管理不同的模組，包括在UI中建立、更新和刪除各種模組。 例如，[啟用對象](/help/guide/collaborate/activate.md)的功能。 |

{style="table-layout:auto"}

運用稽核記錄功能，您可以維護Real-Time CDP Collaboration執行個體中所有活動的清楚詳細記錄，以確保透明度和問責制。
