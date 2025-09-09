---
title: Real-Time CDP Collaboration快速入門手冊
description: 瞭解如何在Real-Time CDP Collaboration中建立您的組織，包括設定角色和組織、對象來源、啟用和測量。 本指南協助共同作業人員設定連線設定，以開始安全有效地使用對象。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: 849bae30b4e617a6c49f68b2baedc0ab8a822854
workflow-type: tm+mt
source-wordcount: '1394'
ht-degree: 0%

---

# Real-Time CDP Collaboration快速入門手冊

{{limited-availability-release-note}}

透過設定您的組織、sourcing audiences及啟用以隱私權為中心的啟用和測量，開始使用Real-Time CDP Collaboration。

## 先決條件

開始之前，請確定您具備下列條件：

- 有效的Real-Time CDP Collaboration授權。
- [系統或產品管理員存取Adobe Experience Platform](./permissions/overview.md)。
- [已布建使用者存取權](./permissions/manage-user-access.md)。
- 為您的組織建立並指派給使用者的[角色](./permissions/manage-roles.md)。
- 存取品牌化資產，例如貴組織的名稱、標誌和橫幅。
- [定義的相符金鑰策略](./setup/onboard-account.md#set-up-match-keys)
- （選用）如果您未使用Experience Platform進行對象管理，請存取支援的雲端來源(Amazon S3或Snowflake)。

## 步驟1：完成角色型設定 {#complete-role-based-setup}

您組織的存取角色會決定使用者可以在Collaboration中檢視及執行的動作。 繼續進行之前，請確定已正確設定角色型許可權，以確保在平台中擁有適當的存取權和可見度。

**資源：**

- [使用者存取權檔案](./permissions/manage-user-access.md)
- [角色設定檔案](./permissions/manage-roles.md)


觀看此影片以瞭解如何使用Admin Console和Experience Platform為Collaboration指派產品存取權和許可權。

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## 步驟2：設定您的Collaboration帳戶 {#set-up-your-account}

您必須先在Collaboration中設定帳戶，才能取得受眾。 這會控制您顯示在介面中的方式以及您可在介面中存取的內容。

如果您沒有必要的存取權，請參考步驟1，或連絡您組織的管理員，以取得完成此設定的協助。

定義您的帳戶在Collaboration中的角色、提供品牌資產，並設定比對索引鍵以跨連線對齊對象。

>[!NOTE]
>
>您可以在設定期間建立一或多個帳戶（例如廣告商和發佈者）。 某些欄位（例如品牌推廣資產和連絡人電子郵件）稍後可在&#x200B;**[!UICONTROL 設定]**&#x200B;工作區中更新。

- **指派角色** — 判斷您的帳戶是廣告商還是發行者。 您的角色會定義您在Collaboration中擁有哪些功能。 若要進一步瞭解角色對共同作業工作流程的影響，請參閱[角色](./overview/roles.md)指南。
- **品牌推廣資產** — 新增下列專案至您的帳戶：
   - 帳戶名稱（最多100個字元）
   - 說明（最多1,000個字元）
   - 標誌(SVG &lt;20KB，理想為正方形)

>[!NOTE]
>
>如果您正在建立發佈者帳戶，並希望在Collaboration的連線目錄中公開顯示，請聯絡您的Adobe帳戶代表。 發佈者帳戶需要自訂品牌橫幅(JPG 2688x1536)；此檔案可直接與您的代表共用。

- **連絡人電子郵件** — 提供商務電子郵件，供共同作業人員在建立連線後使用。
- **設定比對索引鍵** — 選取用於對象比對的識別碼。

若要進一步瞭解初始帳戶設定，包括如何定義角色、上傳品牌化資產，以及設定比對金鑰，請參閱[初始帳戶設定](./setup/onboard-account.md#initial-account-setup){target="_blank"}指南。

觀看此影片以逐步瞭解廣告商設定，包括帳戶建立、品牌推廣和比對關鍵設定。

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## 步驟3： Source對象(來自Experience Platform或雲端來源) {#source-audiences}

建立帳戶並設定品牌和相符金鑰後，您就可以開始尋找受眾了。 根據您的資料存放區和業務需求，選擇下列其中一種來源方法。

### 選項A：來自Experience Platform的Source

[使用Collaboration連結包含對象的沙箱](./setup/onboard-audiences.md)。 使用此自助方法，從您的Experience Platform例項中參考現有的受眾區段。

#### 設定對象

設定如何準備、比對和控管受眾，以用於連線。

- **選取對象** *(僅限Experience Platform)* — 選擇具有支援識別碼的對象區段。
- **對應相符金鑰** — 將對象欄位與設定的相符金鑰對齊。
- **視需要套用轉換** — 雜湊純文字值（例如電子郵件）。
- **排程重新整理** — 定義更新頻率（例如，每日）。
- **設定同意設定** — 選取同意模式，以決定哪些設定檔符合加入連線的資格：選擇加入、選擇退出或無。

>[!NOTE]
>
>您可以直接在Collaboration中新增或移除對象，以及更新重新整理排程。 若要變更其他設定（例如比對索引鍵或同意模式），您必須刪除並重新建立資料連線。

>[!IMPORTANT]
>
>**每個共同作業人員角色的最大對象數：**
>
>- **廣告商**&#x200B;最多可以取得25個對象。
>- **發佈者**&#x200B;最多可以取得250個對象（每個對象至少有1,000個ID）。

>[!IMPORTANT]
>
>**符合索引鍵需求：**
>
>所有相符金鑰必須為&#x200B;**修剪**，**小寫**
>&#x200B;>雜湊比對金鑰必須為&#x200B;**SHA256-hashed**。\
>如果您提供使用大寫字元的雜湊值，Collaboration會自動將其轉換為小寫。\
>如果您的來源包含&#x200B;**純文字識別碼**，請使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;選項來套用雜湊處理。 此選項僅適用於從Experience Platform取得受眾，雲端型來源不支援時。
>
>如需詳細資訊，請參閱來源和管理對象指南的[對應欄位](./setup/onboard-audiences.md#map-fields)區段。

若要檢視如何使用Collaboration取得對象的完整逐步解說，請觀看以下影片。

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

或者，您也可以參閱Collaboration[中](./setup/onboard-audiences.md#source-and-manage-audiences)sourcing audiences的檔案。

### 選項B：來自Snowflake或Amazon S3的Source

若要設定雲端來源（例如[!DNL AWS S3]或[!DNL Snowflake]），請使用下列[對象規格PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf)準備您的對象資料。 完成後，或如有疑問，請聯絡您的Adobe客戶代表以完成設定。 此方法並非自助式，需要Adobe協助。

>[!IMPORTANT]
>
>雲端型對象檔案必須符合對象規格PDF中概述的必要結構。 檔案必須包含雜湊識別碼（小寫SHA256）、`segment_name`和`activation_id`等必要中繼資料欄位，並使用支援的格式，例如CSV或Parquet。 Adobe不會在啟用前標準化資料。 TTL會根據對象的生命週期強制執行。
>
>在此階段，上傳檔案中的所有對象都已完整來源。 [對象可見度設定](/help/guide/setup/onboard-audiences.md#metadata-visibility)會決定您的共同作業人員是否可以檢視您的對象，以及是否透過Collaboration UI進行管理。

## 步驟4：啟用對象(前往Experience Platform或雲端目的地) {#activate-audiences}

接下來，在您的Experience Platform執行個體或雲端目的地啟用對象。

### 選項A：啟動至Experience Platform

完成[將Adobe Experience Platform設定為目的地](/help/guide/destinations/experience-platform.md)指南中概述的下列步驟。

- **建立目的地** — 使用使用者介面設定Experience Platform目的地（沙箱層級）。
- **對應比對索引鍵** — 選取識別碼（例如，`hashedEmail`）。
- **定義TTL** — 設定到期日（1-30天）。
- **在對象入口網站中驗證** — 共同作業人員傳送對象給您後，請確定該對象出現在來源「[!UICONTROL Real-Time CDP Collaboration]」下的對象入口網站中。

### 選項B：啟用至雲端

若要設定雲端目的地（例如，[!DNL AWS S3]或[!DNL Snowflake]），請聯絡您的Adobe客戶代表以啟動設定程式。 根據雲端目的地，您需要提供雲端目的地詳細資訊，例如檔案路徑、憑證、帳戶位置等。 提供必要資訊後，Adobe將設定雲端目的地設定。

傳送至雲端目的地的對象資料會遵循預先定義的結構描述。 如需必要欄位和格式的詳細說明，請下載[Collaboration Audience Activation指南](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf)。

## 步驟5：設定測量（選擇性） {#set-up-measurement}

>[!AVAILABILITY]
>
>此功能目前處於&#x200B;**測試版**&#x200B;中，僅供有限可用性計畫的客戶使用。 請聯絡您的Adobe代表以要求存取權。

>[!IMPORTANT]
>
>**[!UICONTROL Measure]**&#x200B;工作區只有在連線程式&#x200B;**[!UICONTROL 期間已啟用]**&#x200B;的[Measurement](./connect/establishing-connections.md#connection-settings)使用案例時才可用。 如需使用案例的詳細資訊，請參閱[管理專案](./collaborate/manage-projects.md#project-use-cases)指南。

Collaboration提供多種報表，可分析行銷活動的觸及率、頻率和成效。 雖然&#x200B;**[!UICONTROL Measure]**&#x200B;工作區可在UI中使用，但完整的報告功能可能需要後端啟用。

若要瞭解如何檢視和解讀測量報告，請參閱[測量指南](./collaborate/measure.md)。 它涵蓋歸因、行銷活動摘要量度和控制面板，例如觸及曲線和頻率分佈。

<!-- 
Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."

### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. 
-->

## 步驟6：與共同作業人員交流 {#connect-with-collaborators}

設定完成後，您的組織現在已準備好透過傳送或接受邀請並提交專案設定以進行核准，與共同作業人員連線。 此連線程式包含傳送或接收邀請、檢閱及提交連線設定（例如使用案例和信用沖銷），以及確認連線。

作為廣告商，請使用左側導覽功能表中的&#x200B;**[!UICONTROL Connect]**&#x200B;工作區來瀏覽可用的發行者。 或者，共同作業人員可透過[私人連線邀請](./connect/establishing-connections.md#private-connection-invite){target="_blank"}直接相互連線。

>[!NOTE]
>
>目前，只有廣告商可以瀏覽發佈者。 發佈者無法瀏覽或啟動與廣告商的連線。

如需此流程的概觀，請參閱[建立連線指南](./connect/establishing-connections.md){target="_blank"}。 如需連線程式的視覺化逐步解說，包括瀏覽共同作業人員和管理連線設定，請觀看[廣告商帳戶設定影片](https://experienceleague.adobe.com/zh-hant/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}。

## 後續步驟

您現在已經完成初始設定，並將您的組織設定為安全共同作業。 接下來，探索下列資源，以加深您對啟動、測量和資料控管的瞭解：

- [Audience Activation工作流程檔案](./collaborate/activate.md)
- [測量使用案例](./collaborate/measure.md)
- [Collaboration治理最佳實務](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
