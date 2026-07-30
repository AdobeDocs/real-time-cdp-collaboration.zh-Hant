---
title: 設定和管理雲端儲存空間目的地
description: 瞭解如何在Real-Time CDP Collaboration中設定、檢視和刪除雲端儲存空間目的地。
audience: admin, publisher
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 60124235569ca9b17b3bb1cef502d57d39e82e1f
workflow-type: tm+mt
source-wordcount: 885
ht-degree: 2%

---

# 設定和管理雲端儲存空間目的地

使用本指南從&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區設定、檢視及刪除雲端儲存空間目的地。 使用「**[!UICONTROL 目錄]**」標籤設定目的地、「**[!UICONTROL 目的地]**」標籤來管理目的地，並使用「**[!UICONTROL 啟用的對象]**」標籤檢閱啟用至目的地的對象。

設定目的地後，當您啟用對象時即可使用該目的地。 若要檢視支援的目的地完整清單，請參閱[可用的目的地](./overview.md#available-destinations)表格。

>[!NOTE]
>
> 本指南以&#x200B;**[!DNL Amazon S3]**&#x200B;目的地為例。 引導式設定工作流程會在支援的雲端儲存空間目的地型別之間共用，但驗證方法、必填欄位和聯結器功能可能會有所不同。 在設定目的地之前，請先檢閱[雲端儲存空間目的地需求](./cloud-storage-destination-requirements.md)，其連結至相對應的Adobe Experience Platform目的地檔案。
>
> Adobe Experience Platform在Real-Time CDP Collaboration中有獨立的設定工作流程。 若要進行設定，請參閱[將Adobe Experience Platform設定為目的地](./experience-platform.md)。

## 先決條件 {#prerequisites}

在設定目的地之前，請確定：

* 您可以存取&#x200B;**[!UICONTROL 啟用]**&#x200B;工作區。
* 您擁有雲端儲存空間提供者所需的連線資訊。
* 如果您需要建立帳戶，則需具備所需的認證或許可權。
* 您已檢閱您的雲端儲存空間目的地[&#128279;](./cloud-storage-destination-requirements.md)的需求。

## 設定目的地 {#configure-destination}

當您設定目的地時，請將雲端儲存空間帳戶連線至Real-Time CDP Collaboration並定義將受眾資料匯出至該帳戶的方式。

瀏覽至&#x200B;**[!UICONTROL 啟用]** > **[!UICONTROL 目錄]**。

**[!UICONTROL 目錄]**&#x200B;索引標籤會顯示可用的目的地提供者。 每個目的地都會顯示為一個卡片。 視目的地而定，其卡片可顯示已設定的帳戶和動作，以檢視其他資訊。

![顯示目的地提供者卡片的目錄標籤。](/help/assets/destinations/manage-destinations/destination-provider-catalog.png)

找到您要設定的目的地提供者，然後選取&#x200B;**[!UICONTROL 設定]**。

目的地組態引導式安裝程式會開啟，並引導您完成四個步驟： **[!UICONTROL 驗證]**、**[!UICONTROL 建立目的地]**、**[!UICONTROL 對應欄位]**&#x200B;以及&#x200B;**[!UICONTROL 檢閱]**。

### 驗證 {#authenticate}

**[!UICONTROL 驗證]**&#x200B;步驟會在Real-Time CDP Collaboration和您的目的地帳戶之間建立連線。

如果現有帳戶可用，請從帳戶選擇器中選取它。 若要建立帳戶，請選取&#x200B;**[!UICONTROL 新增帳戶]**。

選取驗證方法並提供所需的帳戶資訊。 可用的驗證方法和欄位取決於選取的目的地提供者。 如需聯結器特定需求，請參閱[雲端儲存空間目的地需求](./cloud-storage-destination-requirements.md)。

選取&#x200B;**[!UICONTROL 連線至Amazon S3]**。 對於其他目的地提供者，按鈕會顯示對應的提供者名稱。

成功驗證帳戶後，選取&#x200B;**[!UICONTROL 下一步]**。

![驗證步驟顯示帳戶選取和新帳戶建立。](/help/assets/destinations/manage-destinations/authenticate-destination-account.png)

### 建立目標 {#create-destination}

**[!UICONTROL 建立目的地]**&#x200B;步驟定義傳遞對象匯出檔案的位置和方式。

輸入目的地名稱，並完成必要的儲存和匯出設定。 可用的欄位視選取的目的地提供者而定。 如需定義和聯結器特定需求，請參閱從[雲端儲存空間目的地需求](./cloud-storage-destination-requirements.md)連結的目的地檔案。

完成所有必要欄位後，選取&#x200B;**[!UICONTROL 下一步]**。 引導式設定會前進到欄位對應步驟。

![顯示目的地設定欄位的「建立目的地」步驟。](/help/assets/destinations/manage-destinations/configure-new-destination.png)

### 對應欄位 {#map-fields}

**[!UICONTROL 對應欄位]**&#x200B;步驟定義如何將對象比對索引鍵對應到目的地預期的身分欄位。

與標準Real-Time CDP目的地工作流程不同，Real-Time CDP Collaboration會在建立目的地時設定這些對應。 對象比對索引鍵會顯示為來源欄位。 將每個來源欄位對應到對應的目標身分識別，讓目的地可以識別匯出的識別碼，並將其與預期的使用者建立關聯。

選取&#x200B;**[!UICONTROL 新增欄位]**&#x200B;以新增其他比對索引鍵對應，或選取刪除圖示以移除對應。 檢閱及設定所有必要的對應。

完成對應後，選取&#x200B;**[!UICONTROL 下一步]**。 引導式設定會前進到稽核步驟。

![顯示啟動比對金鑰對應設定的[對應]欄位步驟。](/help/assets/destinations/manage-destinations/map-destination-fields.png)

### 檢閱 {#review-destination}

**[!UICONTROL 檢閱]**&#x200B;步驟在建立目的地組態之前會摘要列出該目的地組態。

檢閱目的地設定。 若要進行變更，請選取鉛筆圖示![鉛筆圖示。](../../assets/icons/edit.png) 以取得適用的區段並更新設定。

設定正確時，選取&#x200B;**[!UICONTROL 完成]**。 目的地隨即建立，並可供對象啟用。

![檢閱步驟在完成前顯示目的地組態摘要。](/help/assets/destinations/manage-destinations/review-destination-configuration.png)

## 檢視已設定的目的地 {#view-configured-destinations}

設定目的地後，該目的地會顯示在目的地詳細目錄中。 您可以從詳細目錄檢閱其狀態和啟用它的對象。

導覽至&#x200B;**[!UICONTROL 啟用]** > **[!UICONTROL 目的地]**。 **[!UICONTROL 目的地]**&#x200B;索引標籤會顯示已設定目的地的表格。

![顯示已設定目的地的[目的地]索引標籤。](/help/assets/destinations/manage-destinations/configured-destinations-list.png)

## 刪除目的地 {#delete-destination}

在對象啟動不再需要目的地時將其刪除。 刪除目的地會將其從目的地詳細目錄中移除，並防止對象日後對其啟用。

>[!IMPORTANT]
>
>刪除目的地不會移除先前匯出至該目的地的對象資料。 直接從目的地資料存放區移除先前匯出的資料。

導覽至&#x200B;**[!UICONTROL 啟用]** > **[!UICONTROL 目的地]**。

找到您要移除的目的地，選取&#x200B;**[!UICONTROL 動作]**&#x200B;資料行中的省略符號圖示，然後選取&#x200B;**[!UICONTROL 刪除]**。

![啟用工作區的[目的地]索引標籤，以省略符號圖示和[刪除]動作反白顯示。](/help/assets/destinations/manage-destinations/delete-configured-destination.png)

確認對話方塊隨即顯示。 檢閱將移除的目的地，然後選取&#x200B;**[!UICONTROL 刪除]**&#x200B;進行確認。

目的地會從目的地詳細目錄中移除，且無法再用於對象啟用。

## 後續步驟 {#next-steps}

設定目的地之後，您就可以開始[啟用專案中的對象](../collaborate/activate.md)。
