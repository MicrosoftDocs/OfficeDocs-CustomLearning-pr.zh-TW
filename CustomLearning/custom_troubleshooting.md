---
author: pkrebs
ms.author: pkrebs
title: 學習路徑的 Microsoft 365 的疑難排解
ms.date: 02/10/2019
description: 了解如何疑難排解 Microsoft 365 學習路徑
ms.openlocfilehash: de46b9c754dac36de230b36ec4a5542518a1dcd5
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247678"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="b4a52-103">學習路徑的 Microsoft 365 的疑難排解</span><span class="sxs-lookup"><span data-stu-id="b4a52-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="b4a52-104">在這裡進行疑難排解時使用 Microsoft 365 學習路徑或 SharePoint Online 佈建服務可能發生的問題的秘訣。</span><span class="sxs-lookup"><span data-stu-id="b4a52-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="b4a52-105">如何知道您是否擁有租用戶系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="b4a52-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="b4a52-106">登入 SharePoint Online 佈建服務和佈建自訂學習需要租用戶系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="b4a52-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="b4a52-107">如果您急需登入 SharePoint Online 佈建服務的問題，請確定您已獲指派全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="b4a52-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="b4a52-108">自訂學習解決方案需要租用戶系統管理員權限，又稱為 Office 365 全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="b4a52-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="b4a52-109">以下是如何判斷是否您已獲指派全域系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="b4a52-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="b4a52-110">登入 Office.com。</span><span class="sxs-lookup"><span data-stu-id="b4a52-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="b4a52-111">按一下 [**系統管理**</span><span class="sxs-lookup"><span data-stu-id="b4a52-111">Click **Admin**</span></span>
3.  <span data-ttu-id="b4a52-112">[**使用者**] 下方選取 [**作用中使用者**</span><span class="sxs-lookup"><span data-stu-id="b4a52-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="b4a52-113">搜尋您的名稱</span><span class="sxs-lookup"><span data-stu-id="b4a52-113">Search for your name</span></span>
5.  <span data-ttu-id="b4a52-114">按一下您在搜尋結果中的名稱。</span><span class="sxs-lookup"><span data-stu-id="b4a52-114">Click your name in Search results.</span></span> <span data-ttu-id="b4a52-115">全域系統管理員應該會看到您的角色。</span><span class="sxs-lookup"><span data-stu-id="b4a52-115">You should see Global administrator for your role.</span></span>

![cg globaladminrole.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="b4a52-117">如果您沒有全域系統管理員角色</span><span class="sxs-lookup"><span data-stu-id="b4a52-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="b4a52-118">尋找組織中的全域系統管理員和擁有該登入服務，或已將其指派給您的全域系統管理員角色的人員。</span><span class="sxs-lookup"><span data-stu-id="b4a52-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="b4a52-119">疑難排解的租用戶應用程式目錄</span><span class="sxs-lookup"><span data-stu-id="b4a52-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="b4a52-120">自訂學習需要應用程式目錄]，以目標租用戶中佈建。</span><span class="sxs-lookup"><span data-stu-id="b4a52-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="b4a52-121">建立的應用程式目錄需要全域系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="b4a52-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="b4a52-122">以下是為一般應用程式目錄問題進行疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="b4a52-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="b4a52-123">如何知道您是否擁有租用戶應用程式目錄</span><span class="sxs-lookup"><span data-stu-id="b4a52-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="b4a52-124">首先，請確定您具備全域系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="b4a52-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="b4a52-125">請參閱上述的租用戶系統管理員權限的步驟。</span><span class="sxs-lookup"><span data-stu-id="b4a52-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="b4a52-126">從 Office 365 中，按一下 [**系統管理員**，請按一下展開箭頭 >，按一下 [**顯示所有** > **系統管理中心** > **SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="b4a52-127">按一下 [**傳統系統 SharePoint 管理中心** > **apps** > **應用程式目錄**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="b4a52-128">在**應用程式**，您應該會看到標題為**Distribute SharePoint 相關應用程式**的磚。</span><span class="sxs-lookup"><span data-stu-id="b4a52-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="b4a52-129">如果您看到磚，您必須租用戶應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="b4a52-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="b4a52-130">請參閱以下 [**如何確定您是網站 Colllection...** ] 區段。</span><span class="sxs-lookup"><span data-stu-id="b4a52-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="b4a52-131">如果您沒有看到 [您需要建立您的租用戶的租用戶應用程式目錄] 磚。</span><span class="sxs-lookup"><span data-stu-id="b4a52-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="b4a52-132">請參閱 <<c0>如何建立租用戶應用程式目錄] 區段下方。</span><span class="sxs-lookup"><span data-stu-id="b4a52-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="b4a52-133">如何確保您的租用戶應用程式目錄網站集合擁有人</span><span class="sxs-lookup"><span data-stu-id="b4a52-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="b4a52-134">若要佈建學習路徑的 Microsoft 365，您必須是租用戶應用程式目錄網站集合擁有人。</span><span class="sxs-lookup"><span data-stu-id="b4a52-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="b4a52-135">以下是如何判斷您是否擁有者。</span><span class="sxs-lookup"><span data-stu-id="b4a52-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="b4a52-136">從 Office 365 中，按一下 [**系統管理員**，請按一下展開箭頭 >，按一下 [**顯示所有** > **系統管理中心** > **SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="b4a52-137">按一下 [**傳統系統 SharePoint 管理中心**]，然後選取 [**應用程式目錄**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="b4a52-138">選取**擁有者**，並請確定您是網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="b4a52-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="b4a52-139">它看起來應該像這樣。</span><span class="sxs-lookup"><span data-stu-id="b4a52-139">It should look something like this.</span></span>
 
![cg sitecollectionowner.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="b4a52-141">如何建立租用戶應用程式目錄，如果其中一個不存在</span><span class="sxs-lookup"><span data-stu-id="b4a52-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="b4a52-142">使用您的 SharePoint Online 系統管理員帳戶登入 Office 365。</span><span class="sxs-lookup"><span data-stu-id="b4a52-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="b4a52-143">按一下 [**系統**]。</span><span class="sxs-lookup"><span data-stu-id="b4a52-143">Click **Admin**.</span></span>
3. <span data-ttu-id="b4a52-144">在**系統管理中心**中，按一下 [ **SharePoint**]。</span><span class="sxs-lookup"><span data-stu-id="b4a52-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="b4a52-145">按一下 [**應用程式** > **應用程式目錄**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="b4a52-146">按一下 [**建立新的應用程式目錄網站**]，然後按一下 [**確定]**。</span><span class="sxs-lookup"><span data-stu-id="b4a52-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="b4a52-147">輸入應用程式目錄的資訊。</span><span class="sxs-lookup"><span data-stu-id="b4a52-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="b4a52-148">您可能想要包含一個以上的系統管理員。</span><span class="sxs-lookup"><span data-stu-id="b4a52-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="b4a52-149">下列範例會示範。</span><span class="sxs-lookup"><span data-stu-id="b4a52-149">The following shows an example.</span></span>  

![cg appcatalogfinish.png](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="b4a52-151">這樣就完成了。</span><span class="sxs-lookup"><span data-stu-id="b4a52-151">That’s it.</span></span> <span data-ttu-id="b4a52-152">您已經完成。</span><span class="sxs-lookup"><span data-stu-id="b4a52-152">You’re done.</span></span> <span data-ttu-id="b4a52-153">但是，您將移至佈建自訂學習之前，您需要等候至少 30 分鐘，以確定應用程式目錄建立完畢。</span><span class="sxs-lookup"><span data-stu-id="b4a52-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="b4a52-154">請等候至少 30 分鐘後再佈建自訂學習建立租用戶應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="b4a52-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="b4a52-155">這可確保佈建程序的應用程式目錄是 SharePoint 內完成。</span><span class="sxs-lookup"><span data-stu-id="b4a52-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 