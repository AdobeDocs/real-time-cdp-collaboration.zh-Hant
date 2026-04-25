---
title: 測量績效
description: 衡量不同管道中行銷活動的績效。 瞭解如何使用和解讀各種報表。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
TQID: https://experienceleague.adobe.com/pr-qF4sd-NHd55kxh1dCstHRnVCUEhIvtv-47-ljiu4
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 2612
ht-degree: 5%

---

# 測量績效

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Measure]**&#x200B;工作區只有在連線程式](../connect/establishing-connections.md#connection-settings)期間已啟用[的&#x200B;**Measurement**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

瞭解Adobe Real-Time CDP Collaboration中的可用報表，並瞭解如何測量和分析各種管道中行銷活動的效能。

## 先決條件 {#prerequisites}

您必須先執行下列作業，才能存取Collaboration中的測量報表：

* [連線](/help/guide/connect/establishing-connections.md)，與啟用&#x200B;**Measurement**&#x200B;使用案例的共同作業人員
* 與您的共同作業人員至少在一個專案上共同作業。 瞭解如何[建立專案](/help/guide/collaborate/manage-projects.md#create-project)。
* 執行您的行銷活動，並確定已提供行銷活動的[行銷活動ID](../collaborate/manage-projects.md#manage-campaign-id)：
   * 如果您是發佈者，請輸入連結至廣告商促銷活動的Campaign ID。
   * 如果您是廣告商，請要求共同作業人員（發佈者）提供促銷活動ID。 這是在Measure工作區](#create-measurement-report)中[產生報表的必要專案。
* 如果要[建立歸因報表](#create-attribution-report)，請[將測量資料](/help/guide/setup/onboard-measurement-data.md)上傳到Collaboration。

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
>abstract="透過一段時間內的量度視圖，了解您的創意在整個行銷活動期間所顯示的印象總數量。 您可以選擇在報告中顯示最多兩個維度。"

透過一段時間內的量度視圖，了解您的創意在整個行銷活動期間所顯示的印象總數量。 請注意，您最多可以選取兩個量度，以在報表中顯示和分析。

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

### 累計轉換 {#cumulative-conversions}

此檢視提供您選擇以表格格式測量的轉換事件的詳細劃分。 此表格包含：

* **轉換事件**：您正在追蹤的每個轉換事件名稱。
* **轉換計數**：每個事件發生的轉換總數。
* **預估收入**：歸因於每個轉換事件的預估值。

Review this table to evaluate the effectiveness of your campaign in driving the desired actions.

![Cumulative conversions.](/help/assets/collaborate/measure/cumulative-conversions.png)

### 按日轉換 {#conversions-by-day}

This chart provides a day-by-day breakdown of conversions for each event set up when you create an Attribution report. Use this view to uncover daily patterns, identify periods of high or low conversion activity, and compare how different conversion events perform across your campaign timeline.

![Conversions by day.](/help/assets/collaborate/measure/conversions-by-day.gif)

## 建立衡量報告 {#create-measurement-report}

In Collaboration, you can create two main types of measurement reports:

* **Campaign Summary**: Provides high-level metrics such as reach, impressions, average frequency, and delivery by channel, giving a quick overview of overall campaign performance.
* **Attribution**: Measures how campaign exposures drive downstream actions like conversions or purchases, helping you understand campaign effectiveness.

You can run Campaign Summary report on its own, while Attribution report requires both report types to be selected together.

### Create campaign summary report {#create-campaign-summary-report}

Both publishers and advertisers can generate **Campaign Summary** reports to evaluate campaign performance. Use these reports to gain insights into key metrics such as [reach](#cumulative-reach-curve), [frequency](#frequency-distribution), and [impressions](#impressions-by-placement), and understand how your campaign was delivered and its overall impact.

To generate a **Campaign Summary** report, navigate to the project workspace from the **[!UICONTROL Collaborator]** workspace. From the **[!UICONTROL Measure]** tab, select the add icon (![Add icon.](/help/assets/icons/plus.png)) and then select **[!UICONTROL Measure]**.

If this is your first report, you may also select the **[!UICONTROL Run report]** option.

![The Measure tab highlighting the Run report option and the Measure option.](/help/assets/collaborate/measure/run-measure-report.png)

The **[!UICONTROL Create measurement report]** screen appears with information and input fields grouped under **[!UICONTROL Billing details]**, **[!UICONTROL Campaign details]**, and **[!UICONTROL Report details]** sections.

#### 計費詳細資料 {#billing-details}

This section explains how credits are used when generating measurement reports. Credit responsibility is established during [connection setup](../connect/establishing-connections.md#credit-split). Before running any reports, make sure to review and confirm the credit split settings and reporting roles with your collaborator.

#### 行銷活動詳細資料 {#campaign-details}

In the **[!UICONTROL Campaign details]** section, select the appropriate **Advertiser ID** to associate with your report. These advertiser names or IDs were added during [connection setup](../connect/establishing-connections.md#advertiser-names). If only one name was configured, it appears by default. If no name was set up, the **[!UICONTROL Advertiser ID (Name)]** field is disabled and prefilled with the advertiser account name.

![顯示「廣告商ID （名稱）」選項的建立測量報告畫面已停用。](/help/assets/collaborate/measure/advertiser-id.png)

然後，從&#x200B;**[!UICONTROL 促銷活動ID]**&#x200B;下拉式功能表中選取所需的促銷活動。 此功能表會列出發佈者為您的專案輸入的所有促銷活動ID。 如果您需要的行銷活動無法使用，請在產生報告之前[將它新增到UI](./manage-projects.md#manage-campaign-id)。

![建立測量報告畫面顯示Campaign ID下拉式功能表已展開。](/help/assets/collaborate/measure/campaign-id.png)

接著，指定您要報表涵蓋的期間。 選取&#x200B;**[!UICONTROL 報告日期範圍]**，然後使用行事曆選擇開始和結束日期。

![顯示報告日期範圍行事曆的建立測量報告畫面。](/help/assets/collaborate/measure/report-date-range.png)

#### 報告詳細資料 {#report-details}

**報告執行日期**

在&#x200B;**[!UICONTROL 報告詳細資料]**&#x200B;區段中，選擇報告應該執行的日期。 選取&#x200B;**[!UICONTROL 報告執行日期]**，並從行事曆中選擇您偏好的日期。

* 如果您選擇今天的日期或過去的日期，**行銷活動摘要**&#x200B;報告就會立即執行。
* 如果您選擇未來的日期，**行銷活動摘要**&#x200B;報告將排程在該日執行。

![顯示報告執行日期行事曆的建立測量報告畫面。](/help/assets/collaborate/measure/report-run-date.png)

**報告型別**

* 如果您是廣告商，您可以從可用選項中選取&#x200B;**[!UICONTROL 行銷活動摘要]**&#x200B;報告型別。 只有廣告商可以產生歸因報表。
* 如果您是發佈者，**[!UICONTROL 行銷活動摘要]**&#x200B;報告型別是預先選取且無法變更。 發佈者目前無法執行歸因報表。

![「建立測量報告」畫面會將「行銷活動摘要」選項顯示為預先選取且無法變更的報告型別。](/help/assets/collaborate/measure/cs-report-type.png)

最後，檢閱您的設定並選取&#x200B;**[!UICONTROL 建立]**。 如果執行日期為當天或之前，或是在所選的未來日期，則會立即產生行銷活動摘要報表。 您可以在排程報告執行日期之前編輯排程報告。 如需逐步指示，請參閱[編輯測量報告]區段。

一旦可用，您就可以隨時在專案工作區的&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤中檢視報告。

![「建立測量報告」畫面會顯示相關資訊，且「建立」選項反白顯示。](/help/assets/collaborate/measure/cs-review.png)

### 建立歸因報表 {#create-attribution-report}

作為廣告商，您可以產生&#x200B;**歸因**&#x200B;報告，以評估您的行銷活動曝光對註冊或購買等關鍵結果的貢獻。 使用這些報表來瞭解使用者與行銷活動的互動、識別哪些接觸點帶來最大的影響，並告知更有效率的行銷策略。

>[!IMPORTANT]
>
> 您必須先將測量資料](../setup/onboard-measurement-data.md#add-measurement-data)來源至Collaboration，才能產生歸因報表。[
>![具有測量資料需求及停用的測量選項的[測量]索引標籤。](/help/assets/collaborate/measure/require-measurement-data.png)

若要產生&#x200B;**歸因**&#x200B;報告，請從&#x200B;**[!UICONTROL Collaborator]**&#x200B;工作區瀏覽至專案工作區。 從&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤中，選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） 然後選取&#x200B;**[!UICONTROL 量值]**。

如果這是您的第一個報告，您也可以選取&#x200B;**[!UICONTROL 執行報告]**&#x200B;選項。

![醒目提示「執行報告」選項和「計量」選項的「計量」標籤。](/help/assets/collaborate/measure/run-measure-report-attribution.png)

**[!UICONTROL 建立測量報告]**&#x200B;畫面顯示，其中資訊和輸入欄位分組在&#x200B;**[!UICONTROL 帳單詳細資料]**、**[!UICONTROL 行銷活動詳細資料]**&#x200B;和&#x200B;**[!UICONTROL 報告詳細資料]**&#x200B;區段。

閱讀並遵循[建立行銷活動摘要報告](#create-campaign-summary-report)區段中的步驟來設定下列設定：

* [帳單詳細資料](#billing-details)
* [行銷活動詳細資料](#campaign-details)

#### 歸因報表的報表詳細資料 {#report-details-attribution}

**報告執行日期**

>[!IMPORTANT]
>
> 對於歸因報表，報表執行日期必須是未來的日期，且必須在報表日期範圍的結束日期加上已定義回顧期間的完整期間後至少一天發生。
> **報告執行日期≥報告結束日期+回顧期間+ 1**
> 
> 例如，如果您的報表日期範圍在6月15日結束且回顧期間為14天，則報表執行日期為6月30日或之後日期。

在&#x200B;**[!UICONTROL 報告詳細資料]**&#x200B;區段中，選擇報告應該執行的日期。 選取&#x200B;**[!UICONTROL 報告執行日期]**，並從行事曆中選擇您偏好的日期。

**報告型別**

作為廣告商，除了&#x200B;**[!UICONTROL 行銷活動摘要]**&#x200B;之外，您還可以選取&#x200B;**[!UICONTROL 歸因]**&#x200B;作為報表型別。 選擇「歸因」報表時，您的結果會包含標準「促銷活動摘要」量度和詳細的「歸因」分析，以提供促銷活動績效的完整檢視。

![建立測量報告畫面會醒目顯示選取的行銷活動摘要和歸因報告型別。](/help/assets/collaborate/measure/attribution-report-type.png)

當您選取&#x200B;**[!UICONTROL 歸因]**&#x200B;作為報表型別時，會出現&#x200B;**[!UICONTROL 歸因]**&#x200B;組態區段，其中包含其他必要的設定：

* **以天為單位的回顧期間**：定義報告在每次轉換前要考慮多久以前的促銷活動曝光數。 只有此期間的曝光才符合歸因點數的資格。
* **轉換事件**：指定您要測量的轉換動作，例如購買或註冊。 當您[將測量資料](../setup/onboard-measurement-data.md#add-conversion-event)來源至Collaboration時，必須預先設定這些事件。

首先，輸入&#x200B;**[!UICONTROL 以天]**&#x200B;為單位的回顧期間值，或使用增加/減少選項進行調整。

![建立測量報告畫面會醒目顯示以天為單位的回顧期間值。](/help/assets/collaborate/measure/lookback-window-in-days.png)

接著，從可用清單中選擇最多&#x200B;**3**&#x200B;個轉換事件。 如需特定事件的詳細資訊，請選取&#x200B;**[!UICONTROL i]**&#x200B;圖示以檢視其詳細資料。

![建立測量報告畫面會醒目顯示選取的轉換事件和購買事件的資訊。](/help/assets/collaborate/measure/attribution-conversion-events.png)

最後，檢閱您的設定並選取&#x200B;**[!UICONTROL 建立]**&#x200B;以排程報告。 您的歸因報告將會在指定的執行日期產生。 您可以在排程報告執行日期之前編輯排程報告。 如需逐步指示，請參閱[編輯測量報告]區段。

一旦可用，您就可以隨時在專案工作區的&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤中檢視報告。

![「建立測量報告」畫面會顯示相關資訊，且「建立」選項反白顯示。](/help/assets/collaborate/measure/attribution-review.png)

## 編輯衡量報告 {#edit-measurement-report}

>[!IMPORTANT]
>
>只有在排程於未來執行時，您才能編輯測量報告的設定。 對於已執行的報表，無法變更設定。

更新測量報告設定，以確保報告提供特定期間內行銷活動的正確分析，並在所需日期執行。

若要開始，請導覽至您要更新之測量報告的工作區。 選取刪除圖示旁的編輯圖示（![編輯圖示](/help/assets/icons/edit.png)）。

![強調顯示「編輯」圖示的測量報告工作區。](/help/assets/collaborate/measure/edit-report.png)

>[!TIP]
>
>在&#x200B;**[!UICONTROL 量值]**&#x200B;標籤中，瀏覽至您要編輯的報告區段。 選取&#x200B;**[!UICONTROL 檢視完整報告]**&#x200B;旁的編輯圖示（![編輯圖示](/help/assets/icons/edit.png)）以更新其設定。
>![在報表區段中反白顯示「編輯」圖示的「計量」標籤。](/help/assets/collaborate/measure/measure-tab-edit-report.png)

The **[!UICONTROL Edit measurement report]** dialog appears with the current settings of the report in the following sections:

* [**Billing details**](#billing-details): Displays information about credits when running measurement reports. No configuration is required.
* [**Campaign details**](#campaign-details): Displays settings for the advertiser, campaign ID, reporting period, and a user-friendly report name.
* [**Report details**](#report-details): Displays settings for the report type, report run date, and configuration options specifically for attribution reports.

![The Edit measurement report dialog showing the current settings under Billing details, Campaign details, and Report details sections.](/help/assets/collaborate/measure/edit-measurement-report-dialog.png)

### Edit campaign details {#edit-campaign-details}

In the **[!UICONTROL Edit measurement report]** dialog, use the **[!UICONTROL Advertiser ID (Name)]** and **[!UICONTROL Campaign ID]** dropdown menus to edit the advertiser and campaign ID for your report.

![The Edit measurement report dialog highlighting the Campaign ID dropdown menu open.](/help/assets/collaborate/measure/edit-campaign-id.png)

Next, select **[!UICONTROL Report date range]** and use the calendar to change the start and end dates of the report.

![The Edit measurement report dialog highlighting the Report date range calendar open.](/help/assets/collaborate/measure/edit-report-date-range.png)

Enter an updated friendly report name to capture your recent changes. This helps you recognize and find this report in the future.

![The Edit measurement report dialog highlighting the updated friendly report name.](/help/assets/collaborate/measure/edit-friendly-report-name.png)

### Edit report details {#edit-report-details}

To schedule the report for a different date, navigate to the **[!UICONTROL Report details]** section. Select the current run date option, then use the calendar to choose your preferred date.

![The Edit measurement report dialog highlighting the Report run date calendar.](/help/assets/collaborate/measure/edit-report-run-date.png)

As an advertiser, you have the option to select or remove the **[!UICONTROL Attribution]** report type in addition to **[!UICONTROL Campaign summary]**. If you choose **[!UICONTROL Attribution]**, your attribution report includes both standard Campaign Summary metrics and in-depth Attribution insights. For more information about the **Campaign summary** and **Attribution** report types, refer to the [create measurement report](#create-measurement-report) section.

>[!IMPORTANT]
>
>If you are a **publisher**, the default report type is **[!UICONTROL Campaign summary]** and cannot be changed at this time.

* If you choose **[!UICONTROL Attribution]** as the report type, you must fill out the required fields in the **[!UICONTROL Attribution]** section. For setup instructions, see the [attribution report details](#report-details-attribution) section.
* If you previously configured attribution settings when creating the report, you can choose to edit the lookback window (measured in days) and select which conversion events to report on.

若要以天數&#x200B;]**更新**[!UICONTROL &#x200B;回顧期間，請輸入數值，或使用增加/減少選項進行調整。 接著，選取您要報告的轉換事件。 您可以從可用清單中選擇最多&#x200B;**3**&#x200B;個轉換。

![「編輯測量報告」對話方塊會醒目顯示更新的轉換事件。](/help/assets/collaborate/measure/edit-conversion-events.png)

完成之後，請檢閱更新並選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以套用您的變更。

![反白顯示[編輯]選項的[編輯測量報告]對話方塊。](/help/assets/collaborate/measure/edit-report-confirm.png)

確認對話方塊會確認您的報告已成功儲存。

## 刪除測量報告 {#delete-measurement-report}

刪除Collaboration中的測量報告會將其從系統中永久移除。 此動作無法還原。 若要這麼做，請在&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤中選取您要刪除的報告。

在測量報表工作區中，選取刪除圖示（![刪除圖示](/help/assets/common/delete.svg)）。

![反白顯示「刪除」圖示的測量報告工作區。](/help/assets/collaborate/measure/delete-report.png)

**[!UICONTROL 刪除報告]**&#x200B;對話方塊會出現，提示您確認刪除。 選取「**[!UICONTROL 刪除]**」。

![反白顯示[刪除]選項的[刪除報告]對話方塊。](/help/assets/collaborate/measure/delete-report-confirm.png)

確認對話方塊會確認報告已成功刪除。
