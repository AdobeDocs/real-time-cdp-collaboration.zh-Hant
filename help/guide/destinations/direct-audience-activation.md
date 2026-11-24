---
title: 直接啟用對象(1P Audience Activation) - Beta
description: 瞭解如何在沒有專案的情況下啟用您自己的或共用的第一方對象、選取目的地、檢閱欄位對應及設定啟用排程。
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%
---

# 直接啟用對象(1P Audience Activation) {#activate-audiences-directly}

在[!DNL Adobe Real-Time CDP Collaboration]中使用直接第一方(1P)對象啟用，將對象傳送至目的地而不建立專案。 啟用您擁有的對象或與您共用的對象以供第一方使用。

從設定的目的地或&#x200B;**[!UICONTROL 啟用的對象]**&#x200B;開始，然後選取對象並設定啟用排程。

若要透過共同作業專案傳送及啟用對象，請參閱[傳送及啟用專案中的對象](/help/guide/collaborate/activate.md)。

## 啟用的對象存取權 {#audience-access-for-activation}

檢查對象來源，以判斷您是否需要在啟用前獲得授權。

| 客群來源 | 存取需求 |
| --- | --- |
| 您自己的對象 | 您擁有對象。 |
| 與您共用的對象 | 您需要具有直接啟用許可權的主動授予。 提供者保留擁有權。 |

{style="table-layout:auto"}

虛擬對象授權可讓您透過參考存取共用的對象，而不需移動其資料。 然後您可以啟用對象，將其資料傳送至您選取的目的地。

如需有關授權與提供者控制項的詳細資訊，請參閱[虛擬對象存取（對象授權）](/help/guide/setup/virtual-audience-access.md)。

## 先決條件 {#prerequisites}

開始之前，請確認您擁有：

* 您擁有的受眾或透過合格第一方(1P)授權共用的受眾。
* 由您控制且支援直接啟用的已設定目的地。
* 目的地至少有一個比對索引鍵欄位對應。

若要啟用共用對象，請確認其作用中、連線範圍的授與符合[適用性條件](#check-shared-audience-access)。 使用&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區。 您不需要專案。

### 共用的受眾資格 {#check-shared-audience-access}

授權必須符合每個條件才能支援直接啟用。

| 需求 | 條件 |
| --- | --- |
| 對象許可權 | 此授權包含直接啟用許可權。 |
| 存取期間 | 授與會無限期或於指定日期範圍內有效。 |

{style="table-layout:auto"}

單獨的&#x200B;**[!UICONTROL 建立新對象]**&#x200B;許可權可讓您使用共用的對象來建立同類群組對象。 您不需要此許可權即可直接啟用。

### 目的地欄位對應 {#review-destination-field-mappings}

直接啟用會使用為您的目的地設定的相符金鑰對應。 啟用期間您沒有選取相符金鑰。

若要設定目的地，請參閱[目的地概觀](../destinations/overview.md)。

## 開始直接啟用 {#start-direct-activation}

從已設定的目的地或已啟用的對象清單開始。 Adobe Experience Platform目的地不支援第一方啟用。

### 從目的地開始 {#start-from-a-destination}

若要在選取的目的地開啟工作流程，請從設定的目的地開始。 首先，開啟&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區並選取&#x200B;**[!UICONTROL 目的地]**。

接著，從您要使用之目的地的動作中選取&#x200B;**[!UICONTROL 啟用對象]**。

工作流程隨即開啟，並選取目的地。 然後繼續[設定啟動](#configure-the-activation)。

### 從啟用的對象開始 {#start-from-activated-audiences}

若要在工作流程中選擇目的地，請從啟用的對象清單開始。 首先，開啟&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區並選取&#x200B;**[!UICONTROL 啟用的對象]**。

接著，選取頁面上的&#x200B;**[!UICONTROL 啟用對象]**&#x200B;或選取新增圖示（![新增對象啟用。](/help/assets/icons/plus.png)）以啟動工作流程 然後&#x200B;**[!UICONTROL 啟用對象]**。

工作流程會開啟，但不選取目的地。 然後繼續[設定啟動](#configure-the-activation)。

## 設定啟動 {#configure-the-activation}

Select會根據您自己的對象或與您共用的對象，為每一次啟用啟用傳送一個對象。 使用預先選取的目的地，或選擇已設定的目的地（若未選取）。 工作流程會套用針對該目的地設定的[現有對應](#review-destination-field-mappings)。

選擇何時執行啟動，然後在提交前檢閱選取的對象、目的地和排程。

## 存取變更和排定的執行 {#access-changes-and-scheduled-runs}

僅在提供者授予存取許可權時啟用共用對象。

| 存取許可權變更 | 效果 |
| --- | --- |
| 授與到期 | 系統會每小時處理過期時間。 收件者在處理到期後失去虛擬對象存取權。 |
| 提供者會撤銷授權 | 收件者會立即失去虛擬對象存取權。 |
| 已排程的啟動執行 | 系統會檢查授權。 擁有已撤銷或過期授權的受眾不符合啟用資格。 |

{style="table-layout:auto"}

到期或撤銷不會移除已傳送至目的地的對象資料。

## 後續步驟 {#next-steps}

啟用對象後，請使用這些指南來管理目的地或共同作業人員連線。

* [設定和管理目的地](/help/guide/destinations/manage-destinations.md)
* [管理共同作業人員連線](/help/guide/connect/manage-connections.md)
