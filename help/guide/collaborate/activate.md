---
title: 啟用客群
description: 瞭解如何將受眾傳送給共同作業人員，並手動將收到的受眾啟用至Adobe Real-Time CDP Collaboration中的目的地。
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 87a7ddb5b6ef1661e347a3dd7842523639d54859
workflow-type: tm+mt
source-wordcount: 1589
ht-degree: 2%

---

# 啟用客群

使用專案中的&#x200B;**[!UICONTROL 啟用]**&#x200B;標籤將對象傳送給您的共同作業人員、檢閱從您的共同作業人員收到的對象，並啟用收到的對象以傳送至設定的目的地。 若要從最上層&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區設定和管理目的地，請參閱[目的地概觀](../destinations/overview.md)。

>[!IMPORTANT]
>
>**[!UICONTROL 啟用]**&#x200B;索引標籤只有在連線程式[&#128279;](../connect/establishing-connections.md#connection-settings)期間啟用&#x200B;**對象啟用**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)。

使用[探索標籤](./discover.md)來識別最符合行銷活動的對象，然後傳送給您的共同作業人員。 接收共同作業人員會選取已設定的目的地，並排程要啟用的接收對象。

傳送和啟用是不同的動作。 傳送可讓您的共同作業人員存取對象。 然後，接收共同作業人員會選取目的地，並手動啟用接收的對象。

您可以使用的區段和動作取決於您的組織是傳送還是接收專案中的對象。 **[!UICONTROL 啟動]**&#x200B;索引標籤包含下列區段：

| 區域 | 說明 |
|---|---|
| **[!UICONTROL 傳送對象給[共同作業人員]]** | 您已傳送給共同作業人員的對象。 |
| **[!UICONTROL 已接收對象]** | 共同作業人員已傳送給您且可啟用的對象。 |
| **[!UICONTROL 啟用的對象]** | 收到您已啟用至目的地的對象。 |

![專案層級的「啟動」索引標籤頂端有摘要計數，並展開「傳送的對象」、「接收的對象」和「啟動的對象」區段。 每個區段都會顯示狀態計數和對象詳細資訊表格。](/help/assets/collaborate/activate/activate-dashboard.png)

## 先決條件 {#prerequisites}

在傳送或啟用對象之前，請確定：

- 受眾是來源且可供傳送。 如需詳細資訊，請參閱[Source和管理對象](../setup/onboard-audiences.md)。
- 如果您需要啟用收到的對象，則至少會設定一個目的地。 如需詳細資訊，請參閱[目的地概觀](../destinations/overview.md)。

## 傳送客群 {#send-audiences}

傳送受眾，讓您的共同作業人員擁有存取權。 傳送對象後，該對象會顯示在您的&#x200B;**[!UICONTROL 傳送給[共同作業人員]]**&#x200B;區段以及共同作業人員的&#x200B;**[!UICONTROL 已接收對象]**&#x200B;區段中。

導覽至&#x200B;**[!UICONTROL 共同作業]**，開啟專案，然後選取&#x200B;**[!UICONTROL 啟用]**&#x200B;索引標籤。

在&#x200B;**[!UICONTROL 將對象傳送至[共同作業人員]]**&#x200B;區段中，選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)）。 如果尚未傳送對象，請改為從空白顯示選取&#x200B;**[!UICONTROL 傳送對象]**。

![未傳送任何對象時，專案層級的「啟動」標籤。 空白顯示訊息說明您尚未傳送對象，並顯示[傳送對象]按鈕。](/help/assets/collaborate/activate/activate-new-audiences.png)

**[!UICONTROL 傳送對象]**&#x200B;工作流程隨即開啟。 使用對象選擇器來尋找對象，或選取&#x200B;**[!UICONTROL 瀏覽對象]**&#x200B;來比較可用的對象。

>[!IMPORTANT]
>
>只有具有超過1000個重疊身分的對象才可供啟用。 如果對象重疊接近1000身分臨界值，啟用可能會失敗。

![包含對象選擇器和「瀏覽對象」按鈕的「傳送對象」工作流程。 工作流程可讓寄件者在設定比對金鑰和存取設定之前選擇對象。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 瀏覽對象]**&#x200B;對話方塊中，檢閱每個對象的&#x200B;**[!UICONTROL 身分計數]**、**[!UICONTROL 重疊身分]**&#x200B;和&#x200B;**[!UICONTROL 重疊%]**。

