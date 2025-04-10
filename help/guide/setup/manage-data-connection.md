---
title: 管理資料連線
description: 瞭解如何在即時 CDP 協作中管理數據連接，包括匹配鍵、日程安排、用例和對象篩選
audience: administrator, data engineer
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 4%

---

# 管理資料連線

{{limited-availability-release-note}}

## 概觀

在即時CDP協作中使用數據連接從各種來源導入受眾。 瞭解如何為現有數據連接管理匹配鍵並計劃數據導入。 此外，您還可以按不同的屬性過濾受眾，以獲得更精細的見解。

在此處管理數據連接之前，應首先在對象載入工作流程](./onboard-audiences.md)期間[設置它們。這將確保連接正確的數據源以便在即時CDP協作中使用。

## 檢視數據連線

>[!IMPORTANT]
>
>即時 CDP 協作用戶介面目前不支援刪除數據連接。 要刪除數據連接，請聯繫您的Adobe 代表或 [創建客戶支持票證](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support){target="_blank"}。

若要視圖現有數據連接，請導航到“設置>我的受眾&#x200B;]**”，**[!UICONTROL &#x200B;然後選擇“**[!UICONTROL 管理數據連接]**”。 ****

![設定工作區並醒目提示管理資料連線。](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}

這會顯示您目前設定之所有資料連線的檢視，以及每個連線中的對象數、資料連線來源等資訊。 選擇檢視数据連接&#x200B;]**以**[!UICONTROL &#x200B;視圖有關匹配鍵、日程安排以及屬於此數據連接一部分的受眾的信息。

![管理強調顯示連接檢視數據連接工作環境數據連接。 ](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}

### 比對索引鍵 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="比對索引鍵"
>abstract="匹配鍵決定如何匹配來自不同來源的數據。 選擇與您的使用案例和隱私權準則最相關的匹配鍵。"

符合鍵是用來協調來自不同數據源之觀眾的成員的標識碼。 可用的符合鍵包括：

- **哈希電子郵件**

您無法編輯此資料連接中使用的匹配金鑰。

![資料連線工作區中反白了比對索引鍵區段。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 正在安排 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="正在安排"
>abstract="此視圖顯示您最初為数据連接選擇的計劃選項。"

您無法編輯最初為資料連接選擇的計劃選項。 有關計劃選項的詳細信息，視圖對象 [匯入工作流程文件中的計劃部分](/help/guide/setup/onboard-audiences.md#schedule) 。

![工作環境突出顯示「計劃」部分的數據連接。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 管理物件 {#manage-audiences}

從數據連接查看訪問群體清單時，可以選擇視圖訪問群體、編輯其類別或將其從數據連接中刪除。

![強調顯示與觀眾工作環境的數據連線。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 後續步驟

管理您的資料連線後，您可以[探索您的對象與共同作業人員已發現的對象之間的重疊](/help/guide/collaborate/discover.md)。
