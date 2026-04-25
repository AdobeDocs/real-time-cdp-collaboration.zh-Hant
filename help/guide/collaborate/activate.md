---
title: 啟用客群
description: 瞭解如何在Adobe Real-Time CDP Collaboration中啟用對象。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1012
ht-degree: 3%

---

# 啟用客群

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 啟用]**&#x200B;工作區只有在連線程式[&#128279;](../connect/establishing-connections.md#connection-settings)期間啟用&#x200B;**對象啟用**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

對象啟用可讓您啟用對象，以用於行銷活動。 根據連線[&#128279;](/help/guide/connect/establishing-connections.md#configure-connection-settings)中設定的對象啟用設定，可由共同作業人員完成啟用。 在您[探索行銷活動的最佳對象](./discover.md)後，請啟用對象以供使用。 當您啟用對象時，系統會將其傳送至共同作業人員預先設定的目的地（例如Adobe Experience Platform），以便在行銷活動中使用。 如需設定目的地的詳細資訊，請參閱[目的地概觀](../destinations/overview.md)指南。

## 啟用新對象 {#activate-new-audiences}

若要開始啟用對象，請導覽至專案工作區中的「**[!UICONTROL 啟用]**」索引標籤。

>[!IMPORTANT]
>
>**在**&#x200B;您可以啟用對象之前，您的共同作業人員&#x200B;**必須**&#x200B;設定目的地。 當您啟用對象時，會自動傳送至共同作業人員設定的目的地。 如果未設定目的地，則無法啟用對象。
>
>![當共同作業人員未設定目的地時，啟動工作區。](/help/assets/collaborate/activate/no-destination-configured.png)

選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)），或選取&#x200B;**[!UICONTROL 啟用對象]**&#x200B;選項（如果先前未傳送對象供啟用）。

![未新增任何對象的專案中的「啟動工作區」。](/help/assets/collaborate/activate/activate-new-audiences.png)

啟用對象工作流程隨即開啟，您可在其中選取要傳送給共同作業人員的對象。 使用下拉式清單來選取對象，或搜尋特定對象。 若要在選取之前檢視對象的詳細資訊，請選取&#x200B;**[!UICONTROL 瀏覽對象]**

![使用下拉式清單和瀏覽對象選項反白顯示的對象啟用工作流程。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 瀏覽對象]**&#x200B;中，您可以看到每個對象的&#x200B;**[!UICONTROL 身分計數]**、**[!UICONTROL 重疊身分]**&#x200B;和&#x200B;**[!UICONTROL 重疊%]**。

