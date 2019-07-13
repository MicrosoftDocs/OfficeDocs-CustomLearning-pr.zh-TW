---
author: karuanag
ms.author: karuanag
title: 常見問題集的 Microsoft 365 學習路徑
ms.date: 02/10/2019
description: Microsoft 365 學習路徑的常見問題集資訊
ms.openlocfilehash: 66149439f0ca13b319bee3bea9c2773b43e98e25
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2019
ms.locfileid: "35636107"
---
# <a name="frequently-asked-questions"></a>常見問題集

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>我最近所看到的部落格文章，自訂 Office 365 學習要重新命名為 Microsoft 365 學習路徑。 是否有一部分重新命名工作新增至解決方案的其他變更？ 應該更新解決方案在我的組織中？

學習路徑版 Microsoft 365 是以符合 Microsoft 365 品牌的 rebranding 努力專用於變更解決方案的名稱。 如果您有自訂學習目前正在執行順利在組織中的 Office 365 時，它不需要這一次更新解決方案。  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>安裝 Microsoft 365 學習路徑到我的租用戶環境的需求是甚麼？

- SharePoint Online 和通訊網站啟用。
- 佈建 CLO365 個別必須安裝目標租用戶的租用戶系統管理員。
- 租用戶 '應用程式目錄' 必須是 SharePoint 系統管理中心的 「 應用程式' 選項中可用的。
- 如果在建立新的應用程式目錄，30 分鐘或更久的等候時間有要完全佈建的應用程式目錄。 嘗試佈建 Microsoft 365 學習路徑建立租用戶應用程式目錄之後，直接將會導致學習佈建錯誤路徑解決方案。 
- 佈建 CLO365 個別必須在目標租用戶以供安裝的應用程式目錄網站集合管理員。

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>為什麼會 Microsoft 詢問租用戶權限安裝 Microsoft 365 學習路徑時 

- SharePoint Online 佈建服務使用的權限，若要佈建學習路徑 SharePoint 網站，請建立的網站] 頁面，以及安裝 Microsoft 365 學習其租用戶中的啟用應用程式。 這是我們要求的權限的唯一原因。 沒有 SharePoint 佈建服務無法執行要求的權限的命令，會自動安裝學習路徑的網站範本和網頁組件。 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>學習路徑正在 Beta 預覽中的 Microsoft 365 的影響為何？ 

Microsoft 365 學習路徑目前是 Beta 預覽中。 當您評估、 規劃及實作 Microsoft 365 學習路徑，請考慮下列：

- 為與任何 Beta 解決方案我們的服務管理小組的權利服務和其元件進行變更。 當我們主動已解決錯誤和 UX 問題可能需要更新網頁組件。
- 若要更新的網頁組件，您必須下載來自我們 GitHub 存放庫，並將其上傳到您的租用戶的應用程式目錄。 請參閱 Microsoft 365 學習路徑[讀我](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)檔案 」 更新解決方案 」 一節。 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>哪些語言 Microsoft 365 學習路徑中可用？

Microsoft 365 學習路徑是目前僅提供英文版本。 自動端對端佈建只適用於英文的租用戶。 我們計劃推行 CY19 Q4 這些九個語言的多語系支援： 

- 簡體中文 
- 荷蘭文 (荷蘭) 
- 法文  
- 德文 
- 義大利文 (義大利) 
- 日文 （日本）  
- 葡萄牙文 （巴西） 
- 俄文 （俄羅斯）  
- 西班牙文 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>如何將它需要花費時間我們租用戶環境中安裝網站？

根據我們的測試的安裝，它應該採取小於 15 分鐘。 這不包括自訂網站，您的需求所需的時間。

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>為 Microsoft 365 學習路徑開放原始碼解決方案，以及它們所造成影響？

學習路徑的 Microsoft 365 是開啟來源軟體 (OS) 解決方案，因此執行一組的優勢及考量 OSS 密切關係：

#### <a name="benefits"></a>效益 
- **學習路徑的 Microsoft 365 是免費的解決方案：** 客戶可以其租用戶中安裝解決方案、 自訂及提供給使用者
- **OSS 可讓開發速度和共同作業：** 所有的開放原始碼解決方案可廣泛社群參與者。  Microsoft 致力於主導狀態的創新此方法。  若要確保我們會提供福利我們的客戶的最寬集經驗我們核心服務管理小組，會保留至判斷哪些捐款已合併成我們正式組建權利。  
- **OSS 可讓與合作夥伴共同作業：** Microsoft 會使用數個學習合作夥伴，支援其努力未來的擴充功能和 Microsoft 365 學習路徑的貢獻。 我們將提供這些計劃成為完成的更多資訊。 
    
#### <a name="implications"></a>影響
- **OSS 不是售產品：** 商業產品包括更新及修補程式，而且會包含在付費支援合約。 Microsoft 目前提供文件，而更新及修補用於 Microsoft 365 學習路徑它根據我們致力於改善此特定的商務案例。 我們計劃来繼續投資學習路徑，但客戶應該要知道我們的服務管理小組在未來可能變更的策略。 Microsoft 365 學習路徑任何未來的變更會傳達遲生效。 
- **透過 GitHub 上的線上的問題清單支援為 OSS、 Microsoft 365 學習路徑**： Microsoft 365 學習路徑未涵蓋的任何現有的 Microsoft 支援合約。 送出的問題會由 Microsoft 365 學習路徑服務擁有者和社群進行分級。 此問題： 解決方案服務層級不是做為付費的 Microsoft 支援合約相同層級。  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>我們讓學習路徑 Microsoft 365 我們主要 SharePoint 網站集合的子網站？

否。 網站根據通訊網站範本，這一律是用來在根網站集合。

> [!NOTE]
> 請務必考慮您的使用者需要存取網站的權限。 大多數的組織已定義的安全性或使用者群組。 一旦您準備好要啟動至您的員工社群，必須將適當的安全性群組新增至新的訓練入口網站。

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>我需要重新安裝網站;我該怎麼辦？

請遵循安裝指示發佈[以下](custom_provision.md)。

> [!NOTE]
> 如果您有已停用您先前的安裝中的遙測，可能會想要繼續使用遙測停用，您必須遵循指示來停用遙測以下。

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>我們對更新我們實作的 Microsoft 365 學習路徑。 如果我們重新安裝網站，我們有遺失 （對網站範本，播放清單） 這些更新會嗎？

如果您透過您目前安裝重新安裝網站自訂個別頁面及自訂播放清單將會遺失。  