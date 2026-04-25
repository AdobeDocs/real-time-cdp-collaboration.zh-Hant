---
title: 設定和管理目的地
description: Learn how to configure and manage destinations in Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b4b26761-46ac-420f-b9f7-6e829d67aec9
TQID: https://experienceleague.adobe.com/3JoqIEJ0ilX3NHYOVersSkaa98kgPzOhqk94UP6Xc50
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 401
ht-degree: 4%

---

# 設定和管理目的地

{{limited-availability-release-note}}

Destinations are integrations used to send targeted audiences to external platforms. These integrations enable you to activate audiences across various marketing channels and platforms for use in campaigns and customer engagement.

Collaborators can configure destinations to send audiences to external platforms, such as Adobe Experience Platform, for use in campaigns. Collaborators can then [activate audiences within a project](../collaborate/activate.md), which are sent to their connection&#39;s configured destination. 根據連線[&#128279;](/help/guide/connect/establishing-connections.md#configure-connection-settings)中設定的對象啟用設定，可由共同作業人員完成啟用。

![The My destinations tab in the Setup workspace showing an active Adobe Experience Platform destinations.](/help/assets/setup/manage-destinations/my-destinations-overview.png)

To learn more about destinations, refer to the [destinations overview](../destinations/overview.md) guide.

## Configure destinations {#configure-destinations}

Desintations are configured in the **[!UICONTROL Setup]** section of Collaboration. To configure a destination, navigate to **[!UICONTROL Setup]** and then select the **[!UICONTROL My destinations]** tab. Here, you can view all available destinations.

>[!IMPORTANT]
>
>To configure and manage desintations, your user must have a role with the **Manage Audience Data** permission assigned to them. For more information about managing roles, refer to the [manage roles](../permissions/manage-roles.md) guide.

![The My destinations tab in the Setup workspace showing the available destinations.](/help/assets/setup/manage-destinations/my-destinations.png)

The set up process for destinations is dependent on the destination you are configuring. Refer to the [available destinations](../destinations/overview.md#available-destinations) catalog to view the available destinations and their configuration guides.

>[!NOTE]
>
>Currently, only Adobe Experience Platform is available as a self-serve destination within Real-Time CDP Collaboration. If you are interested in configuring a different destination, please contact your Adobe representative.

## 刪除目的地 {#delete-destinations}

Deleting a destination removes it from your account, removes any previously sent audiences from the destination, and prevents any future audiences from being sent to that destination.

To delete a destination, navigate to the **[!UICONTROL My destinations]** tab in the **[!UICONTROL Setup]** section. Select the **[!UICONTROL Delete]** option for the destination that you want to remove.

![針對Adobe Experience Platform目的地反白顯示「我的目的地」工作區與「刪除」選項。](/help/assets/setup/manage-destinations/delete-destination.png)

確認對話方塊隨即顯示，您可以在其中確認要刪除目的地。 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以移除目的地。

![反白顯示[刪除]選項的[刪除]目的地對話方塊。](/help/assets/setup/manage-destinations/delete-destination-confirmation.png)

## 後續步驟

設定目的地後，您就可以開始透過連線共同作業，以在專案中啟用[目標對象](../collaborate/activate.md)。
