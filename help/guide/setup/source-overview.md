---
title: 來源概觀
description: 瞭解Adobe Real-Time CDP Collaboration中的來源聯結器
audience: admin, publisher, advertiser
source-git-commit: 23f7d91d37d0d9c9b352716caa4827dcc87093d8
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 10%

---

# 來源概觀

在Adobe Real-Time CDP Collaboration中，來源（或資料連線）是您對象資料的來源。 您可以從您的本機系統連線到各種來源型別，例如Adobe應用程式、雲端儲存空間或檔案，以便[為您的Collaboration專案提供來源並管理對象](./onboard-audiences.md)。 在對象來源工作流程中，您可以根據組織的需求選擇及設定偏好的來源。

## 連接來源 {#connect-a-source}

若要連線來源，您必須輸入sourcing工作流程。 首先，導覽至&#x200B;**[!UICONTROL 設定]**&#x200B;工作區中的&#x200B;**[!UICONTROL 我的對象]**&#x200B;索引標籤。

選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)） 然後選取&#x200B;**[!UICONTROL 對象]**&#x200B;以開始來源工作流程。

![我的受眾工作區，其中的[新增]選項和[受眾]選項已反白顯示。](/help/assets/setup/add-manage-audiences/add-audiences.png)

在工作流程期間，系統將提示您選取來源以新增資料連線。 您選擇的來源會決定如何將對象資料帶入Collaboration。 如需所有支援來源的清單，請參閱[可用的來源](#available-sources)表格。

![反白顯示[新增資料連線]選項的[新增對象]工作區。](/help/assets/setup/add-manage-audiences/add-data-connection.png)

選取來源後，工作流程會引導您完成連線特定的設定步驟，包括驗證、欄位對應、排程和對象選擇。

### 可用來源 {#available-sources}

Collaboration中有以下來源。 若要檢視該來源的sourcing逐步指南，請選取下表中的來源名稱。 如果您對目前無法取得的來源感興趣，請聯絡您的Adobe代表。

| 來源 | 說明 | 可用性 |
| --- | --- | --- |
| [Adobe Experience Platform](./onboard-audiences.md) | 從連線的Experience Platform例項引進對象，並重複使用現有的客戶區段。 | 可用 |
| [Amazon S3](./configure-aws-s3-audience-sourcing.md) | 連線您的S3儲存貯體，從您的雲端基礎結構取得大型第一方資料集。 | 可用 |
| [[!DNL Snowflake]](./configure-snowflake-audience-sourcing.md) | 連線您的[!DNL Snowflake Secure Data Share]以引入大規模受眾資料集。 | 可用 |
| [[!DNL Google Cloud Storage]](./configure-gcs-audience-sourcing.md) | 連線您的GCS貯體，以匯入儲存在您的[!DNL Google Cloud]環境中的對象資料。 | 可用 |
| [CSV檔案上傳](./upload-csv-audience-sourcing.md) | 直接從您的本機系統上傳格式化的CSV檔案。 | 可用 |
| [Adobe Audience Manager](./configure-aam-audience-sourcing.md) | 將現有的Audience Manager區段帶入您的Collaboration專案。 | 可用 |
| [[!DNL Databricks Delta Share]](./configure-databricks-audience-sourcing.md) | 連線您的[!DNL Databricks Delta Share]，以從您的[!DNL Databricks]環境引入大型受眾資料集。 | 可用 |
| [[!DNL Azure Blob Storage]](./configure-azure-storage-audience-sourcing.md) | 將您的[!DNL Azure Blob Storage]容器連線至您[!DNL Microsoft Azure]環境中的來源第一方資料集。 | 可用 |
| [[!DNL Azure Data Lake Storage]](./configure-azure-storage-audience-sourcing.md) | 連線您的[!DNL Azure Data Lake Storage Gen 2]帳戶，以匯入儲存在[!DNL Azure]資料湖中的對象資料。 | 可用 |

{style="table-layout:auto"}

## 後續步驟

連線來源並引進受眾後，您可以檢視詳細資料、更新設定或刪除現有來源。 如需詳細資訊，請參閱[管理資料連線](./manage-data-connection.md)指南。
