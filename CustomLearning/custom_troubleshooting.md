---
author: pkrebs
ms.author: pkrebs
title: 疑難排解 Microsoft 365 學習路徑
ms.date: 02/10/2019
description: 深入瞭解如何疑難排解 Microsoft 365 教學路徑
ms.service: sharepoint online
ms.openlocfilehash: 8d8b418c7a4b2c025391eb4527af86b02738c532
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233865"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="a7745-103">疑難排解 Microsoft 365 教學路徑</span><span class="sxs-lookup"><span data-stu-id="a7745-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="a7745-104">以下是 Microsoft 365 教學路徑或 SharePoint 線上布建服務可能發生之問題的疑難排解提示。</span><span class="sxs-lookup"><span data-stu-id="a7745-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="a7745-105">如何知道您是否有承租人系統管理員許可權</span><span class="sxs-lookup"><span data-stu-id="a7745-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="a7745-106">登入 SharePoint 線上布建服務，以及布建自訂學習要求承租人系統管理員許可權。</span><span class="sxs-lookup"><span data-stu-id="a7745-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="a7745-107">如果您遇到 SharePoint 線上布建服務的登入問題，請確定您已被指派全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="a7745-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="a7745-108">自訂學習解決方案需要租使用者系統管理員許可權，否則稱為 Office 365 全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="a7745-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="a7745-109">以下是判斷您是否已被指派全域系統管理員角色的方法。</span><span class="sxs-lookup"><span data-stu-id="a7745-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="a7745-110">登入 Office.com。</span><span class="sxs-lookup"><span data-stu-id="a7745-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="a7745-111">按一下 [**管理**]</span><span class="sxs-lookup"><span data-stu-id="a7745-111">Click **Admin**</span></span>
3.  <span data-ttu-id="a7745-112">在 [**使用者**] 底下，選取 [作用中**使用者**]</span><span class="sxs-lookup"><span data-stu-id="a7745-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="a7745-113">搜尋您的名稱</span><span class="sxs-lookup"><span data-stu-id="a7745-113">Search for your name</span></span>
5.  <span data-ttu-id="a7745-114">按一下搜尋結果中的名稱。</span><span class="sxs-lookup"><span data-stu-id="a7745-114">Click your name in Search results.</span></span> <span data-ttu-id="a7745-115">您應該會看到全域管理員的角色。</span><span class="sxs-lookup"><span data-stu-id="a7745-115">You should see Global administrator for your role.</span></span>

