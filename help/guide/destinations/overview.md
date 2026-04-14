---
title: 設計概述
description: 瞭解Real-Time CDP Collaboration中的目的地。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
source-git-commit: 87e7feb1360d905d46032b49217f3cfee4cc6d6b
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# 目的地概觀

{{limited-availability-release-note}}

目的地是用來將目標對象傳送至外部平台的整合。 這些整合可讓您啟用各行銷管道和平台上的對象，以用於行銷活動和客戶參與。

共同作業人員可設定目的地，以將對象傳送至外部平台，例如Adobe Experience Platform，以用於行銷活動。 共同作業人員可以[啟用專案中的對象](../collaborate/activate.md)，這些對象會傳送至其連線的設定目的地。 根據連線[&#128279;](/help/guide/connect/establishing-connections.md#configure-connection-settings)中設定的對象啟用設定，可由共同作業人員完成啟用。

>[!IMPORTANT]
>
>目前，當共同作業人員啟用專案中的對象時，會自動傳送至其連線所設定的目的地。 您&#x200B;**必須**&#x200B;先設定目的地，共同作業人員才能在專案中啟用對象。

## 設定目的地 {#configure-destinations}

若要設定目的地，請瀏覽至&#x200B;**[!UICONTROL 設定]**，然後選取&#x200B;**[!UICONTROL 我的目的地]**&#x200B;索引標籤。 在這裡，您可以檢視所有可用的目的地。

>[!NOTE]
>
> 目前，Collaboration中只有Adobe Experience Platform可做為自助目的地。 如果您有興趣設定Amazon S3或Snowflake之類的目的地，請聯絡您的Adobe代表。

![設定工作區中的「我的目的地」索引標籤顯示可用的目的地。](/help/assets/destinations/overview/my-destinations-overview.png)

若要開始設定目的地，請在您選擇的目的地中選取&#x200B;**[!UICONTROL 設定]**&#x200B;選項。 如需設定特定目的地的詳細資訊，請參閱[可用目的地](#available-destinations)表格中的指南。

![針對Adobe Experience Platform目的地反白顯示「我的目的地」工作區與「設定」選項。](/help/assets/destinations/overview/my-destinations-set-up.png)

### 可用的目的地 {#available-destinations}

下列目的地可用於Collaboration中的設定。 若要檢視該目的地的組態指南，請在下表中選取目的地名稱。 如果您想要設定目前無法使用的目的地，請聯絡您的Adobe代表。

| 目標 | 可用性 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 可用 |
| [!DNL Amazon S3] | 即將推出。 |
| [!DNL Snowflake] | 即將推出。 |
| [!DNL Google Cloud Storage] | 即將推出。 |
| [!DNL Azure Blob Storage] | 即將推出。 |

>[!NOTE]
>
>此資料表中的&#x200B;**[!DNL Google Cloud Storage]**&#x200B;參考&#x200B;**目的地** （Collaboration會在啟用期間傳送對象）。 若要&#x200B;**從**&#x200B;[!UICONTROL &#x200B;設定&#x200B;]&#x200B;**工作區中的GCS儲存貯體**&#x200B;取得對象，請參閱[設定對象來源的GCS](../setup/configure-gcs-audience-sourcing.md)。

## 後續步驟

設定目的地後，您就可以開始[啟用專案中的目標對象](../collaborate/activate.md)。
