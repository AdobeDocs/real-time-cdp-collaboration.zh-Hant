---
title: 在「展開」中建立展開對象
description: 瞭解如何在Adobe Real-Time CDP Collaboration中使用共同作業人員的受眾族群，從種子受眾建立擴充受眾。
source-git-commit: d2585628407acf10ad8388231259c77991a9a0b0
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 1%
---
# (Beta)在「展開」中建立展開對象

使用專案中的&#x200B;**[!UICONTROL 展開]**&#x200B;標籤，從您的其中一個對象建立展開對象。 Collaboration會使用共同作業人員的受眾母體來尋找與種子受眾類似的設定檔，協助您觸及新的潛在客戶，而不會公開共同作業人員的基礎受眾資料。 產生的擴充對象會傳送給您的共同作業人員以進行啟用。

## 先決條件 {#prerequisites}

在使用&#x200B;**[!UICONTROL 展開]**&#x200B;標籤之前，您應該要：

* [來源](/help/guide/setup/onboard-audiences.md)至少一個要作為種子對象的對象
* [已連線](/help/guide/connect/establishing-connections.md)共同作業人員
* [已與該共同作業人員建立專案](/help/guide/collaborate/manage-projects.md)
* 如果您正在接收擴充對象，則設定[目的地](/help/guide/destinations/overview.md)來接收啟用的對象

## 展開概觀 {#expand-overview}

瀏覽至&#x200B;**[!UICONTROL 共同作業]** > **[!UICONTROL 我的專案]**，開啟專案，然後選取&#x200B;**[!UICONTROL 展開]**&#x200B;索引標籤。

**[!UICONTROL 展開]**&#x200B;頁面會顯示為此共同作業人員建立的展開對象，以及建立新對象的選項。

![此「展開」標籤會顯示「展開對象」表格，其中包含「名稱」、「狀態」、「模型大小」、「對象範圍」和「上次更新時間」欄。](/help/assets/collaborate/expand/expand-overview.png){zoomable="yes"}

**[!UICONTROL 擴充對象]**&#x200B;表格列出專案中建立的每個擴充對象：

