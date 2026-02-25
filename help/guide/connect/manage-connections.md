---
title: 管理連線
description: 瞭解如何在Real-Time CDP Collaboration中管理連線。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 50120839-4a20-4ec1-8887-9342bd17c52d
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 1%

---

# 管理連線 {#manage-connections}

{{limited-availability-release-note}}

**[!UICONTROL 我的連線]**&#x200B;工作區提供管理連線的集中位置。 您可以在&#x200B;**[!UICONTROL 現有連線]**&#x200B;區段中檢視現有連線，並在&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段中檢視任何需要動作的連線。

## 檢視連線 {#view-connection}

若要檢視您現有的連線，請瀏覽至&#x200B;**[!UICONTROL 連線]**&#x200B;工作區。 您的現有連線身為發佈者，將會顯示出來。 身為廣告商，您應該導覽至&#x200B;**[!UICONTROL 我的連線]**。

![在[我的連線]工作區中，針對連線反白顯示[檢視連線]選項。](/help/assets/connect/manage-connections/view-connection.png){zoomable="yes"}

連線總覽工作區隨即顯示，顯示有關連線及其使用中專案的詳細資訊。 選取&#x200B;**[!UICONTROL 連線設定]**&#x200B;以檢視連線設定。

![連線總覽工作區中反白顯示的[連線設定]選項。](/help/assets/connect/manage-connections/connection-overview.png){zoomable="yes"}

