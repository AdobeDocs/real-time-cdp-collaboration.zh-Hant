---
title: 管理資料連線
description: 瞭解如何在Real-Time CDP Collaboration中管理資料連線，包括比對索引鍵、排程、使用案例和對象篩選
audience: administrator, data engineer
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 16%

---

# 管理資料連線

{{limited-availability-release-note}}

## 概觀

在Real-Time CDP Collaboration中使用資料連線，從各種來源匯入對象。 瞭解如何管理比對索引鍵及排程現有資料連線的資料匯入。 此外，您將可依不同屬性篩選對象，以獲得更精細的深入分析。

## 檢視資料連線

若要檢視現有的資料連線，請瀏覽至&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的資料連線]**&#x200B;索引標籤。 系統會顯示您目前的所有資料連線，並顯示每個連線的簡短概觀。 若要完整檢視資料連線的資訊，包括其比對索引鍵、排程詳細資料和對象，請選取對應連線上的&#x200B;**[!UICONTROL 檢視資料連線]**。

![設定工作區，顯示[我的資料連線]索引標籤檢視並反白顯示。](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 比對索引鍵 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵會決定如何比對來自不同來源的資料。選擇與您的使用案例和隱私權準則最相關的比對索引鍵。"

比對索引鍵是用於調和來自不同資料來源之客群成員的識別碼。您無法編輯您最初為資料連線選取的相符金鑰。

可用的比對索引鍵包括：

- **雜湊電子郵件**

![資料連線工作區中反白了比對索引鍵區段。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 排程 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="排程"
>abstract="此視圖會顯示您最初為資料連線所選取的排程選項。"

您無法編輯您一開始為資料連線選取的排程選項。 如需排程選項的詳細資訊，請檢視對象匯入工作流程檔案中的[排程區段](/help/guide/setup/onboard-audiences.md#schedule)。

![強調顯示[排程]區段的資料連線工作區。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 刪除資料連線

刪除資料連線將會移除整個平台的所有基礎對象、相關設定和使用情況。 此動作無法復原。

若要刪除現有的資料連線，請選取個別資料連線工作區中的刪除圖示（![刪除圖示](/help/assets/common/delete.svg)）。

![以刪除選項反白顯示的資料連線工作區。](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

確認對話方塊隨即顯示。 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以完成刪除資料連線。

![反白顯示[刪除]選項的[刪除資料連線]對話方塊。](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 管理對象 {#manage-audiences}

附加至資料連線的對象清單會顯示在工作區底部。 此清單會顯示每個對象的簡短概觀，包括其狀態、來源和連線存取。 若要編輯對象的類別、連線存取或中繼資料可見性，請選取對象名稱。 如需管理對象的完整指南，請參閱[檢視個別對象](./onboard-audiences.md#view-individual-audiences)指南。

![標示受眾的資料連線工作區。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 後續步驟

管理您的資料連線後，您可以[探索您的對象與共同作業人員已發現的對象之間的重疊](/help/guide/collaborate/discover.md)。