![cg-globaladminrole.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="a7745-117">如果您沒有全域系統管理員角色</span><span class="sxs-lookup"><span data-stu-id="a7745-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="a7745-118">尋找組織中的全域系統管理員，讓該人員登入服務，或讓他們為您指派全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="a7745-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="a7745-119">租使用者應用程式目錄疑難排解</span><span class="sxs-lookup"><span data-stu-id="a7745-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="a7745-120">自訂學習需要在目標租使用者中布建應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="a7745-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="a7745-121">建立應用程式目錄需要全域管理員許可權。</span><span class="sxs-lookup"><span data-stu-id="a7745-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="a7745-122">以下是常見應用程式目錄問題的疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="a7745-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="a7745-123">如何知道您是否有租使用者應用程式目錄</span><span class="sxs-lookup"><span data-stu-id="a7745-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="a7745-124">針對初學者，請確定您具有全域管理員許可權。</span><span class="sxs-lookup"><span data-stu-id="a7745-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="a7745-125">請參閱上述租使用者管理員許可權的步驟。</span><span class="sxs-lookup"><span data-stu-id="a7745-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="a7745-126">從 Office 365，按一下 [**管理**]，按一下展開箭號 >，然後按一下 [**顯示所有**系統  >  **管理中心**]  >  **SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="a7745-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="a7745-127">按一下 [**傳統系統管理員 SharePoint 中心**  >  **應用**  >  **程式] 應用程式目錄**。</span><span class="sxs-lookup"><span data-stu-id="a7745-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="a7745-128">在 [ **應用程式**] 底下，您應該會看到一個貼上標題為「 **散佈應用程式 SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="a7745-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="a7745-129">如果您看到的是磚，表示您有租使用者應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="a7745-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="a7745-130">請參閱 how **to 確定您的網站 Colllection ...** ] 區段。</span><span class="sxs-lookup"><span data-stu-id="a7745-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="a7745-131">如果您看不到所需的磚，您將需要為您的租使用者建立承租人應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="a7745-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="a7745-132">請參閱 **如何建立租使用者應用程式目錄** 一節。</span><span class="sxs-lookup"><span data-stu-id="a7745-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="a7745-133">如何確保您是租使用者應用程式目錄上的網站集合擁有者</span><span class="sxs-lookup"><span data-stu-id="a7745-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="a7745-134">若要布建 Microsoft 365 學習路徑，您必須是租使用者應用程式目錄上的網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="a7745-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="a7745-135">以下是判斷您是否為擁有者的方式。</span><span class="sxs-lookup"><span data-stu-id="a7745-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="a7745-136">從 Office 365，按一下 [**管理**]，按一下展開箭號 >，然後按一下 [**顯示所有**系統  >  **管理中心**]  >  **SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="a7745-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="a7745-137">按一下 [ **傳統 Admin SharePoint Center**]，然後選取 **應用程式目錄**。</span><span class="sxs-lookup"><span data-stu-id="a7745-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="a7745-138">選取 [ **擁有**者]，然後確定您是網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="a7745-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="a7745-139">它看起來應該像這樣。</span><span class="sxs-lookup"><span data-stu-id="a7745-139">It should look something like this.</span></span>
 
![cg-sitecollectionowner.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="a7745-141">如何建立租使用者應用程式目錄（若有的話）</span><span class="sxs-lookup"><span data-stu-id="a7745-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="a7745-142">使用您的 SharePoint 線上系統管理員帳戶登入 Office 365。</span><span class="sxs-lookup"><span data-stu-id="a7745-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="a7745-143">按一下 [ **管理**]。</span><span class="sxs-lookup"><span data-stu-id="a7745-143">Click **Admin**.</span></span>
3. <span data-ttu-id="a7745-144">在 [系統 **管理中心**] 底下，按一下 [ **SharePoint**]。</span><span class="sxs-lookup"><span data-stu-id="a7745-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="a7745-145">按一下 [**應用**  >  **程式應用程式目錄**]。</span><span class="sxs-lookup"><span data-stu-id="a7745-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="a7745-146">按一下 [ **建立新的應用程式目錄網站**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="a7745-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="a7745-147">輸入應用程式目錄的資訊。</span><span class="sxs-lookup"><span data-stu-id="a7745-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="a7745-148">您可能想要包含一個以上的系統管理員。</span><span class="sxs-lookup"><span data-stu-id="a7745-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="a7745-149">下列範例所示。</span><span class="sxs-lookup"><span data-stu-id="a7745-149">The following shows an example.</span></span>  

![cg-appcatalogfinish.png](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="a7745-151">這樣就完成了。</span><span class="sxs-lookup"><span data-stu-id="a7745-151">That’s it.</span></span> <span data-ttu-id="a7745-152">您已經完成。</span><span class="sxs-lookup"><span data-stu-id="a7745-152">You’re done.</span></span> <span data-ttu-id="a7745-153">但在您進入自訂教學之前，您至少需要等候30分鐘，確定應用程式目錄建立已完成。</span><span class="sxs-lookup"><span data-stu-id="a7745-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="a7745-154">在建立承租人應用程式目錄之後，請至少等候30分鐘，再提供自訂學習。</span><span class="sxs-lookup"><span data-stu-id="a7745-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="a7745-155">這可確保應用程式目錄布建程式在 SharePoint 內完成。</span><span class="sxs-lookup"><span data-stu-id="a7745-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 