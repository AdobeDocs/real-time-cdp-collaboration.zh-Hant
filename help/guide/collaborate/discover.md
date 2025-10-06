---
title: 探索重疊並比較對象
description: 探索您和共同作業人員的對象之間的重疊。 瞭解如何探索最佳對象，以用於您的行銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: 2cd03a98228e1e379396360942227ddbcab8f6ca
workflow-type: tm+mt
source-wordcount: '2107'
ht-degree: 17%

---

# 探索重疊並比較對象

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 探索]**&#x200B;工作區只有在連線程式&#x200B;**期間已啟用**&#x200B;的[對象探索](../connect/establishing-connections.md#connection-settings)使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

在[建立專案](/help/guide/collaborate/manage-projects.md)之後，您可以比較對象與共同作業人員。 這可幫助您識別行銷活動的相關對象，並決定要將哪些對象傳送給共同作業人員以進行啟用。

>[!IMPORTANT]
>
>任何[未更新或未重新整理的資料草圖](/help/guide/glossary.md#sketches)將在7天後刪除。 發生此情況時，此頁面上各種重疊報表中顯示的數字會變成零，且這些過期的對象將無法共用對象。 具有[作用中重新整理排程](/help/guide/setup/onboard-audiences.md#schedule)的對象會自動重新整理資料草圖。

在連線程式[期間，已設定](/help/guide/connect/establishing-connections.md#connection-settings)用來探索和比較對象的比對金鑰。 相符索引鍵會用於計算對象之間的重疊，且可切換為開啟或關閉。 若要編輯比對索引鍵，請選取&#x200B;**[!UICONTROL 編輯比對索引鍵]**&#x200B;選項。

![Dicover標籤工作區，展示Audience深入分析。](/help/assets/collaborate/discover/discover-overview.png)

**[!UICONTROL 編輯相符鍵]**&#x200B;對話方塊開啟，您可以在其中關閉不想使用的相符鍵。 選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存您的變更。

![探索工作區中的[編輯相符金鑰]對話方塊。](/help/assets/collaborate/discover/edit-match-keys.png)

## 先決條件 {#prerequisites}

若要開始使用專案中的&#x200B;**[!UICONTROL Discover]**&#x200B;標籤，您應該：

* [來源對象](/help/guide/setup/onboard-audiences.md)放入您的帳戶
* [已連線](/help/guide/connect/establishing-connections.md)，共同作業人員已啟用&#x200B;**對象探索**&#x200B;使用案例
* [已建立您與共同作業人員之間的專案](/help/guide/collaborate/manage-projects.md)

在滿足這些先決條件後，您就可以開始探索和比較您與共同作業人員的對象之間的重疊。

>[!NOTE]
>
>此&#x200B;**[!UICONTROL Discover]**&#x200B;工作區與廣告平台的共同作業無關。 目前，Amazon Marketing Cloud是Real-Time CDP Collaboration中唯一可用的廣告平台。 如需[!DNL AMC] **[!UICONTROL 探索]**&#x200B;工作區的詳細資訊，請閱讀[Amazon Marketing Cloud](/help/guide/collaborate/advertising-platforms/amc.md)指南。

## 比較客群 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="比較客群"
>abstract="探索您和協作者之客群間的重疊處。您可以調整下拉式選單選擇器中的設定，找出您的一個或多個客群與協作者的一個或多個客群之間的重疊部分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="您的身分識別計數"
>abstract="您所選取客群中唯一 ID 的數量，以您和協作者針對專案所同意的比對索引鍵為依據。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="協作者身分識別數量"
>abstract="您的協作者之客群中唯一 ID 的數量，以您和協作者針對專案所同意的比對索引鍵為依據。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重疊的身分識別數量"
>abstract="您和協作者之客群中唯一 ID 的數量，以您和協作者針對專案所同意的比對索引鍵為依據。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="身分識別重疊百分比"
>abstract="您和協作者選取的客群之間身分識別重疊的百分比。"

使用比較對象區段，取得您和共同作業人員的對象之間重疊的豐富資訊。 若要變更對象選擇，請使用&#x200B;**[!UICONTROL 比較對象]**&#x200B;區段頂端的下拉式選擇器。 您可以選取一或全部對象，以及一或全部共同作業人員的對象來相互比較。

![在[比較對象]區段中反白顯示對象選擇器的Discover工作區。](/help/assets/collaborate/discover/compare-audiences-selector.png)

在比較對象區段中，您可以看到以下量度，這些量度是根據您和您的共同作業人員針對專案議定的相符索引鍵：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** （您的） | 您所選對象中的唯一ID數量。 |
| **[!UICONTROL 身分計數]** （您的共同作業人員） | 共同作業人員對象中的唯一ID數量。 |
| **[!UICONTROL 重疊的身分]** | 您的和共同作業人員的對象中同時存在的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 您和您的協作者所選客群間的輪廓重疊百分比。 |
| **[!UICONTROL 對象索引]** | 根據基礎受眾計數和重疊來指出一個受眾與另一個受眾之間關聯程度的分數。 若要深入瞭解分數涵義，請閱讀[對象索引分數](#audience-index-score)區段。 與共同作業人員的基準（所有對象）進行比較時，無法使用對象索引分數。 |
| **[!UICONTROL 依比對索引鍵劃分的身分]** | 根據每個共同作業人員的選取對象，針對專案中選取的每個相符金鑰所比對的身分細目。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重疊百分比數字和對象索引分數不一定適用於所有對象。 重疊百分比和對象索引分數的可見度取決於您的共同作業人員為[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中的對象選擇的設定。

如果您的共同作業人員尚未啟用對象索引或重疊百分比，則對象將沒有任何可用的比較資料。

## 相關客群 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相關客群"
>abstract="根據重疊百分比，這些客群可能是您的行銷活動的理想目標。<br><br><b>身分識別計數</b>是協作者的客群大小。<br><br> <b>重疊的身分識別</b>代表建議客群與所有客群之間的重疊部分。<br><br><b>重疊百分比</b>表示重疊身分識別的數量除以<i>所有</i>客群大小的數值。"

**[!UICONTROL 探索]**&#x200B;標籤中的&#x200B;**[!UICONTROL 相關對象]**&#x200B;區段會根據共同作業人員的對象與所有對象之間的重疊百分比，提供前五個對象的精選清單。 此功能可協助您快速識別重疊程度最高的對象，讓您更有效地鎖定行銷活動。 使用區段右上角的頁面選取器，在相關對象之間切換。

![醒目提示「發現相關對象」區段的Discover工作區。](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>共同作業人員對象的可見度取決於共同作業人員在[連線存取區段](/help/guide/setup/onboard-audiences.md#connection-access)和[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中為對象選擇的設定。 如果您的共同作業人員已將所有對象設為私人，此區段將不會顯示任何對象。

**[!UICONTROL 相關對象]**&#x200B;區段會顯示每個建議對象的下列資訊：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** | 對象中的唯一ID數量。 |
| **[!UICONTROL 重疊的身分]** | 建議的對象與您的所有對象之間重疊的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 建議的對象與您的所有對象之間的重疊身分百分比。 |
| **[!UICONTROL 對象索引]** | 根據基礎受眾計數和重疊來指出一個受眾與另一個受眾之間關聯程度的分數。 若要深入瞭解分數涵義，請閱讀[對象索引分數](#audience-index-score)區段。 |
| **[!UICONTROL 對象類別]** | 您的共同作業人員已指派給對象的類別。 |
| **[!UICONTROL 相符金鑰]** | 共同作業人員為對象選取的相符金鑰。 |

{style="table-layout:auto"}

如果您為任何共同作業人員的對象啟用對象索引分數，則相關對象將會根據對象索引分數，而未啟用對象索引的任何對象將不會包括在內。 系統會根據對象索引分數來排序相關對象，因此會先顯示最高索引分數。 如果您未針對任何共同作業人員的對象啟用對象索引，則相關對象將會根據重疊百分比。

## 探索重疊 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="探索與個別客群的重疊處"
>abstract="取得您與協作者的客群之間重疊情況的深入分析。"

探索重疊，以深入瞭解您的對象與共同作業人員的對象相較之下的情形。 依預設，此區段會將您的所有對象與您的共同作業人員的每個對象進行比較。 使用區段底部的分頁控制項，以導覽至可用的對象。

![反白顯示Discover重疊區段的Discover工作區。](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>共同作業人員對象的可見度取決於共同作業人員在[連線存取區段](/help/guide/setup/onboard-audiences.md#connection-access)和[中繼資料可見度區段](/help/guide/setup/onboard-audiences.md#metadata-visibility)中為對象選擇的設定。 如果您的共同作業人員已將所有對象設為私人，此區段將不會顯示任何對象。

如果您的共同作業人員尚未啟用對象索引或重疊百分比，則不會顯示對象。

若要變更您的對象選擇，請選取&#x200B;**[!UICONTROL 變更對象]**。

![醒目提示「探索工作區」的「變更對象」選項。](/help/assets/collaborate/discover/change-audience.png)

**[!UICONTROL 變更對象]**&#x200B;對話方塊開啟，您可以在其中選取特定對象，與共同作業人員的對象進行比較。 選取想要的對象，或清除您的選取以選取所有對象，然後選取[儲存]。**&#x200B;**

![探索工作區中的[變更對象]對話方塊。](/help/assets/collaborate/discover/change-audience-selection.png)

選取所需的對象後，**[!UICONTROL 探索重疊]**&#x200B;區段會顯示每個對象的下列資訊：

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** | 對象中的唯一ID數量。 |
| **[!UICONTROL 重疊的身分]** | 建議的對象與您的所有對象之間重疊的唯一ID數量。 |
| **[!UICONTROL 重疊%]** | 建議的對象與您的所有對象之間的重疊身分百分比。 |
| **[!UICONTROL 對象索引]** | 根據基礎受眾計數和重疊來指出一個受眾與另一個受眾之間關聯程度的分數。 若要深入瞭解分數涵義，請閱讀[對象索引分數](#audience-index-score)區段。 |
| **[!UICONTROL 對象類別]** | 您的共同作業人員已指派給對象的類別。 |
| **[!UICONTROL 相符金鑰]** | 共同作業人員為對象選取的相符金鑰。 |

{style="table-layout:auto"}

## 客群指數分數 {#audience-index-score}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_audience_index_score"
>title="客群指數分數"
>abstract="客群指數分數是一項考量細微差別的量度，會根據基礎客群數量和重疊度顯示受眾之間的關聯程度。原始指數分數會轉換為相關性區間，將客群指數分數從極低到極高進行分類。這一樣來，您便可以快速評估自己的客群與協作者客群之間的關係強度。"

客群指數分數是一項考量細微差別的量度，會根據基礎客群數量和重疊度顯示受眾之間的關聯程度。這有助於您將對象深入解析化為內容，並找出潛在客戶和行銷活動鎖定目標的高潛力對象。

索引分數使用下列公式計算：

![計算索引分數的公式。](/help/assets/collaborate/discover/index-score-formula.png)

假設有一家汽車製造商想要與一家大型電視發行商就一款新SUV車型展開廣告攻勢。 汽車製造商擁有目前擁有類似車型的資料，並且想要使用這些資料來尋找其他潛在客戶，以便將其轉換為客戶。 汽車製造商會檢視CTV發佈商的受眾，找出與目前SUV擁有者幾乎相符的相關受眾。

![汽車廣告商與CTV發佈者對象。](/help/assets/collaborate/discover/audience-index-score-example.png)

會計算索引分數，並可用於判斷行銷活動是否成功：

| CTV發佈者對象 | 公式 | 索引分數(i) | 解譯 |
|------------------------|-------------|----------------|----------------|
| 基線（所有對象） | (（1.3米/1.3米） / （50米/50米）) * 100 | 100 | 這是與共同作業人員其他對象進行比較的基準。 |
| 觀賞者 | ((500K / 1.3M) / (20M / 50M)) * 100 | 96 | 如果鎖定此對象，相較於基準線，您觸及SUV擁有者的可能性會降低4%。 |
| 喜劇愛好者 | ((200K / 1.3M) / (6M / 50M)) * 100 | 128 | 如果鎖定此對象，相較於基準線，您接觸SUV擁有者的可能性會增加28%。 |
| 男性25-34 | ((700K / 1.3M) / (12M / 50M)) * 100 | 224 | 以這些對象為目標，相較於基準線，您觸及SUV擁有者的可能性高了124%。 |
| 技術愛好者 | ((500K / 1.3M) / (8M / 50M)) * 100 | 240 | 透過鎖定此對象，相較於基準線，您接觸SUV擁有者的可能性高了140%。 |

{style="table-layout:auto"}

為了更瞭解索引分數如何影響您的行銷活動，會與分數一起提供相關性範圍。

### 關聯性範圍 {#audience-index-relevance-bands}

為了方便比較不同對象和促銷活動，Collaboration會將索引分數轉譯為關聯性範圍（從非常低到非常高）。 這一樣來，您便可以快速評估自己的客群與協作者客群之間的關係強度。

| 索引分數(i) | 關聯性範圍 | 說明 |
|---------------|----------|-----------|
| i &lt; 60 | 非常低 | 與您的對象相比，重疊在目標對象中較少發生，這表示關係非常薄弱。 使用此對象的客戶觸及目標對象的可能性低得多。 |
| 60 &lt; i &lt; 80 | 低 | 相較於您的對象，重疊在目標對象中不太普遍，這表示關係較弱。 使用此受眾的客戶觸及目標受眾的可能性較低。 |
| 80 &lt; i &lt; 120 | 媒體 | 重疊在目標對象中和您的對象中一樣普遍，這表示典型的關係。 使用此對象的客戶平均可能會達到其目標對象。 |
| 120 &lt; i &lt; 140 | 高 | 相較於您的對象，重疊在目標對象中更為普遍，表現出強烈的關係。 使用此對象的客戶更容易觸及目標對象。 |
| i > 140 | 非常高 | 相較於您的對象，重疊在目標對象中更為普遍，反映了非常牢固的關係。 使用此對象的客戶更容易觸及目標對象。 |

{style="table-layout:auto"}

在探索重疊區段中，對象索引分數將會與分數一起顯示相關性範圍。 分數會以色彩標示出來，以指出關聯性範圍，讓您一眼就能輕鬆識別關聯性的強度。 極低和極低關聯頻帶會以橘色顯示、中等關聯頻帶以黑色顯示、高和極高關聯頻帶以綠色顯示。

## 後續步驟

探索及探索所需的對象後，是時候[啟用](/help/guide/collaborate/activate.md)應該用於行銷活動的對象。
