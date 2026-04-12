---
title: 身分識別交叉對照表
description: 瞭解Real-Time CDP Collaboration中身分交叉通路的所有資訊，包括如何從不同來源引進身分交叉通路，以及如何管理身分交叉通路
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: 61545ee26359d06191a55d0d96103dc41852cc3a
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 24%

---

# 身分識別交叉對照表

{{limited-availability-release-note}}

瞭解Real-Time CDP Collaboration中身分交叉通路的所有資訊，包括如何從不同來源引進身分交叉通路，以及如何管理身分交叉通路。

身分交叉通路可促進跨多個資料集和平台的安全且符合隱私權要求的客戶身分連結。 透過使用雜湊識別碼，Real-Time CDP Collaboration可確保使用者同步並調解身分，而不需揭露個人識別資訊(PII)。 這可讓客戶獲得統一的檢視，以便進行更好的共同作業和目標式行銷工作。

首先，您必須將身分橫幅匯入至Real-Time CDP Collaboration。 若要將身分交叉通路匯入Real-Time CDP Collaboration，請閱讀以下章節：

>[!NOTE]
>
>在Real-Time CDP Collaboration的Beta版中，您可以從Real-Time CDP中的資料集匯入身分交叉通道。 後續版本將提供其他選項。

## 將身分交叉通路匯入Real-Time CDP Collaboration {#import-crosswalk}

導覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 身分識別交叉管道]**&#x200B;標籤，選取新增圖示（![新增圖示。](/help/assets/icons/plus.png)），然後選取&#x200B;**[!UICONTROL 身分識別交叉管道]**

![錄製如何進入熒幕以新增身分交叉通道](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### 選取交叉對照表來源

選取要從中匯入身分交叉路徑的來源。 在Real-Time CDP Collaboration的第一個版本中，Experience Platform是匯入人行橫幅的唯一支援來源。

>[!TIP]
>
>您從Experience Platform匯入的交叉分析在Platform中稱為&#x200B;*資料集*。

選取Experience Platform作為行人穿越道的來源後，選取您要匯入身分識別行人穿越道的[Experience Platform沙箱](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/sandbox/home)。

![如何選取人行橫線來源的錄製](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### 選取交叉對照表

選取Experience Platform作為行人穿越道的來源後，

### 提供詳細資料

提供您要匯入產品中的身分交叉路線的名稱和描述。

### 選取聯結索引鍵 {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="聯結索引鍵"
>abstract="聯結索引鍵用於比對和連結不同資料集間之記錄的唯一識別碼。 可確保來自各種來源的資料能夠準確地與同一個體或實體相關聯。 所選取之交叉對照表中任何欄標題都可以做為聯結索引鍵。"

聯結索引鍵用於比對和連結不同資料集間之記錄的唯一識別碼。 可確保來自各種來源的資料能夠準確地與同一個體或實體相關聯。 藉由選取適當的聯結索引鍵，您可以有效地合併與調解資料，進而提高行銷活動的正確性與完整性。

所選取之交叉對照表中任何欄標題都可以做為聯結索引鍵。

選取交叉分析表所需的聯結索引鍵，並選取&#x200B;**[!UICONTROL 下一步]**&#x200B;以繼續執行下一個步驟。

### 檢閱

檢閱先前畫面中的任何選取專案。 對您的選擇感到滿意時，選取&#x200B;**[!UICONTROL 下一步]**&#x200B;以完成工作流程。

## 後續步驟

瞭解如何將身分交叉管道匯入Real-Time CDP後，您就可以檢視目前新增至Real-Time CDP Collaboration的所有身分交叉管道。 您現在也可以使用將受眾匯入Real-Time CDP Collaboration時匯入的身分交叉通道。
