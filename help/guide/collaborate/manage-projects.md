---
title: 建立和管理專案
description: 瞭解如何在Adobe Real-Time CDP Collaboration中建立和管理專案
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: ae492846-bc0a-4422-86ca-577bcc1fa60c
TQID: https://experienceleague.adobe.com/IZIkK4lv29vqrah48fsJsnMOFtyh7rOo1IT2yLOW9Ec
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 9b1c698c251acb2efd2c125b64f0bd56e3b62403
workflow-type: tm+mt
source-wordcount: 702
ht-degree: 12%

---

# 建立和管理專案

{{limited-availability-release-note}}

專案是Adobe Real-Time CDP Collaboration工作流程的核心。 與共同作業人員取得聯絡後，請建立專案以執行對象重疊計算，並探索行銷活動的相關對象。

如需將對象來源至Collaboration以及用於Discover、Activate和Measure專案的概述，請參閱[對象概述](../setup/audiences-overview.md)。

>[!TIP]
>
>專案通常應該與單一行銷活動相關聯。

![顯示所有目前專案的[共同作業]儀表板。](/help/assets/collaborate/manage-view-projects/projects-overview-page.png){zoomable="yes"}

您可以使用篩選器來檢視您已與特定共同作業人員開始的專案，如下所示：

![使用單一共同作業人員的專案篩選檢視。](/help/assets/collaborate/manage-view-projects/filtered-project-view.png){zoomable="yes"}

## 建立專案 {#create-project}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_create_project_advertisername_amc"
>title="廣告商名稱 (Amazon Marketing Cloud)"
>abstract="對於 Amazon Marketing Cloud (AMC) 連線，此欄位代表您 Amazon Ads 登入有權存取的 AMC 執行個體。 其不會反映廣告商名稱。 若未列出必要的執行個體，請聯絡您的 Amazon Marketing Cloud 管理員要求存取權。"

若要建立專案，您必須先與共同作業人員[建立連線](/help/guide/connect/establishing-connections.md)。 建立連線後，您可以與該共同作業人員建立專案。

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_projects_advertisername"
>title="廣告商名稱"
>abstract="從下拉式選單中選取廣告商名稱。 此選項由發佈者在連線設定中預先設定，以確保與其系統的相容性。"

導覽至&#x200B;**[!UICONTROL 共同作業]**，然後導覽至&#x200B;**[!UICONTROL 我的專案]**。 如果這是您的第一個專案，您可以選取&#x200B;**[!UICONTROL 建立專案]**。 否則，您可以選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） 隨時建立新專案。

![選取加號或建立專案以設定新專案。](/help/assets/collaborate/manage-view-projects/create-project.png){zoomable="yes"}

**[!UICONTROL 建立專案]**&#x200B;對話方塊就會顯示。 透過下拉式清單，選取您正在建立專案的&#x200B;**[!UICONTROL 共同作業人員]**。 如果您是發佈者，且在連線設定期間設定了廣告商名稱，則可以選取&#x200B;**[!UICONTROL 廣告商名稱]**。

>[!NOTE]
>
> 如果您在連線設定中設定了單一廣告商名稱，預設會顯示該名稱。 如果未設定廣告商名稱，則會預先選取廣告商的&#x200B;**[!UICONTROL 名稱]**&#x200B;作為&#x200B;**[!UICONTROL 廣告商名稱]**。

![建立專案對話方塊，其中已選取共同作業人員，並反白顯示廣告商名稱。](/help/assets/collaborate/manage-view-projects/create-project-advertiser-names.png){zoomable="yes"}

接下來，為您的專案新增&#x200B;**[!UICONTROL 專案名稱]**&#x200B;和&#x200B;**[!UICONTROL 描述]**。 然後，選取要代表專案的影像。 此影像有助於區分專案概觀頁面中的專案。 完成後，選取&#x200B;**[!UICONTROL 建立]**&#x200B;以建立專案。

![設定新專案所需的選項](/help/assets/collaborate/manage-view-projects/create-project-required-info.png){zoomable="yes"}

您現在可以根據連線設定期間選取的使用案例，檢視您的新專案、其詳細資料和可用區段。

![專案概述工作區。](/help/assets/collaborate/manage-view-projects/project-overview.png){zoomable="yes"}

## 管理行銷活動ID {#manage-campaign-id}

**行銷活動識別碼**&#x200B;會將您的專案連結至特定行銷活動，且是[產生測量報告](./measure.md#create-measurement-report)的必要專案。 如果您使用相同共同作業人員執行數個行銷活動，可以將多個行銷活動ID新增至一個專案。 所有這些行銷活動都可在報表中選擇。

- **發行者**：在執行報表之前，請先在Collaboration UI中輸入或更新行銷活動ID和相關名稱。
- **廣告商**：請要求您的共同作業人員（發行者）視需要新增行銷活動ID。

若要新增或更新行銷活動ID，請導覽至&#x200B;**[!UICONTROL 共同作業]**&#x200B;工作區，然後在相關專案卡中選取&#x200B;**[!UICONTROL 檢視]**。

![在專案卡片中，以檢視選項突出顯示的共同作業工作區。](/help/assets/collaborate/manage-view-projects/view-project.png){zoomable="yes"}

對應的&#x200B;**[!UICONTROL 專案概述]**&#x200B;工作區會以&#x200B;**[!UICONTROL 促銷活動ID和名稱]**&#x200B;區段出現，其中列出連結至專案的所有促銷活動。 如果您尚未新增行銷活動，請選取&#x200B;**[!UICONTROL 新增]**。 如果行銷活動已存在，請選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以更新詳細資訊或新增其他行銷活動。

![專案概述工作區顯示「行銷活動ID」和「名稱」區段，並反白顯示「編輯」選項。](/help/assets/collaborate/manage-view-projects/edit-campaign-id.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 行銷活動識別碼和名稱]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL 新增行銷活動識別碼]**&#x200B;以新增一列，您可在此輸入行銷活動詳細資料。

![在選取[新增行銷活動ID]選項之後，顯示空白行銷活動列的行銷活動ID和名稱對話方塊。](/help/assets/collaborate/manage-view-projects/add-campaign-row.png){zoomable="yes"}

提供&#x200B;**[!UICONTROL 促銷活動識別碼]**&#x200B;和&#x200B;**[!UICONTROL 促銷活動名稱]**，然後選取&#x200B;**[!UICONTROL 儲存]**。

![顯示新行銷活動詳細資料和「儲存」選項的行銷活動ID和名稱對話方塊已反白顯示。](/help/assets/collaborate/manage-view-projects/save-campaign-id.png){zoomable="yes"}

檢查&#x200B;**[!UICONTROL 行銷活動ID和名稱]**&#x200B;區段以檢視您的最新行銷活動和最近的變更。 您現在可以使用新的Campaign ID來產生測量報表。

![專案概述工作區會顯示更新的行銷活動ID和名稱區段。](/help/assets/collaborate/manage-view-projects/view-updated-campaigns.png){zoomable="yes"}
