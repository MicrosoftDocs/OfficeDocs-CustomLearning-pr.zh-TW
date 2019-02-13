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
# <a name="frequently-asked-questions"></a><span data-ttu-id="4e164-103">常見問題集</span><span class="sxs-lookup"><span data-stu-id="4e164-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="4e164-104">1.什麼是 Office 365 安裝自訂學習到我的用戶環境的需求？</span><span class="sxs-lookup"><span data-stu-id="4e164-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="4e164-105">SharePoint Online 並已啟用的通訊網站。</span><span class="sxs-lookup"><span data-stu-id="4e164-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="4e164-106">佈建 CLO365 個別必須以供安裝目標租用戶的租用戶系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4e164-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="4e164-107">承租人 '應用程式目錄' 必須可以在 SharePoint 管理中心的 「 應用程式' 選項。</span><span class="sxs-lookup"><span data-stu-id="4e164-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="4e164-108">佈建 CLO365 個別必須以供安裝目標租用戶中應用程式目錄網站集合管理員。</span><span class="sxs-lookup"><span data-stu-id="4e164-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="4e164-109">2.哪些語言是提供了 Office 365 適用的自訂？</span><span class="sxs-lookup"><span data-stu-id="4e164-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="4e164-p101">自訂的 Office 365 學習是目前只適用於英文。自動端對端佈建只適用於英文租用戶。其他語言可能會新增在未來版本。</span><span class="sxs-lookup"><span data-stu-id="4e164-p101">Custom Learning for Office 365 is currently available only in English. Automatic end-to-end provisioning only works with English tenants. Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="4e164-113">3.將多少時間我們用戶環境中安裝網站？</span><span class="sxs-lookup"><span data-stu-id="4e164-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="4e164-p102">根據我們測試的安裝，它應該採取小於 15 分鐘。這不包括自訂您的需求網站所需的時間。</span><span class="sxs-lookup"><span data-stu-id="4e164-p102">Based on our testing of the installation, it should take less than 15 minutes. This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="4e164-116">4.我們進行 Office 365 學習我們主要的 SharePoint 網站集合的子網站的自訂吗？</span><span class="sxs-lookup"><span data-stu-id="4e164-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="4e164-p103">[否]。網站根據通訊的網站範本，這一律原本用意是根網站集合。</span><span class="sxs-lookup"><span data-stu-id="4e164-p103">No. The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="4e164-p104">請務必考量您的使用者需要存取網站的權限。大部分組織已定義的安全性或使用者群組。之後即可啟動至您的員工社群，您必須將適當的安全性群組新增至新的訓練入口網站中。</span><span class="sxs-lookup"><span data-stu-id="4e164-p104">It is important to consider the permissions your end users will need to access the site. Most organizations have defined security or user groups. You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="4e164-122">5.我需要重新安裝網站 ；我該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="4e164-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="4e164-123">請遵循安裝指示發佈[此處](installsitepackage.md)。</span><span class="sxs-lookup"><span data-stu-id="4e164-123">Follow the installation instructions published [here](installsitepackage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="4e164-124">如果您有已停用先前安裝中的遙測及想要停用遙測繼續執行，您必須遵循指示來停用的遙測。</span><span class="sxs-lookup"><span data-stu-id="4e164-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="4e164-p105">6.我們對我們實作自訂學習 Office 365 進行更新。將我們會遺失這些更新 （網站範本、 播放清單） 如果我們重新安裝網站吗？</span><span class="sxs-lookup"><span data-stu-id="4e164-p105">6. We made updates to our implementation of Custom Learning for Office 365. Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="4e164-127">若您要重新安裝網站透過目前安裝自訂個別頁面與自訂播放清單將會遺失。</span><span class="sxs-lookup"><span data-stu-id="4e164-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  