| 欄 | 說明 |
|---|---|
| **[!UICONTROL 名稱]** | 擴充對象的名稱。 預設為種子對象名稱，直到編輯為止。 |
| **[!UICONTROL 狀態]** | 展開對象的目前狀態。 如需詳細資訊，請參閱[擴充對象狀態](#expansion-audience-status)。 |
| **[!UICONTROL 模型大小]** | 產生的擴充對象的大小。 在模型完成處理前無法使用。 |
| **[!UICONTROL 對象範圍]** | 用於擴充對象的對象觸及設定。 |
| **[!UICONTROL 上次更新時間]** | 上次更新擴充對象的日期和時間。 |

{style="table-layout:auto"}

### 擴充對象狀態 {#expansion-audience-status}

擴充對象會經過下列狀態：

| 狀態 | 說明 |
|---|---|
| **[!UICONTROL 正在處理]** | 擴充模式仍在產生擴充對象。 |
| **[!UICONTROL 草稿]** | 模型已完成，且展開對象已準備好供您檢閱並傳送給您的共同作業人員。 |
| **[!UICONTROL 作用中]** | 您已傳送擴充對象給共同作業人員。 |

{style="table-layout:auto"}

>[!NOTE]
>
>狀態不會即時更新。 重新開啟或重新整理&#x200B;**[!UICONTROL 展開]**&#x200B;標籤以檢視最新狀態。

## 建立擴充對象 {#create-expansion-audience}

若要建立新的擴充對象，請選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） 在&#x200B;**[!UICONTROL 展開]**&#x200B;頁面上，然後選取&#x200B;**[!UICONTROL 建立展開的對象]**。


**[!UICONTROL 產生擴充對象]**&#x200B;對話方塊就會顯示。 完成每個欄位以產生擴充對象。

![此產生對象展開對話方塊包含種子對象、對象範圍、比對索引鍵及種子對象成員欄位。](/help/assets/collaborate/expand/generate-expansion-audience-dialog.png){zoomable="yes"}

### 選取您的種子對象 {#select-seed-audience}

從&#x200B;**[!UICONTROL 選取種子對象]**&#x200B;下拉式清單中選取您自己的對象。 Collaboration會使用此對象作為在您的共同作業人員母體中尋找類似設定檔的基礎。

![產生對象展開對話方塊中的種子對象欄位。](/help/assets/collaborate/expand/select-seed-audience.png){zoomable="yes"}

### 選取比對索引鍵 {#select-match-key}

為擴充對象啟用一個比對索引鍵。 您無法啟用多個專案。

| 人員 ID | 裝置 ID |
|---|---|
| **[!UICONTROL 雜湊電子郵件]** | **[!UICONTROL 雜湊IPv4]** |
| **[!UICONTROL 雜湊電話]** | **[!UICONTROL GAID]** |
| **[!UICONTROL 忠誠度識別碼]** | **[!UICONTROL IDFA]** |
| **[!UICONTROL CRM ID]** | **[!UICONTROL Demdex ID]** |

{style="table-layout:auto"}

>[!NOTE]
>
>如果您的種子對象不包含指定的相符金鑰，則該選項顯示為停用且無法選取。

![在[產生對象]展開對話方塊中，使用可用的比對索引鍵選項的[比對索引鍵]區段。](/help/assets/collaborate/expand/select-match-key.png){zoomable="yes"}

### 選取您的對象觸及範圍 {#select-audience-reach}

使用&#x200B;**[!UICONTROL 對象觸及率]**&#x200B;下拉式清單，以平衡與您的種子對象相似性與整體觸及率。 選取&#x200B;**[!UICONTROL 平衡]**，以取得與您的種子對象相似度和整體觸及之間的中間地帶。

![在「產生對象擴展」對話方塊中，已選取「平衡」選項及其下方的描述文字的「對象範圍」欄位。](/help/assets/collaborate/expand/select-audience-reach.png){zoomable="yes"}

### 包含或排除您的種子對象 {#include-exclude-seed-audience}

使用&#x200B;**[!UICONTROL 種子對象]**&#x200B;選項按鈕，選擇您的原始種子對象是包含在最終擴充對象中還是從最終擴充對象中排除。

![使用「是」和「否」選項按鈕的「產生對象擴展」對話方塊中的「種子對象成員」欄位。](/help/assets/collaborate/expand/include-exclude-seed-audience.png){zoomable="yes"}

### 產生擴充對象 {#generate-expansion-audience}

完成所有欄位後，請選取&#x200B;**[!UICONTROL 產生擴充對象]**。 確認訊息會確認Collaboration正在建立擴充對象，而且您可以在&#x200B;**[!UICONTROL 展開]**&#x200B;頁面上追蹤其進度。

## 檢閱並傳送擴充對象 {#review-send-expansion-audience}

擴充對象的狀態更新為&#x200B;**[!UICONTROL 草稿]**&#x200B;後，請從&#x200B;**[!UICONTROL 擴充對象]**&#x200B;表格中選取其名稱以開啟。

![擴充對象詳細資訊頁面，顯示對象中繼資料、模型大小、種子對象大小和傳送按鈕。](/help/assets/collaborate/expand/expansion-audience-detail.png){zoomable="yes"}

從這個檢視，您可以：

* 編輯擴充對象名稱
* 檢視建立日期和時間
* 比較種子對象人數與產生的擴充對象人數
* 檢閱用來產生對象的比對索引鍵

準備就緒後，選取&#x200B;**[!UICONTROL 傳送給合作夥伴]**，將擴充對象傳送給您的共同作業人員。 在您傳送對象之前，對象會一直保持在&#x200B;**[!UICONTROL 草稿]**&#x200B;狀態，然後更新為&#x200B;**[!UICONTROL 作用中]**。

>[!NOTE]
>
>如果您的共同作業人員未設定目的地，將無法使用&#x200B;**[!UICONTROL 傳送給合作夥伴]**。 訊息會說明您的共同作業人員需要先設定目的地。

>[!IMPORTANT]
>
>如果未傳送給您的共同作業人員，擴充對象會在產生7天後過期。

## 接收並啟用擴充對象 {#receive-activate-expansion-audience}

當您傳送擴充對象時，Collaboration會根據為連線設定的啟用設定，將其傳送給您的共同作業人員：

* 如果已啟用&#x200B;**自動啟用**，Collaboration會自動將擴充對象啟用至共同作業人員設定的目的地，而且會顯示在他們的[啟用索引標籤](./activate.md#activated-audiences)中。
<!-- Beta release: automatic activation is the only available activation setting. Uncomment the manual activation guidance below when manual activation is introduced with the GA release. -->
<!-- * If **manual activation** is enabled, the expansion audience appears in your collaborator's [Received audiences](./activate.md#received-audiences) section of the **[!UICONTROL Activate]** tab, and your collaborator must manually activate it. -->

## 後續步驟

傳送擴充對象後，請使用[探索標籤](./discover.md)與其他對象進行比較，或使用[啟用標籤](./activate.md)追蹤其啟用。
