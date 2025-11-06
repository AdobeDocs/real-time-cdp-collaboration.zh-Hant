---
title: 設定Audience Sourcing的AWS許可權
description: 瞭解如何設定AWS Identity and Access Management (IAM)許可權，以授予Adobe對您的 [!DNL Amazon S3] 貯體的安全、唯讀存取權，用於Real-Time CDP Collaboration中的受眾來源。
source-git-commit: 4f223890dabb4897c9e9264655ff9217e323dc91
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 設定對象來源的AWS許可權

使用本指南來設定AWS Identity and Access Management (IAM)原則與角色，授予Adobe對Amazon S3儲存貯體的安全、唯讀存取權。 此存取權可讓Real-Time CDP Collaboration從S3貯體取得受眾。

## 先決條件 {#prerequisites}

在繼續之前，請確認您符合下列需求並有權存取必要資訊。

### 必要的AWS許可權

若要完成此設定，您的帳戶必須擁有AWS管理員存取權。 管理員存取權可確保您可建立並管理授權Adobe存取您的S3儲存貯體所需的IAM原則和角色。 如果您沒有管理員許可權，請在繼續之前聯絡您的AWS管理員。

### 必要資訊

進行下列步驟時，請注意下列資訊。 這些詳細資料用於[[!DNL Amazon S3] 對象來源UI指南](./configure-aws-s3-audience-sourcing.md)。

* 儲存對象檔案的S3 Bucket名稱。
* 您的對象檔案所在的資料夾路徑（首碼）。
* 您新建立之IAM角色的Amazon資源名稱(ARN)，例如： `arn:aws:s3:::my-company-data/audience-files/`

>[!TIP]
>
>Amazon資源名稱(ARN)可唯一識別AWS資源，例如S3貯體和IAM角色。 請使用下列格式來指定儲存貯體和選用資料夾路徑：
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## 建立IAM原則 {#create-policy}

若要開始設定，請先建立授予S3儲存貯體&#x200B;**唯讀存取權**&#x200B;的IAM原則。 此原則可讓Adobe讀取對象來源所需的檔案，但不會授與寫入或刪除許可權。

開啟[AWS管理主控台](https://aws.amazon.com/console/)，並導覽至&#x200B;**[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**。

在AWS建立原則工作區中，選取&#x200B;**JSON**&#x200B;索引標籤並貼上以下原則範例。

>[!NOTE]
>
>以您特定的S3 ARN取代`<Your AWS ARN for bucket folder path>`和`<Your AWS ARN for bucket>`。 指定儲存貯體資料夾路徑時，在ARN結尾包含`/*` （例如，`arn:aws:s3:::my-company-data/audience-files/*`）。 這可確保Adobe可存取指定資料夾路徑中的所有檔案和子資料夾。

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

檢閱原則設定並選取&#x200B;**[!DNL Create policy]**。 記錄原則名稱，以供稍後步驟使用。

>[!TIP]
>
>若要尋找您的儲存貯體名稱和資料夾路徑，請開啟&#x200B;**Amazon S3管理主控台**。 在&#x200B;**貯體**&#x200B;頁面上，選取您的貯體名稱以開啟。 **物件**&#x200B;檢視會列出您的檔案和資料夾，頁面頂端的路徑會顯示您目前的資料夾路徑。

## 建立IAM角色 {#create-role}

接下來，建立IAM角色，並將Real-Time CDP Collaboration AWS IAM角色設定為&#x200B;**信任的實體**。 這可讓Adobe的服務擔任此角色，並安全地讀取您的S3受眾資料。

在Amazon S3管理主控台的&#x200B;**[!DNL IAM]**&#x200B;標籤中，導覽至&#x200B;**[!DNL Roles]** > **[!DNL Create role]**。

在[!DNL Step 1]工作流程的[!DNL Create role]下，在&#x200B;**[!DNL Trusted entity type]**&#x200B;區段中，選取&#x200B;**[!DNL Custom trust policy]**。 然後，在&#x200B;**[!DNL Custom trust policy]**&#x200B;編輯器中，貼上以下範例並以您所在地區的值取代`<Adobe IAM Role ARN>`。

* 適合您地區的Adobe IAM角色ARN：

| 區域 | Adobe IAM角色ARN |
|---------|-------------------|
| 北美 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| 澳洲 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |

信任原則範例：

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

檢閱原則並選取&#x200B;**下一步**&#x200B;以繼續。

在[!DNL Step 2]工作流程的&#x200B;**[!DNL Add permissions]** [!DNL Create role]區段中，搜尋並附加您先前建立的[IAM原則](#create-policy)。 選取原則，接著選取&#x200B;**[!DNL Next]**&#x200B;以繼續進行[!DNL Step 3]。

在[!DNL Step 3] **[!DNL Name review, and create - Role details]**&#x200B;區段中，提供角色名稱（例如，`s3-iam-role`）和選用的說明。

此頁面會顯示信任的實體原則、許可權原則摘要，以及您可能為內部組織和追蹤而新增的任何標籤。

最後，選取&#x200B;**建立角色**&#x200B;以確認設定。

>[!IMPORTANT]
>
>在建立角色後，您必須記錄Amazon資源名稱(ARN)。 在&#x200B;**設定AWS S3以取得對象來源**&#x200B;工作流程的[驗證您的S3連線](./configure-aws-s3-audience-sourcing.md)步驟中，您將需要提供IAM角色ARN。

## 後續步驟 {#next-steps}

此設定會授予Adobe對您的S3儲存貯體的唯讀存取權，並與Adobe的IAM角色建立受信任的連線。

接下來，請繼續進行[設定AWS S3以取得對象來源](./configure-aws-s3-audience-sourcing.md)，將您的S3貯體連線至Collaboration。

如需來源受眾的詳細資訊，請參閱[Source及管理受眾](./onboard-audiences.md)。
