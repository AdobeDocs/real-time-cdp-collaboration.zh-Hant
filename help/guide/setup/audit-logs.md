---
title: 稽核記錄
description: 瞭解如何使用Real-Time CDP Collaboration中的稽核記錄功能來追蹤使用者活動和變更。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
TQID: https://experienceleague.adobe.com/zb09-bUpxJ2VPDknETHeayMuLpNRCaQ2VTnV9QnTRgE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 950
ht-degree: 2%

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

Audit logs provide several benefits for organizations using Collaboration:

* **Data Governance**: Use audit logs to ensure that all activities within the platform are tracked and auditable.
* **Regulatory Compliance**: The feature provides a trail of user activities to meet regulatory requirements.
* **Troubleshooting**: Audit logs assist in identifying and resolving issues by providing detailed logs of user actions.

## Categories and actions reference

The table below provides a reference of all categories and actions for Real-Time CDP Collaboration.

![Available categories highlighted in Real-Time CDP Collaboration audit logs.](/help/assets/setup/audit-logs/available-categories.png)

| 類別 | 動作 | 說明 |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration Instance]** | create, update, delete | Manage accounts, including creating, updating, and deleting accounts. To learn morel, read the [configuring your accounts](/help/guide/setup/onboard-account.md) guide. |
| **[!UICONTROL Collaboration Connection Invite]** | create, update, delete, approve, reject | Manage connection invites, including creating, updating, deleting, approving, and rejecting invites. For more information, read the [establishing connections](/help/guide/connect/establishing-connections.md) guide. |
| **[!UICONTROL Collaboration Connection]** | create, update, delete, approve, reject, request approval | Manage connections, including creating, updating, deleting, approving, rejecting, and requesting approval for connections. |
| **[!UICONTROL Collaboration Data Connection]** | create, update, delete | Manage the data connections from where you source and manage audiences, including creating, updating, and deleting data connections. For more information, read the [managing data connections](/help/guide/setup/manage-data-connection.md) guide. |
| **[!UICONTROL Collaboration Data Entity]** | create, update, delete | Manage data entities for Collaboration, including creating, updating, and deleting data entities. Data entities in this context refers to audiences. For more information, read the [sourcing and managing audiences](/help/guide/setup/onboard-audiences.md) guide. |
| **[!UICONTROL Collaboration Project]** | create, update, delete | Manage projects within Collaboration, including creating, updating, and deleting projects. For more information, read the [managing projects](/help/guide/collaborate/manage-projects.md) guide. |
| **[!UICONTROL Collaboration Module]** | create, update, delete | Manage different modules within projects, including creating, updating, and deleting various modules in the UI. For example, the ability to [activate audiences](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

By leveraging the audit logs functionality, you can maintain a clear and detailed record of all activities within Collaboration, ensuring transparency and accountability.
