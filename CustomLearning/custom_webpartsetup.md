---
author: pkrebs
ms.author: pkrebs
title: 布建自訂學習網站
ms.date: 02/10/2019
description: 透過 SharePoint 布建引擎提供 Office 365 網站的自訂學習
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233755"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="dd270-103">提供自訂學習</span><span class="sxs-lookup"><span data-stu-id="dd270-103">Provision Custom Learning</span></span>

<span data-ttu-id="dd270-104">使用 SharePoint 線上布建服務，Office 365 租使用者管理員只需稍按一次即可啟動布建程式。</span><span class="sxs-lookup"><span data-stu-id="dd270-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="dd270-105">布建服務是提供自訂學習的建議方式。</span><span class="sxs-lookup"><span data-stu-id="dd270-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="dd270-106">速度很快，而且只需要數分鐘的時間即可開始處理常式。</span><span class="sxs-lookup"><span data-stu-id="dd270-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="dd270-107">在開始布建服務之前，請確定您已符合布建的必要條件。</span><span class="sxs-lookup"><span data-stu-id="dd270-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd270-108">必要條件</span><span class="sxs-lookup"><span data-stu-id="dd270-108">Prerequisites</span></span>
 
<span data-ttu-id="dd270-109">若要使用提供服務 [SharePoint 線上](https://provisioning.sharepointpnp.com)布建服務成功設定自訂教學，進行布建的人員必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="dd270-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="dd270-110">人員布建的自訂學習必須是租使用者 Administratorof 的承租人，將會布建自訂教學。</span><span class="sxs-lookup"><span data-stu-id="dd270-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="dd270-111">租使用者應用程式目錄必須可在 SharePoint 系統管理中心的 [App] 選項內使用。</span><span class="sxs-lookup"><span data-stu-id="dd270-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="dd270-112">如果您的組織沒有 SharePoint 租使用者應用程式目錄，請參閱 [SharePoint 線上檔](https://docs.microsoft.com/sharepoint/use-app-catalog) 以建立一個。</span><span class="sxs-lookup"><span data-stu-id="dd270-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="dd270-113">人員布建的自訂學習必須是租使用者應用程式目錄的網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="dd270-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="dd270-114">如果人員布建自訂學習不是應用程式目錄的網站集合擁有者，請 [完成這些指示](addappadmin.md) 並繼續。</span><span class="sxs-lookup"><span data-stu-id="dd270-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="dd270-115">提供自訂學習</span><span class="sxs-lookup"><span data-stu-id="dd270-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="dd270-116">前往 http://provisioning.sharepointpnp.com 首頁右上角的位置並登 **入** 。</span><span class="sxs-lookup"><span data-stu-id="dd270-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="dd270-117">以您計畫安裝網站範本之目標租使用者的認證登入。</span><span class="sxs-lookup"><span data-stu-id="dd270-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="dd270-119">請清除 **您組織的同意** ，然後選取 [ **接受**]。</span><span class="sxs-lookup"><span data-stu-id="dd270-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

!["](media/inst_perms.png)

3. <span data-ttu-id="dd270-121">從方案庫中選取 **Office 365 的自訂學習** 。</span><span class="sxs-lookup"><span data-stu-id="dd270-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

!["](media/inst_select.png)

4. <span data-ttu-id="dd270-123">從解決方案首頁中，選取 [**新增至您的租使用者**]</span><span class="sxs-lookup"><span data-stu-id="dd270-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="dd270-125">請視安裝需要完成填寫佈建資訊頁面上的欄位。</span><span class="sxs-lookup"><span data-stu-id="dd270-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="dd270-126">您可以至少輸入您要取得其布建程式及網站目的地 URL 相關通知的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="dd270-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="dd270-127">將網站的目的地 URL 做為便於員工（如 "/sites/MyTraining" 或 "/teams/LearnOffice365"）的內容。</span><span class="sxs-lookup"><span data-stu-id="dd270-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="dd270-129">若準備將自訂教學安裝到您的租使用者環境 **，請選取** [布建]。</span><span class="sxs-lookup"><span data-stu-id="dd270-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="dd270-130">佈建程序最多會需要 15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="dd270-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="dd270-131">網站準備好供存取時，系統會透過電子郵件通知您 (傳送到您在 [佈建] 頁面輸入的通知電子郵件地址)。</span><span class="sxs-lookup"><span data-stu-id="dd270-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dd270-132">布建自訂學習網站的承租人管理員必須移至網站，然後開啟 CustomLearningAdmin 以初始化自訂學習管理屬性。</span><span class="sxs-lookup"><span data-stu-id="dd270-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="dd270-133">此時，租使用者管理員也應指派網站的擁有者。</span><span class="sxs-lookup"><span data-stu-id="dd270-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="dd270-134">驗證布建成功</span><span class="sxs-lookup"><span data-stu-id="dd270-134">Validate Provisioning Success</span></span>

<span data-ttu-id="dd270-135">布建完成後，租使用者系統管理員會從 PnP 布建服務接收電子郵件。</span><span class="sxs-lookup"><span data-stu-id="dd270-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="dd270-136">系統管理員可以複製電子郵件中提供之網站的連結，然後依照指示移至網站。</span><span class="sxs-lookup"><span data-stu-id="dd270-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="dd270-137">另外，租使用者管理員可以流覽 <網站集合 URL>/SitePages/CustomLearningAdmin.aspx。</span><span class="sxs-lookup"><span data-stu-id="dd270-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="dd270-138">這會初始化 CustomConfig 清單專案，以設定第一次使用的自訂學習。</span><span class="sxs-lookup"><span data-stu-id="dd270-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="dd270-139">第一次開啟此頁面的人員必須是承租人管理員、網站集合管理員或網站擁有者。</span><span class="sxs-lookup"><span data-stu-id="dd270-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="dd270-140">您應該會看到如下所示的頁面：</span><span class="sxs-lookup"><span data-stu-id="dd270-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="dd270-141">將擁有者新增至網站</span><span class="sxs-lookup"><span data-stu-id="dd270-141">Add Owners to Site</span></span>
<span data-ttu-id="dd270-142">作為租使用者系統管理員，您不太可能是自訂網站的人員，所以您必須指派網站的擁有者。</span><span class="sxs-lookup"><span data-stu-id="dd270-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="dd270-143">擁有者具有網站的管理許可權，可供使用者修改網站頁面及才能重塑網站。</span><span class="sxs-lookup"><span data-stu-id="dd270-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="dd270-144">他們也可以隱藏及顯示透過自訂學習網頁元件傳遞的內容。</span><span class="sxs-lookup"><span data-stu-id="dd270-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="dd270-145">他們也可以建立自訂的播放清單並將其指派給自訂子類別。</span><span class="sxs-lookup"><span data-stu-id="dd270-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="dd270-146">在 [SharePoint **設定** ] 功能表中，按一下 [ **網站許可權**]。</span><span class="sxs-lookup"><span data-stu-id="dd270-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="dd270-147">按一下 [ **高級許可權設定**]。</span><span class="sxs-lookup"><span data-stu-id="dd270-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="dd270-148">按一下 [ **自訂學習的 Office 365 擁有**者]。</span><span class="sxs-lookup"><span data-stu-id="dd270-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="dd270-149">按一下 [**新增**  >  **使用者至此群組**]，新增您要擁有者的人員，然後按一下 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="dd270-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="dd270-150">按一下頁面右上角的 **下列** 選項，以追蹤網站。</span><span class="sxs-lookup"><span data-stu-id="dd270-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="dd270-151">後續步驟</span><span class="sxs-lookup"><span data-stu-id="dd270-151">Next Steps</span></span>
- <span data-ttu-id="dd270-152">探索 webpart 中包含的 [預設內容](sitecontent.md) 。</span><span class="sxs-lookup"><span data-stu-id="dd270-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>
