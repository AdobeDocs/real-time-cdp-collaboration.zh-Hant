---
title: 透過許可權管理角色
description: 瞭解提供對即時 CDP 協作UI中不同元件的訪問許可權的所有可用角色資源。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: 56872a2cd91ae040aba51ed5784c86b055f88756
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# 管理角色 {#manage-roles}

{{limited-availability-release-note}}

要管理用戶對即時 CDP 協作UI不同元件的訪問許可權， [管理員可以](./manage-user-access.md#system-admin-gain-access) 定義和分配角色。 角色定義管理員或用戶對組織中資源](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#permissions){target="_blank"}的訪問許可權[。此指南將提供有關即時 CDP 協作中提供的標準角色的資訊，以及可分配給自定義角色的各個許可權。

要開始管理角色，管理員需要Experience Platform產品的訪問許可權。 有關獲取管理訪問許可權或獲取Experience Platform訪問許可權的信息，請閱讀 [管理用戶訪問許可權](./manage-user-access.md#manage-user-access-through-permissions) 指南。

## 標準角色 {#standard-roles}

為您提供了兩個標準角色，用於填寫兩種常見的存取控制用例。 這些是「只讀」角色，表示無法自定義。

| 角色名稱 | 角色說明 | 權限 |
| --- | --- | --- | 
| 協作經理 | 這是完全存取權限，包含全部 15 項許可權。 這允許用戶讀取、創建和編輯所有數據。 它還提供對 Experience Platform 中的 Prod ]**沙盒的**[!UICONTROL &#x200B;訪問，允許您將受眾導入即時 CDP 協作。 | 全部來自下表。 |
| 協作查看器 | 這是只讀存取權限。 用戶可以讀取和發現數據、活動、連接等。 它還提供對 Experience Platform 中的 Prod ]**沙盒的**[!UICONTROL &#x200B;訪問，允許您將受眾導入即時 CDP 協作。 | 下表中的所有讀取許可權。 |

{style="table-layout:auto"}

## 建立特定存取角色 {#specific-access-roles}

你可能希望創建其他角色，以便為不同的使用者提供不同級別的訪問許可權。 創建角色時，您可以通過在協作&#x200B;]**資源中選擇**[!UICONTROL &#x200B;特定許可權來管理不同的訪問級別。若要瞭解如何創建和管理角色，請參閱 [角色](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"} 指南。

>[!NOTE]
> 要訪問即時 CDP 協作，用戶必須有權訪問 **[!UICONTROL Experience Platform 中的 Prod]** 沙盒。 要授予用戶對此沙箱的訪問許可權，必須將其分配給包含沙箱資源中的 **[!UICONTROL Prod]** 權限的角色&#x200B;**[!UICONTROL 。]**

以下是協作資源中可用許可權清單：

| 高級許可權 | 說明 |
| --- | --- |
| 管理協作實例 | 檢視、創建、更新和刪除組織的 共同作業 例項。 Discover其他組織的共同作業例項。 |
| 讀取協作實例 | 讀取組織的 共同作業 例項並發現其他組織的共同作業例項。 |
| 管理連接邀請 | 檢視、創建和刪除組織發起的連接邀請。 接受和拒絕其他組織發起的連接邀請。 |
| 讀取連接邀請 | 檢視連接邀請。 |
| 管理協作連接 | 廣告商可以視圖、创建和更新設置，以及提交和刪除連接。 發佈者可以視圖、接受或拒絕連接。 |
| 讀取協作連接 | 檢視連接。 |
| 管理受眾數據 | 加入並發現受眾。 更新公共、私人和自定義受眾，並管理受眾清單中繼資料設置。 |
| 讀取對象數據 | 閱讀並發現受眾。 |
| 管理測量數據 | 載入、更新和刪除測量數據。 |
| 讀取測量數據 | 讀取測量數據。 |
| 管理專案 | 檢視、創建、更新和刪除任何發現、共用、啟動和度量活動的專案。 |
| 讀取專案 | 檢視任何發現、共用、啟動和測量活動的專案。 |
| 讀取用戶活動 | 讀取用戶活動。 |
| 匯出用戶活動 | 匯出用戶活動。 |
| 閱讀協作信用監控 | 組織和執行個體層面的信用監控。 |

{style="table-layout:auto"}

## 後續步驟

創建定義即時 CDP 協作存取權限的角色後，您需要 [將角色](./manage-user-access.md#assign-a-role) 分配給管理員和使用者。 有關管理角色的完整概述，請參閱 [角色](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions) 指南的管理許可權。
