---
title: 端對端工作流程
description: 根據您的共同作業模式，瞭解使用Real-Time CDP Collaboration的端對端工作流程。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限可用性" type="Informative" url="https://helpx.adobe.com/tw/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 901b17c7493e76b17e780b6f7b05a69fa22303d2
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# 端對端工作流程

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，端對端工作流程會依您選擇的共同作業模式而有所不同。 工作流程概述設定及執行共同作業專案的相關步驟，從建立帳戶和來源受眾，到建立連線和專案。 瞭解此工作流程是有效運用平台功能達成行銷目標的關鍵。

## 快速入門

開始之前，請確定您已確實瞭解以下重要概念：

- **Collaboration模式**：這些模式定義共同作業人員如何共同作業。 共有五種不同的模式：
   - [廣告商對發佈者](./collaboration-patterns.md#advertiser-to-publisher)
   - [品牌對品牌](./collaboration-patterns.md#brand-to-brand)
   - [廣告商對資料合作夥伴](./collaboration-patterns.md#advertiser-to-data-partner)
   - [代理商對發佈商](./collaboration-patterns.md#agency-to-publisher)
   - [廣告商對機構平台](./collaboration-patterns.md#advertiser-to-agency-platform)
- **帳戶角色**：帳戶角色決定您在平台中的權能。 藍圖應與您組織的目標、品牌和目標一致。 有四個帳戶角色： [廣告商](./roles.md#advertiser)、[發佈者](./roles.md#publisher)、[機構](./roles.md#agency)和[資料夥伴](./roles.md#data-partner)。
- **使用案例**：使用案例會定義您如何善用Collaboration達成行銷目標。 有三個共同作業使用案例： [探索](./use-cases.md#discover)、[啟動](./use-cases.md#activate)以及[測量](./use-cases.md#measure)。

本指南將使用三位模擬共同作業人員來說明端對端工作流程：

- **[!UICONTROL Luma]**：運動服裝品牌。 他們是廣告商，想要透過鎖定目標的行銷活動觸及特定對象。
- **[!UICONTROL 電視管]**：數位串流提供者。 它們是提供受眾資料以供廣告商使用的發佈者。
- **[!UICONTROL 適合服飾]**：另一個運動服飾品牌。 他們為想要共同作業以分享對象資料和深入分析的第二位廣告商，藉此提升行銷成效。
- **[!UICONTROL 代理商99]**：媒體代理商。 他們可在工作區中管理多個使用者端帳戶，並與發佈者和廣告商連結。
- **[!UICONTROL DataM8]**：協力廠商資料提供者。 它們提供受眾資料供廣告商使用。
- **[!UICONTROL Holdco]**：代理商持有公司行銷與廣告服務平台，內部代理商團隊用它來管理客戶行銷活動。

## 廣告商對發佈商的工作流程 {#advertiser-to-publisher-workflow}

[!UICONTROL Luma] （一家體育零售公司）想要與數位串流供應商[!UICONTROL TV Tube]建立連線，以透過鎖定目標的行銷活動觸及特定對象。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)，而[!UICONTROL TV Tube]則以發佈者角色建立帳戶。

建立帳戶之後，[!UICONTROL Luma]和[!UICONTROL TV Tube]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 只有[!UICONTROL TV Tube]會啟用行銷活動的對象，因此他們需要[設定目的地](../setup/manage-destinations.md)。

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../connect/discover-collaborators.md)功能尋找[!UICONTROL 電視管]並起始連線要求。 在[!UICONTROL TV Tube]接受連線要求後，[!UICONTROL Luma]會設定連線設定以定義他們將如何共同作業。 [!UICONTROL TV Tube]接受連線要求，以建立兩個品牌之間的安全連結。

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

在[!UICONTROL Luma]設定好帳戶後，他們便已準備好在平台內[與[!DNL AMC]建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../connect/discover-collaborators.md)功能尋找[!UICONTROL Amazon Marketing Cloud]並[起始連線要求](../connect/advertising-platforms/amc.md)。 透過[!DNL Amazon]登入頁面驗證並授權連線後，已建立與[!DNL AMC]的連線。

建立連線之後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)以開始他們與[!DNL AMC]的協同合作。 連線設定（包括使用案例）會根據廣告平台進行預先設定。 針對[!DNL AMC]，可用的使用案例是[探索](../collaborate/advertising-platforms/amc.md#discover)。

[!UICONTROL Luma]利用[Discover](../collaborate/advertising-platforms/amc.md#discover)使用案例從[!DNL AMC]取得深入分析和對象資料。 使用這些深入分析，[!UICONTROL Luma]可以最佳化行銷策略，並提高行銷活動的成效。

## 廣告商對資料合作夥伴工作流程 {#advertiser-to-data-partner-workflow}

[!UICONTROL Luma] （一家體育零售公司）想要與協力廠商資料提供者[!UICONTROL DataM8]共同作業，以豐富客戶設定檔並改善對象鎖定目標。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)，而[!UICONTROL DataM8]則以資料合作夥伴角色建立帳戶。

建立帳戶之後，[!UICONTROL Luma]和[!UICONTROL DataM8]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 兩個共同作業人員都可以啟用行銷活動的對象，因此他們每個人都需要[設定目的地](../setup/manage-destinations.md)。

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../collaborate/discover.md)功能尋找[!UICONTROL DataM8]並起始連線要求。 在[!UICONTROL DataM8]接受連線要求後，[!UICONTROL Luma]會設定連線設定以定義他們將如何共同作業。 [!UICONTROL DataM8]接受連線要求，以便在兩個共同作業人員之間建立安全連結。

建立連線後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)以開始他們與[!UICONTROL DataM8]的協同合作。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)使用案例來深入分析[!UICONTROL DataM8]的對象資料。 在[!UICONTROL Luma]識別目標對象區段後，他們[啟用](../collaborate/activate.md)這些對象。

[!UICONTROL DataM8]也可以[啟用](../collaborate/activate.md)其對象至[!UICONTROL Luma]。 [!UICONTROL Luma]使用這些功能將第三方屬性附加至其客戶設定檔並分析對象構成。 透過其CDP中直接提供的豐富資料，[!UICONTROL Luma]可以建立更精確的受眾，並將其啟用至付費媒體目的地，無需將資料移出其受管理的環境。

## 代理商對發佈商工作流程 {#agency-to-publisher-workflow}

[!UICONTROL Agency99]，一家媒體代理商，想要與數位串流供應商[!UICONTROL TV Tube]合作，透過鎖定目標的行銷活動觸及特定對象。

若要開始，[!UICONTROL Agency99]需要[以代理角色](../setup/onboard-account.md)建立帳戶，而[!UICONTROL TV Tube]則以發佈者角色建立帳戶。

建立帳戶之後，[!UICONTROL Agency99]和[!UICONTROL 電視管]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 [!UICONTROL Agency99]將會在其工作區中設定使用者端子帳戶和來源使用者端資料。 只有[!UICONTROL TV Tube]會啟用行銷活動的對象，因此他們需要[設定目的地](../setup/manage-destinations.md)。

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Agency99]使用[探索共同作業人員](../collaborate/discover.md)功能尋找[!UICONTROL 電視管]並起始連線要求。 [!UICONTROL Agency99]將針對一或多個想要與[!UICONTROL TV Tube]共同作業的使用者端執行此動作。 在[!UICONTROL TV Tube]接受連線要求之後，[!UICONTROL Agency99]會設定連線設定，以定義每個共同作業的方式。 [!UICONTROL TV Tube]接受連線要求，以建立兩個品牌之間的安全連結。

建立連線之後，[!UICONTROL Agency99] [會建立專案](../collaborate/manage-projects.md)，以開始與每個使用者端子帳戶中的[!UICONTROL TV Tube]共同作業。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Agency99]利用[Discover](../collaborate/discover.md)使用案例來深入瞭解[!UICONTROL 電視管]的對象資料。 一旦[!UICONTROL Agency99]識別目標對象區段，他們[啟用](../collaborate/activate.md)這些對象。

