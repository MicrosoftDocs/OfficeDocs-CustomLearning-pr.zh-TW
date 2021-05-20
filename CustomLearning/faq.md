---
title: Microsoft 365 學習路徑常見問題
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: Microsoft 365 學習路徑的常見問題資訊
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: f24f16455ba41724d300d038a01dc04c2170dc4a
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575918"
---
# <a name="frequently-asked-questions"></a>常見問題集

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>我最近看到過的博客文章會將 Office 365 的自訂教學重新命名成 Microsoft 365 學習路徑。 在重新命名的工作量中，是否要將其他變更新增至解決方案？ 我應該更新組織中的方案嗎？

Microsoft 365 學習途徑是一項 ..org 工作，專門用來變更解決方案的名稱，使其符合 Microsoft 365 署名。 如果您已在組織中成功執行 Office 365 的自訂教學，則目前不需要更新解決方案。  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>在我的租使用者環境中安裝 Microsoft 365 學習路徑的需求為何？

- 已啟用 SharePoint Online 和通訊網站。
- 將要布建 CLO365 的個人必須是安裝目標租使用者的租使用者系統管理員。
- 租使用者 "應用程式目錄" 必須可用於 SharePoint 系統管理中心的「應用程式」選項中。
- 如果建立新的應用程式目錄，則需要30分鐘以上的等候時間，才能完全布建應用程式目錄。 嘗試在建立租使用者應用程式目錄之後，直接布建 Microsoft 365 學習路徑，將會產生「學習路徑」解決方案的布建錯誤。 
- 將會布建 CLO365 的個人必須是目標租使用者中應用程式目錄的網站集合管理員，才可進行安裝。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>為什麼 Microsoft 在安裝 Microsoft 365 學習路徑時要求租使用者許可權 

- SharePoint 線上布建服務使用將學習路徑布建 SharePoint 網站、建立網站頁面，以及在其承租人內安裝 Microsoft 365 教學路徑應用程式的許可權。 這是我們要求許可權的唯一原因。 若沒有要求的許可權，SharePoint 提供服務無法執行自動安裝學習路徑網站範本與網頁元件的命令。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>在 Beta Preview 中 Microsoft 365 學習路徑的含義為何？ 

Microsoft 365 學習路徑目前是 Beta 預覽。 評估、規劃及實施 Microsoft 365 學習路徑時，請考慮下列事項：

- 就像在任何 Beta 方案中，我們的服務管理小組都會保留變更服務及其元件的權利。 當您積極解決 bug 和 UX 問題時，可能需要更新 WebPart。
- 若要更新網頁元件，您必須從我們的 GitHub 存放庫中下載該網頁元件，並將其上傳至您的租使用者應用程式目錄。 請參閱 Microsoft 365 學習路徑[自述](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)檔的「更新解決方案」一節。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>可用的教學途徑 Microsoft 365 哪些語言？

目前只有英文版本的教學 Microsoft 365。 自動端對端布建只適用于英文承租人。 在2020的第二季度，我們計畫推出下列語言的多語系支援。 

- 簡體中文 
- 法文  
- 德文 
- 義大利文 (義大利) 
- 日本 (日本)   
- 葡萄牙文 (巴西)  
- 俄文 (俄文)   
- 西班牙文 

> 對荷蘭文言的支援，將不會包含在教學路徑的後續版本中的支援。 我們將在未來繼續評估新的語言選項。

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>在我們的承租人環境中安裝網站所需的時間多久？

根據我們的安裝測試，它應該需要不到15分鐘的時間。 這不包括按您的需求自訂網站所需的時間。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 學習路徑是開放來源解決方案，以及有何影響？

Microsoft 365 學習途徑是一種開放來源軟體 (OSS) 解決方案，也就是將一組優點和考慮因素 germane 至 OSS：

#### <a name="benefits"></a>優點 
- **Microsoft 365 學習途徑是免費的解決方案：** 客戶可以在他們的承租人中安裝解決方案，加以自訂，並讓使用者可以使用
- **OSS 可讓您快速開發及**  共同作業： 所有的「開放來源」解決方案皆可供廣大投稿小組群組使用。  Microsoft 致力於這種促進創新的方法。  為了確保我們所提供的體驗可為我們最廣泛的客戶提供好處，我們的核心服務管理小組會預約適當的權利，以判斷哪些發佈內容會與我們的官方組建合併。  
- **OSS 可與合作夥伴** 共同作業：Microsoft 與數名學習協力廠商合作，以支援其未來擴充的工作，以及 Microsoft 365 教學路徑的貢獻。 我們將在這些計畫變成定稿時提供詳細資訊。 
    
#### <a name="implications"></a>影響
- **OSS 並非商業可用產品：** 商業產品包括更新及修補程式，並隨附于收費支援合同中。 雖然 Microsoft 目前提供檔、更新及修補 Microsoft 365 教學路徑，是根據我們對於改進此特定商務案例的承諾而定。 我們的計畫是在學習路徑中繼續投資，請注意我們的服務管理小組以後可能會變更策略。 任何未來對 Microsoft 365 學習路徑的變更都會在生效時進行傳遞。 
- **在 OSS 中，您可以透過 GitHub 上的線上問題清單支援 Microsoft 365 教學路徑**： Microsoft 365 學習路徑不是由任何現有的 Microsoft 支援合同所涵蓋。 Microsoft 365 學習路徑服務擁有者和社區中，會將提交的問題會審。 問題解決方式服務層級與「付費的 Microsoft 支援合同」不符。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>我們是否可以讓 Microsoft 365 學習路徑成為我們主要 SharePoint 網站集合的子網站？

否。 網站是以通訊網站範本為基礎，該範本永遠是根網站集合。

> [!NOTE]
> 請務必考慮您的使用者存取網站所需的許可權。 大多陣列織已定義安全性或使用者群組。 您準備好將適當的安全性群組新增至您的員工群組之後，您必須將適當的安全性群組新增至新的訓練入口網站。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>我需要重新安裝網站;我該怎麼做？

遵循 [這裡](custom_provision.md)發佈的安裝指示。

> [!NOTE]
> 如果您已在先前的安裝中停用遙測，且想要繼續遙測停用，您必須遵循在此停用遙測的指示。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>我們對 Microsoft 365 學習路徑的實施進行更新。 如果重新安裝網站，將無法 (網站範本，播放清單) 進行這些更新？

如果您在目前的安裝上重新安裝網站，將會遺失個別頁面和自訂播放清單的自訂。  
