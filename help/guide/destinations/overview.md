---
title: Desintations overview
description: Learn about destinations in Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
TQID: https://experienceleague.adobe.com/1VvnSt3Z65dfQBfXnjJJi3H0Oj9BxFStexq3icVKxkY
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 6%

---

# 目的地概觀

{{limited-availability-release-note}}

Destinations are integrations used to send targeted audiences to external platforms. These integrations enable you to activate audiences across various marketing channels and platforms for use in campaigns and customer engagement.

Collaborators can configure destinations to send audiences to external platforms, such as Adobe Experience Platform, for use in campaigns. Collaborators can then [activate audiences within a project](../collaborate/activate.md), which are sent to their connection&#39;s configured destination. 根據連線[&#128279;](/help/guide/connect/establishing-connections.md#configure-connection-settings)中設定的對象啟用設定，可由共同作業人員完成啟用。

>[!IMPORTANT]
>
>Currently, when collaborators activate audiences within a project, they are automatically sent to their connection&#39;s configured destination. You **must** configure a destination before your collaborator can activate audiences within a project.

## Configure destinations {#configure-destinations}

To configure a destination, navigate to **[!UICONTROL Setup]** and then select the **[!UICONTROL My destinations]** tab. Here, you can view all available destinations.

>[!NOTE]
>
> Currently, only Adobe Experience Platform is available as a self-serve destination within Collaboration. If you are interested in configuring a destination such as Amazon S3 or Snowflake, please contact your Adobe representative.

![The My destinations tab in the Setup workspace showing the available destinations.](/help/assets/destinations/overview/my-destinations-overview.png)

To begin configuring a destination, select the **[!UICONTROL Set up]** option within the destination of your choice. For information on configuring specific destinations, refer to the guides in the [available destinations](#available-destinations) table.

![The My destinations workspace with the Set up option highlighted for the Adobe Experience Platform desintation.](/help/assets/destinations/overview/my-destinations-set-up.png)

### Available destinations {#available-destinations}

The following destinations are available for configuration in Collaboration. To view the configuration guide for that destination, select the destination name in the table below. If you are interested in configuring a destination that is not currently available, please contact your Adobe representative.

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
