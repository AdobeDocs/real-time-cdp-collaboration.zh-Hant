---
title: 探索重疊並比較對象
description: 探索您和共同作業人員的對象之間的重疊。 瞭解如何探索最佳對象，以用於您的行銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 11%

---

# 探索重疊並比較對象

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 探索]**&#x200B;工作區只有在連線程式](../connect/establishing-connections.md#connection-settings)期間已啟用[的&#x200B;**對象探索**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

在[建立專案](/help/guide/collaborate/manage-projects.md)之後，您可以比較對象與共同作業人員。 這可協助您識別行銷活動的相關對象，並決定要將哪些對象傳送給發佈者以進行啟用。

>[!IMPORTANT]
>
>任何[未更新或未重新整理的資料草圖](/help/guide/glossary.md#sketches)將在7天後刪除。 發生此情況時，此頁面上各種重疊報表中顯示的數字會變成零，且這些過期的對象將無法共用對象。 具有[作用中重新整理排程](/help/guide/setup/onboard-audiences.md#schedule)的對象會自動重新整理資料草圖。

在連線程式](/help/guide/connect/establishing-connections.md#connection-settings)期間，已設定[用來探索和比較對象的比對金鑰。 比對索引鍵會用於計算對象之間的重疊，且可切換開啟和關閉。 若要編輯比對索引鍵，請選取&#x200B;**[!UICONTROL 編輯比對索引鍵]**&#x200B;選項。 這個

![Dicover標籤工作區，展示Audience深入分析。](/help/assets/collaborate/discover/discover-overview.png)

**[!UICONTROL 編輯相符鍵]**&#x200B;對話方塊開啟，您可以在其中關閉不想使用的相符鍵。 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您的變更。

![探索工作區中的[編輯相符金鑰]對話方塊。](/help/assets/collaborate/discover/edit-match-keys.png)

## 先決條件 {#prerequisites}

若要開始使用專案中的&#x200B;**[!UICONTROL Discover]**&#x200B;標籤，您應該：

* [已將對象](/help/guide/setup/onboard-audiences.md)匯入您的組織
* [已連線](/help/guide/connect/establishing-connections.md)，共同作業人員已啟用&#x200B;**對象探索**&#x200B;使用案例
* [已建立您與共同作業人員之間的專案](/help/guide/collaborate/manage-projects.md)

滿足這些先決條件後，您就可以開始探索及比較您與共同作業人員的對象之間的重疊。

## 比較客群 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="比較客群"
>abstract="探索您和協作者之客群間的重疊處。您可以調整下拉式選單選擇器中的設定，找出您的一個或多個客群與協作者的一個或多個客群之間的重疊部分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="您的身分識別計數"
>abstract="根據您和您的共同作業人員針對專案議定的相符索引鍵，選定對象中的唯一ID數量。"
>
[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="協作者身分識別計數"
>abstract="共同作業人員的對象中的唯一ID數量，根據您和共同作業人員針對專案協定的相符索引鍵。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重疊的身分識別計數"
>abstract="根據您和您的共同作業人員針對專案協定的相符索引鍵，您的和共同作業人員的對象中同時存在的唯一ID數量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="重疊身分識別百分比"
>abstract="您與共同作業人員所選對象之間的重疊身分百分比。"

使用比較對象區段，取得您和共同作業人員的對象之間重疊的豐富資訊。 若要變更對象選擇，請使用&#x200B;**[!UICONTROL 比較對象]**&#x200B;區段頂端的下拉式選擇器。 您可以選取一或全部對象，以及一或全部共同作業人員的對象來相互比較。

![在[比較對象]區段中反白顯示對象選擇器的Discover工作區。](/help/assets/collaborate/discover/compare-audiences-selector.png)

在比較對象區段中，您可以看到以下量度，這些量度是根據您和您的共同作業人員針對專案議定的相符索引鍵：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** （您的） | 您所選對象中的唯一ID數量。 |
| **[!UICONTROL 身分計數]** （您的共同作業人員） | 共同作業人員對象中的唯一ID數量。 |
| **[!UICONTROL 重疊的身分]** | 您的和共同作業人員的對象中同時存在的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 您和您的協作者所選客群間的輪廓重疊百分比。 |
| **[!UICONTROL 依比對索引鍵劃分的身分]** | 根據每個共同作業人員的選取對象，專案中選擇的每個相符索引鍵的識別項劃分。 |

{style="table-layout:auto"}

>[!TIP]
>
>並非所有對象都一定可使用重疊百分比圖。 重疊百分比指標的可見度取決於您的共同作業人員為[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中的對象選擇的設定。

## 相關客群 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相關客群"
>abstract="根據重疊百分比，這些發佈者客群可能非常適合您的行銷活動。<br><br><b>身分識別計數</b>為發佈者的客群大小。<br><br> <b>重疊的身分識別</b>代表建議的發佈者客群與所有廣告商客群之間的重疊部分。<br><br><b>重疊百分比</b>表示重疊之身分識別的數量，除以<i>所有</i>廣告商客群之大小的數值。"

**[!UICONTROL 探索]**&#x200B;標籤中的&#x200B;**[!UICONTROL 相關對象]**&#x200B;區段會根據共同作業人員的對象與所有對象之間的重疊百分比，提供前五個對象的精選清單。 此功能可協助您快速識別重疊程度最高的對象，讓您更有效地鎖定行銷活動。 使用區段右上角的頁面選取器，在相關對象之間切換。

![醒目提示「發現相關對象」區段的Discover工作區。](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>共同作業人員對象的可見度取決於共同作業人員在[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中為對象選擇的設定。 如果您的共同作業人員已將所有對象設為私人，此區段將不會顯示任何對象。

**[!UICONTROL 相關對象]**&#x200B;區段會顯示每個建議對象的下列資訊：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** | 對象中的唯一ID名稱。 |
| **[!UICONTROL 重疊的身分]** | 建議的對象與您的所有對象之間重疊的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 建議的對象與您的所有對象之間的重疊身分百分比。 |
| **[!UICONTROL 對象類別]** | 您的共同作業人員已指派給對象的類別。 |
| **[!UICONTROL 相符金鑰]** | 共同作業人員為對象選取的相符金鑰。 |

{style="table-layout:auto"}

>[!NOTE]
>
>共同作業人員對象的可見度取決於共同作業人員在[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中為對象選擇的設定。 如果您的共同作業人員已將所有對象設為私人，此區段將不會顯示任何對象。

## 探索重疊 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="探索與個別客群的重疊處"
>abstract="深入瞭解您的對象與共同作業人員的對象之間的重疊。"

探索重疊，以深入瞭解您的對象與共同作業人員的對象相較之下的情形。 依預設，此區段會將您的所有對象與您的共同作業人員的每個對象進行比較。 使用區段底部的分頁控制項，以導覽至可用的對象。

![反白顯示Discover重疊區段的Discover工作區。](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>共同作業人員對象的可見度取決於共同作業人員在[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中為對象選擇的設定。 如果您的共同作業人員已將所有對象設為私人，此區段將不會顯示任何對象。

若要變更您的對象選擇，請選取&#x200B;**[!UICONTROL 變更對象]**。

![醒目提示「探索工作區」的「變更對象」選項。](/help/assets/collaborate/discover/change-audience.png)

**[!UICONTROL 變更對象]**&#x200B;對話方塊開啟，您可以在其中比較特定對象與共同作業人員的對象。 選取想要的對象，或清除您的選取以選取所有對象，然後選取[儲存]。****

![探索工作區中的[變更對象]對話方塊。](/help/assets/collaborate/discover/change-audience-selection.png)

選取所需的對象後，**[!UICONTROL 探索重疊]**&#x200B;區段會顯示每個對象的下列資訊：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** | 對象中的唯一ID名稱。 |
| **[!UICONTROL 重疊的身分]** | 建議的對象與您的所有對象之間重疊的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 建議的對象與您的所有對象之間的重疊身分百分比。 |
| **[!UICONTROL 對象類別]** | 您的共同作業人員已指派給對象的類別。 |
| **[!UICONTROL 相符金鑰]** | 共同作業人員為對象選取的相符金鑰。 |

{style="table-layout:auto"}

## 後續步驟

探索及探索所需的對象後，是時候[啟用](/help/guide/collaborate/activate.md)應該用於行銷活動的對象。
