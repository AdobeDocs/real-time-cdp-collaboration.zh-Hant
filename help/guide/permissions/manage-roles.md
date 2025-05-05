---
title: 透過許可權管理角色
description: 瞭解可讓您存取Real-Time CDP Collaboration UI中不同元件的所有可用角色資源。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: 56872a2cd91ae040aba51ed5784c86b055f88756
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# 管理角色 {#manage-roles}

{{limited-availability-release-note}}

若要管理Real-Time CDP Collaboration UI不同元件的使用者存取權，[管理員](./manage-user-access.md#system-admin-gain-access)可以定義並指派角色。 角色定義系統管理員或使用者對貴組織中[資源](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/access-control/home#permissions){target="_blank"}的存取權。 本指南將提供Real-Time CDP Collaboration所提供標準角色的資訊，以及可指派給自訂角色的個別許可權。

若要開始管理角色，管理員需要存取Experience Platform產品。 如需取得管理存取權或取得Experience Platform存取權的資訊，請參閱[管理使用者存取權](./manage-user-access.md#manage-user-access-through-permissions)指南。

## 標準角色 {#standard-roles}

提供給您的兩個標準角色可填入兩個常見的存取控制使用案例。 這些是「唯讀」角色，表示無法加以自訂。

| 角色名稱 | 角色說明 | 權限 |
| --- | --- | --- | 
| Collaboration管理員 | 此為「完全存取」許可權，包含全部15個許可權。 這可讓使用者讀取、建立及編輯所有資料。 它也能讓您存取Experience Platform中的&#x200B;**[!UICONTROL Prod]**&#x200B;沙箱，好讓您將對象匯入Real-Time CDP Collaboration。 | 全部來自下表。 |
| Collaboration檢視器 | 此為唯讀存取許可權。 使用者可以讀取和探索資料、活動、連線等。 它也能讓您存取Experience Platform中的&#x200B;**[!UICONTROL Prod]**&#x200B;沙箱，好讓您將對象匯入Real-Time CDP Collaboration。 | 下表中的所有讀取許可權。 |

{style="table-layout:auto"}

## 建立特定的存取角色 {#specific-access-roles}

您可能會想要建立其他角色，為不同使用者提供不同等級的存取權。 建立角色時，您可以選取&#x200B;**[!UICONTROL 共同作業]**&#x200B;資源中的特定許可權，以管理不同的存取層級。 若要瞭解如何建立和管理角色，請參閱[角色](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"}指南。

>[!NOTE]
> 若要存取Real-Time CDP Collaboration，使用者必須擁有Experience Platform中&#x200B;**[!UICONTROL Prod]**&#x200B;沙箱的存取權。 若要授與使用者存取此沙箱的許可權，必須將他們指派給&#x200B;**[!UICONTROL 沙箱]**&#x200B;資源中包含&#x200B;**[!UICONTROL Prod]**&#x200B;許可權的角色。

以下是Collaborations資源中的可用許可權清單：

| 高階許可權 | 說明 |
| --- | --- |
| 管理Collaboration執行個體 | 檢視、建立、更新及刪除組織的共同作業執行個體。 探索其他組織的共同作業執行個體。 |
| 讀取Collaboration執行個體 | 讀取組織的共同作業執行個體並探索其他組織的共同作業執行個體。 |
| 管理連線邀請 | 檢視、建立及刪除貴組織所起始的連線邀請。 接受並拒絕其他組織所起始的連線邀請。 |
| 讀取連線邀請 | 檢視連線邀請。 |
| 管理Collaboration連線 | 廣告商可以檢視、建立和更新設定，以及提交和刪除連線。 發行者可以檢視、接受或拒絕連線。 |
| 讀取Collaboration連線 | 檢視連線。 |
| 管理受眾資料 | 入門和探索對象。 更新公開、私人和自訂對象，並管理對象詳細目錄中繼資料設定。 |
| 讀取對象資料 | 閱讀和探索對象。 |
| 管理測量資料 | 上線、更新及刪除測量資料。 |
| 讀取測量資料 | 讀取測量資料。 |
| 管理專案 | 檢視、建立、更新和刪除任何探索、共用、啟用和測量活動的專案。 |
| 讀取專案 | 檢視任何探索、共用、啟用和測量活動的專案。 |
| 讀取使用者活動 | 讀取使用者活動。 |
| 匯出使用者活動 | 匯出使用者活動。 |
| 閱讀Collaboration信用監控 | 組織與執行環境層次的信用監控。 |

{style="table-layout:auto"}

## 後續步驟

建立可定義Real-Time CDP Collaborations存取權的角色後，您需要[將角色](./manage-user-access.md#assign-a-role)指派給管理員和使用者。 如需管理角色的完整概觀，請參閱[角色的管理許可權](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/access-control/abac/permissions-ui/permissions)指南。
