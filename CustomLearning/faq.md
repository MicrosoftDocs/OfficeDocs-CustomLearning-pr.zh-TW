---
author: karuanag
ms.author: karuanag
title: 常見問題集的自訂學習 Office 365 解決方案
ms.date: 02/10/2019
description: Office 365 的自訂學習問題資訊的常見問題集
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952601"
---
# <a name="frequently-asked-questions"></a>常見問題集

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1.什麼是 Office 365 安裝自訂學習到我的用戶環境的需求？

- SharePoint Online 並已啟用的通訊網站。
- 佈建 CLO365 個別必須以供安裝目標租用戶的租用戶系統管理員。
- 承租人 '應用程式目錄' 必須可以在 SharePoint 管理中心的 「 應用程式' 選項。
- 佈建 CLO365 個別必須以供安裝目標租用戶中應用程式目錄網站集合管理員。

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2.哪些語言是提供了 Office 365 適用的自訂？

自訂的 Office 365 學習是目前只適用於英文。自動端對端佈建只適用於英文租用戶。其他語言可能會新增在未來版本。

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3.將多少時間我們用戶環境中安裝網站？

根據我們測試的安裝，它應該採取小於 15 分鐘。這不包括自訂您的需求網站所需的時間。

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4.我們進行 Office 365 學習我們主要的 SharePoint 網站集合的子網站的自訂吗？

[否]。網站根據通訊的網站範本，這一律原本用意是根網站集合。

> [!NOTE]
> 請務必考量您的使用者需要存取網站的權限。大部分組織已定義的安全性或使用者群組。之後即可啟動至您的員工社群，您必須將適當的安全性群組新增至新的訓練入口網站中。

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5.我需要重新安裝網站 ；我該怎麼辦？

請遵循安裝指示發佈[此處](installsitepackage.md)。

> [!NOTE]
> 如果您有已停用先前安裝中的遙測及想要停用遙測繼續執行，您必須遵循指示來停用的遙測。

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6.我們對我們實作自訂學習 Office 365 進行更新。將我們會遺失這些更新 （網站範本、 播放清單） 如果我們重新安裝網站吗？

若您要重新安裝網站透過目前安裝自訂個別頁面與自訂播放清單將會遺失。  