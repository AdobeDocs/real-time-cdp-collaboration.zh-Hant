---
title: 設計概述
description: 瞭解Real-Time CDP Collaboration中的目的地。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 5%

---

# 目的地概觀

{{limited-availability-release-note}}

目的地是用來將目標對象傳送至外部平台的整合。 這些整合可讓您啟用各行銷管道和平台上的對象，以用於行銷活動和客戶參與。

目前，目的地僅適用於Real-Time CDP Collaboration中的發佈者。 發佈者可設定目的地，以將受眾傳送至外部平台，例如Adobe Experience Platform，以用於行銷活動。 然後廣告商就可以[啟用專案中的對象](../collaborate/activate.md)，這些對象會傳送到發佈者設定的目的地。

>[!IMPORTANT]
>
>目前，當廣告商在您的專案中啟用對象時，會自動傳送至發佈者設定的目的地。 身為發行者，您&#x200B;**必須**&#x200B;在&#x200B;*您的共同作業人員啟動對象之前，先設定目的地*。 如果未設定目的地，則會將對象傳送給您，並顯示在專案的「**[!UICONTROL 啟用]**」標籤中，但不會啟用。

## 設定目的地 {#configure-destinations}

若要設定目的地，請導覽至&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的目的地]**&#x200B;索引標籤。 在這裡，您可以檢視所有可用的目的地。

>[!NOTE]
>
> 目前，Real-Time CDP Collaboration中只有Adobe Experience Platform可做為自助目的地。 如果您有興趣設定Amazon S3或Snowflake之類的目的地，請聯絡您的Adobe代表。

![設定工作區中的「我的目的地」索引標籤顯示可用的目的地。](/help/assets/destinations/overview/my-destinations-overview.png)

若要開始設定目的地，請在您選擇的目的地中選取&#x200B;**[!UICONTROL 設定]**&#x200B;選項。 如需設定特定目的地的詳細資訊，請參閱[可用目的地](#available-destinations)表格中的指南。

![針對Adobe Experience Platform目的地反白顯示「我的目的地」工作區與「設定」選項。](/help/assets/destinations/overview/my-destinations-set-up.png)

### 可用的目的地 {#available-destinations}

下列目的地可用於Real-Time CDP Collaboration中的設定。 若要檢視該目的地的組態指南，請在下表中選取目的地名稱。 如果您想要設定目前無法使用的目的地，請聯絡您的Adobe代表。

| 目標 | 可用性 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 可用 |
| Amazon S3 | 即將推出。 |
| Snowflake | 即將推出。 |
| Google Cloud Storage | 即將推出。 |
| Azure Blob 儲存體 | 即將推出。 |

## 後續步驟

設定目的地後，您就可以開始[啟用專案中的目標對象](../collaborate/activate.md)。
