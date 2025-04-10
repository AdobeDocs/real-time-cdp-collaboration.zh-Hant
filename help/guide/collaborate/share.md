---
title: 共用客群
description: 瞭解如何與您的共同作業人員共用受眾，以利進行廣告行銷活動。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%

---

# 共用客群

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 共用]**&#x200B;工作區只有在連線程式](../connect/establishing-connections.md#connection-settings)期間[啟用&#x200B;**對象共用與啟用**&#x200B;使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./manage-projects.md#project-use-cases)指南。

作為廣告商，瞭解如何與您的發佈者共用對象，以便他們能夠執行行銷活動。 如果您的共同作業已啟用&#x200B;**探索對象**&#x200B;使用案例，請先在[探索標籤](/help/guide/collaborate/discover.md)執行重疊報表，以識別要共用的最佳對象。

## 共用新對象

若要開始共用對象，請導覽至專案工作區中的&#x200B;**[!UICONTROL 共用]**&#x200B;索引標籤。 只有&#x200B;**廣告商組織**&#x200B;可以共用行銷活動的對象。 在此標籤中，您可以查看和管理共享的觀眾。

選擇加 **號 （+），**&#x200B;如果沒有 **[!UICONTROL 共用以前的受眾，請選擇共用對象]** 選項，以開始對象共享過程。

![沒有共享觀眾的默認視圖。](/help/assets/collaborate/share/share-new-audiences.png)

新面板隨即顯示，您可以在其中選擇要與協作者共用的受眾。

![共用新的對象工作流程。](/help/assets/collaborate/share/share-audiences-workflow.png)

### 選取要共用的對象

在對象選擇窗口中，您可以通過在搜尋欄中輸入對象名稱來搜尋特定受眾進行共享。 選擇 **[!UICONTROL 瀏覽對象]** ，然後使用可用的排序選項查找所需的確切物件。

![瀏覽物件視圖已選取物件。](/help/assets/collaborate/share/browse-audiences-view.png)

### 編輯匹配鍵並設置目標定位選項

選擇要共享的所需受眾後，您現在可以為共享活動選擇其他配置選項。

![編輯匹配鍵並目標或抑制突出显示選擇器](/help/assets/collaborate/share/match-keys-and-targeting.png)

選取&#x200B;**[!UICONTROL 編輯相符金鑰]**&#x200B;以指示應該用於對象中身分識別的相符金鑰。 這些選項繼承自最初設定共同作業人員之間連線時選取的設定。 如果選取的相符金鑰不適用於此特定行銷活動，您可以移除該時選取的相符金鑰，但此時您無法新增相符金鑰。

![編輯相符金鑰。](/help/assets/collaborate/share/update-match-keys.png)

對於每個對象，選擇是將該對象的成員按讚為目標還是在行銷活動中禁止顯示。 禁止顯示的配置文件尤其不屬於發佈者所啟動的對象。

### 設置刷新對象頻率和間隔

最後，設定對象重新整理的所需頻率和日期範圍。 目前支援的對象重新整理模式為&#x200B;**[!UICONTROL 一次]**&#x200B;和&#x200B;**[!UICONTROL 每日]**。

選取&#x200B;**[!UICONTROL 一次]**&#x200B;時，在行銷活動期間不會重新整理對象會籍。 選取&#x200B;**[!UICONTROL 每日]**&#x200B;時，對象會籍會在行銷活動期間每天重新整理一次。

![反白顯示頻率選項。](/help/assets/collaborate/share/audience-refresh-frequency.png)

如果滿意您的選擇，請選取&#x200B;**[!UICONTROL 共用]**&#x200B;以完成工作流程。

>[!SUCCESS]
>
>您現在可以在「共享&#x200B;]**」標籤中看到**[!UICONTROL &#x200B;新的「對象共享」活動。如果需要，您可以返回並編輯您所做的任何選擇。

## 檢視目前共享的物件

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
| **[!UICONTROL 身分計數]** | 根據最新的標識計數評估，指示與此對象關聯的所有標識的配置文件數。 這些數位每 24 小時刷新一次。 |
| **[!UICONTROL 身份重疊]** | 表示此對象成員之間的重疊身分數目，以及共同作業人員詳細目錄中的設定檔總母體。 |
| **[!UICONTROL 比對索引鍵劃分]** | 顯示對象中使用的每個身分的身分計數。 例如，50萬名使用者的身分總數中，可能包括40萬名使用者中斷了雜湊電子郵件身分識別，以及10萬名使用者中斷了行動身分識別身分識別。 請注意，在此說明的範例中，同一個人可能會以其電子郵件和行動ID身分出現在對象中兩次。 |
| **[!UICONTROL 目標]** | **[!UICONTROL 抑制]** 或 **[!UICONTROL Target]**。 顯示受眾成員是應該鎖定目標還是應該從行銷活動中排除。 |

該頁面也提供控件供您 **[!UICONTROL 暫停分享]** 及 **[!UICONTROL 編輯物件]**。

## 編輯客群 {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="鎖定或隱藏使用案例"
>abstract="<p>如果您想要對象中的設定檔在行銷活動中顯示廣告，請選取&#x200B;**Target**。</p> <p>如果您要將對象中的設定檔從行銷活動訊息中排除，請選取&#x200B;**隱藏**。</p>"

選擇 **[!UICONTROL 編輯受眾]** 以更改在對象共享模組中共享的物件，以及更改與共享受眾方式相關的多個配置。

![编辑物件模式檢視](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## 後續步驟

發佈者收到共享的觀眾之後，就會 [在數位廣告促銷活動中啟用](/help/guide/collaborate/activate.md) 這些觀眾。
