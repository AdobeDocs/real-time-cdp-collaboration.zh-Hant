---
title: 管理資料連線
description: 瞭解如何在Real-Time CDP Collaboration中管理資料連線，包括比對索引鍵、排程、使用案例和對象篩選
audience: administrator, data engineer
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 管理資料連線

{{limited-availability-release-note}}

## 概觀

在Real-Time CDP Collaboration中使用資料連線，從各種來源匯入對象。 瞭解如何管理比對索引鍵及排程現有資料連線的資料匯入。 此外，您將可依不同屬性篩選對象，以獲得更精細的深入分析。

在這裡管理您的資料連線之前，您應該先在[對象上線工作流程](./onboard-audiences.md)期間進行設定。 這將確保連線正確的資料來源，以便在Real-Time CDP Collaboration中使用。

## 檢視資料連線

>[!IMPORTANT]
>
>Real-Time CDP Collaboration使用者介面目前不支援刪除資料連線。 若要刪除資料連線，請聯絡您的Adobe代表或[建立客戶支援票證](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support){target="_blank"}。

若要檢視現有的資料連線，請瀏覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 我的對象]**，然後選取&#x200B;**[!UICONTROL 管理資料連線]**。

![設定工作區並醒目提示管理資料連線。](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}

這會顯示您目前設定之所有資料連線的檢視，以及每個連線中的對象數、資料連線來源等資訊。 選取&#x200B;**[!UICONTROL 檢視資料連線]**&#x200B;以檢視此資料連線中相符金鑰、排程和對象的相關資訊。

![使用連線管理資料連線工作區檢視反白顯示的資料連線。](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}

### 比對索引鍵 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵會決定如何比對來自不同來源的資料。選擇與您的使用案例和隱私權準則最相關的比對索引鍵。"

比對索引鍵是用於調和來自不同資料來源之客群成員的識別碼。可用的比對索引鍵包括：

- **雜湊電子郵件**

您無法編輯此資料連線中使用的相符金鑰。

![資料連線工作區中反白了比對索引鍵區段。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 排程 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="排程"
>abstract="此視圖會顯示您最初為資料連線所選取的排程選項。"

您無法編輯您一開始為資料連線選取的排程選項。 如需排程選項的詳細資訊，請檢視對象匯入工作流程檔案中的[排程區段](/help/guide/setup/onboard-audiences.md#schedule)。

![強調顯示[排程]區段的資料連線工作區。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 管理對象 {#manage-audiences}

從您的資料連線中檢視對象清單時，您可以選擇檢視對象、編輯其類別或從資料連線中移除對象。

![標示受眾的資料連線工作區。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 後續步驟

管理您的資料連線後，您可以[探索您的對象與共同作業人員已發現的對象之間的重疊](/help/guide/collaborate/discover.md)。