啟用對象後，[!UICONTROL TV Tube]會執行目標式行銷活動，並將資料上傳至[測量](../collaborate/measure.md)結果，以評估其行銷活動的成效。

## 廣告商對機構平台工作流程 {#advertiser-to-agency-platform-workflow}

[!UICONTROL Luma]是運動零售公司，想要與代理平台[!UICONTROL Holdco]共同合作，以共用資料並接收付費媒體深入分析。

若要開始，[!UICONTROL Luma]需要以廣告商角色[建立帳戶](../setup/onboard-account.md)，而[!UICONTROL Holdco]則以代理商角色建立帳戶。 

建立帳戶之後，[!UICONTROL Luma]和[!UICONTROL Holdco]都必須[建立資料連線和來源對象](../setup/onboard-audiences.md)。 兩個共同作業人員都可以啟用行銷活動的對象，因此他們每個人都需要[設定目的地](../setup/manage-destinations.md)。 

兩個共同作業人員設定好帳戶後，就可以在平台內[建立連線](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[探索共同作業人員](../collaborate/discover.md)功能尋找[!UICONTROL Holdco]並起始連線要求。 在[!UICONTROL Holdco]接受連線要求之後，[!UICONTROL Luma]會設定連線設定以定義他們將如何共同作業。

[!UICONTROL Holdco]接受連線要求，以便在兩個共同作業人員之間建立安全連結。

建立連線之後，[!UICONTROL Luma] [會建立專案](../collaborate/manage-projects.md)以開始他們與[!UICONTROL Holdco]的協同合作。 在專案設定期間，他們選擇最符合其目標的共同作業使用案例： [探索](../collaborate/discover.md)、[啟動](../collaborate/activate.md)以及[測量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)使用案例來深入分析[!UICONTROL Holdco]的對象資料。 在[!UICONTROL Luma]識別目標對象區段後，他們[啟用](../collaborate/activate.md)這些對象。

[!UICONTROL Holdco]也可以[啟用](../collaborate/activate.md)其對象至[!UICONTROL Luma]。 [!UICONTROL Luma]使用這些功能，從機構執行的行銷活動中接收付費媒體深入分析，以用於深入分析、CDP設定檔附加和自有媒體協調。
