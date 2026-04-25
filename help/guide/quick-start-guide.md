---
title: Real-Time CDP Collaboration Quick Start & Setup Guide
description: 了解如何設定 Real-Time CDP Collaboration、設定角色和帳戶、獲取客群來源、啟用資料，以及安全地與合作夥伴連線。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
TQID: https://experienceleague.adobe.com/rhIArZZm0Thkj3E-qiHtVHO6qxpr1vd-Qs4hWt4tf1U
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1417
ht-degree: 3%

---

# Real-Time CDP Collaboration quick start guide

{{limited-availability-release-note}}

Get started with Real-Time CDP Collaboration by configuring your organization, sourcing audiences, and enabling privacy-focused activation and measurement.

## 先決條件

Before you begin, ensure you have the following:

- An active Real-Time CDP Collaboration license.
- [System or product administrator access to Adobe Experience Platform](./permissions/overview.md).
- [Access provisioned for end users](./permissions/manage-user-access.md).
- [Roles created for your organization and assigned to users](./permissions/manage-roles.md).
- Access to branding assets, such as your organization&#39;s name, logo, and banner.
- A [defined match key strategy](./setup/onboard-account.md#set-up-match-keys)
- (Optional) Access to a supported cloud source (Amazon S3, Google Cloud Storage, or Snowflake) if you&#39;re not using Experience Platform for audience management.

## Step 1: Complete role-based setup {#complete-role-based-setup}

Your organization&#39;s access roles determine what users can see and do in Collaboration. Before proceeding, make sure role-based permissions are set up correctly to ensure appropriate access and visibility in the platform.

**Resources:**

- [User Access Documentation](./permissions/manage-user-access.md)
- [Role Setup Documentation](./permissions/manage-roles.md)


Watch this video to learn how to assign product access and permissions for Collaboration using the Admin Console and Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## Step 2: Set up your Collaboration account {#set-up-your-account}

Before you can source audiences, you must configure your account in Collaboration. This governs how you appear and what you have access to in the interface.

If you don&#39;t have the necessary access, please refer back to step 1 or contact your organization&#39;s administrator for help completing this setup.

Define your account&#39;s role in Collaboration, provide branding assets, and configure match keys to align audiences across connections.

>[!NOTE]
>
>You can create one or more accounts (such as advertiser and a publisher) during setup. Certain fields, like branding assets and contact email, can be updated later in the **[!UICONTROL Settings]** workspace.

- **指派角色** — 判斷您的帳戶是廣告商還是發行者。 您的角色會定義您在Collaboration中擁有哪些功能。 若要進一步瞭解角色對共同作業工作流程的影響，請參閱[角色](./overview/roles.md)指南。
- **品牌推廣資產** — 新增下列專案至您的帳戶：
   - 帳戶名稱（最多100個字元）
   - 說明（最多1,000個字元）
   - 標誌（SVG &lt;20KB，理想為正方形）

>[!NOTE]
>
>如果您正在建立發佈者帳戶，並希望在Collaboration的連線目錄中公開顯示，請聯絡您的Adobe帳戶代表。 發佈者帳戶需要自訂品牌橫幅(JPG 2688x1536)；此檔案可直接與您的代表共用。

- **連絡人電子郵件** — 提供商務電子郵件，供共同作業人員在建立連線後使用。
- **設定比對索引鍵** — 選取用於對象比對的識別碼。

若要進一步瞭解初始帳戶設定，包括如何定義角色、上傳品牌化資產，以及設定比對金鑰，請參閱[初始帳戶設定](./setup/onboard-account.md#initial-account-setup){target="_blank"}指南。

觀看此影片以逐步瞭解廣告商設定，包括帳戶建立、品牌推廣和比對關鍵設定。

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## 步驟3： Source對象（來自Experience Platform或雲端來源） {#source-audiences}

建立帳戶並設定品牌和相符金鑰後，您就可以開始尋找受眾了。 根據您的資料存放區和業務需求，選擇下列其中一種來源方法。

### 選項A：來自Experience Platform的Source

[使用Collaboration連結包含對象的沙箱](./setup/onboard-audiences.md)。 使用此自助方法，從您的Experience Platform例項中參考現有的受眾區段。

#### 設定對象

設定如何準備、比對和控管受眾，以用於連線。

- **選取對象** *（僅限Experience Platform）* — 選擇具有支援識別碼的對象區段。
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
>雜湊比對金鑰必須為&#x200B;**SHA256-hashed**。\
>如果您提供使用大寫字元的雜湊值，Collaboration會自動將其轉換為小寫。\
>如果您的來源包含&#x200B;**純文字識別碼**，請使用&#x200B;**[!UICONTROL 套用轉換]**&#x200B;選項來套用雜湊處理。 此選項僅適用於從Experience Platform取得受眾，雲端型來源不支援時。
>
>如需詳細資訊，請參閱來源和管理對象指南的[對應欄位](./setup/onboard-audiences.md#map-fields)區段。

若要檢視如何使用Collaboration取得對象的完整逐步解說，請觀看以下影片。

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

或者，您也可以參閱Collaboration[&#128279;](./setup/onboard-audiences.md#source-and-manage-audiences)中sourcing audiences的檔案。

### 選項B：來自Snowflake、Amazon S3或Google雲端儲存空間的Source

若要設定雲端來源（例如[!DNL Snowflake]、[!DNL Amazon S3]或[!DNL Google Cloud Storage]），請使用[對象規格PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)準備您的對象資料

您可以將[!DNL Amazon S3]、[!DNL Google Cloud Storage]或[!DNL Snowflake]設定為自助資料來源。 如需設定指示，請參閱[Amazon S3來源指南](./setup/configure-aws-s3-audience-sourcing.md)、[GCS來源指南](./setup/configure-gcs-audience-sourcing.md)或[Snowflake來源指南](./setup/configure-snowflake-audience-sourcing.md)。

如需其他雲端服務提供者，請聯絡您的Adobe客戶代表以完成設定。

>[!IMPORTANT]
>
>雲端型對象檔案必須符合對象規格PDF中概述的必要結構。 檔案必須包含雜湊識別碼（小寫SHA256）、`segment_name`和`activation_id`等必要中繼資料欄位，並使用支援的格式，例如CSV或Parquet。 Adobe不會在啟用前標準化資料。 TTL會根據對象的生命週期強制執行。
>
>在此階段，上傳檔案中的所有對象都已完整來源。 The [audience visibility setting](/help/guide/setup/onboard-audiences.md#metadata-visibility) determines whether your collaborators can view your audience and is managed through the Collaboration UI.

## Step 4: Activate audiences (to Experience Platform or a cloud destination) {#activate-audiences}

Next, activate audiences to either your Experience Platform instance or a cloud destination.

### Option A: Activate to Experience Platform

Complete the following steps outlined in the [configure Adobe Experience Platform as a destination](/help/guide/destinations/experience-platform.md) guide.

- **Create a destination** – Use the UI to set up an Experience Platform destination (sandbox-level).
- **Map match keys** – Select the identifier (e.g., `hashedEmail`).
- **Define TTL** – Set expiration (1–30 days).
- **Verify in Audience Portal** – Once a collaborator sends you an audience, verify that it appears in the Audience Portal under the origin &quot;[!UICONTROL Real-Time CDP Collaboration].&quot;

### Option B: Activate to cloud

To configure a cloud destination (for example, [!DNL AWS S3] or [!DNL Snowflake]), contact your Adobe account representative to initiate the setup process. Depending on the cloud destination, you will need to provide cloud destination details such as file path, credentials, account locators etc. Once required information is provided, Adobe will configure the cloud destination setup.

Audience data sent to a cloud destination follows a predefined schema. For a detailed description of the required fields and format, download the [Collaboration Audience Activation Guide](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

## Step 5: Set up measurement (optional) {#set-up-measurement}

>[!IMPORTANT]
>
>The **[!UICONTROL Measure]** workspace is only available if the **[!UICONTROL Measurement]** use case was enabled [during the connection process](./connect/establishing-connections.md#connection-settings). 如需使用案例的詳細資訊，請參閱[管理專案](./collaborate/manage-projects.md#project-use-cases)指南。

Collaboration offers a variety of reports to analyze campaign reach, frequency, and effectiveness. While the **[!UICONTROL Measure]** workspace is available in the UI, full reporting functionality may require backend enablement.

To learn how to view and interpret measurement reports, see the [Measurement guide](./collaborate/measure.md). It covers attribution, campaign summary metrics, and dashboards such as reach curves and frequency distribution.

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

## Step 6: Connect with collaborators {#connect-with-collaborators}

With setup complete, your organization is now ready to connect with collaborators by sending or accepting invitations and submitting project settings for approval. This connection process involves sending or receiving invitations, reviewing and submitting connection settings (such as use cases and credit consumption), and confirming the connection.

As an advertiser, use the **[!UICONTROL Connect]** workspace from the left navigation menu to browse available publishers. 或者，共同作業人員可透過[私人連線邀請](./connect/establishing-connections.md#private-connection-invite){target="_blank"}直接相互連線。

>[!NOTE]
>
>目前，只有廣告商可以瀏覽發佈者。 發佈者無法瀏覽或啟動與廣告商的連線。

如需此流程的概觀，請參閱[建立連線指南](./connect/establishing-connections.md){target="_blank"}。 如需連線程式的視覺化逐步解說，包括瀏覽共同作業人員和管理連線設定，請觀看[廣告商帳戶設定影片](https://experienceleague.adobe.com/zh-hant/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}。

## 後續步驟

您現在已經完成初始設定，並將您的組織設定為安全共同作業。 接下來，探索下列資源，以加深您對啟動、測量和資料控管的瞭解：

- [Audience Activation工作流程檔案](./collaborate/activate.md)
- [測量使用案例](./collaborate/measure.md)
- [Collaboration治理最佳實務](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
