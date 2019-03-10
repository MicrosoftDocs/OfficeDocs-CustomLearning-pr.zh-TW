---
author: pkrebs
ms.author: pkrebs
title: 佈建自訂學習網站
ms.date: 02/10/2019
description: 佈建 SharePoint 佈建引擎透過 Office 365 網站自訂學習
ms.openlocfilehash: a11975c7df1af9d01e2ca323d41cb5be602a1248
ms.sourcegitcommit: c358dcc2d69cc3db8fd24a1011550edebe0721fe
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2019
ms.locfileid: "30518154"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="0398a-103">佈建自訂學習</span><span class="sxs-lookup"><span data-stu-id="0398a-103">Provision Custom Learning</span></span>

<span data-ttu-id="0398a-104">SharePoint Online 佈建服務時，Office 365 租用戶系統管理員可以啟動簡單按幾下的佈建程序。</span><span class="sxs-lookup"><span data-stu-id="0398a-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="0398a-105">佈建服務是佈建自訂學習建議的方式。</span><span class="sxs-lookup"><span data-stu-id="0398a-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="0398a-106">它是快速又簡單，而且只需幾分鐘開始程序。</span><span class="sxs-lookup"><span data-stu-id="0398a-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="0398a-107">開始之前與佈建服務，但請確定您已符合佈建的必要條件。</span><span class="sxs-lookup"><span data-stu-id="0398a-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0398a-108">必要條件</span><span class="sxs-lookup"><span data-stu-id="0398a-108">Prerequisites</span></span>
 
