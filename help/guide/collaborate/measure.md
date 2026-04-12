---
title: 測量績效
description: 衡量不同管道中行銷活動的績效。 瞭解如何使用和解讀各種報表。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: e06ee94afdd1edbf86430cbe348dc448419b8f4e
workflow-type: tm+mt
source-wordcount: '2612'
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

請檢閱此表格，以評估促銷活動在推動所需動作方面的成效。

![累計轉換。](/help/assets/collaborate/measure/cumulative-conversions.png)

### 按日轉換 {#conversions-by-day}

此圖表提供您建立歸因報表時為每個設定的事件逐日劃分轉換。 使用此檢視來發現每日模式、識別高轉換活動或低轉換活動的期間，並比較不同轉換事件在行銷活動時間軸上的執行方式。

![依日期轉換。](/help/assets/collaborate/measure/conversions-by-day.gif)

## 建立衡量報告 {#create-measurement-report}

在Collaboration中，您可以建立兩種主要型別的測量報表：

* **行銷活動摘要**：提供高層級量度，例如觸及率、曝光數、平均頻率以及依據管道的傳遞，快速瞭解整體行銷活動績效。
* **歸因**：測量行銷活動曝光度如何推動轉換或購買等下游動作，協助您瞭解行銷活動的成效。

您可以自行執行「行銷活動摘要」報表，而「歸因」報表需要同時選取這兩種報表型別。

### 建立行銷活動摘要報告 {#create-campaign-summary-report}

發佈者和廣告商都可以產生&#x200B;**行銷活動摘要**&#x200B;報告，以評估行銷活動績效。 使用這些報告深入瞭解關鍵量度，例如[達到](#cumulative-reach-curve)、[頻率](#frequency-distribution)和[曝光數](#impressions-by-placement)，並瞭解您的行銷活動的傳遞方式及其整體影響。

若要產生&#x200B;**行銷活動摘要**&#x200B;報告，請從&#x200B;**[!UICONTROL Collaborator]**&#x200B;工作區導覽至專案工作區。 從&#x200B;**[!UICONTROL 量值]**&#x200B;索引標籤中，選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） 然後選取&#x200B;**[!UICONTROL 量值]**。

如果這是您的第一個報告，您也可以選取&#x200B;**[!UICONTROL 執行報告]**&#x200B;選項。

![醒目提示「執行報告」選項和「計量」選項的「計量」標籤。](/help/assets/collaborate/measure/run-measure-report.png)

**[!UICONTROL 建立測量報告]**&#x200B;畫面顯示，其中資訊和輸入欄位分組在&#x200B;**[!UICONTROL 帳單詳細資料]**、**[!UICONTROL 行銷活動詳細資料]**&#x200B;和&#x200B;**[!UICONTROL 報告詳細資料]**&#x200B;區段。

#### 計費詳細資料 {#billing-details}

本節說明如何在產生測量報表時使用積分。 在[連線設定](../connect/establishing-connections.md#credit-split)期間已建立信用責任。 在執行任何報表之前，請務必與共同作業人員檢閱並確認信用分割設定和報告角色。

#### 行銷活動詳細資料 {#campaign-details}

在&#x200B;**[!UICONTROL 行銷活動詳細資料]**&#x200B;區段中，選取適當的&#x200B;**廣告商ID**&#x200B;以與您的報告產生關聯。 這些廣告商名稱或ID是在[連線設定](../connect/establishing-connections.md#advertiser-names)期間新增的。 如果只設定了一個名稱，預設會顯示該名稱。 如果未設定名稱，則會停用&#x200B;**[!UICONTROL 廣告商ID （名稱）]**&#x200B;欄位，並預先填入廣告商帳戶名稱。

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

**[!UICONTROL 編輯測量報告]**&#x200B;對話方塊會出現，並在下列區段中顯示報告目前的設定：

* [**帳單詳細資料**](#billing-details)：執行測量報告時顯示信用額的相關資訊。 不需要設定。
* [**行銷活動詳細資料**](#campaign-details)：顯示廣告商、行銷活動ID、報告期間和使用者友善的報告名稱的設定。
* [**報告詳細資料**](#report-details)：顯示歸因報告專屬的報告型別、報告執行日期和組態選項的設定。

![「編輯測量報告」對話方塊顯示「計費詳細資料」、「行銷活動詳細資料」和「報告詳細資料」區段下的目前設定。](/help/assets/collaborate/measure/edit-measurement-report-dialog.png)

### 編輯行銷活動詳細資料 {#edit-campaign-details}

在&#x200B;**[!UICONTROL 編輯測量報告]**&#x200B;對話方塊中，使用&#x200B;**[!UICONTROL 廣告商ID （名稱）]**&#x200B;和&#x200B;**[!UICONTROL 促銷活動ID]**&#x200B;下拉式功能表，編輯報告的廣告商和促銷活動ID。

![醒目提示行銷活動ID下拉式功能表的「編輯測量報告」對話方塊開啟。](/help/assets/collaborate/measure/edit-campaign-id.png)

接著，選取&#x200B;**[!UICONTROL 報告日期範圍]**&#x200B;並使用行事曆變更報告的開始和結束日期。

![醒目提示報表日期範圍行事曆的「編輯測量報表」對話方塊開啟。](/help/assets/collaborate/measure/edit-report-date-range.png)

輸入更新的易記報告名稱以擷取您最近的變更。 這可協助您日後識別並尋找此報表。

![「編輯測量報告」對話方塊會醒目提示更新的好記報告名稱。](/help/assets/collaborate/measure/edit-friendly-report-name.png)

### 編輯報告詳細資訊 {#edit-report-details}

若要將報表排程為不同的日期，請導覽至&#x200B;**[!UICONTROL 報表詳細資料]**&#x200B;區段。 選取目前的執行日期選項，然後使用行事曆選擇您偏好的日期。

![醒目提示報告執行日期行事曆的[編輯測量報告]對話方塊。](/help/assets/collaborate/measure/edit-report-run-date.png)

作為廣告商，除了&#x200B;**[!UICONTROL 行銷活動摘要]**&#x200B;之外，您還可以選擇選取或移除&#x200B;**[!UICONTROL 歸因]**&#x200B;報告型別。 如果您選擇&#x200B;**[!UICONTROL 歸因]**，則您的歸因報表會包含標準「促銷活動摘要」量度和深入的「歸因」深入分析。 如需&#x200B;**促銷活動摘要**&#x200B;和&#x200B;**歸因**&#x200B;報告型別的詳細資訊，請參閱[建立測量報告](#create-measurement-report)區段。

>[!IMPORTANT]
>
>如果您是&#x200B;**發佈者**，預設的報表型別是&#x200B;**[!UICONTROL 行銷活動摘要]**，目前無法變更。

* 如果您選擇&#x200B;**[!UICONTROL 歸因]**&#x200B;作為報表型別，則必須在&#x200B;**[!UICONTROL 歸因]**&#x200B;區段中填寫必填欄位。 如需設定指示，請參閱[歸因報告詳細資料](#report-details-attribution)區段。
* 如果您先前在建立報告時已設定歸因設定，您可以選擇編輯回顧期間（以天為單位測量），並選取要報告的轉換事件。

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
