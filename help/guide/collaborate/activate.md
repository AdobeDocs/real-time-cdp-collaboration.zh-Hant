---
title: 啟用客群
description: 瞭解如何在Adobe Real-Time CDP Collaboration中啟用對象。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# 啟用客群

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 啟用]**&#x200B;工作區只有在連線程式[&#128279;](../connect/establishing-connections.md#connection-settings)期間啟用&#x200B;**對象啟用**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

Audience Activation可讓您在行銷活動中啟用對象。 啟動程式是廣告商與發佈商之間的共同作業。 在[為您的行銷活動](./discover.md)探索到最佳對象之後，對象可以啟動鎖定目標的對象。 啟用的對象會傳送至發佈者預先設定的目的地(例如Adobe Experience Platform)，以用於行銷活動。 如需設定目的地的詳細資訊，請參閱[目的地概觀](../destinations/overview.md)指南。

>[!IMPORTANT]
>
>目前，當廣告商啟用受眾時，系統會自動將受眾啟用至發佈商為其組織設定的目的地。 發佈者&#x200B;**必須**&#x200B;在&#x200B;*廣告商啟用對象之前，先設定目的地*。 如果未設定目的地，則會將對象傳送給發佈者，但無法在任何行銷活動中啟用。

## 啟用新對象

若要開始啟用對象，請導覽至專案工作區中的「**[!UICONTROL 啟用]**」索引標籤。

選取新增圖示(![新增圖示。](/help/assets/icons/plus.png))，或是&#x200B;**[!UICONTROL 啟用對象]**&#x200B;選項（如果先前未傳送對象供啟用）。

![未新增任何對象的專案中的「啟動工作區」。](/help/assets/collaborate/activate/activate-new-audiences.png)

啟用對象工作流程隨即開啟，您可在其中選取要傳送給共同作業人員的對象。 使用下拉式清單來選取對象，或搜尋特定對象。 若要在選取之前檢視對象的詳細資訊，請選取&#x200B;**[!UICONTROL 瀏覽對象]**

![使用下拉式清單和瀏覽對象選項反白顯示的對象啟用工作流程。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 瀏覽對象]**&#x200B;中，您可以看到每個對象的&#x200B;**[!UICONTROL 身分計數]**、**[!UICONTROL 重疊身分]**&#x200B;和&#x200B;**[!UICONTROL 重疊%]**。

![顯示可用對象的[瀏覽對象]對話方塊。](/help/assets/collaborate/activate/browse-audiences.png)

選取您要在行銷活動中啟用的對象，然後選取&#x200B;**[!UICONTROL 儲存]**。 對象現在已顯示出來，您可以看到所選對象的&#x200B;**[!UICONTROL 身分計數]**、**[!UICONTROL 重疊身分]**&#x200B;和&#x200B;**[!UICONTROL 重疊%]**。

![已顯示選定對象的Audience啟用工作流程。](/help/assets/collaborate/activate/audience-selected.png)

### 編輯比對索引鍵

接著，您可以在選取的對象中選取&#x200B;**[!UICONTROL 編輯相符金鑰]**，以編輯對象的相符金鑰。 共同作業人員之間的連線最初設定時，這些選項繼承自您相符的關鍵選項。 如果選取的相符金鑰未套用至特定行銷活動，您可以移除這些相符金鑰，但您無法新增相符金鑰。

![標示「編輯相符金鑰」選項的「對象」啟用工作流程。](/help/assets/collaborate/activate/edit-match-keys.png)

**[!UICONTROL 編輯相符鍵]**&#x200B;對話方塊開啟，您可以在其中關閉不想使用的相符鍵。 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您的變更。

>[!NOTE]
>
>至少必須選取一個符合索引鍵。 在目前的版本中，唯一可用的相符金鑰是&#x200B;**[!UICONTROL 雜湊電子郵件]**，因此您無法移除此相符金鑰。

![受眾啟動工作流程中的[編輯相符金鑰]對話方塊。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 設定對象重新整理頻率和間隔

最後，設定對象重新整理的所需頻率和日期範圍。 在目前的版本中，唯一支援的頻率選項是&#x200B;**[!UICONTROL 一次]**。 **[!UICONTROL 一次]**&#x200B;頻率表示對象僅啟用一次，不會重新整理。 **[!UICONTROL 日期]**&#x200B;選項會自動填入目前的日期。

![已反白顯示「頻率」區段的Audience啟用工作流程。](/help/assets/collaborate/activate/audience-frequency.png)

對您的選取感到滿意時，請選取&#x200B;**[!UICONTROL 啟動]**&#x200B;以完成工作流程。 對象現在已啟用，您可以在&#x200B;**[!UICONTROL 啟用]**&#x200B;標籤中檢視對象。 您的共同作業人員也可以在&#x200B;**[!UICONTROL 啟用]**&#x200B;索引標籤中使用此功能，以便在行銷活動中使用。

您可以編輯對象的名稱編輯圖示（![鉛筆圖示）。](/help/assets/icons/edit.png))或選取&#x200B;**[!UICONTROL 停用]**&#x200B;以停用對象。

![已啟動對象的「啟動」標籤已顯示，且「編輯」和「停用」選項已反白顯示。](/help/assets/collaborate/activate/edit-activate-audience.png)

## 檢視啟用的對象

在&#x200B;**[!UICONTROL 啟用]**&#x200B;標籤中，發佈者和廣告商都可以檢視目前啟用的對象。 目前，當廣告商啟用對象後，系統會自動將對象傳送至發佈商已設定的目的地。

![啟用標籤的總覽，展示啟用的對象。](/help/assets/collaborate/activate/activate-overview.png)

在每個已啟用的對象中，您會看到下列量度：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 啟用的身分]** | 表示對象中啟用的身分數量。 |
| **[!UICONTROL 重疊的身分]** | 表示此對象之間的重疊身分數目，以及共同作業人員詳細目錄中的設定檔總母體。 |
| **[!UICONTROL 比對索引鍵劃分]** | 顯示對象中使用的每個身分的身分計數。 例如，50萬名使用者的身分總數中，可能包括40萬名使用者中斷了雜湊電子郵件身分識別，以及10萬名使用者中斷了行動身分識別身分識別。 請注意，在此說明的範例中，同一個人可能會以其電子郵件和行動ID身分出現在對象中兩次。 |

## 後續步驟 {#next-steps}

啟用資料並執行行銷活動後，請與Adobe啟用與工程團隊合作，上傳測量資料並檢視對應的[測量報告](/help/guide/collaborate/measure.md)。