連線設定工作區隨即顯示，顯示您與共同作業人員之間的連線詳細資料。 在這裡，您可以檢視連線過程中選取的所有設定、連線的目前狀態、連線擁有者，以及共同作業人員的連絡資訊。 如需特定連線設定的詳細資訊，請參閱[連線設定](/help/guide/connect/establishing-connections.md#connection-settings)指南。

![顯示連線詳細資料的連線設定工作區。](/help/assets/connect/manage-connections/connection-settings.png){zoomable="yes"}

## 刪除連線 {#delete-connection}

您可以刪除與共同作業人員之間不想繼續使用的任何連線。 若要刪除連線，請瀏覽至您要刪除的連線，然後在連線工作區中選取刪除圖示![刪除圖示](/help/assets/common/delete.svg)。

![連線工作區中反白顯示的刪除圖示。](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

確認對話方塊會出現，要求您確認刪除連線。 選取&#x200B;**[!UICONTROL 刪除]**&#x200B;以確認刪除。

![刪除連線的確認對話方塊。](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>刪除連線後，共同作業中的所有現有專案將會永久刪除且無法復原。 在&#x200B;**[!UICONTROL 我的連線]**&#x200B;內的&#x200B;**[!UICONTROL 需要動作]**&#x200B;區段內，連線要求將保持擱置狀態，但連線及其設定將不再有效。 如果您想要再次與共同作業人員連線，則需要重新建立連線。

## 編輯連線 {#edit-connection}

身為共同作業連線的擁有者，您可以在建立連線後編輯與共同作業人員的連線設定。 您可以：

* 新增使用案例
* 新增相符金鑰。 未來將支援移除相符金鑰。
* 更新對象啟用許可權
* 更新信用分攤設定

>[!IMPORTANT]
>
>使用案例或比對金鑰新增至連線後，即無法移除。

>[!TIP]
>
>**所有者**&#x200B;是透過傳送邀請給&#x200B;**收件者**&#x200B;來啟動連線的共同作業人員。 如需詳細資訊，請參閱[與共同作業人員建立連線檔案](./establishing-connections.md)。

若要編輯連線設定，請瀏覽至連線設定工作區。 選取三點圖示(![三點圖示。](/help/assets/icons/more.png))以檢視可用的動作，然後選取&#x200B;**[!UICONTROL 編輯]**。

![連線設定工作區中反白顯示[編輯]選項。](/help/assets/connect/manage-connections/edit-connection.png){zoomable="yes"}

此時會出現一個對話方塊，提示您編輯並提交設定變更，以供共同作業人員檢閱。 選取&#x200B;**[!UICONTROL 編輯]**。

![反白顯示[編輯]選項的[編輯連線設定]對話方塊。](/help/assets/connect/manage-connections/edit-connection-settings-dialog.png){zoomable="yes"}

### 編輯對象啟用 {#edit-audience-activation}

對象啟用設定決定連線中的哪個共同作業人員可將對象啟用至目的地。 若要變更這些設定，請在&#x200B;**[!UICONTROL 對象啟用]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![顯示[對象啟動]區段和[編輯]選項的編輯連線設定畫面。](/help/assets/connect/manage-connections/edit-audience-activation.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 對象啟用]**&#x200B;對話方塊中，使用下拉式功能表來更新對象啟用許可權。 您可以選擇單一共同作業人員，或允許兩個共同作業人員啟用對象。

![展開的[對象啟用]對話方塊醒目提示下拉式功能表，可更新對象啟用許可權。](/help/assets/connect/manage-connections/audience-activation-dropdown-menu.png){zoomable="yes"}

完成後，選取&#x200B;**[!UICONTROL 儲存]**。

![此對象啟用對話方塊顯示新的對象啟用許可權和[儲存]選項。](/help/assets/connect/manage-connections/audience-activation-dialog.png){zoomable="yes"}

### 新增使用案例 {#add-use-cases}

在Collaboration中，「探索」、「啟動」和「測量」等使用案例會決定您可與共同作業人員使用的專案區段和功能。 您可以將其他使用案例新增到現有連線中，以供日後專案使用。 如需詳細資訊，請參閱[共同作業使用案例](../overview/use-cases.md)。

若要新增使用案例，請在&#x200B;**[!UICONTROL 使用案例]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![編輯連線設定畫面會醒目提示「使用案例」區段和「編輯」選項。](/help/assets/connect/manage-connections/edit-use-cases.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 使用案例]**&#x200B;對話方塊中，開啟您要新增的使用案例，然後開啟&#x200B;**[!UICONTROL 儲存]**。

![顯示[儲存]選項的[使用案例]對話方塊反白顯示。](/help/assets/connect/manage-connections/use-cases-dialog.png){zoomable="yes"}

>[!NOTE]
>
>當您[新增使用案例](#add-use-cases) （例如「對象啟用」或「測量」）時，編輯連線設定畫面會更新以包含&#x200B;**[!UICONTROL 對象啟用]**&#x200B;和&#x200B;**[!UICONTROL 信用分割]**&#x200B;區段。 您必須針對這些新使用案例進行適當的設定。 如需詳細資訊，請參閱[對象啟用](../connect/establishing-connections.md#audience-activation)與[信用分割](../connect/establishing-connections.md#credit-split)指南。
>
>![新增使用案例後，編輯連線設定畫面會顯示對象啟用和信用分割區段。](/help/assets/connect/manage-connections/setup-audience-activation-credit-split.png){zoomable="yes"}

### 新增相符金鑰 {#add-match-keys}

連線只能使用在您的帳戶中設定且由共同作業人員選取的相符金鑰。 一旦您[新增相符金鑰至您的帳戶](../setup/onboard-account.md#edit-match-keys)且您的共同作業人員也選取相同的金鑰後，您就可以在現有的連線中啟用它們。

在編輯連線設定畫面中，選取&#x200B;**[!UICONTROL 比對索引鍵]**&#x200B;區段內的&#x200B;**[!UICONTROL 編輯]**。

![編輯連線設定畫面醒目提示[符合索引鍵]區段和[編輯]選項。](/help/assets/connect/manage-connections/edit-connection-match-keys.png){zoomable="yes"}

出現&#x200B;**[!UICONTROL 比對金鑰]**&#x200B;對話方塊，顯示為連線設定的現有比對金鑰。 選取您要新增的相符金鑰，然後選取&#x200B;**[!UICONTROL 儲存]**。

![[比對金鑰]對話方塊顯示選取的新比對金鑰與[儲存]選項。](/help/assets/connect/manage-connections/connection-match-keys-dialog.png){zoomable="yes"}

### 編輯評分分割 {#edit-credit-split}

信用分攤設定可指定由哪個共同作業人員負責與連線中每個使用案例相關的成本。 若要更新這些設定，請在&#x200B;**[!UICONTROL 信用分割]**&#x200B;區段中選取&#x200B;**[!UICONTROL 編輯]**。

![編輯連線設定畫面醒目提示[信用分割]區段和[編輯]選項。](/help/assets/connect/manage-connections/edit-credit-split.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 信用分割]**&#x200B;對話方塊中，選取[!UICONTROL 啟用比對]與[!UICONTROL 測量]的偏好設定。 然後，選取&#x200B;**[!UICONTROL 儲存]**&#x200B;以進行確認。

![顯示信用分割設定和[儲存]選項的[信用分割]對話方塊。](/help/assets/connect/manage-connections/credit-split-dialog.png){zoomable="yes"}

### 檢閱並提交變更 {#review-and-submit-changes}

當您完成編輯連線設定時，請檢閱並選取&#x200B;**[!UICONTROL 送出變更]**。 連線設定更新將會傳送給您的共同作業人員以供檢閱。

![編輯連線設定畫面會顯示更新和[送出變更]選項。](/help/assets/connect/manage-connections/review-and-submit-changes.png){zoomable="yes"}

#### 將連線設定變更儲存為草稿

您可以將連線設定變更儲存為草稿，並隨時返回完成連線設定的更新。

若要將變更儲存為草稿，請選取&#x200B;**[!UICONTROL 送出變更]**&#x200B;旁的&#x200B;**[!UICONTROL 取消]**。 然後，在&#x200B;**[!UICONTROL 未提交的變更]**&#x200B;對話方塊中，選取&#x200B;**[!UICONTROL 稍後繼續]**&#x200B;以確認。

![編輯連線設定畫面。](/help/assets/connect/manage-connections/unsubmitted-changes-dialog.png){zoomable="yes"}

您的變更現在會儲存為草稿。 在連線設定工作區中，您可以看到一則通知，指出有未提交的變更。 若要進行進一步的更新，請選取&#x200B;**[!UICONTROL 繼續編輯]**。

![連線設定工作區中的通知，顯示有未提交的變更等待檢閱和提交。](/help/assets/connect/manage-connections/continue-editing-connection.png){zoomable="yes"}
