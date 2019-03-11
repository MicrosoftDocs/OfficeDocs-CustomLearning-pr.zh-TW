---
author: pkrebs
ms.author: pkrebs
title: 概觀
ms.date: 02/18/2019
description: 自訂學習 for Office 365 系統管理員的概觀
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523017"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="f35eb-103">自訂的學習體驗</span><span class="sxs-lookup"><span data-stu-id="f35eb-103">Customize the Learning Experience</span></span>

<span data-ttu-id="f35eb-104">簡介自訂學習運作的 Office 365，Microsoft 提供的新的解決方案設計用來加速使用情況和採用 Office 365 組織內。</span><span class="sxs-lookup"><span data-stu-id="f35eb-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="f35eb-105">自訂學習，您可以進行下列作業：</span><span class="sxs-lookup"><span data-stu-id="f35eb-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="f35eb-106">量身訂做為您的環境的 Office 365 學習和採用率內容</span><span class="sxs-lookup"><span data-stu-id="f35eb-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="f35eb-107">隱藏或顯示內容以反映服務或貴組織中支援的功能</span><span class="sxs-lookup"><span data-stu-id="f35eb-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="f35eb-108">保留內容和使用者目前與學習從 Microsoft 內容的最新摘要</span><span class="sxs-lookup"><span data-stu-id="f35eb-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="f35eb-109">建立自訂播放清單及製作特別為您的使用者需求的類別</span><span class="sxs-lookup"><span data-stu-id="f35eb-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg introducing.png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="f35eb-111">自訂學習如何運作？</span><span class="sxs-lookup"><span data-stu-id="f35eb-111">How does Custom Learning work?</span></span>

<span data-ttu-id="f35eb-112">了解 Office 365 （簡稱為自訂學習） 的自訂是由三個部分所組成：</span><span class="sxs-lookup"><span data-stu-id="f35eb-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="f35eb-113">Microsoft online 目錄內容的即時摘要</span><span class="sxs-lookup"><span data-stu-id="f35eb-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="f35eb-114">SharePoint 通訊網站</span><span class="sxs-lookup"><span data-stu-id="f35eb-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="f35eb-115">SharePoint 網頁組件</span><span class="sxs-lookup"><span data-stu-id="f35eb-115">a SharePoint web part</span></span> 

![cg howitworks.png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="f35eb-117">需求和權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-117">Requirements and Permissions</span></span>

<span data-ttu-id="f35eb-118">開始之前與本指南，確保自訂學習具有已設定由您 SharePoint 租用戶系統管理員。</span><span class="sxs-lookup"><span data-stu-id="f35eb-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="f35eb-119">如果您不確定如果它設定好之後，請連絡您的 SharePoint 租用戶系統管理員，若要確認已佈建自訂學習。</span><span class="sxs-lookup"><span data-stu-id="f35eb-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="f35eb-120">也請務必要取得自訂學習 SharePoint 網站的 URL。</span><span class="sxs-lookup"><span data-stu-id="f35eb-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="f35eb-121">如果您是租用戶系統管理員，而且尚未佈建自訂學習，請參閱 <<c0>佈建自訂學習。</span><span class="sxs-lookup"><span data-stu-id="f35eb-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="f35eb-122">佈建自訂學習的權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="f35eb-123">租用戶系統管理員，也就是 Office 365 全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="f35eb-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="f35eb-124">SharePoint 網站集合管理員與擁有者網站的權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="f35eb-125">使用自訂學習管理功能的權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="f35eb-126">網站集合管理員</span><span class="sxs-lookup"><span data-stu-id="f35eb-126">Site Collection Administrator</span></span>
- <span data-ttu-id="f35eb-127">SharePoint 擁有者或成員的權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="f35eb-128">若要使用自訂學習站台作為使用者的權限</span><span class="sxs-lookup"><span data-stu-id="f35eb-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="f35eb-129">Office 365 使用者權限/SharePoint 網站訪客權限或更高層級</span><span class="sxs-lookup"><span data-stu-id="f35eb-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="f35eb-130">自訂快速入門</span><span class="sxs-lookup"><span data-stu-id="f35eb-130">Get started with customization</span></span>
<span data-ttu-id="f35eb-131">一旦您已確定滿足您有自訂的網站和網頁組件的必要權限，該是時候來開始使用的自訂程序。</span><span class="sxs-lookup"><span data-stu-id="f35eb-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="f35eb-132">若要開始，請參閱[移至的自訂學習網站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="f35eb-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>