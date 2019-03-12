---
author: karuanag
ms.author: karuanag
title: 常見問題集的 Office 365 方案的自訂學習
ms.date: 02/10/2019
description: Office 365 的自訂學習問題資訊的常見問題集
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543763"
---
# <a name="frequently-asked-questions"></a>常見問題集

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1.什麼是 Office 365 的安裝自訂學習到我的租用戶環境的需求？

- SharePoint Online 和通訊網站啟用。
- 佈建 CLO365 個別必須安裝目標租用戶的租用戶系統管理員。
- 租用戶 '應用程式目錄' 必須是 SharePoint 系統管理中心的 「 應用程式' 選項中可用的。
- 佈建 CLO365 個別必須在目標租用戶以供安裝的應用程式目錄網站集合管理員。

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2.什麼語言是自訂學習運作的 Office 365 中可用？

自訂 Office 365 學習是目前僅提供英文版本。 自動端對端佈建只適用於英文的租用戶。 其他語言可能會加入在未來版本。

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3.花多少時間會在我們的租用戶環境中安裝網站？

根據我們的測試的安裝，它應該採取小於 15 分鐘。 這不包括自訂網站，您的需求所需的時間。

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4.我們讓 Office 365 學習我們主要 SharePoint 網站集合的子網站的自訂嗎？

否。 網站根據通訊網站範本，這一律是用來在根網站集合。

> [!NOTE]
> 請務必考慮您的使用者需要存取網站的權限。 大多數的組織已定義的安全性或使用者群組。 一旦您準備好要啟動至您的員工社群，必須將適當的安全性群組新增至新的訓練入口網站。

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5.我需要重新安裝網站;我該怎麼辦？

請遵循安裝指示發佈[以下](custom_provision.md)。

> [!NOTE]
> 如果您有已停用您先前的安裝中的遙測，可能會想要繼續使用遙測停用，您必須遵循指示來停用遙測以下。

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6.我們我們實作自訂學習運作的 Office 365 進行更新。 如果我們重新安裝網站，我們有遺失 （對網站範本，播放清單） 這些更新會嗎？

如果您透過您目前安裝重新安裝網站自訂個別頁面及自訂播放清單將會遺失。  