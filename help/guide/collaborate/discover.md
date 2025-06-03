---
title: 探索重疊並比較對象
description: 探索您和共同作業人員的對象之間的重疊。 瞭解如何探索最佳對象，以用於您的行銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 24%

---

# 探索重疊並比較對象

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 探索]**&#x200B;工作區只有在連線程式](../connect/establishing-connections.md#connection-settings)期間已啟用[的&#x200B;**對象探索**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

在廣告商與發佈商之間的共同作業空間內[建立專案](/help/guide/collaborate/manage-projects.md)後，您現在可以將您的對象與共同作業人員的對象進行比較。 如此一來，您便可探索對象之間的重疊，並取得依比對索引鍵或身分劃分的深入分析。 這可協助廣告商決定要將哪些受眾與發佈者共用以進行啟用。

>[!IMPORTANT]
>
>任何[未更新或未重新整理的資料草圖](/help/guide/glossary.md#sketches)將在7天後刪除。 發生此情況時，此頁面上各種重疊報表中顯示的數字會變成零，且這些過期的對象將無法共用對象。 具有[作用中重新整理排程](/help/guide/setup/onboard-audiences.md#schedule)的對象會自動重新整理資料草圖。

![探索重疊](/help/assets/collaborate/discover-overlaps/discover-overlaps.png)

當您[連線到發行者](/help/guide/connect/establishing-connections.md#connection-settings)時，會設定用來探索及比較對象的比對金鑰。 若要變更準備執行行銷活動時指出的重疊百分比，您可以移除相符索引鍵，但此時無法新增相符索引鍵。 若要這麼做，請前往共同作業人員之間的[連線設定](/help/guide/connect/establishing-connections.md#connection-settings)。

![編輯相符鍵畫面](/help/assets/collaborate/discover-overlaps/edit-match-keys.png)

## 先決條件 {#prerequisites}

若要充分利用&#x200B;**[!UICONTROL 共同作業]**&#x200B;工作流程的&#x200B;**[!UICONTROL 探索]**&#x200B;索引標籤中的功能，您已：

* [匯入的對象](/help/guide/setup/onboard-audiences.md)
* [已連線](/help/guide/connect/establishing-connections.md)與所需的廣告商或發行者連線，並啟用&#x200B;**對象探索**&#x200B;使用案例
* [已建立您與共同作業人員之間的專案](/help/guide/collaborate/manage-projects.md)

在滿足上述先決條件後，您就可以開始探索並比較您和共同作業人員的對象之間的重疊。

## 比較客群 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="比較客群"
>abstract="探索您和協作者之客群間的重疊處。您可以調整下拉式選單選擇器中的設定，找出您的一個或多個客群與協作者的一個或多個客群之間的重疊部分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="您的身分識別計數"
>abstract="屬於您所選的客群，且具有所選身分識別的輪廓數量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="協作者身分識別計數"
>abstract="屬於您的協作者所選客群，且具有所選身分識別的輪廓數量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重疊的身分識別計數"
>abstract="在您和您的協作者之客群中同時存在，且具有所選身分識別的輪廓數量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="重疊身分識別百分比"
>abstract="您和您的協作者所選客群間的輪廓重疊百分比。"

使用比較受眾卡片，取得您和共同作業人員的受眾之間重疊的豐富資訊。 您可以選取比較下列任何對象組合：

* 您的其中一個對象與您的共同作業人員的其中一個對象進行對照
* 您的其中一個對象與您的共同作業人員的所有對象
* 針對共同作業人員的其中一個對象來設定所有對象
* 針對共同作業人員的所有對象的所有對象

顯示的資訊與：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** （您的） | 屬於您所選對象的具有所選身分的設定檔數。 |
| **[!UICONTROL 身分計數]** （您的共同作業人員） | 共同作業人員所選對象中具有所選身分的設定檔數。 |
| **[!UICONTROL 重疊的身分]** | 所選身分同時存在於您和共同作業人員的對象中的設定檔數。 |
| **[!UICONTROL 重疊百分比]** | 您和您的協作者所選客群間的輪廓重疊百分比。 |
| **[!UICONTROL 依比對索引鍵劃分的身分]** | 根據您和您的共同作業人員針對專案議定的相符金鑰，依個別相符金鑰檢視重疊計算中的身分組成。 |

{style="table-layout:auto"}

>[!TIP]
>
>並非所有對象都一定可使用重疊百分比圖。 重疊百分比指標的可見度取決於您的共同作業人員為[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中的對象選擇的設定。

## 相關客群 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相關客群"
>abstract="根據重疊百分比，這些發佈者客群可能非常適合您的行銷活動。<br><br><b>身分識別計數</b>為發佈者的客群大小。<br><br> <b>重疊的身分識別</b>代表建議的發佈者客群與所有廣告商客群之間的重疊部分。<br><br><b>重疊百分比</b>表示重疊之身分識別的數量，除以<i>所有</i>廣告商客群之大小的數值。"

**[!UICONTROL Discover]**&#x200B;模組中的&#x200B;**[!UICONTROL 相關對象]**&#x200B;檢視會根據重疊百分比，提供前五個對象的精選清單。 此功能可協助您快速找出與您目前資料重疊程度最高的對象，讓您更有效地鎖定行銷活動。

* **[!UICONTROL 身分計數]**&#x200B;是發行者的對象人數。
* **[!UICONTROL 重疊的身分]**&#x200B;代表建議的發佈者對象與所有廣告商對象之間的重疊。
* **[!UICONTROL 重疊%]**&#x200B;代表重疊身分的數目除以&#x200B;*所有*&#x200B;廣告商對象的大小。

![相關對象檢視](/help/assets/collaborate/discover-overlaps/relevant-audiences-highlighted.png)

## 探索重疊 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="探索與個別客群的重疊處"
>abstract="深入了解此客群之群體，及其與協作者身分識別範圍的重疊部分。"

![探索與不同對象檢視的重疊](/help/assets/collaborate/discover-overlaps/discover-overlaps-cards-view.png)

取得任何共同作業人員對象的廣泛資訊，並檢視這些對象與所有對象中的整個母體計數，或您的特定對象比較的重疊資訊。

>[!TIP]
>
>熒幕擷取畫面中指出的某些數字並不一定適用於所有對象。 其可見性取決於您的共同作業人員為[中繼資料可見性區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中的對象選擇的設定。

## 後續步驟

探索並探索所需的對象後，現在應該[與發佈者](/help/guide/collaborate/share.md)共用應在行銷活動中使用的對象。
