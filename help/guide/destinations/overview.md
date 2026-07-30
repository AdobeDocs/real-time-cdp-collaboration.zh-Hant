---
title: 設計概述
description: 瞭解Real-Time CDP Collaboration中的目的地。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
TQID: https://experienceleague.adobe.com/1VvnSt3Z65dfQBfXnjJJi3H0Oj9BxFStexq3icVKxkY
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 7ab1bc21a4d644e2e6a481d8de594d6a509a92a5
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 11%

---

# 目的地概觀

{{limited-availability-release-note}}

>[!NOTE]
>
>此頁面涵蓋對象在&#x200B;**到**&#x200B;之間啟用的目的地，例如雲端儲存平台。 若要在共用專案中啟用共同作業人員&#x200B;**的對象**，請參閱[啟用對象](/help/guide/collaborate/activate.md)指南。

目的地是用來將目標對象傳送至外部平台的整合。 這些整合可讓您啟用各行銷管道和平台上的對象，以用於行銷活動和客戶參與。

共同作業人員可設定目的地，以將對象傳送至外部平台，例如Adobe Experience Platform或雲端儲存平台，以用於行銷活動。 共同作業人員可以[啟用專案中的對象](../collaborate/activate.md)，這些對象會傳送至其連線的設定目的地。 根據連線[&#128279;](/help/guide/connect/establishing-connections.md#configure-connection-settings)中設定的對象啟用設定，可由共同作業人員完成啟用。

>[!IMPORTANT]
>
>目前，當共同作業人員啟用專案中的對象時，會自動傳送至其連線所設定的目的地。 您&#x200B;**必須**&#x200B;先設定目的地，共同作業人員才能在專案中啟用對象。

## 可用的目的地 {#available-destinations}

下列目的地可用於Collaboration中的設定。 若要檢視該目的地的組態指南，請在下表中選取目的地名稱。

| 目標 | 可用性 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 可用 |
| [[!DNL Amazon S3]](./manage-destinations.md) | 可用 |
| [[!DNL Snowflake]](./manage-destinations.md) | 可用 |
| [[!DNL Google Cloud Storage]](./manage-destinations.md) | 可用 |
| [[!DNL Azure Blob Storage]](./manage-destinations.md) | 可用 |
| [[!DNL SFTP]](./manage-destinations.md) | 可用 |
| [[!DNL Data Landing Zone]](./manage-destinations.md) | 可用 |

>[!NOTE]
>
>此資料表中的&#x200B;**[!DNL Google Cloud Storage]**&#x200B;參考&#x200B;**目的地** （Collaboration會在啟用期間傳送對象）。 若要&#x200B;**從**&#x200B;[!UICONTROL &#x200B;設定&#x200B;]&#x200B;**工作區中的GCS儲存貯體**&#x200B;取得對象，請參閱[設定對象來源的GCS](../setup/configure-gcs-audience-sourcing.md)。

## 後續步驟

若要設定目的地，請參閱[設定和管理目的地](./manage-destinations.md)指南。 設定目的地後，您就可以開始[啟用專案中的目標對象](../collaborate/activate.md)。
