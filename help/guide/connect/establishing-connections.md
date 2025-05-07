---
title: 與廣告商或發佈商連結
description: 在發現潛在的共同作業人員後，瞭解如何建立連線並開始共同作業專案。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: e0894fb3cb290334e0e95d5c26288705967d9dbe
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 13%

---

# 與廣告商或發佈商連結

{{limited-availability-release-note}}

共同作業的兩方（最常見的是廣告商和發佈商）之間建立連線，是Real-Time CDP Collaboration中共同處理行銷活動的公司的先決條件。 發佈者和廣告商都可以設定連線。 之後啟動連線的任何一方將成為&#x200B;*連線擁有者*。

## 高階工作流程

從高層面來看，若要在廣告商和發佈商之間建立連線，工作流程如下所示：

1. 廣告商[瀏覽他們想要使用的發行者並發現](/help/guide/connect/discover-publishers.md)個發行者
2. 廣告商傳送連線邀請。
3. 發行者接受邀請。
4. 廣告商會傳送連線設定，包括比對索引鍵和其他。 這些連線設定代表共同作業的產品內條款。
5. 發行者接受連線設定。 如果需要，發佈者可以拒絕初始連線設定，並要求廣告商提交修訂後的連線設定。

![廣告商 — 發佈商連線程式的高階圖表。](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

完成上述專案後，共同作業人員即可繼續[建立專案](/help/guide/collaborate/manage-projects.md#create-project)至[執行重疊報表](/help/guide/collaborate/discover.md)，並展開廣告行銷活動。

>[!IMPORTANT]
>
>建立兩位共同作業人員之間的連線後，將無法再修訂連線設定。

## 傳送邀請 {#send-invite}

若要設定連線，請在探索發行者畫面中瀏覽發行者詳細目錄時選取&#x200B;**[!UICONTROL 連線]**。

![連線選擇器](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

此時，邀請已退出，您可以預覽連線設定，但無法編輯。 您可以在&#x200B;**[!UICONTROL 我的連線]**&#x200B;標籤中檢視擱置中的邀請。 連線的狀態為&#x200B;**[!UICONTROL 已傳送邀請]**。

![傳送給發行者的擱置邀請會顯示在[我的連線]檢視中。](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

共同作業人員接受邀請後，您就可以設定連線設定，並傳送給共同作業人員檢閱和接受。

## 連線設定 {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="使用案例"
>abstract="使用案例會預先填入所有選項。您可以在提交連線設定之前編輯使用案例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="比對索引鍵"
>abstract="比對索引鍵會預先填入您在組織層級選取的內容。您可以將不想於此連線中使用的任何比對索引鍵切換為關閉。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="點數分割"
>abstract="此區段會決定誰要為 Real-Time CDP Collaboration 中的相應活動付費。目前，只有客群共用使用案例是可設定的。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="客群共用"
>abstract="客群共用是指一方請求合作夥伴啟動其相符的資料時所進行的活動。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="衡量"
>abstract="此使用案例可讓您在Real-Time CDP Collaboration中執行活動，以產生行銷活動績效報表和深入分析。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="法律協議"
>abstract="驗證雙方之間是否存在資料共用協議。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="廣告商名稱"
>abstract="表示發佈者知道廣告商的別名。 "

傳送邀請後，您可以預覽連線設定。 您必須先接受邀請，才能完成連線的設定。

![處於預覽狀態的連線設定檢視。](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

您的共同作業人員接受連線後，您現在就可以開始設定連線的連線設定。 連線設定可定義共同作業的條款，例如要一起完成的使用案例、要在專案中使用的比對索引鍵等等。

若要設定連線設定並與您的共同作業人員共用，請瀏覽至&#x200B;**[!UICONTROL 我的連線]**。 對於狀態為&#x200B;**[!UICONTROL 擱置中]**&#x200B;的任何連線，您可以選取&#x200B;**[!UICONTROL 設定連線]**&#x200B;來設定連線設定。

![我的連線檢視（具有擱置中的連線）及其[設定連線]選項已反白顯示。](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

您可以編輯並定義下列欄位：

![設定連線檢視](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++使用案例

使用案例已預先填入所有可用的使用案例。 您可以選取&#x200B;**[!UICONTROL 編輯]**&#x200B;並切換任何您不想要的使用案例，以選擇連線將使用的使用案例。 選取的使用案例會影響專案中[可用的檢視和選項](../collaborate/manage-projects.md#project-use-cases)。

![使用案例](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++比對索引鍵

相符金鑰已預先填入您在組織層級[選取的金鑰](/help/guide/setup/onboard-organization.md#set-up-match-keys)。 您可以關閉不在此連線中使用的任何相符金鑰，但無法新增在設定組織時未選取的任何相符金鑰。

![相符金鑰](/help/assets/connect/establish-connection/match-keys.png)

+++

+++信用分割

使用信用分割區段來決定兩個共同作業關係人中哪一個會涵蓋活動的成本。

![信用分割](/help/assets/connect/establish-connection/edit-billing-ownership.png)

+++

+++協定

在繼續進行此連線之前，您必須確認雙方之間存在資料共用協定。

![法律協定。](/help/assets/connect/establish-connection/legal-agreement.png)

+++

完成選取後，選取&#x200B;**[!UICONTROL 提交]**&#x200B;將建議的設定傳送給共同作業人員檢閱。

如果您從共同作業人員收到提議的連線設定，您可以&#x200B;**[!UICONTROL 接受]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**&#x200B;這些設定。 接受連線設定前，您必須確認並確認您與共同作業人員之間已有法律協定。 如果您拒絕連線設定，請在產品外部聯絡您的共同作業人員，討論他們應如何修訂連線設定以讓您接受。

## 刪除連線 {#delete-connections}

您可以刪除與共同作業人員之間不想繼續使用的任何連線。 若要刪除現有的連線：

1. 瀏覽至&#x200B;**[!UICONTROL 連線]** > **[!UICONTROL 我的連線]**。
2. 選取[連線卡]上的[檢視連線]，以存取您要刪除的連線。****
3. 選取刪除圖示![刪除圖示](/help/assets/common/delete.svg)以開啟刪除連線確認對話方塊。
   ![刪除醒目提示的連線圖示。](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. 選取&#x200B;**[!UICONTROL 刪除]**以確認刪除。
   ![確認刪除連線的對話方塊。](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>刪除連線後，您將不會再與共同作業人員連線，而屬於共同作業一部分的所有現有專案將會永久刪除且無法復原。

## 後續步驟

與共同作業人員建立連線後，您和共同作業人員現在可以[建立專案](/help/guide/collaborate/manage-projects.md#create-project)。
