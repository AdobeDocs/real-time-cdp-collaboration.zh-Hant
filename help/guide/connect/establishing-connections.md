---
title: 與廣告商或發佈商連結
description: 在發現潛在的共同作業人員後，瞭解如何建立連線並開始共同作業專案。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: c9b96753a9a78bd85002ede3369c5f20eb430548
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 6%

---

# 與廣告商或發佈商連結

{{limited-availability-release-note}}

共同作業人員（通常是廣告商和發佈商）必須先建立連線，才能在行銷活動中合作。 此連線可讓他們啟用對象、建立專案，以及執行行銷活動績效報表。

## 高階工作流程

若要在廣告商和發佈商之間建立連線，需要下列步驟：

1. 廣告商[瀏覽他們想要使用的](/help/guide/connect/discover-publishers.md)發行者並發現它。
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

![在特定發行者上反白顯示[連線]選項的[連線]儀表板。](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

傳送邀請後，您可以預覽（但不能編輯）連線設定。 在&#x200B;**[!UICONTROL 我的連線]**&#x200B;索引標籤中檢視擱置邀請。 連線狀態顯示為&#x200B;**[!UICONTROL 已傳送邀請]**。

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
>abstract="本節會決定哪些人要為Real-Time CDP Collaboration中的對應活動付款。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="客群共用"
>abstract="會根據為啟用準備的相符ID數量，使用對象啟用積分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="測量"
>abstract="執行活動以產生行銷活動績效報表和深入分析。 銷退折讓是根據所有行銷活動的行銷活動報告列數和報告頻率（每日、每三天或每週）。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="法律協議"
>abstract="驗證雙方之間是否存在資料共用協議。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="廣告商名稱"
>abstract="<p>選擇性設定。 表示發佈者知道廣告商的名稱和ID。</p><p>您在此新增的廣告商名稱將會預先填入建立專案步驟。</p><ul><li>如果發行者設定了多個名稱，請從清單中選取一個名稱。</li><li>如果只設定一個名稱，則會自動預先選取該名稱。</li><li>如果未設定名稱，則欄位會預先填入Real-Time CDP Collaboration中的廣告商帳戶名稱。</li></ul>"
>additional-url="https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="建立專案"

傳送邀請後，您可以預覽連線設定。 您必須先接受邀請，才能完成連線的設定。

![處於預覽狀態的連線設定檢視。](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

### 廣告商連線設定 {#advertiser-connection-settings}

共同作業人員接受連線後，請設定連線設定。 這些設定會定義您的共同作業條件，包括您將處理的使用案例、專案的相符索引鍵及其他設定。

若要開始，請瀏覽至&#x200B;**[!UICONTROL 我的連線]**。 對於狀態為&#x200B;**[!UICONTROL 擱置中]**&#x200B;的任何連線，您可以選取&#x200B;**[!UICONTROL 設定連線]**&#x200B;來設定連線設定。

![「我的連線」工作區的「連線擱置中」及其「設定連線」選項已反白顯示。](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

您可以編輯並定義下列欄位：

![連線設定工作區填入之前。](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++使用案例

使用案例已預先填入所有可用選項。 若要自訂這些專案，請在&#x200B;**[!UICONTROL 使用案例]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**，然後關閉您不想要的任何專案。 選取的使用案例決定哪些檢視和選項可在您的專案中[使用](../collaborate/manage-projects.md#project-use-cases)。

![連線設定工作區中的使用案例設定。](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++比對索引鍵

相符金鑰已預先填入您在[設定組織](/help/guide/setup/onboard-organization.md#set-up-match-keys)時所選取的金鑰。 您可以關閉任何不想使用的相符鍵，但無法新增在組織設定期間未選取的相符鍵。

![連線設定工作區中的[相符金鑰]設定。](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++信用分割

使用信用分割區段來決定兩個共同作業關係人中哪一個會涵蓋活動的成本。 評分分割選項由連線選取的使用案例決定。 雖然&#x200B;**[!UICONTROL Measurement]**&#x200B;使用案例需要一方支付成本，但&#x200B;**[!UICONTROL 啟用 — 比對]**&#x200B;使用案例會提供額外的選項，讓各方支付各自的成本。 如需有關成本明細的資訊，請閱讀[信用活動型別](/help/guide/setup/my-activity.md#types-of-activities)指南。

>[!NOTE]
>
>對象 — 輸出一律由接收對象的共同作業人員涵蓋，因此不需要選取。

![具有連線工作區中選項的[信用分割]對話方塊。](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}
+++

+++協定

在繼續進行此連線之前，您必須確認雙方之間存在資料共用協定。

![連線工作區中強調並確認[法律協定]區段。](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

完成選擇後，選取&#x200B;**[!UICONTROL 提交]**&#x200B;將建議的設定傳送給共同作業人員檢閱。

### 發行者連線設定 {#publisher-connection-settings}

發佈者接著需要檢閱連線設定，然後接受或拒絕連線設定。 若要檢閱連線設定，請瀏覽至&#x200B;**[!UICONTROL 我的連線]**，並在連線卡中選擇&#x200B;**[!UICONTROL 檢閱連線設定]**。

![[檢閱連線設定]選項在[我的連線]檢視中反白顯示。](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

檢閱共同作業人員提議的設定。 接受連線設定前，您必須確認您與共同作業人員之間已有法律協定。 此外，您可以新增在您的系統中通知您廣告商的任何廣告商名稱。

![連線設定工作區包含共同作業人員以及反白顯示的廣告商名稱與合約區段的建議設定。](/help/assets/connect/establish-connection/publisher-connection-settings.png){zoomable="yes"}

+++廣告商名稱

身為處理連線設定的發佈者，您可以選取新增在您的系統中您知道該廣告商的任何廣告商名稱。 身為發佈商，您可以將多個廣告商名稱新增至連線，例如您所處理的廣告商出現在多個地理位置時。 在程式後面的步驟中，當[建立要共同作業的專案](/help/guide/collaborate/manage-projects.md#create-project)時，您或您的共同作業人員將能夠選取要與專案關聯的廣告商名稱。

![連線設定工作區中的[廣告商名稱]對話方塊。](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

廣告商名稱選取在建立專案時的運作方式如下：

1. **未設定廣告商名稱**：如果未新增廣告商名稱，Real-Time CDP Collaboration預設會使用廣告商名稱做為廣告商名稱。
2. **一個廣告商名稱集**：如果新增了單一廣告商名稱，Real-Time CDP Collaboration會自動使用該名稱作為專案的廣告商名稱。
3. **設定多個廣告商名稱**：如果新增多個廣告商名稱，您或您的共同作業人員可以在建立專案時選取任何提供的名稱。

![已填入廣告商名稱區段的連線設定工作區。](/help/assets/connect/establish-connection/advertiser-names.png)

+++

>[!NOTE]
>
> 接受連線設定後，您將無法再新增或編輯廣告商名稱。

如果您對提議的連線設定感到滿意，請選取&#x200B;**[!UICONTROL 接受]**&#x200B;以建立連線。 如果您想要要求變更連線設定，請選取&#x200B;**[!UICONTROL 拒絕]**。 接著，共同作業人員可以修訂連線設定，並重新傳送以進行檢閱。

## 刪除連線 {#delete-connections}

您可以刪除與共同作業人員之間不想繼續使用的任何連線。 若要刪除現有的連線，請瀏覽至&#x200B;**[!UICONTROL 連線]**。 然後廣告商應該導覽至&#x200B;**[!UICONTROL 我的連線]**。 選取[連線卡]上的[檢視連線]，以開啟您要刪除的連線。**&#x200B;**

![[我的連線]檢視中反白顯示的[檢視]連線選項。](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

選取連線工作區中的刪除圖示![刪除圖示](/help/assets/common/delete.svg)以刪除連線。

![連線工作區中反白顯示的刪除圖示。](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

確認對話方塊會出現，要求您確認刪除連線。 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以確認刪除。

![刪除連線的確認對話方塊。](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>刪除連線後，您將不會再與共同作業人員連線，而屬於共同作業一部分的所有現有專案將會永久刪除且無法復原。

## 後續步驟

與共同作業人員建立連線後，您和共同作業人員現在可以[建立專案](/help/guide/collaborate/manage-projects.md#create-project)。
