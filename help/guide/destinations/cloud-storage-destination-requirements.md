---
title: 目的地連線需求
description: 檢閱在Real-Time CDP Collaboration中設定支援的目的地所需的連線資訊。
audience: admin, publisher
source-git-commit: c84582bb81289ce761c664af7db177535ff00a00
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# 目的地連線需求

在Real-Time CDP Collaboration中設定目的地之前，請先取得目的地提供者所需的憑證和連線資訊。

此頁面概述Collaboration中可用的驗證方法。 如需建立認證、指派許可權、設定網路存取權或準備目的地系統的指示，請參閱連結的Adobe Experience Platform目的地檔案。

>[!NOTE]
>
>連結的Adobe Experience Platform檔案說明標準目的地工作流程。 在Real-Time CDP Collaboration中設定目的地時，部分步驟、欄位或選項可能不適用。

## 需求一覽 {#requirements-at-a-glance}

| 目標 | 驗證或連線方法 | 開始前準備 | 詳細需求 |
|---|---|---|---|
| [!DNL Amazon S3] | 存取金鑰和秘密金鑰，或假定的角色 | AWS存取金鑰組或IAM角色ARN；貯體和資料夾資訊 | [[!DNL Amazon S3] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3) |
| SFTP | 密碼或SSH金鑰 | 伺服器網域、連線埠、使用者名稱、驗證認證和資料夾路徑 | [SFTP目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp) |
| [!DNL Azure Blob Storage] | 連接字串 | Azure儲存體連線字串、容器和資料夾資訊 | [[!DNL Azure Blob Storage] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob) |
| [!DNL Google Cloud Storage] | 存取金鑰ID和機密存取金鑰 | [!DNL Google Cloud Storage]互通性認證、貯體和資料夾資訊 | [[!DNL Google Cloud Storage] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage) |
| [!DNL Snowflake Batch] | [!DNL Snowflake]資料共用 | [!DNL Snowflake]帳戶識別碼、地區、私人連結狀態以及存取私人清單 | [[!DNL Snowflake Batch] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch) |
| [!DNL Data Landing Zone] | 不需要個別驗證 | 目的地資料夾路徑和檔案輸出偏好設定 | [[!DNL Data Landing Zone] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone) |

## 聯結器附註 {#connector-notes}

在設定目的地之前，請先檢閱下列聯結器專用驗證方法和工作流程差異。

### [!DNL Amazon S3] {#amazon-s3}

Collaboration支援&#x200B;**[!UICONTROL 存取金鑰]**&#x200B;和&#x200B;**[!UICONTROL 假定的角色]**&#x200B;驗證。 存取金鑰驗證需要存取金鑰和機密存取金鑰。 假定的角色驗證需要AWS IAM角色的ARN，Adobe可假定。

如需認證、角色和許可權設定，請參閱[驗證 [!DNL Amazon S3] 目的地](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3#authenticate)。

### SFTP {#sftp}

Collaboration支援使用密碼的&#x200B;**[!UICONTROL SFTP]**&#x200B;和使用SSH金鑰&#x200B;**驗證的** SFTP。 這兩種方法都需要伺服器網域、連線埠和使用者名稱。 連線埠預設為`22`。

如需SSH金鑰格式、伺服器、網路和允許清單需求，請參閱[SFTP驗證資訊](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp#authentication-information)。

### [!DNL Azure Blob Storage] {#azure-blob-storage}

Collaboration會使用儲存帳戶連線字串來驗證[!DNL Azure Blob Storage]。

如需取得連線字串及指派儲存許可權的指示，請參閱[向 [!DNL Azure Blob Storage] 目的地](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob#authenticate)驗證。

### [!DNL Google Cloud Storage] {#google-cloud-storage}

Collaboration需要透過[!DNL Google Cloud Storage]互通性設定產生的[!DNL Google Cloud Storage]存取金鑰識別碼和機密存取金鑰。

如需產生認證和儲存貯體許可權的要求，請參閱[驗證 [!DNL Google Cloud Storage] 目的地](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage#authenticate)。

### [!DNL Snowflake Batch] {#snowflake-batch}

[!DNL Snowflake Batch]使用[!DNL Snowflake]資料共用，而非將檔案匯出至客戶管理的儲存空間。 在Collaboration中，沒有單獨的驗證步驟。 輸入目的地建立期間的Snowflake帳戶ID、地區、私人連結狀態和帳戶所有權確認。

如需帳戶準備和私密清單需求，請參閱[[!DNL Snowflake Batch] 目的地檔案](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch)。

### [!DNL Data Landing Zone] {#data-landing-zone}

[!DNL Data Landing Zone]由Adobe布建，不需要在Collaboration中另外執行驗證步驟。 在建立目的地期間，請指定目的地資料夾路徑和檔案輸出設定。

如需有關存取AWS布建的[!DNL Data Landing Zone]的資訊，請參閱[驗證AWS布建的資料登陸區域](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone#authenticate-dlz-aws)。

## 後續步驟 {#next-steps}

取得必要的連線資訊後，[設定並管理目的地](./manage-destinations.md)。
