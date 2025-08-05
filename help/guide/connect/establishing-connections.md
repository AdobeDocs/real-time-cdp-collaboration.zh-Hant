---
title: 建立連線
description: 在發現潛在的共同作業人員後，瞭解如何建立連線並開始共同作業專案。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: d460cb12b43b6c250a5fb491c1efc223c53abb23
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 7%

---

# 建立連線

{{limited-availability-release-note}}

共同作業人員必須建立連線，才能共同處理行銷活動。 此連線可讓他們啟用對象、建立專案，以及執行行銷活動績效報表。

系統會根據您選擇的共同作業模式來建立連線。 Collaboration支援兩種關鍵共同作業模式：廣告商對發佈商和品牌對品牌。 若要深入瞭解這些模式，請參閱[使用案例](/help/guide/overview/use-cases.md)指南。

<!-- REPLACE THE LINK ABOVE WITH THE CORRECT LINK AFTER PAGE IS ESTABLISHED -->

若要瞭解如何建立連線，請閱讀以下與您的共同作業模式對應的章節：

- [廣告商與發佈商的連線](#advertiser-to-publisher-connection)
- [品牌對品牌連線](#brand-to-brand-connection)

## 廣告商與發佈商的連線 {#advertiser-to-publisher-connection}

![廣告商 — 發佈商連線程式的高階圖表。](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

在廣告商對發佈者模式中，廣告商會透過&#x200B;**[!UICONTROL Discover publishers]**&#x200B;工作區發現他們想要使用的發佈者，並傳送連線邀請。 發佈者接著會稽核並接受邀請，允許廣告商提出連線設定。 發佈者接受連線設定後，連線就會建立，兩個共同作業人員就可以開始一起處理專案。

### 高層級概觀

若要在廣告商與發佈商之間建立連線，需執行下列步驟：

1. [探索發行者](#discover-publishers)：廣告商會識別可與其合作的潛在發行者。
1. [傳送邀請](#send-invite)：廣告商傳送連線邀請給選取的發行者。
1. [接受邀請](#accept-invite)：發行者稽核並接受邀請。
1. [設定連線設定](#configure-connection-settings)：廣告商會設定連線設定，並將設定傳送給發佈者進行稽核。
1. [確認連線設定](#establish-connection)：發行者檢閱連線設定，然後接受或拒絕連線設定。 如果接受，則會建立連線。 若遭拒絕，發佈者可針對產品外部的修訂提供意見回饋。 然後廣告商可以修訂設定並重新傳送以進行稽核。

接受連線設定後，連線即建立，共同作業人員已準備好[建立專案](/help/guide/collaborate/manage-projects.md#create-project)以開始共同作業行銷活動。

## 品牌對品牌連線 {#brand-to-brand-connection}

![品牌對品牌連線程式的高階圖表。](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>術語&#x200B;**品牌**&#x200B;是用來指代Collaboration以外的公司或品牌。 術語&#x200B;**共同作業人員**&#x200B;是指任何可以在Collaboration中建立連線的帳戶，無論其是否為廣告商或發佈者。

在品牌對品牌模式中，在產品外部溝通的兩個品牌，可以使用[私人連線邀請](#private-connection-invite)直接在Collaboration中連線。 品牌可以是廣告商或發佈者。 對於不符合傳統廣告商 — 發佈商模式的品牌（例如兩個廣告商或兩個發佈商），此模式特別實用。

共同作業人員若要開始，會傳送私人連線邀請給其他共同作業人員。 收件者會檢閱邀請並接受邀請，允許擁有者提出連線設定。 一旦收件者接受連線設定，連線就會建立，而且共同作業人員可以開始一起處理專案。

### 高層級概觀

>[!TIP]
>
>討論連線程式時，**所有者**&#x200B;和&#x200B;**收件者**&#x200B;之間會有區別。 擁有者是透過傳送邀請來啟動連線的共同作業人員，而收件者是接收及檢閱邀請的共同作業人員。

兩個品牌之間的連線程式涉及幾個步驟。 在連線程式開始之前，必須滿足幾個先決條件：

1. 兩個品牌在產品外部溝通，討論可能的連線。
1. 品牌[在Collaboration中建立帳戶](/help/guide/setup/onboard-account.md) （如果尚未建立），請務必選取適當的角色型別（廣告商或發佈商）。

   滿足先決條件後，即可開始連線程式。 下列步驟概述此程式：

1. [傳送私人連線邀請](#send-private-connection-invite)：一個共同作業人員傳送私人連線邀請給另一個共同作業人員。
1. [接受私人連線邀請](#accept-private-connection-invite)：收件者檢閱並接受私人連線邀請。
1. [設定連線設定](#configure-connection-settings)：擁有者設定連線設定，並將設定傳送給收件者進行檢閱和接受。
1. [確認連線設定](#establish-connection)：收件者會檢閱連線設定，然後接受或拒絕連線設定。

接受連線設定後，連線即建立，共同作業人員已準備好[建立專案](/help/guide/collaborate/manage-projects.md#create-project)以開始共同作業行銷活動。

## CONNECT {#connect}

**[!UICONTROL 連線]**&#x200B;工作區可讓您管理與共同作業人員的連線、傳送連線邀請，以及廣告商可瀏覽發佈者目錄。 工作區分為兩個主要標籤：

### 探索發佈者 {#discover-publishers}

>[!IMPORTANT]
>
>只有廣告商可以使用&#x200B;**[!UICONTROL Discover publishers]**&#x200B;工作區來探索發佈者。 若要瞭解如何與共同作業人員連線，而不論其角色為何，請閱讀[品牌對品牌連線](#brand-to-brand-connection)區段。

若要探索發行者，請瀏覽至&#x200B;**[!UICONTROL 連線]**&#x200B;索引標籤中的&#x200B;**[!UICONTROL 探索發行者]**&#x200B;工作區。 在這裡，您可以使用工作區底部的分頁控制項，瀏覽可用的發佈者清單。 若要深入瞭解&#x200B;**[!UICONTROL Discover發行者]**&#x200B;工作區，請參閱[Discover發行者](/help/guide/connect/discover-publishers.md)指南。

![Discover發行者工作區顯示可用的發行者清單。](/help/assets/connect/establish-connection/discover-publishers.png){zoomable="yes"}

### 傳送邀請 {#send-invite}

>[!IMPORTANT]
>
>本節說明廣告商透過&#x200B;**[!UICONTROL Discover publishers]**&#x200B;工作區傳送連線邀請給發佈者的程式。 若要瞭解如何在品牌之間建立連線，而不論其角色為何，請閱讀[品牌對品牌連線](#brand-to-brand-connection)區段或造訪[私人連線邀請](#private-connection-invite)區段。

識別要共同作業的發行者後，請選取發行者卡片上的&#x200B;**[!UICONTROL 連線]**&#x200B;選項。 這個動作會啟動連線程式。

![在Discover發行者工作區中的特定發行者上反白顯示[連線]選項。](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

會出現一個對話方塊，提示您傳送連線邀請給發行者。 選取&#x200B;**[!UICONTROL 傳送邀請]**&#x200B;以繼續。

![反白顯示[傳送邀請]按鈕的[傳送連線邀請]對話方塊。](/help/assets/connect/establish-connection/send-connection-invite-dialog.png){zoomable="yes"}

>[!NOTE]
>
>如果您想要與產品外部的發行者聯絡，可以使用私人連線邀請選項。 若要深入瞭解，請參閱[私人連線邀請](#private-connection-invite)區段。

擱置邀請會顯示在&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段的&#x200B;**[!UICONTROL 我的連線]**&#x200B;索引標籤中。 連線狀態顯示為&#x200B;**[!UICONTROL 已傳送邀請]**。 您可以選取&#x200B;**[!UICONTROL 預覽連線]**&#x200B;來預覽連線設定，但只有發行者接受邀請後，才能編輯連線設定。

![擱置的連線會顯示在[需要動作]區段的[我的連線]工作區中。](/help/assets/connect/establish-connection/preview-connection.png){zoomable="yes"}

### 私人連線邀請 {#private-connection-invite}

私人連線邀請可讓您使用&#x200B;**[!UICONTROL 連線代碼]**，與產品外部的合作者連線。 若要建立私人連線，您必須從產品外部要連線的共同作業人員取得&#x200B;**[!UICONTROL 連線代碼]**。 然後，您可以使用此程式碼傳送私人連線邀請給&#x200B;**[!UICONTROL 連線]**&#x200B;工作區中的共同作業人員。

#### 連接代碼 {#connect-code}

在您傳送私人連線邀請之前，您想要的共同作業人員必須提供您唯一的&#x200B;**[!UICONTROL 連線代碼]**。 若要尋找並複製您的&#x200B;**[!UICONTROL 連線代碼]**，請瀏覽至&#x200B;**[!UICONTROL 設定]**&#x200B;工作區中的&#x200B;**[!UICONTROL 我的帳戶]**&#x200B;索引標籤。 **[!UICONTROL 連線代碼]**&#x200B;會顯示在您的帳戶詳細資料中。

![設定工作區中的「我的帳戶」索引標籤中，反白顯示Connect程式碼。](/help/assets/connect/establish-connection/connect-code.png){zoomable="yes"}

選取![Connect程式碼](/help/assets/icons/copy.png)旁的復製圖示（**[!UICONTROL 復製圖示]**）以將其複製到剪貼簿。 然後，您便可以在產品外部將此程式碼與您的共同作業人員共用。

![反白顯示復製圖示的Connect程式碼。](/help/assets/connect/establish-connection/copy-connect-code.png){zoomable="yes"}

##### 重新整理連執行緒式碼 {#refresh-connect-code}

您可以隨時重新整理您的&#x200B;**[!UICONTROL 連線代碼]**。 重新整理程式碼會產生新的唯一程式碼，供您與共同作業人員共用。 如果您基於安全考量想讓先前的程式碼失效，這個方法很有用。 使用舊程式碼建立的任何連線都將保持作用中，但新的共同作業人員需要使用新程式碼與您連線。

>[!IMPORTANT]
>
>在擱置邀請期間重新整理您的&#x200B;**[!UICONTROL 連執行緒式碼]**&#x200B;可能會使邀請無法被接受。 如果您重新整理程式碼，您的共同作業人員可能需要使用新程式碼重新傳送私人連線邀請。

若要重新整理您的&#x200B;**[!UICONTROL 連線代碼]**，請選取![連線代碼](/help/assets/icons/refresh.png)旁的重新整理圖示（**[!UICONTROL 重新整理圖示]**）。

![反白顯示重新整理圖示的Connect程式碼。](/help/assets/connect/establish-connection/refresh-connect-code.png){zoomable="yes"}

>[!IMPORTANT]
>
>在引入&#x200B;**[!UICONTROL 連線代碼]**&#x200B;功能之前建立的任何帳戶將不會有產生的連線代碼，而且連線欄位將顯示為&#x200B;**[!UICONTROL 無法使用]**。 使用重新整理選項來產生新的連線代碼。

#### 傳送私人連線邀請 {#send-private-connection-invite}

從共同作業人員取得&#x200B;**[!UICONTROL 連線代碼]**&#x200B;後，您就可以傳送私人連線邀請。 若要這麼做，請導覽至&#x200B;**[!UICONTROL 連線]**&#x200B;工作區，並選取右上角的加號圖示（![加號圖示](/help/assets/icons/plus.png)）。

![連線工作區中反白的加號圖示。](/help/assets/connect/establish-connection/private-connection-invite.png){zoomable="yes"}

出現&#x200B;**[!UICONTROL 連線]**&#x200B;對話方塊，提示您輸入要連線的共同作業人員的&#x200B;**[!UICONTROL 連線代碼]**。 將程式碼貼到文字欄位中，並選取&#x200B;**[!UICONTROL 繼續]**&#x200B;以繼續。

![已填入[連線]程式碼欄位且[繼續]選項反白顯示的[連線]對話方塊。](/help/assets/connect/establish-connection/private-connection-invite-connect.png){zoomable="yes"}

接著，**[!UICONTROL 連線]**&#x200B;對話方塊會顯示與程式碼關聯的共同作業人員，讓您確認連線的是正確的共同作業人員。 如果共同作業人員正確，請選取&#x200B;**[!UICONTROL 連線]**&#x200B;以傳送私人連線邀請。

![顯示[連線]對話方塊，其中顯示共同作業程式詳細資料，並反白顯示[連線]選項。](/help/assets/connect/establish-connection/private-connection-invite-connect-confirm.png){zoomable="yes"}

### 接受邀請 {#accept-invite}

>[!TIP]
>
>討論連線程式時，**所有者**&#x200B;和&#x200B;**收件者**&#x200B;之間會有區別。 擁有者是透過傳送邀請來啟動連線的共同作業人員，而收件者是接收及檢閱邀請的共同作業人員。

在擁有者可以設定連線設定之前，收件者必須接受連線邀請。 若要這麼做，請瀏覽至&#x200B;**[!UICONTROL 連線]**&#x200B;工作區，並在&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段中尋找擱置的連線。 連線狀態顯示為&#x200B;**[!UICONTROL 收到邀請]**。 選取&#x200B;**[!UICONTROL 接受]**&#x200B;以接受邀請。

![會顯示擱置的連線。連線工作區的[需要動作]區段會反白顯示[接受]選項。](/help/assets/connect/establish-connection/accept-connection.png){zoomable="yes"}

會出現對話方塊，提示您接受邀請。 選取&#x200B;**[!UICONTROL 接受邀請]**&#x200B;以繼續。

![ Accept連線邀請對話方塊中反白顯示Accept邀請選項。](/help/assets/connect/establish-connection/accept-connection-invite.png){zoomable="yes"}

連線的狀態變更為&#x200B;**[!UICONTROL 擱置中]**。 擁有者現在可以設定連線設定。

### 設定連線設定 {#configure-connection-settings}

連線設定會定義兩個共同作業人員之間的術語。 這些設定包括使用案例、比對索引鍵、信用分割和法律協定。 與廣告商連線的共同作業人員也可以將廣告商名稱新增到連線設定，這將在建立專案時使用。

收件者接受邀請後，擁有者即可進行連線設定。 若要這麼做，請瀏覽至&#x200B;**[!UICONTROL 我的連線]**，並在&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段中尋找擱置的連線。 選取&#x200B;**[!UICONTROL 設定連線]**&#x200B;以設定連線設定。

![在[需要動作]區段中反白顯示[連線工作區]與[設定連線]選項。](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

連線設定工作區隨即顯示，可讓您設定連線的各種設定。

![連線設定工作區。](/help/assets/connect/establish-connection/connection-set-up.png){zoomable="yes"}

<!-- FIX THE ABOVE SCREENSHOT TO INCLUDE ADV NAMES, AS WELL AS THE ONES BELOW -->

#### 連線設定 {#connection-settings}

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
>abstract="此區段會確定誰要為 Collaboration 中相應的活動付費。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="客群共用"
>abstract="我們根據準備供啟用使用的相符 ID 數量來消耗 Audience Activation 點數。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="測量"
>abstract="執行活動以產生行銷活動效能報告和深入分析。根據所有行銷活動當中活動報告的資料列數量以及產生報告的頻率 (每日、每三日或每週)，系統會消耗相應的點數。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="法律協議"
>abstract="驗證雙方之間是否存在資料共用協議。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="廣告商名稱"
>abstract="<p>選擇性設定。表示發佈者所知的廣告商名稱和 ID。</p><p>您於此處新增的廣告商名稱，會在建立專案的步驟中預先填入。</p><ul><li>若發佈者設定有多個名稱，請從清單中選取一個。</li><li>若僅設定一個名稱，則會自動預先選取該名稱。</li><li>若未設定任何名稱，則該欄位會預先填入取自 Collaboration 的廣告商帳戶名稱。</li></ul>"
>additional-url="https://experienceleague.adobe.com/zh-hant/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="建立專案"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_activation"
>title="Audience Activation"
>abstract="您可以透過 Audience Activation 選取能夠啟動 Audience Activation 的協作者。"

您可以設定下列連線設定：

+++受眾啟用

>[!IMPORTANT]
>
>在引入&#x200B;**[!UICONTROL 對象啟用]**&#x200B;功能之前建立的任何連線都會自動將對象啟用設定設定設為連線擁有者。 如果您想要允許兩位共同作業人員啟用對象，您需要[刪除目前的連線](#delete-connections)，並使用更新的設定建立新的連線。

對象啟用可讓您選取哪些共同作業人員可以在連線中啟用對象。 只有選取&#x200B;**[!UICONTROL 對象啟用]**&#x200B;使用案例時，才會提供對象啟用選項。 如果您選擇在連線過程中移除使用案例，則會從連線設定中移除對象啟用設定。 若要深入瞭解對象啟用，請參閱[啟用](/help/guide/collaborate/activate.md)指南。

若要設定對象啟用，請在&#x200B;**[!UICONTROL 對象啟用]**&#x200B;區段中選取&#x200B;**[!UICONTROL 設定]**。 使用下拉式選單來指定哪些共同作業人員可以啟用對象。 您可以選擇單一共同作業人員，或允許兩個共同作業人員啟用對象。

![在連線設定工作區中使用選項的[對象啟用]對話方塊。](/help/assets/connect/establish-connection/audience-activation.png){zoomable="yes"}

完成後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

![連線設定工作區中具有「儲存」選項的「對象啟動」對話方塊。](/help/assets/connect/establish-connection/audience-activation-confirm.png){zoomable="yes"}

+++

+++使用案例

使用案例會自動填入所有可用選項。 所選的使用案例決定您的專案中可用的檢視和選項。 若要深入瞭解，請閱讀[專案使用案例](/help/guide/collaborate/manage-projects.md#project-use-cases)指南。

若要自訂您的使用案例，請在&#x200B;**[!UICONTROL 使用案例]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**，並關閉任何您不想要與共同作業人員加入的專案。 完成後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

![連線設定工作區中的使用案例設定。](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++比對索引鍵

比對金鑰會自動填入您在[設定您的帳戶](/help/guide/setup/onboard-account.md#set-up-match-keys)時所選取的金鑰。 您可以關閉任何不想使用的相符金鑰，但無法新增在帳戶設定期間未選取的相符金鑰。

若要自訂您的相符金鑰，請在&#x200B;**[!UICONTROL 相符金鑰]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**，並關閉您不想要在此連線中使用的相符金鑰。 完成後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

![連線設定工作區中的[相符金鑰]設定。](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++信用分割

使用信用分割區段來決定兩個共同作業關係人中哪一個會涵蓋活動的成本。 評分分割選項由連線選取的使用案例決定。 雖然&#x200B;**[!UICONTROL Measurement]**&#x200B;使用案例需要一方支付成本，但&#x200B;**[!UICONTROL 啟用 — 比對]**&#x200B;使用案例會提供額外的選項，讓各方支付各自的成本。 如需有關成本明細的資訊，請閱讀[信用活動型別](/help/guide/setup/my-activity.md#types-of-activities)指南。

>[!NOTE]
>
>對象 — 輸出一律由接收對象的共同作業人員涵蓋，因此不需要選取。

若要設定信用分割，請在&#x200B;**[!UICONTROL 信用分割]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。 然後，您可以為每個使用案例選取適當的選項。 完成後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

![在連線設定工作區中使用選項的[信用分割]對話方塊。](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}

+++

+++協定

您必須確認您與共同作業人員之間已有法律協定。 本協定概述資料共用和共同作業的條款。 您可以選取&#x200B;**[!UICONTROL 確認並確認]**&#x200B;核取方塊，以確認此合約存在。

![連線工作區中強調並確認[法律協定]區段。](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

+++廣告商名稱

>[!NOTE]
>
>此選項可能會出現在連線設定組態或檢閱連線設定期間，視起始連線的人員而定。

如果您是發行者，與廣告商形成連線，則可選擇在連線設定中新增廣告商名稱。 這可讓您新增在您的系統中通知廣告商的多個名稱。 如果廣告商出現在多個地理位置，或在不同內容中以不同的名稱識別，這會特別有用。 稍後，當您建立專案時，您可以從連線設定中所設定的名稱清單中選取適當的廣告商名稱。

![連線設定工作區中的廣告商名稱。](/help/assets/connect/establish-connection/advertiser-names.png){zoomable="yes"}

若要新增廣告商名稱，請在&#x200B;**[!UICONTROL 廣告商名稱]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。 然後，您可以輸入在您的系統中您知道的廣告商的&#x200B;**[!UICONTROL 廣告商ID]**，以及要在Collaboration中與該ID建立關聯的&#x200B;**[!UICONTROL 廣告商名稱]**。 您可以選取&#x200B;**[!UICONTROL 新增]**&#x200B;選項，以新增多個廣告商名稱。

![在連線設定工作區中使用選項的[廣告商名稱]對話方塊。](/help/assets/connect/establish-connection/advertiser-names-dialog.png){zoomable="yes"}

完成後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

建立專案時，廣告商名稱將根據連線期間建立的下列設定預先填入    ：

1. **未設定廣告商名稱**：如果未新增廣告商名稱，Collaboration預設會使用廣告商名稱做為廣告商名稱。
1. **一個廣告商名稱集**：如果新增了單一廣告商名稱，Collaboration會自動使用該名稱作為專案的廣告商名稱。
1. **設定多個廣告商名稱**：如果新增多個廣告商名稱，您或您的共同作業人員可以在建立專案時選取任何提供的名稱。

>[!NOTE]
>
> 傳送連線設定後，您將無法再新增或編輯廣告商名稱。

![已填入廣告商名稱區段的連線設定工作區。](/help/assets/connect/establish-connection/add-advertiser-names.png)

+++

選取之後，選取&#x200B;**[!UICONTROL 提交]**&#x200B;將建議的設定傳送給收件者進行檢閱。

### 審核連線設定 {#review-connection-settings}

接著，收件者需要檢閱擁有者提出的連線設定。 收件者可以瀏覽至&#x200B;**[!UICONTROL 連線]**&#x200B;工作區中的&#x200B;**[!UICONTROL 我的連線]**&#x200B;索引標籤來執行此動作。 連線將顯示在&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段中。 選取&#x200B;**[!UICONTROL 檢閱連線設定]**&#x200B;以檢閱建議的連線設定。

![反白顯示[檢閱連線設定]選項的[我的連線]工作區。](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

檢閱共同作業人員提議的設定。 您可以接受或拒絕連線設定。 如果您拒絕連線設定，則必須與共同作業人員溝通您要在產品外部進行的變更。 共同作業人員的連絡資訊會顯示在連線設定工作區的&#x200B;**[!UICONTROL 連絡人]**&#x200B;區段中。 然後，擁有者可以修訂連線設定，並重新傳送它們以供檢閱。

如果您對提議的連線設定感到滿意，則必須確認您與共同作業人員之間已達成法律協定。 選取&#x200B;**[!UICONTROL 確認並確認]**&#x200B;核取方塊，以確認此合約存在。

![連線設定工作區中強調的[法律協定]區段。](/help/assets/connect/establish-connection/legal-agreement-review.png){zoomable="yes"}

此外，如果您是發行者且正在連線廣告商，您現在可以在連線設定中新增廣告商名稱。 若要深入瞭解此程式，請參閱[連線設定](#connection-settings)區段。

>[!NOTE]
>
> 接受連線設定後，您將無法再新增或編輯廣告商名稱。

接著，選取&#x200B;**[!UICONTROL 接受]**&#x200B;以繼續連線。 連線狀態將變更為&#x200B;**[!UICONTROL 作用中]**，您現在可以開始共同作業專案。

## 刪除連線 {#delete-connections}

您可以刪除與共同作業人員之間不想繼續使用的任何連線。 若要刪除現有的連線，請瀏覽至&#x200B;**[!UICONTROL 連線]**。 您的現有連線身為發佈者，將會顯示出來。 身為廣告商，您應該導覽至&#x200B;**[!UICONTROL 我的連線]**。

在您要刪除的連線卡上選取&#x200B;**[!UICONTROL 檢視連線]**。

![[我的連線]檢視中反白顯示的[檢視]連線選項。](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

選取連線工作區中的刪除圖示![刪除圖示](/help/assets/common/delete.svg)以刪除連線。

![連線工作區中反白顯示的刪除圖示。](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

確認對話方塊會出現，要求您確認刪除連線。 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以確認刪除。

![刪除連線的確認對話方塊。](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>刪除連線後，共同作業中的所有現有專案將會永久刪除且無法復原。 連線要求將維持擱置狀態，但連線及其設定將不再有效。 如果您想要再次與共同作業人員連線，則需要重新建立連線。

## 後續步驟

與共同作業人員建立連線後，您和共同作業人員現在可以[建立專案](/help/guide/collaborate/manage-projects.md#create-project)。