![瀏覽對象對話方塊列出可用的對象，及其身分計數、重疊身分計數和重疊百分比。](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>如果對象使用多個比對索引鍵，則每個選取的比對索引鍵都必須符合必要的重疊臨界值。 使用[探索標籤](./discover.md)確認對象符合重疊需求，再傳送。

選取您要傳送的對象，然後選取[儲存]。**&#x200B;**

所選對象會以其身分和重疊資訊出現在工作流程中。

![傳送對象工作流程中，選取的對象顯示其身分計數、重疊身分計數、重疊百分比、相符金鑰以及編輯相符金鑰選項。](/help/assets/collaborate/activate/audience-selected.png)

### 編輯比對索引鍵 {#edit-match-keys}

使用為Collaborator連線設定的相符金鑰，或移除任何不適用於對象的相符金鑰。

在選取的對象中選取&#x200B;**[!UICONTROL 編輯相符金鑰]**。

![在「傳送對象」工作流程中，選取「編輯相符索引鍵」選項的對象。](/help/assets/collaborate/activate/edit-match-keys.png)

**[!UICONTROL 編輯比對索引鍵]**&#x200B;對話方塊就會顯示。 關閉任何您不想使用的相符金鑰，然後選取&#x200B;**[!UICONTROL 儲存]**。

>[!NOTE]
>
>至少必須選取一個比對索引鍵。

![「編輯相符金鑰」對話方塊具有切換控制項，可透過Collaborator連線和「儲存」按鈕取得相符金鑰。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 設定對象存取權 {#configure-audience-access}

設定傳送對象的方式，以及共同作業人員可存取對象的時間。

使用&#x200B;**[!UICONTROL 存取持續時間]**&#x200B;控制項來選取下列其中一個選項：

- **[!UICONTROL 立即傳送（一次性）]**：傳送對象一次。 接收的共同作業人員可以將其啟用一次。
- **[!UICONTROL 排程週期性對象傳送]**：在指定的存取期間重新整理對象。 使用&#x200B;**[!UICONTROL 日期範圍]**&#x200B;控制項來選取開始和結束日期。

![「傳送對象」工作流程中的「存取期間」步驟，其中包含傳送對象一次或排程週期性對象傳送的選項。 循環選項會顯示定義存取期間的日期控制項。](/help/assets/collaborate/activate/activation-frequency.png)

當對象和存取設定完成時，請選取&#x200B;**[!UICONTROL 傳送]**。

對象會顯示在您的&#x200B;**[!UICONTROL 傳送給[共同作業人員]]**&#x200B;區段中的對象。 您的共同作業人員可以在其&#x200B;**[!UICONTROL 已接收對象]**&#x200B;區段中加以檢閱。

## 檢視已傳送的對象 {#view-sent-audiences}

使用「**[!UICONTROL 傳送至[共同作業人員]]**」區段來檢閱您已傳送的對象並監視其目前的存取狀態。

每個傳送的對象會顯示下列資訊：

| 欄 | 說明 |
|---|---|
| **[!UICONTROL 對象名稱]** | 已傳送對象的名稱。 |
| **[!UICONTROL 狀態]** | 對象的目前存取狀態。 |
| **[!UICONTROL 身分計數]** | 對象中的身分數量。 |
| **[!UICONTROL 重疊的身分]** | 與共同作業人員的詳細目錄重疊的身分數量。 |
| **[!UICONTROL 已建立]** | 第一次傳送對象的日期和時間。 |
| **[!UICONTROL 上次傳送時間]** | 對象資料最近傳送給共同作業人員的日期和時間。 |
| **[!UICONTROL 存取期間]** | 傳送對象時設定的存取設定。 |
| **[!UICONTROL 相符金鑰]** | 傳送對象時使用的相符金鑰。 |

### 刪除已傳送的對象 {#delete-sent-audience}

刪除已傳送的對象，以將其從已傳送對象清單中移除，並撤銷共同作業人員的存取權。

選取刪除圖示（![刪除圖示。](/help/assets/icons/delete.png)） 在&#x200B;**[!UICONTROL 傳送對象給[共同作業人員]]**&#x200B;區段中的對象旁。

![對象列旁會顯示刪除圖示的「已傳送對象」區段。](/help/assets/collaborate/activate/delete-sent-audiences.png)

確認對話方塊隨即顯示。 請選取「**[!UICONTROL 刪除]**」完成確認。

![傳送的對象刪除確認對話方塊，說明將移除對象，共同作業人員將失去存取權，並附上「取消」和「刪除」按鈕。](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

對象會從區段移除，而您的共同作業人員會失去其存取權。

## 檢視收到的對象 {#received-audiences}

使用&#x200B;**[!UICONTROL 已接收對象]**&#x200B;區段來檢閱您的共同作業人員已傳送給您的對象。 收到的對象資料傳送至目的地前，必須先手動啟用。

每個收到的對象都會顯示下列資訊：

| 欄 | 說明 |
|---|---|
| **[!UICONTROL 對象名稱]** | 已接收對象的名稱。 |
| **[!UICONTROL 狀態]** | 對象的目前存取狀態。 |
| **[!UICONTROL 身分計數]** | 對象中的身分數量。 |
| **[!UICONTROL 重疊的身分]** | 和您的詳細目錄重疊的身分數量。 |
| **[!UICONTROL 上次資料流執行]** | 對象最近一次資料流執行的日期和時間。 |
| **[!UICONTROL 存取期間]** | 傳送對象的共同作業人員所設定的存取設定。 |
| **[!UICONTROL 相符金鑰]** | 用於對象的比對索引鍵。 |

![具有使用中及過期受眾規模的「已接收對象」區段。 每個對象列會顯示其名稱、狀態、身分資訊、上次資料流執行、存取持續時間、比對金鑰，以及用於開始啟用的新增圖示。](/help/assets/collaborate/activate/received-audiences-section.png)

### 啟用已接收的對象 {#activate-received-audience}

啟用已接收的對象，將其資料傳送至您設定的其中一個目的地。

在&#x200B;**[!UICONTROL 已接收對象]**&#x200B;區段中，選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） ，位於您要啟用的對象旁。

**[!UICONTROL 啟用對象]**&#x200B;對話方塊就會顯示。

使用&#x200B;**[!UICONTROL 目的地]**&#x200B;來選取接收對象資料的目的地。 如果目的地清單是空的，請先設定目的地，然後再繼續。 如需指示，請參閱[目的地概觀](../destinations/overview.md)。

使用&#x200B;**[!UICONTROL 日期]**&#x200B;選取啟動執行的日期，然後選取&#x200B;**[!UICONTROL 啟動]**。

![從接收對象開啟「啟用對象」對話方塊。 此對話方塊包含用於選取已設定目的地的「目的地」下拉式清單、具有行事曆控制項的「日期」欄位，以及「取消」和「啟動」按鈕。](/help/assets/collaborate/activate/activate-received-audience.png)

對話方塊關閉，且啟動會顯示在&#x200B;**[!UICONTROL 已啟動對象]**&#x200B;區段中。 已接收的對象在&#x200B;**[!UICONTROL 已接收的對象]**&#x200B;區段中仍可使用，而其存取權仍保持作用中。

## 檢視啟用的對象 {#activated-audiences}

使用「**[!UICONTROL 已啟用的對象]**」區段來確認已啟用的已接收對象，並檢閱其目的地和傳遞狀態。

每個已啟用的對象會顯示下列資訊：

| 欄 | 說明 |
|---|---|
| **[!UICONTROL 對象名稱]** | 啟用的對象名稱。 |
| **[!UICONTROL 狀態]** | 目前的啟用狀態。 |
| **[!UICONTROL 啟動計數]** | 啟用到目的地的身分數量。 |
| **[!UICONTROL 上次重新整理時間]** | 啟用的對象最近重新整理的日期和時間。 |
| **[!UICONTROL 目標]** | 接收受眾資料的目的地。 |
| **[!UICONTROL 頻率]** | 啟用頻率。 手動啟用顯示&#x200B;**[!UICONTROL 一次]**。 |
| **[!UICONTROL 日期]** | 啟動執行的日期。 |
| **[!UICONTROL 相符金鑰]** | 啟用的對象中包含的相符索引鍵。 |

![啟用對象區段具有使用中、已封存及已暫停的啟用計數。 每一列會顯示對象名稱、狀態、啟用計數、上次重新整理日期、目的地、頻率、啟用日期、比對索引鍵以及刪除圖示。](/help/assets/collaborate/activate/activated-audiences-section.png)

### 刪除已啟用的對象 {#delete-activated-audience}

刪除啟用的對象，以從&#x200B;**[!UICONTROL 啟用的對象]**&#x200B;區段移除啟用。

選取刪除圖示（![刪除圖示。](/help/assets/icons/delete.png)） 位於已啟用的對象旁。

確認對話方塊隨即顯示。 請選取「**[!UICONTROL 刪除]**」完成確認。

![啟動的對象刪除確認對話方塊說明對象將從啟動的對象清單中移除，稍後可以使用[取消]和[刪除]按鈕再次啟動。](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

啟動會從清單中移除。 您可以在接收對象的存取保持作用中時，再次啟用該對象。

## 後續步驟 {#next-steps}

傳送或啟用對象後，請在&#x200B;**[!UICONTROL 傳送給[共同作業人員]]**&#x200B;和&#x200B;**[!UICONTROL 啟用的對象]**&#x200B;區段中監視其狀態。 行銷活動完成時，請與Adobe啟用與工程團隊合作，上傳測量資料並檢視對應的[測量報告](./measure.md)。