![顯示可用對象的[瀏覽對象]對話方塊。](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>啟用使用多個相符金鑰的受眾時，如果一個（或多個）相符金鑰沒有重疊、無受眾規模或低於臨界值，則整個啟用將會失敗。 啟用之前，請確認您的對象有足夠的重疊，並符合所有相符索引鍵中1000 ID的最低臨界值。

選取您要在行銷活動中啟用的對象，然後選取&#x200B;**[!UICONTROL 儲存]**。 對象現在已顯示出來，您可以看到所選對象的&#x200B;**[!UICONTROL 身分計數]**、**[!UICONTROL 重疊身分]**&#x200B;和&#x200B;**[!UICONTROL 重疊%]**。

![已顯示選定對象的Audience啟用工作流程。](/help/assets/collaborate/activate/audience-selected.png)

### 編輯比對索引鍵 {#edit-match-keys}

接著，您可以在選取的對象中選取&#x200B;**[!UICONTROL 編輯相符金鑰]**，以編輯對象的相符金鑰。 共同作業人員之間的連線最初設定時，這些選項繼承自您相符的關鍵選項。 如果選取的相符金鑰未套用至特定行銷活動，您可以移除這些相符金鑰，但您無法新增相符金鑰。

![標示「編輯相符金鑰」選項的「對象」啟用工作流程。](/help/assets/collaborate/activate/edit-match-keys.png)

**[!UICONTROL 編輯相符鍵]**&#x200B;對話方塊開啟，您可以在其中關閉不想使用的相符鍵。 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您的變更。

>[!NOTE]
>
>至少必須選取一個符合索引鍵。 在目前的版本中，唯一可用的相符金鑰是&#x200B;**[!UICONTROL 雜湊電子郵件]**，因此您無法移除此相符金鑰。

![受眾啟動工作流程中的[編輯相符金鑰]對話方塊。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 設定對象重新整理頻率 {#set-audience-refresh-frequency}

最後，設定對象重新整理的所需頻率和日期範圍。 在目前的版本中，唯一支援的頻率選項是&#x200B;**[!UICONTROL 一次]**。 **[!UICONTROL 一次]**&#x200B;頻率表示對象僅啟用一次，不會重新整理。 **[!UICONTROL 日期]**&#x200B;選項會自動填入目前的日期。

![已反白顯示「頻率」區段的Audience啟用工作流程。](/help/assets/collaborate/activate/audience-frequency.png)

對您的選取感到滿意時，請選取&#x200B;**[!UICONTROL 啟動]**&#x200B;以完成工作流程。

## 啟用儀表板 {#activate-dashboard}

在&#x200B;**[!UICONTROL 啟用]**&#x200B;標籤中，您可以檢視傳送給共同作業人員的所有對象，以及共同作業人員已啟用至目的地的所有對象。

![顯示「已傳送的對象」和「已啟動的對象」區段的「啟動」儀表板。](/help/assets/collaborate/activate/activate-dashboard.png)

## 檢視已傳送的對象 {#view-sent-audiences}

在&#x200B;**[!UICONTROL 將對象傳送至]**&#x200B;共同作業人員區段中，將會列出您傳送的所有對象。 目前，在您傳送對象後，對象會自動傳送至共同作業人員設定的目的地。 在共同作業人員的檢視中，這些對象會顯示在「**[!UICONTROL 已啟動對象]**」區段中。

在每個已傳送的對象中，您可以看到下列量度：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 名稱]** | 對象名稱。 |
| **[!UICONTROL 狀態]** | 已傳送對象的狀態。 |
| **[!UICONTROL 身分計數]** | 對象中的身分數量。 |
| **[!UICONTROL 重疊的身分]** | 此對象與共同作業人員詳細目錄中的設定檔總人口之間的重疊身分數。 |
| **[!UICONTROL 已建立]** | 最初傳送對象的日期。 |
| **[!UICONTROL 上次傳送時間]** | 上次傳送對象給共同作業人員的日期。 |
| **[!UICONTROL 相符金鑰]** | 表示用於對象的比對索引鍵。 |

## 檢視啟用的對象 {#view-activated-audiences}

在「**[!UICONTROL 啟用的對象]**」區段中，您可以看到所有已啟用至您目的地的對象。

在每個已啟用的對象中，您會看到下列量度：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 名稱]** | 對象名稱。 |
| **[!UICONTROL 狀態]** | 已啟動對象的狀態。 |
| **[!UICONTROL 身分計數]** | 根據共同作業人員傳送對象時的重疊身分啟用的身分數量。 |
| **[!UICONTROL 已建立]** | 啟用對象的日期。 |
| **[!UICONTROL 上次重新整理時間]** | 根據啟動期間選擇的重新整理排程，上次重新整理對象的日期。 |
| **[!UICONTROL 目標]** | 受眾啟用的目的地。 |
| **[!UICONTROL 相符金鑰]** | 表示用於對象的比對索引鍵。 |

## Delete sent audiences {#delete-sent-audiences}

You can delete sent audiences that you no longer want to activate. When you delete a sent audience, it is removed from the **[!UICONTROL Sent audiences to]** section, and it will no longer be activated to your collaborator&#39;s destination.

To delete a sent audience, select the **[!UICONTROL Delete]** icon (![Delete icon.](/help/assets/icons/delete.png)) next to the audience in the **[!UICONTROL Sent audiences to]** section.

![The Delete option in the Sent audiences to section.](/help/assets/collaborate/activate/delete-sent-audiences.png)

A confirmation dialog opens, asking you to confirm the deletion. 請選取「**[!UICONTROL 刪除]**」完成確認。

![The Delete confirmation dialog.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## 後續步驟 {#next-steps}

After activating audiences and running campaigns, work with the Adobe enablement and engineering team to upload measurement data and view the corresponding [measurement reports](/help/guide/collaborate/measure.md).