<span data-ttu-id="0398a-109">若要成功設定自訂學習與[SharePoint Online 佈建服務](https://provisioning.sharepointpnp.com)的佈建服務，執行佈建的人員必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="0398a-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="0398a-110">佈建自訂學習的人員必須是租用戶 Administratorof 租用戶會佈建自訂學習。</span><span class="sxs-lookup"><span data-stu-id="0398a-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="0398a-111">租用戶應用程式目錄必須能夠使用中的 SharePoint 系統管理中心的 [應用程式] 選項。</span><span class="sxs-lookup"><span data-stu-id="0398a-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="0398a-112">如果您的組織沒有 SharePoint 租用戶應用程式目錄，請參閱[SharePoint Online 的文件](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)建立一個。</span><span class="sxs-lookup"><span data-stu-id="0398a-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="0398a-113">佈建自訂學習的人員必須是租用戶應用程式目錄網站集合擁有人。</span><span class="sxs-lookup"><span data-stu-id="0398a-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="0398a-114">如果佈建自訂學習人員不是網站集合擁有人的應用程式目錄[完成這些指示](addappadmin.md)，並繼續執行。</span><span class="sxs-lookup"><span data-stu-id="0398a-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="0398a-115">若要佈建自訂學習</span><span class="sxs-lookup"><span data-stu-id="0398a-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="0398a-116">移至 [ http://provisioning.sharepointpnp.com ，並從 [首頁] 頁面的右上角的 [**登入**。</span><span class="sxs-lookup"><span data-stu-id="0398a-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="0398a-117">使用認證登入您要安裝網站範本已設定目標租用戶。</span><span class="sxs-lookup"><span data-stu-id="0398a-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="0398a-119">清除**同意代表您的組織**，然後選取 [**接受**]。</span><span class="sxs-lookup"><span data-stu-id="0398a-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![在](media/inst_perms.png)

3. <span data-ttu-id="0398a-121">從解決方案庫中選取**自訂學習運作的 Office 365** 。</span><span class="sxs-lookup"><span data-stu-id="0398a-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![在](media/inst_select.png)

4. <span data-ttu-id="0398a-123">從 [解決方案] 首頁上選取 [**新增至您的租用戶**</span><span class="sxs-lookup"><span data-stu-id="0398a-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="0398a-125">完成安裝適當地佈建的 [資訊] 頁面上的欄位。</span><span class="sxs-lookup"><span data-stu-id="0398a-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="0398a-126">在最低限度下輸入想要取得以佈建到網站佈建程序與目的地 URL 的相關通知的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="0398a-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="0398a-127">讓您網站的目的地 URL 至員工，例如 「 / 網站/MyTraining 」 或 「 / teams/LearnOffice365 「 易記的某個項目。</span><span class="sxs-lookup"><span data-stu-id="0398a-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="0398a-129">選取 [**佈建**時安裝自訂學習到您的租用戶環境準備就緒]。</span><span class="sxs-lookup"><span data-stu-id="0398a-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="0398a-130">佈建程序需要 15 分鐘。</span><span class="sxs-lookup"><span data-stu-id="0398a-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="0398a-131">將會透過 （若要在佈建] 頁面所輸入的通知電子郵件地址） 的電子郵件通知您該網站時可供存取。</span><span class="sxs-lookup"><span data-stu-id="0398a-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="0398a-132">租用戶系統管理員佈建自訂學習網站必須移至網站，並再開啟 [CustomLearningAdmin.aspx 初始化自訂學習系統屬性。</span><span class="sxs-lookup"><span data-stu-id="0398a-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="0398a-133">現階段，租用戶系統管理員也應該將指派擁有者至網站。</span><span class="sxs-lookup"><span data-stu-id="0398a-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="0398a-134">驗證佈建成功</span><span class="sxs-lookup"><span data-stu-id="0398a-134">Validate Provisioning Success</span></span>

<span data-ttu-id="0398a-135">佈建完成時，租用戶系統管理員會收到一封電子郵件從 PnP 佈建服務。</span><span class="sxs-lookup"><span data-stu-id="0398a-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="0398a-136">系統管理員可以將連結複製到提供的電子郵件中的網站，然後依照 [移至網站的指示。</span><span class="sxs-lookup"><span data-stu-id="0398a-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="0398a-137">或者，租用戶系統管理員可以瀏覽至 [<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx。</span><span class="sxs-lookup"><span data-stu-id="0398a-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="0398a-138">這會初始化為其第一次使用設定自訂學習 CustomConfig 清單項目。</span><span class="sxs-lookup"><span data-stu-id="0398a-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="0398a-139">第一次開啟此頁面上的人員必須是租用戶系統管理員、 網站集合管理員或網站擁有者。</span><span class="sxs-lookup"><span data-stu-id="0398a-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="0398a-140">您應該會看到看起來像這樣的頁面：</span><span class="sxs-lookup"><span data-stu-id="0398a-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="0398a-141">將擁有者新增至網站</span><span class="sxs-lookup"><span data-stu-id="0398a-141">Add Owners to Site</span></span>
<span data-ttu-id="0398a-142">租用戶系統管理員，也不太可能您要自訂網站，讓您將需要指派至網站的擁有者的人。</span><span class="sxs-lookup"><span data-stu-id="0398a-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="0398a-143">讓他們可以修改網站頁面並 rebrand 網站擁有人在網站上擁有系統管理權限。</span><span class="sxs-lookup"><span data-stu-id="0398a-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="0398a-144">他們也能夠隱藏和顯示內容傳遞到自訂學習網頁組件。</span><span class="sxs-lookup"><span data-stu-id="0398a-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="0398a-145">他們也必須建立自訂播放清單，並將它們指派給自訂的子類別的能力。</span><span class="sxs-lookup"><span data-stu-id="0398a-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="0398a-146">從 SharePoint**設定**] 功能表中，按一下 [**網站權限**]。</span><span class="sxs-lookup"><span data-stu-id="0398a-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="0398a-147">按一下 [**進階權限設定**。</span><span class="sxs-lookup"><span data-stu-id="0398a-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="0398a-148">按一下 [**自訂學習 for Office 365 擁有者**。</span><span class="sxs-lookup"><span data-stu-id="0398a-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="0398a-149">按一下 [**新增** > **將使用者新增到這個群組**，新增您想要擁有者的人員，然後按一下 [**共用**。</span><span class="sxs-lookup"><span data-stu-id="0398a-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="0398a-150">按一下**下列**選項中的右上角的頁面追蹤網站。</span><span class="sxs-lookup"><span data-stu-id="0398a-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="0398a-151">後續步驟</span><span class="sxs-lookup"><span data-stu-id="0398a-151">Next Steps</span></span>
- <span data-ttu-id="0398a-152">瀏覽網頁組件中包含[預設的內容](sitecontent.md)。</span><span class="sxs-lookup"><span data-stu-id="0398a-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>
