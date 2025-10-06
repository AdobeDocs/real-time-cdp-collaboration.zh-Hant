---
title: Amazon Marketing Cloud
description: 瞭解如何在Real-Time CDP Collaboration中與Amazon Marketing Cloud合作。
audience: publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 57b847c25edbf88f4708bda74be41fe6141472a7
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 4%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

與[!DNL Amazon Marketing Cloud] ([!DNL AMC])建立連線後，廣告商可以[建立專案](../manage-projects.md#create-project)以與[!DNL AMC]共同作業，以利用其進階分析功能。 建立專案後，您可以使用&#x200B;**[!UICONTROL 探索]**&#x200B;區段來比較對象深入分析，並探索行銷活動的相關對象。

>[!IMPORTANT]
>
>[!DNL AMC]唯一支援的使用案例是&#x200B;**對象探索**&#x200B;和&#x200B;**測量**。 目前，您的專案中只有&#x200B;**[!UICONTROL Discover]**&#x200B;區段可以使用[!DNL AMC]。

## 探索 {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="比較客群"
>abstract="比較您的對象與透過您的Amazon廣告觸及的所有消費者。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="相關客群"
>abstract="僅考慮Amazon曝光數，DSP鎖定對象具有最高重疊次數的區段(這些區段只能在DSP中定位)。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="已解析的 ID"
>abstract="Amazon的身分解析能夠使用您的對象資料解析的ID數量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="重疊的廣告曝光 ID"
>abstract="這代表已上傳對象中也透過Amazon Ads向廣告公開的「已解決ID」數量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="重疊 %"
>abstract="已透過Amazon Ads向廣告公開的「已解決ID」比例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="依 Amazon 廣告產品劃分"
>abstract="Amazon Ads贊助產品及/或Amazon Ads DSP達到的「重疊廣告公開ID」劃分。"

在&#x200B;**[!UICONTROL 探索]**&#x200B;區段中，您可以將AMC對象與您的Amazon廣告觸及的所有消費者進行比較。 您也可以檢視對象與最高重疊率的Amazon目標定位區段，僅考量DSP曝光數(這些區段只能在DSP中定位)。

>[!IMPORTANT]
>
>系統會從上傳至您[!DNL Amazon Ads]帳戶的對象中處理對象資料。 若要瞭解如何使用Experience Platform的目的地功能傳送您的對象到您的[!DNL Amazon Ads]帳戶，請閱讀[Amazon Ads連線](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/destinations/catalog/advertising/amazon-ads)指南。

![使用Amazon Marketing Cloud的專案中的Discover區段。](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### 比較客群 {#compare-audiences}

**[!UICONTROL 比較對象]**&#x200B;區段提供您的[!DNL AMC]對象如何與您的Amazon廣告觸及的消費者重疊的深入分析。 在&#x200B;**[!UICONTROL 比較對象]**&#x200B;區段中，您可以檢視下列量度：

| 量度 | 說明 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的對象資料能夠解析的ID數量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重疊的廣告公開ID] | 已上傳對象中已透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]的數量。 |
| [!UICONTROL 重疊%] | 已透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]比例。 |
| 依Amazon廣告產品[!UICONTROL 劃分] | 由[!UICONTROL 贊助的產品]和/或[!UICONTROL DSP]所達到的[!UICONTROL 重疊廣告公開的ID]劃分。 每個廣告都會以廣告公開ID總數的個別百分比表示。 由於識別碼同時屬於[!UICONTROL 贊助產品]和[!UICONTROL DSP]，所以百分比總和不能為100%。 |


### 相關客群 {#relevant-audiences}

「**[!UICONTROL 相關對象]**」區段提供您對象與最高重疊區域之[!DNL Amazon]目標定位區段或對象的深入分析，僅考慮DSP曝光數(這些區段只能在DSP中定位)。 您可以切換所有相關的對象，並在每個區段中檢視下列量度：

| 量度 | 說明 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的對象資料能夠解析的ID數量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重疊的廣告公開ID] | 這代表已上傳對象中也透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]數目。 這只會考慮DSP曝光數。 |
| [!UICONTROL 重疊%] | 已透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]比例。 |
| [!UICONTROL 類別] | 對象所屬的類別。 一個對象可以屬於多個類別。 |

### 探索與[!DNL Amazon Marketing Cloud]的重疊 {#discover-overlaps}

**[!UICONTROL 探索與Amazon Marketing Cloud重疊]**&#x200B;區段可讓您深入瞭解對象如何與[!DNL Amazon]目標定位區段或對象重疊。 您可以檢視下列量度：

| 量度 | 說明 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的對象資料能夠解析的ID數量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重疊的廣告公開ID] | 這代表已上傳對象中也透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]數目。 這只會考慮DSP曝光數。 |
| [!UICONTROL 重疊%] | 已透過[!UICONTROL 向廣告公開的]已解析ID[!DNL Amazon Ads]比例。 |