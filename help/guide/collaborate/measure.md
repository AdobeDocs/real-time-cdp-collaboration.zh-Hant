---
title: 測量績效
description: 衡量不同管道中行銷活動的績效。 瞭解如何使用和解讀各種報表。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 18%

---

# 測量績效

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Measure]**&#x200B;工作區只有在連線程式&#x200B;**期間已啟用**&#x200B;的[Measurement](../connect/establishing-connections.md#connection-settings)使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

瞭解Adobe Real-Time CDP Collaboration中的可用報表，並瞭解如何測量和分析各種管道中行銷活動的效能。

## 先決條件

在存取Collaboration中的測量報表之前，您已：

* [已連線](/help/guide/connect/establishing-connections.md)與想要的廣告商或發行者連線，且已啟用&#x200B;**Measurement**&#x200B;使用案例，並開始在[專案](/help/guide/collaborate/manage-projects.md)上共同作業
* 執行行銷活動並[將測量資料](/help/guide/setup/onboard-measurement-data.md)上傳至Collaboration。

<!--

## Create a report {#create-report}

Hidden until functionality is live. At that point, move the contextualhelp from below into this section. 

The syntax rtcdp_collaboration_measurement_create_report is currently implemented in the UI. However, a preference would be to imlement the other contextualhelp ID from below instead, since that explicitly includes campaignID in the syntax. Need to sync up with UI team. More details in CORE-116991.

-->

## 檢視報告 {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="行銷活動 ID"
>abstract="預留位置，用於在使用者介面中新增有關行銷活動 ID 內容的相關資訊。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="行銷活動 ID"
>abstract="預留位置，用於在使用者介面中新增有關行銷活動 ID 內容的相關資訊。"

若要檢視測量標籤中可用的報表：

1. 瀏覽至&#x200B;**[!UICONTROL 共同作業]** > **[!UICONTROL 我的專案]**。
2. 針對您想要的專案，選取&#x200B;**[!UICONTROL 檢視]**。
3. 在專案中，選取&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤。

選取&#x200B;**[!UICONTROL 檢視完整報告]**&#x200B;以存取各種可用的報告，詳細資訊如下。

![如何進入專案中的測量標籤。](/help/assets/collaborate/measure/measurement.gif)

### 摘要檢視

測量索引標籤中的頁面頂端檢視會顯示行銷活動摘要，其中包含一些可供您參考的高層級數字：

**[!UICONTROL 曝光次數]**：創意內容顯示的總次數。
**[!UICONTROL 唯一範圍]**：看過該創意的個人身分數量。
**[!UICONTROL 總平均頻率]**：曝光次數除以達到的唯一身分識別。 此圖指出每個身分在創意中顯示的頻率。

![行銷活動摘要檢視](/help/assets/collaborate/measure/campaign-summary.png)

### 一段時間內的量度 {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="一段時間內的量度"
>abstract="透過一段時間內的量度視圖，了解您的創意在整個行銷活動期間所顯示的印象總數量。您可以選擇在報告中顯示最多兩個維度。"

透過一段時間內的量度視圖，了解您的創意在整個行銷活動期間所顯示的印象總數量。請注意，您最多可以選取兩個量度，以在報表中顯示和分析。

![一段時間檢視中的量度。](/help/assets/collaborate/measure/metrics-over-time.png)

### 頻率分佈 {#frequency-distribution}

使用頻率分佈檢視來瞭解向每位不重複使用者顯示的曝光次數劃分。 此檢視可協助您在未來的行銷活動中決定要從哪一個時間點開始抑制對象。 例如，您可能想要隱藏已看過三次創意內容的設定檔。

![頻率分佈檢視。](/help/assets/collaborate/measure/frequency-distribution.gif)

### 依維度劃分的量度 {#metric-by-dimension}

根據刊登版位媒體，分析不同的量度，例如曝光數、可檢視曝光數、不重複觸及率、成本等。 分析哪些媒體（例如行動串流、CTV程式化或其他）為您的行銷活動帶來最佳結果。

依維度![量度。](/help/assets/collaborate/measure/metric-by-dimension.png)

### 累計的觸及人數曲線 {#cumulative-reach-curve}

隨著行銷活動進行且曝光次數增加，請瞭解您能夠聯絡的使用者數量是否也有所增加。 行銷活動中的常見模式是，在到達特定點後，達到平台期，創意內容會一遍又一遍地顯示給相同的使用者。 此檢視可幫助您調整未來行銷活動的長度，具體取決於不再聯絡新人的時間。

![累積觸及曲線。](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### 依刊登位置劃分的曝光數 {#impressions-by-placement}

瞭解哪些媒體可提升創意的曝光率。 這可協助您決定要將廣告支出投資於未來行銷活動的位置。

![依位置區分的曝光次數。](/help/assets/collaborate/measure/impressions-by-placement.png)

## 後續步驟

![為廣告商探索、啟用、測量。](/help/assets/end-to-end-workflow/discover-activate-measure.png)

秉承上圖循環的精神，運用您在規劃下一個行銷活動時檢視報表所取得的深入見解。 作為廣告商，如有必要，請返回以探索不同的發佈者，並執行重疊以探索您後續行銷活動的不同受眾。
