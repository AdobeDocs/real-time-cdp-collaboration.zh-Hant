---
title: 端對端工作流程
description: 根據您的共同作業模式，瞭解使用Real-Time CDP Collaboration的端對端工作流程。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 5c08738cdc8e1e208203ee1f9a1cf1891b5b07cb
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# 端對端工作流程

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，端對端工作流程會依您選擇的共同作業模式而有所不同。 工作流程概述設定及執行共同作業專案的相關步驟，從建立帳戶和來源受眾，到建立連線和專案。 瞭解此工作流程是有效運用平台功能達成行銷目標的關鍵。

## 快速入門

開始之前，請確定您已確實瞭解以下重要概念：

- **Collaboration模式**：這些模式定義共同作業人員如何共同作業。 有兩種不同的模式： [廣告商對發佈者](./collaboration-patterns.md#advertiser-to-publisher)和[品牌對品牌](./collaboration-patterns.md#brand-to-brand)。
- **帳戶角色**：帳戶角色決定您在平台中的權能。 藍圖應與您組織的目標、品牌和目標一致。 有兩種帳戶角色： [廣告商](./roles.md#advertiser)和[發佈者](./roles.md#publisher)。
- **使用案例**：使用案例會定義您如何善用Collaboration達成行銷目標。 有三個共同作業使用案例： [探索](./use-cases.md#discover)、[啟動](./use-cases.md#activate)以及[測量](./use-cases.md#measure)。

本指南將使用三位模擬共同作業人員來說明端對端工作流程：

- **[!UICONTROL Luma]**：運動服裝品牌。 他們是廣告商，想要透過鎖定目標的行銷活動觸及特定對象。
- **[!UICONTROL 電視管]**：數位串流提供者。 它們是提供受眾資料以供廣告商使用的發佈者。
- **[!UICONTROL 適合服飾]**：另一個運動服飾品牌。 他們為想要共同作業以分享對象資料和深入分析的第二位廣告商，藉此提升行銷成效。

## 廣告商對發佈商的工作流程 {#advertiser-to-publisher-workflow}

[!UICONTROL Luma] （一家體育零售公司）想要與數位串流供應商[!UICONTROL TV Tube]建立連線，以透過鎖定目標的行銷活動觸及特定對象。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)，而[!UICONTROL TV Tube]則以發佈者角色建立帳戶。

建立帳戶之後，[!UICONTROL Luma]和[!UICONTROL TV Tube]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 只有[!UICONTROL TV Tube]會啟用行銷活動的對象，因此他們需要[設定目的地](../setup/manage-destinations.md)。

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../connect/discover-collaborators.md)功能尋找[!UICONTROL 電視管]並起始連線要求。 在[!UICONTROL TV Tube]接受連線要求後，[!UICONTROL Luma]會設定連線設定以定義共同作業的方式。 [!UICONTROL TV Tube]接受連線要求，以建立兩個品牌之間的安全連結。

建立連線之後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)，以開始他們與[!UICONTROL TV Tube]的協同合作。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)使用案例來深入分析[!UICONTROL TV Tube]的對象資料。 在[!UICONTROL Luma]識別目標對象區段後，他們[啟動](../collaborate/activate.md)這些對象。

啟用對象後，[!UICONTROL TV Tube]會執行目標式行銷活動，並將資料上傳至[測量](../collaborate/measure.md)結果，以評估其行銷活動的成效。

## 品牌對品牌的工作流程 {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel]，運動服裝品牌，想要與另一個運動服裝品牌[!UICONTROL Luma]合作，以分享受眾資料與深入分析，提升行銷成效。

建立帳戶之後，[!UICONTROL Fit Apparel]和[!UICONTROL Luma]都需要[建立資料連線和來源對象](../setup/onboard-audiences.md)。 [!UICONTROL 適合的服飾]和[!UICONTROL Luma]都會啟用行銷活動的對象，因此兩者都需要[設定目的地](../setup/manage-destinations.md)。

在取得其對象後，[!UICONTROL Fit Apparel]和[!UICONTROL Luma] [在平台內建立連線](../connect/establishing-connections.md)，以安全地共用對象資料。 若要這麼做，他們必須使用[私人連線邀請](../connect/establishing-connections.md#private-connection-invite)功能。 [!UICONTROL Luma]與[!UICONTROL Fit服飾]共用其連線代碼，後者會使用它來起始連線要求。 在[!UICONTROL Luma]接受連線要求後，[!UICONTROL Fit Apparel]會設定連線設定以定義他們將如何共同作業。 在設定中，[!UICONTROL Fit Apparel]指定兩個共同作業人員都可以啟用行銷活動的對象。 為了完成連線，[!UICONTROL Luma]接受在兩個品牌之間建立安全連結的要求。

建立連線之後，[!UICONTROL Fit Apparel] [會建立專案](../collaborate/manage-projects.md)，以開始他們與[!UICONTROL Luma]的協同合作。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Fit Apparel]和[!UICONTROL Luma]都可以使用[Discover](../collaborate/discover.md)使用案例來深入瞭解彼此的對象資料。 一旦他們識別出有價值的受眾區段，就會[啟用](../collaborate/activate.md)他們為行銷活動選擇的受眾。

最後，在執行其行銷活動後，兩個品牌都會上傳資料至[測量](../collaborate/measure.md)結果，並評估其共同作業的成效。

## 廣告商對廣告平台工作流程 {#advertiser-to-advertising-platform-workflow}

[!UICONTROL Luma]，一家運動零售公司，想要與[!DNL Amazon Marketing Cloud] ([!DNL AMC])連線，以利用[!DNL AMC]的身分解析度和目標定位工具來增強其行銷能力。 Luma已有使用中的[!DNL Amazon Advertising]帳戶，且已核准使用[!DNL AMC]。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)。 建立帳戶之後，[!UICONTROL Luma]必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 由於[!UICONTROL Luma]會針對行銷活動啟用對象，因此他們需要[設定目的地](../setup/manage-destinations.md)。

在[!UICONTROL Luma]設定好帳戶後，他們便已準備好在平台內[與](../connect/establishing-connections.md)建立連線[!DNL AMC]。 [!UICONTROL Luma]使用[探索共同作業人員](../connect/discover-collaborators.md)功能尋找[!UICONTROL Amazon Marketing Cloud]並[起始連線要求](../connect/advertising-platforms/amc.md)。 透過[!DNL Amazon]登入頁面驗證並授權連線後，已建立與[!DNL AMC]的連線。

建立連線之後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)以開始他們與[!DNL AMC]的協同合作。 連線設定（包括使用案例）會根據廣告平台進行預先設定。 針對[!DNL AMC]，可用的使用案例是[探索](../collaborate/advertising-platforms/amc.md#discover)。

[!UICONTROL Luma]利用[Discover](../collaborate/advertising-platforms/amc.md#discover)使用案例從[!DNL AMC]取得深入分析和對象資料。 使用這些深入分析，[!UICONTROL Luma]可以最佳化行銷策略，並提高行銷活動的成效。
