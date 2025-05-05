---
title: 共用客群
description: 瞭解如何與您的共同作業人員共用受眾，以利進行廣告行銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 共用客群

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 共用]**&#x200B;工作區只有在連線程式[&#128279;](../connect/establishing-connections.md#connection-settings)期間啟用&#x200B;**對象共用與啟用**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

作為廣告商，瞭解如何與您的發佈者共用對象，以便他們能夠執行行銷活動。 如果您的共同作業已啟用&#x200B;**探索對象**&#x200B;使用案例，請先在[探索標籤](/help/guide/collaborate/discover.md)執行重疊報表，以識別要共用的最佳對象。

## 共用新對象

若要開始共用對象，請導覽至專案工作區中的&#x200B;**[!UICONTROL 共用]**&#x200B;索引標籤。 只有&#x200B;**廣告商組織**&#x200B;可以共用行銷活動的對象。 在此標籤中，您可以檢閱及管理共用對象。

選取&#x200B;**加號符號(+)**，或選取&#x200B;**[!UICONTROL 共用對象]**&#x200B;選項（如果尚未共用先前的對象），以開始對象共用程式。

![預設檢視，未共用任何對象。](/help/assets/collaborate/share/share-new-audiences.png)

新面板隨即顯示，您可以在其中選取要與共同作業人員共用的對象。

![共用新的對象工作流程。](/help/assets/collaborate/share/share-audiences-workflow.png)

### 選取要共用的對象

在對象選擇視窗中，您可以在搜尋列中輸入對象名稱，以搜尋要共用的特定對象。 選取&#x200B;**[!UICONTROL 瀏覽對象]**，並使用可用的排序選項來尋找您需要的確切對象。

![瀏覽選取對象的對象檢視。](/help/assets/collaborate/share/browse-audiences-view.png)

### 編輯比對索引鍵並設定鎖定目標選項

選取要共用的對象後，您現在可以為共用活動選取其他設定選項。

![編輯比對索引鍵和目標或隱藏反白顯示的選取器](/help/assets/collaborate/share/match-keys-and-targeting.png)

選取&#x200B;**[!UICONTROL 編輯相符金鑰]**&#x200B;以指示應該用於對象中身分識別的相符金鑰。 這些選項繼承自最初設定共同作業人員之間連線時選取的設定。 如果選取的相符金鑰不適用於此特定行銷活動，您可以移除該時選取的相符金鑰，但此時您無法新增相符金鑰。

![編輯相符金鑰。](/help/assets/collaborate/share/update-match-keys.png)

針對每個對象，選取您要在行銷活動中鎖定或隱藏該對象的成員。 抑制的設定檔將不會是發佈者所啟動之對象的一部分。

### 設定對象重新整理頻率和間隔

最後，設定對象重新整理的所需頻率和日期範圍。 目前支援的對象重新整理模式為&#x200B;**[!UICONTROL 一次]**&#x200B;和&#x200B;**[!UICONTROL 每日]**。

選取&#x200B;**[!UICONTROL 一次]**&#x200B;時，在行銷活動期間不會重新整理對象會籍。 選取&#x200B;**[!UICONTROL 每日]**&#x200B;時，對象會籍會在行銷活動期間每天重新整理一次。

![反白顯示頻率選項。](/help/assets/collaborate/share/audience-refresh-frequency.png)

如果滿意您的選擇，請選取&#x200B;**[!UICONTROL 共用]**&#x200B;以完成工作流程。

>[!SUCCESS]
>
>您現在可以在&#x200B;**[!UICONTROL 共用]**&#x200B;索引標籤中看到新的對象共用活動。 如有需要，您可以返回並編輯您所做的任何選擇。

## 檢視目前共用的對象

在&#x200B;**[!UICONTROL 共用]**&#x200B;標籤中，您可以檢視目前共同作業人員之間共用的對象，這些對象會分組在對象共用活動中。

![共用標籤的總覽。](/help/assets/collaborate/share/share-tab-overview.png)

<!--

The banner at the top of the page shows figures across all audience sharing activities. 

![The hero banner in the sharing tab.](/help/assets/collaborate/share/share-hero-banner.png)


|Metric | Description |
|---------|----------|
| **[!UICONTROL Shared audiences]** | Indicates the number of audiences shared between collaborators in this project, across all audience sharing modules. |
| **[!UICONTROL Estimated addressable reach]** | Indicates the approximate number of profiles that you can reach across all the audiences that are currently shared in the project. [TODO: ADD INFORMATION ABOUT HOW THIS IS CALCULATED] |
| **[!UICONTROL Target identities]** | The number of identities across all audiences shared in this project for which you selected to target the profiles. |
| **[!UICONTROL Suppress identities]** | The number of identities across all audiences shared in this project for which you selected to suppress the profiles and thereby not target them in campaigns. |

-->

在每個受眾共用活動中，您可以取得每個共用受眾的相關資訊。

| 量度 | 說明 |
|---------|----------|
| **[!UICONTROL 身分計數]** | 表示根據最新的身分計數評估，與此對象繫結的所有身分中的設定檔數。 這些數字每24小時會重新整理一次。 |
| **[!UICONTROL 重疊的身分]** | 表示此對象成員之間的重疊身分數目，以及共同作業人員詳細目錄中的設定檔總母體。 |
| **[!UICONTROL 比對索引鍵劃分]** | 顯示對象中使用的每個身分的身分計數。 例如，50萬名使用者的身分總數中，可能包括40萬名使用者中斷了雜湊電子郵件身分識別，以及10萬名使用者中斷了行動身分識別身分識別。 請注意，在此說明的範例中，同一個人可能會以其電子郵件和行動ID身分出現在對象中兩次。 |
| **[!UICONTROL 目標]** | **[!UICONTROL 隱藏]**&#x200B;或&#x200B;**[!UICONTROL 目標]**。 顯示受眾成員是應該鎖定目標還是應該從行銷活動中排除。 |

此頁面也提供控制項，讓您&#x200B;**[!UICONTROL 暫停共用]**&#x200B;和&#x200B;**[!UICONTROL 編輯對象]**。

## 編輯客群 {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="目標或隱藏使用案例"
>abstract="<p>如果您希望在行銷活動中對客群中的輪廓展示廣告，請選取「**目標**」。</p> <p>如果您傳送行銷活動訊息的對象要排除客群中的輪廓，請選取「**隱藏**」。</p>"

選取「**[!UICONTROL 編輯對象]**」以變更對象共用模組中的對象，以及變更與對象共用方式相關的數個設定。

![編輯對象強制回應視窗的檢視](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## 後續步驟

發行者收到共用對象後，現在會在數位廣告行銷活動中[啟用](/help/guide/collaborate/activate.md)這些對象。
