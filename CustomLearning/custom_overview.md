---
author: pkrebs
ms.author: pkrebs
title: 概觀
ms.date: 02/18/2019
description: 自訂學習 office 365 系統管理員的概觀
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087532"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="8aba9-103">自訂學習經驗</span><span class="sxs-lookup"><span data-stu-id="8aba9-103">Customize the Learning Experience</span></span>

<span data-ttu-id="8aba9-p101">Office 365 簡介自訂學習、 新的解決方案使用 microsoft 設計目的在於速度的使用方式和採用 Office 365 組織內。自訂學習您可以進行下列作業：</span><span class="sxs-lookup"><span data-stu-id="8aba9-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="8aba9-106">調整使其適合您環境的 Office 365 學習與採用內容</span><span class="sxs-lookup"><span data-stu-id="8aba9-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="8aba9-107">隱藏或顯示以反映服務或組織中支援的功能</span><span class="sxs-lookup"><span data-stu-id="8aba9-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="8aba9-108">保留內容和使用者目前具有學習內容從 Microsoft 最新摘要</span><span class="sxs-lookup"><span data-stu-id="8aba9-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="8aba9-109">建立自訂播放清單以及類別製作特別針對使用者的需求</span><span class="sxs-lookup"><span data-stu-id="8aba9-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg introducing.png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="8aba9-111">自訂學習如何運作？</span><span class="sxs-lookup"><span data-stu-id="8aba9-111">How does Custom Learning work?</span></span>

<span data-ttu-id="8aba9-112">學習 Office 365 （的簡短的自訂學習） 的自訂包含三個部分：</span><span class="sxs-lookup"><span data-stu-id="8aba9-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="8aba9-113">即時與 Microsoft online 目錄的內容摘要</span><span class="sxs-lookup"><span data-stu-id="8aba9-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="8aba9-114">SharePoint 通訊網站</span><span class="sxs-lookup"><span data-stu-id="8aba9-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="8aba9-115">SharePoint 網頁組件</span><span class="sxs-lookup"><span data-stu-id="8aba9-115">a SharePoint web part</span></span> 

![cg howitworks.png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="8aba9-117">需求和權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-117">Requirements and Permissions</span></span>

<span data-ttu-id="8aba9-p102">之前開始使用本指南，請確定自訂學習具有已設定的 SharePoint 承租人管理員。如果您不確定是否為已設定，請連絡 SharePoint 租用戶系統管理員確認已安裝自訂學習。也請務必要取得自訂學習 SharePoint 網站的 URL。如果未安裝自訂學習租用戶系統管理員，請參閱自訂學習 Office 365 安裝指南 》。</span><span class="sxs-lookup"><span data-stu-id="8aba9-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="8aba9-122">安裝自訂學習權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="8aba9-123">Office 365 全域管理員</span><span class="sxs-lookup"><span data-stu-id="8aba9-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="8aba9-124">SharePoint 管理員</span><span class="sxs-lookup"><span data-stu-id="8aba9-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="8aba9-125">使用自訂學習管理功能的權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="8aba9-126">Office 365 SharePoint 管理員/SharePoint 網站擁有者權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="8aba9-127">SharePoint 網站集合管理員/SharePoint 網站擁有者權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="8aba9-128">使用自訂學習網站的使用者權限</span><span class="sxs-lookup"><span data-stu-id="8aba9-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="8aba9-129">Office 365 使用者的權限/SharePoint 網站 「 訪客 」 權限或更高</span><span class="sxs-lookup"><span data-stu-id="8aba9-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


