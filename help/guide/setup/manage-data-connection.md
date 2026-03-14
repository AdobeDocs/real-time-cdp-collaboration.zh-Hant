---
title: 管理資料連線
description: 瞭解如何在即時CDP協作中管理資料連接，包括匹配鍵、計畫、使用案例和受眾篩選
audience: administrator, data engineer
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: 4bfa57ba36336dd835551fb846f1d567d6830bf9
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 6%

---

# 管理資料連線

{{limited-availability-release-note}}

## 概觀

在即時CDP協作中使用資料連接來源於不同平台的受眾。 瞭解如何管理匹配項和計畫現有資料連接的資料刷新。 此外，您還可以按不同屬性篩選受眾，以獲得更細的洞察力。

## 查看資料連接

要查看現有資料連接，請導航到&#x200B;**[!UICONTROL 安裝程式]**，然後選擇&#x200B;**[!UICONTROL 我的資料連接]**&#x200B;頁籤。 將顯示所有當前資料連接，其中顯示了每個連接的簡要概述。 有關資料連接資訊（包括其匹配項、計畫詳細資訊和受眾）的完整視圖，請在相應連接上選擇&#x200B;**[!UICONTROL 查看資料連接]**。

![顯示並突出顯示了「我的資料連接」頁籤視圖的設定工作區。](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 比對索引鍵 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵會決定如何比對來自不同來源的資料。 如下所示的比對索引鍵是您將來源欄位對應到的目標欄位。"

匹配項是[將源欄位映射到](./onboard-audiences.md#map-fields)的目標欄位。 要瞭解有關匹配項工作方式的詳細資訊，請參閱[匹配項](./onboard-account.md#set-up-match-keys)指南。

![突出顯示了「匹配項」部分的資料連接工作區。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 排程 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="排程"
>abstract="檢視資料連線的排程詳細資料，並根據需要編輯設定。"

查看和管理資料連接的計畫設定。 計畫確定刷新受眾的頻率。

建立資料連接後，您可以直接從資料連接工作區的&#x200B;**[!UICONTROL 計畫]**&#x200B;部分更新其刷新頻率、開始日期和結束日期。

>[!NOTE]
>
>當從Adobe Experience Platform採購觀眾時，在建立資料連接後24小時內，觀眾就可到場。 在初始採購之後，觀眾資料根據定義的頻率刷新。

有關計畫的詳細資訊，請參閱配置觀眾指南中的[計畫部分](/help/guide/setup/onboard-audiences.md#schedule)。

![資料連接的工作區，「計畫」部分突出顯示。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 編輯資料連線 {#edit-data-connection}

閱讀以下各節，瞭解如何更新匹配項和現有資料連接的計畫設定。

### 編輯比對索引鍵 {#edit-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_edit_measurement_data_connection_enrichment"
>title="擴充"
>abstract="不支援關閉濃縮。 可以改變富集連接鍵。"
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-manage-dataconnections" text="擴充"

>[!IMPORTANT]
>
>編輯資料連接的匹配項之前，請注意以下事項：
>
>* 只有為帳戶配置的匹配密鑰才能用於資料連接。
>* 此時，您可以向資料連接添加其他匹配項，但一旦啟用了匹配項，則無法刪除該匹配項。

從&#x200B;**[!UICONTROL 匹配項]**&#x200B;節中選擇&#x200B;**[!UICONTROL 編輯]**。

![選中「編輯」選項的「匹配項」部分。](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

此時將顯示確認對話框，說明對資料連接所做的任何更改都將應用於所有關聯的受眾。 選擇&#x200B;**[!UICONTROL 確定]**&#x200B;進行確認。 您可以選擇在將來跳過此確認。

![確認對話框，顯示對資料連接的任何更改都將應用於所有關聯的受眾。](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配項]**&#x200B;對話框中，可以查看源欄位與其相應目標欄位之間的現有映射（匹配項）。 您可以通過更新映射的源欄位來編輯匹配項，或添加附加的映射欄位行來填充新的匹配項。

![「匹配項」對話框，顯示源欄位和相應目標欄位之間的現有映射。](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### 添加匹配項 {#add-match-keys}

選擇&#x200B;**[!UICONTROL 添加欄位]**&#x200B;以添加新欄位行。

![選擇「添加」欄位後，「匹配項」對話框將顯示一個空的新映射欄位，可供輸入。](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

接下來，選擇空源欄位。 出現&#x200B;**[!UICONTROL 選擇源欄位]**&#x200B;對話框，其中包含&#x200B;**[!UICONTROL 標識命名空間]**&#x200B;和&#x200B;**[!UICONTROL 配置檔案屬性]**&#x200B;選項。 您可以篩選清單，並使用搜索選項查找所需的源欄位。

選擇所需的源欄位，然後是&#x200B;**[!UICONTROL 選擇]**。

![選擇了GAID選項的「選擇源」欄位對話框。](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配鍵]**&#x200B;對話框中，使用下拉菜單將新源欄位映射到目標欄位。 所有可用的目標欄位都是為Collaborator帳戶配置的匹配項。 如果您未看到所需的目標欄位，[請編輯帳戶的匹配項](./onboard-account.md#edit-match-keys)以將其添加。

如果要將非散列欄位源到散列目標欄位，例如，將純文字檔案電子郵件源欄位映射到&#x200B;**[!UICONTROL 散列電子郵件]**&#x200B;目標欄位時，請使用&#x200B;**[!UICONTROL 應用轉換]**&#x200B;選項。

![下拉菜單顯示所有可用的目標欄位以與新源欄位映射。](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

完成映射欄位後，請查看更新，然後選擇&#x200B;**[!UICONTROL 確認]**&#x200B;以應用更改。

![「匹配項」對話框，顯示已更新的欄位映射，並突出顯示「確認」選項。](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

確認對話框確認匹配項已成功更新。

### 編輯計畫 {#edit-scheduling}

建立資料連接後，您可以直接從資料連接工作區的&#x200B;**[!UICONTROL 計畫]**&#x200B;部分更新其刷新頻率、開始日期和結束日期。

您可以編輯現有資料連接的頻率，以更好地控制刷新受眾的頻率。 要編輯計畫，請從計畫卡的資料連接中選擇&#x200B;**[!UICONTROL 編輯]**。

![突出顯示了「編輯」選項的「計畫」部分。](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

此時將顯示確認對話框，說明對資料連接所做的任何更改都將應用於所有關聯的受眾。 選擇&#x200B;**[!UICONTROL 確定]**&#x200B;進行確認。 您可以選擇在將來跳過此確認。

![確認對話框，顯示對資料連接的任何更改都將應用於所有關聯的受眾。](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 計畫]**&#x200B;對話框中，選擇下拉菜單以更新&#x200B;**[!UICONTROL 頻率]**。 將刷新頻率設定為每天或每二到六天運行一次。

![擴展了「頻率」下拉框的「計畫」對話框，可顯示訪問群體刷新頻率選項。](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

接下來，如果要更新填充和刷新受眾的期間，請選擇&#x200B;**[!UICONTROL 日期範圍]**。

![顯示「日期範圍」下拉清單的「計畫」對話框已展開，以編輯訪問群體和刷新的開始和結束日期。](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

完成後，請查看更新並選擇&#x200B;**[!UICONTROL 保存]**&#x200B;以應用您所做的更改。

![突出顯示更新和保存選項的「計畫」對話框。](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## 刪除資料連線

刪除資料連接將刪除整個協作的所有基礎訪問群體、關聯設定和使用。 此動作無法還原。

要刪除現有資料連接，請在單個資料連接的工作區中選擇刪除表徵圖（![刪除表徵圖](/help/assets/common/delete.svg)）。

![帶有突出顯示的刪除選項的資料連接工作區。](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

將出現確認對話框。 選擇&#x200B;**[!UICONTROL 刪除]**&#x200B;以完成刪除資料連接。

![選中了「刪除」選項的「刪除資料連接」對話框。](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 管理受眾 {#manage-audiences}

附加到資料連接的受眾清單顯示在工作區的底部。 該清單顯示每個受眾的簡短概述，包括其狀態、源和連接訪問。 要編輯受眾的類別、連接訪問或元資料可見性，請選擇受眾的名稱。 有關管理受眾的完整指南，請參閱[查看單個受眾](./onboard-audiences.md#view-individual-audiences)指南。

![高亮顯示受眾的資料連接工作區。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 後續步驟

管理資料連接後，您可以[發現您的受眾與您的協作者已發現的受眾之間的重疊](/help/guide/collaborate/discover.md)。
