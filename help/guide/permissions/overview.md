---
title: 訪問控制概述
description: 瞭解如何訪問Adobe Systems即時客戶數據Platform （CDP） 協作。
audience: admin
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: af48f5ea-8258-42a6-a39e-f4a4ca5b4a69
source-git-commit: 56872a2cd91ae040aba51ed5784c86b055f88756
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 2%

---

# 存取控制概覽

{{limited-availability-release-note}}

>[!IMPORTANT]
>
> 如果您是想要存取Real-Time CDP Collaboration的一般使用者，請聯絡您的系統或產品管理員以檢查現有的存取權。 如果您不知道您的系統管理員是誰，請聯絡您的Adobe代表。

Real-Time Customer Data Platform (CDP) Collaboration的存取控制是透過[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}中的Admin Console和許可權所提供。 在本指南中，您將瞭解如何根據使用案例授予自己或團隊其他成員的存取權。

## 存取控制階層 {#hierarchy}

要將存取控制配置為即時 CDP 協作，您必須&#x200B;****&#x200B;具有系統或產品管理員許可權。系統管理員沒有任何限制，並在載入過程中進行預配。 同時，產品管理員可以為其分配到的所有產品提供管理功能。 系統管理員必須授予產品管理員產品和管理存取權。

這些指南將說明如何為系統管理員、產品管理員和一般使用者設定存取權。 請參閱下表以瞭解角色之間的主要區別。

| 角色 | 說明 |
| --- | --- | 
| 系統管理員 | 組織的超級用戶。 他們能夠在Admin Console中執行所有管理任務，並有權將管理功能委派給其他使用者。 |
| 產品管理員 | 管理分配給它們的產品以及所有相關的管理功能，例如向組織添加使用者、在產品配置檔中添加或刪除使用者，以及在產品中添加或刪除其他產品管理員。 |
| 最終使用者 | 組織中使用產品的使用者。 |

{style="table-layout:auto"}

如需管理角色的詳細信息，造訪 [Adobe 支援中心](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!TIP]
>
>這些指南中管理員指的是&#x200B;****&#x200B;系統和產品管理員&#x200B;**。**

## 其他產品 {#products}

在授予即時 CDP 協作的訪問許可權之前，您需要存取多個產品，具體取決於您的 [使用案例](#use-cases)。 隨著您的進行，存取控制指南可能會通過多個用戶介面工作，每個介面在訪問配置過程中都有特定的用途。 請參閱下表，更深入地瞭解每種產品的用途。

| 產品 | 使用 |
| --- | --- |
| [Admin Console](https://adminconsole.adobe.com/) | 管理員使用它來為使用者分配產品和/或管理員訪問許可權。 |
| [權限](https://experience.adobe.com/) | 管理員使用它來分配管理員或最終使用者角色。 |
| [Experience Platform](https://platform.adobe.com/) | 管理員和一般使用者需要獲得Experience Platform產品的存取權，才能將其指派給角色。 |

## 從何處開始 {#use-cases}

現在，您已更深入地瞭解使用者和管理角色，以及不同的Experience Cloud產品，您可以開始授與Real-Time CDP Collaboration的存取權。 有兩個主要因素會影響您需要採取的步驟：

- 如果您正在指派管理員或一般使用者存取權
- 如果使用者已有權存取Experience Platform產品

請参閱下表，根據您的存取控制用例確定配置許可權所需的人員以及開始的位置。 **請務必從起點追隨教學課程直到指南結束。**

>[!TIP]
>
> 超級用戶是指系統管理員可獲得的最高訪問級別。 超級用戶可以執行所有管理任務和用戶功能。 系統管理員沒有開箱即用的產品功能，需要為自己授予適當的訪問許可權，如下圖所示。

| 使用實例 | 必要角色 | 從何處開始 |
| --- | --- | --- | 
| 沒有現有Experience Platform產品存取權的超級使用者。 | 系統管理員。 | [設定產品管理員存取權](./manage-user-access.md#admin-access) |
| 具有Experience Platform UI存取權的&#x200B;**現有 Experience Platform 系統管理員**&#x200B;的超級用戶。 | 系統管理員。 | [配置即時 CDP 協作訪問](./manage-user-access.md#RTCDP-collab-access) |
| 現有Experience Platform系統管理員&#x200B;**的超級使用者，無** Experience Platform UI存取權。 | 系統管理員。 | [設定產品管理員存取權](./manage-user-access.md#admin-access) |
| 新產品管理員的產品管理員許可權和即時CDP協同作業訪問許可權。 | 系統管理員。 | [設定產品管理員存取權](./manage-user-access.md#admin-access) |
| 現有 Experience Platform 產品管理員&#x200B;****&#x200B;具有Experience Platform UI訪問許可權的即時 CDP 協作訪問許可權。 | 系統管理員或產品管理員。 | [配置即時 CDP 協作訪問](./manage-user-access.md#RTCDP-collab-access) |
| 現有 Experience Platform 產品管理員 **的即時 CDP 協作訪問許可權，無需** Experience Platform UI訪問許可權。 | 系統管理員或產品管理員。 | [設定用戶訪問許可權](./manage-user-access.md#user-access) |
| 新一般消費者的即時CDP協作訪問許可權。 | 系統管理員或產品管理員。 | [設定使用者存取權](./manage-user-access.md#user-access) |
| 具有Real-Time CDP Collaboration存取權的現有使用者的Experience Platform存取權。 | 系統或產品管理員。 | [設定Real-Time CDP Collaboration存取權](./manage-user-access.md#RTCDP-collab-access) |

{style="table-layout:auto"}

## 其他許可權

獲得即時 CDP 協作的訪問許可權後，您可能需要一些額外的Experience Platform許可權才能使用特定功能。

### 物件匯入 {#audience-importation}

在開始與協作者共享受眾之前，您需要將受眾導入即時 CDP 協作。 目前，匯入對象唯一支援的資料連線為Experience Platform。 若要開始，管理對象上線的使用者必須獲派包含下列&#x200B;**設定檔管理**&#x200B;資源許可權的角色：

| 權限 | 說明 |
| ---- | ---- |
| 檢視區段 | 允許用戶查看沙盤中可用受眾清單。 |
| 檢視配置文件 | 允許用戶查看可用于映射到共同作業字段的欄位。 |

在下面，您可以看到添加了上述許可權的示例角色。 有關創建或分配角色的詳細資訊，請參閱 [管理角色](./manage-roles.md) 指南。

![資源工作環境許可權中，並將檢視區段和檢視配置文件許可權添加到配置文件管理資源中。](../../assets/permissions/sample-audience-role.png)

>[!NOTE]
>
>導入受眾后，用戶可以在即時CDP協作中與受眾合作，而無需上述任何許可權。

## 後續步驟

確定從哪裡開始后，追隨使用案例的連結，以開始配置訪問許可權。 如果您想瞭解如何在這些用例之外以管理員身份配置對即時 CDP 協作的訪問許可權，請參閱 [管理用戶訪問許可權](manage-user-access.md) 指南。 要瞭解角色及其在配置對即時CDP協作的各種元件的訪問許可權方面的作用，請參閱 [管理角色](manage-roles.md) 指南。
