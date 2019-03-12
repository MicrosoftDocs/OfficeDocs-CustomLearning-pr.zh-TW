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
# <a name="frequently-asked-questions"></a><span data-ttu-id="35976-103">常見問題集</span><span class="sxs-lookup"><span data-stu-id="35976-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="35976-104">1.什麼是 Office 365 的安裝自訂學習到我的租用戶環境的需求？</span><span class="sxs-lookup"><span data-stu-id="35976-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="35976-105">SharePoint Online 和通訊網站啟用。</span><span class="sxs-lookup"><span data-stu-id="35976-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="35976-106">佈建 CLO365 個別必須安裝目標租用戶的租用戶系統管理員。</span><span class="sxs-lookup"><span data-stu-id="35976-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="35976-107">租用戶 '應用程式目錄' 必須是 SharePoint 系統管理中心的 「 應用程式' 選項中可用的。</span><span class="sxs-lookup"><span data-stu-id="35976-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="35976-108">佈建 CLO365 個別必須在目標租用戶以供安裝的應用程式目錄網站集合管理員。</span><span class="sxs-lookup"><span data-stu-id="35976-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="35976-109">2.什麼語言是自訂學習運作的 Office 365 中可用？</span><span class="sxs-lookup"><span data-stu-id="35976-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="35976-110">自訂 Office 365 學習是目前僅提供英文版本。</span><span class="sxs-lookup"><span data-stu-id="35976-110">Custom Learning for Office 365 is currently available only in English.</span></span> <span data-ttu-id="35976-111">自動端對端佈建只適用於英文的租用戶。</span><span class="sxs-lookup"><span data-stu-id="35976-111">Automatic end-to-end provisioning only works with English tenants.</span></span> <span data-ttu-id="35976-112">其他語言可能會加入在未來版本。</span><span class="sxs-lookup"><span data-stu-id="35976-112">Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="35976-113">3.花多少時間會在我們的租用戶環境中安裝網站？</span><span class="sxs-lookup"><span data-stu-id="35976-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="35976-114">根據我們的測試的安裝，它應該採取小於 15 分鐘。</span><span class="sxs-lookup"><span data-stu-id="35976-114">Based on our testing of the installation, it should take less than 15 minutes.</span></span> <span data-ttu-id="35976-115">這不包括自訂網站，您的需求所需的時間。</span><span class="sxs-lookup"><span data-stu-id="35976-115">This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="35976-116">4.我們讓 Office 365 學習我們主要 SharePoint 網站集合的子網站的自訂嗎？</span><span class="sxs-lookup"><span data-stu-id="35976-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="35976-117">否。</span><span class="sxs-lookup"><span data-stu-id="35976-117">No.</span></span> <span data-ttu-id="35976-118">網站根據通訊網站範本，這一律是用來在根網站集合。</span><span class="sxs-lookup"><span data-stu-id="35976-118">The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="35976-119">請務必考慮您的使用者需要存取網站的權限。</span><span class="sxs-lookup"><span data-stu-id="35976-119">It is important to consider the permissions your end users will need to access the site.</span></span> <span data-ttu-id="35976-120">大多數的組織已定義的安全性或使用者群組。</span><span class="sxs-lookup"><span data-stu-id="35976-120">Most organizations have defined security or user groups.</span></span> <span data-ttu-id="35976-121">一旦您準備好要啟動至您的員工社群，必須將適當的安全性群組新增至新的訓練入口網站。</span><span class="sxs-lookup"><span data-stu-id="35976-121">You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="35976-122">5.我需要重新安裝網站;我該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="35976-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="35976-123">請遵循安裝指示發佈[以下](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="35976-123">Follow the installation instructions published [here](custom_provision.md).</span></span>

> [!NOTE]
> <span data-ttu-id="35976-124">如果您有已停用您先前的安裝中的遙測，可能會想要繼續使用遙測停用，您必須遵循指示來停用遙測以下。</span><span class="sxs-lookup"><span data-stu-id="35976-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="35976-125">6.我們我們實作自訂學習運作的 Office 365 進行更新。</span><span class="sxs-lookup"><span data-stu-id="35976-125">6. We made updates to our implementation of Custom Learning for Office 365.</span></span> <span data-ttu-id="35976-126">如果我們重新安裝網站，我們有遺失 （對網站範本，播放清單） 這些更新會嗎？</span><span class="sxs-lookup"><span data-stu-id="35976-126">Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="35976-127">如果您透過您目前安裝重新安裝網站自訂個別頁面及自訂播放清單將會遺失。</span><span class="sxs-lookup"><span data-stu-id="35976-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  