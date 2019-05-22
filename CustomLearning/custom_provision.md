---
author: pkrebs
ms.author: pkrebs
title: 佈建 Microsoft 365 學習路徑網站
ms.date: 02/10/2019
description: 佈建學習路徑網站 SharePoint 佈建服務透過 Microsoft 365
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334739"
---
# <a name="provision-microsoft-365-learning-pathways"></a><span data-ttu-id="1e52e-103">佈建 Microsoft 365 學習路徑</span><span class="sxs-lookup"><span data-stu-id="1e52e-103">Provision Microsoft 365 learning pathways</span></span>

<span data-ttu-id="1e52e-104">SharePoint Online 佈建服務時，Office 365 租用戶系統管理員可以啟動簡單按幾下的佈建程序。</span><span class="sxs-lookup"><span data-stu-id="1e52e-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="1e52e-105">佈建服務是佈建學習路徑的建議的方法。</span><span class="sxs-lookup"><span data-stu-id="1e52e-105">The Provisioning Service is the recommended way to provision learning pathways.</span></span> <span data-ttu-id="1e52e-106">它是快速又簡單，而且只需幾分鐘開始程序。</span><span class="sxs-lookup"><span data-stu-id="1e52e-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="1e52e-107">開始之前與佈建服務，但請確定您已符合佈建的必要條件。</span><span class="sxs-lookup"><span data-stu-id="1e52e-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1e52e-108">截至 5/21/2019，Microsoft 365 學習路徑是以前稱為自訂了解 Office 365 方案的新名稱。</span><span class="sxs-lookup"><span data-stu-id="1e52e-108">As of 5/21/2019, Microsoft 365 learning pathways is the new name for the solution formerly known as Custom Learning for Office 365.</span></span> <span data-ttu-id="1e52e-109">如果您有已佈建自訂了解 Office 365 組織中，而且想要更新的解決方案，請遵循 「 更新方案 」 中的指示， [Microsoft 365 學習路徑讀我檔案](https://github.com/pnp/custom-learning-office-365)。</span><span class="sxs-lookup"><span data-stu-id="1e52e-109">If you have already provisioned Custom Learning for Office 365 in your organization and want to update the solution, follow the “Updating the solution” instructions in the [Microsoft 365 learning pathways ReadMe](https://github.com/pnp/custom-learning-office-365).</span></span> <span data-ttu-id="1e52e-110">如果您在提供 Microsoft 365 學習路徑第一次，請參閱 Microsoft 365 學習路徑文件中的 [[佈建 Microsoft 365 學習路徑指示]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision)。</span><span class="sxs-lookup"><span data-stu-id="1e52e-110">If you are provisioning Microsoft 365 learning pathways for the first time, see [Provision Microsoft 365 learning pathways instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) in the Microsoft 365 learning pathways documentation.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="1e52e-111">必要條件</span><span class="sxs-lookup"><span data-stu-id="1e52e-111">Prerequisites</span></span>
 
<span data-ttu-id="1e52e-112">若要成功設定 Microsoft 365 學習路徑佈建服務時，人員佈建必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="1e52e-112">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="1e52e-113">佈建學習路徑的人員必須是租用戶的租用戶系統管理員，其中學習路徑佈建。</span><span class="sxs-lookup"><span data-stu-id="1e52e-113">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="1e52e-114">租用戶應用程式目錄必須能夠使用中的 SharePoint 系統管理中心的 [應用程式] 選項。</span><span class="sxs-lookup"><span data-stu-id="1e52e-114">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="1e52e-115">如果您的組織沒有 SharePoint 租用戶應用程式目錄，請參閱[SharePoint Online 的文件](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)建立一個。</span><span class="sxs-lookup"><span data-stu-id="1e52e-115">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="1e52e-116">佈建學習路徑的人員必須是租用戶應用程式目錄網站集合擁有人。</span><span class="sxs-lookup"><span data-stu-id="1e52e-116">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="1e52e-117">如果佈建學習路徑的人員不是網站集合擁有人的應用程式目錄[完成這些指示](addappadmin.md)，並繼續。</span><span class="sxs-lookup"><span data-stu-id="1e52e-117">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="1e52e-118">若要佈建學習路徑</span><span class="sxs-lookup"><span data-stu-id="1e52e-118">To provision learning pathways</span></span>

1. <span data-ttu-id="1e52e-119">移至 [ http://provisioning.sharepointpnp.com ，並從 [首頁] 頁面的右上角的 [**登入**。</span><span class="sxs-lookup"><span data-stu-id="1e52e-119">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="1e52e-120">使用認證登入您要安裝網站範本已設定目標租用戶。</span><span class="sxs-lookup"><span data-stu-id="1e52e-120">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="1e52e-122">清除**同意代表您的組織**，然後選取 [**接受**]。</span><span class="sxs-lookup"><span data-stu-id="1e52e-122">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![在](media/inst_perms.png)

<span data-ttu-id="1e52e-124">佈建服務需要這些權限，以建立租用戶應用程式目錄、 安裝應用程式至租用戶應用程式目錄及佈建網站範本。</span><span class="sxs-lookup"><span data-stu-id="1e52e-124">The provisioning service requires these permissions to create the tenant app catalog, install the application into the tenant app catalog and provision the site template.</span></span> <span data-ttu-id="1e52e-125">在您的租用戶上沒有沒有整體影響，而且目的方案安裝明確使用這些權限。</span><span class="sxs-lookup"><span data-stu-id="1e52e-125">There is no overall impact on your tenant and these permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="1e52e-126">您必須接受繼續進行安裝這些權限。</span><span class="sxs-lookup"><span data-stu-id="1e52e-126">You must accept these permissions to proceed with the installation.</span></span>

3. <span data-ttu-id="1e52e-127">捲動 [] 頁面上，選取 [**解決方案**] 索引標籤，然後選取 [**學習運作的 Office 365 的路徑**。</span><span class="sxs-lookup"><span data-stu-id="1e52e-127">Scroll down the page, select the **Solutions** tab, and then select **learning pathways for Office 365**.</span></span> 

![在](media/inst_select.png)

4. <span data-ttu-id="1e52e-129">選取 [**新增至您的租用戶**</span><span class="sxs-lookup"><span data-stu-id="1e52e-129">Select **Add to your tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="1e52e-131">完成安裝適當地佈建的 [資訊] 頁面上的欄位。</span><span class="sxs-lookup"><span data-stu-id="1e52e-131">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="1e52e-132">在最低限度下輸入想要取得以佈建到網站佈建程序與目的地 URL 的相關通知的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="1e52e-132">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="1e52e-133">讓您網站的目的地 URL 至員工，例如 「 / 網站/MyTraining 」 或 「 / teams/LearnMicrosoft365 「 易記的某個項目。</span><span class="sxs-lookup"><span data-stu-id="1e52e-133">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="1e52e-135">選取 [**佈建**時安裝學習路徑至租用戶環境準備就緒]。</span><span class="sxs-lookup"><span data-stu-id="1e52e-135">Select **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="1e52e-136">佈建程序需要 15 分鐘。</span><span class="sxs-lookup"><span data-stu-id="1e52e-136">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="1e52e-137">將會透過 （若要在佈建] 頁面所輸入的通知電子郵件地址） 的電子郵件通知您該網站時可供存取。</span><span class="sxs-lookup"><span data-stu-id="1e52e-137">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="1e52e-138">租用戶系統管理員佈建的學習路徑網站必須移至網站，然後開啟 [ **CustomLearningAdmin.aspx**初始化學習路徑系統屬性。</span><span class="sxs-lookup"><span data-stu-id="1e52e-138">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="1e52e-139">現階段，租用戶系統管理員也應該將指派擁有者至網站。</span><span class="sxs-lookup"><span data-stu-id="1e52e-139">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="1e52e-140">驗證成功佈建並初始化 CustomConfig 清單</span><span class="sxs-lookup"><span data-stu-id="1e52e-140">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="1e52e-141">佈建完成時，租用戶系統管理員佈建網站上，會收到一封電子郵件從 PnP 佈建服務。</span><span class="sxs-lookup"><span data-stu-id="1e52e-141">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="1e52e-142">電子郵件包含網站的連結。</span><span class="sxs-lookup"><span data-stu-id="1e52e-142">The email contains a link to the site.</span></span> <span data-ttu-id="1e52e-143">此時，租用戶系統管理員應移至使用中電子郵件提供和設定用於第一次使用網站的連結的網站：</span><span class="sxs-lookup"><span data-stu-id="1e52e-143">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="1e52e-144">請移至 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="1e52e-144">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="1e52e-145">開啟**CustomLearningAdmin.aspx**初始化設定學習路徑的第一次使用**CustomConfig**清單項目。</span><span class="sxs-lookup"><span data-stu-id="1e52e-145">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="1e52e-146">您應該會看到看起來像這樣的頁面：</span><span class="sxs-lookup"><span data-stu-id="1e52e-146">You should see a page that looks like this:</span></span>

![cg adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="1e52e-148">將擁有者新增至網站</span><span class="sxs-lookup"><span data-stu-id="1e52e-148">Add Owners to Site</span></span>
<span data-ttu-id="1e52e-149">租用戶系統管理員，也不太可能您要自訂網站，讓您將需要指派至網站的幾個擁有者的人。</span><span class="sxs-lookup"><span data-stu-id="1e52e-149">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="1e52e-150">讓他們可以修改網站頁面並 rebrand 網站擁有人在網站上擁有系統管理權限。</span><span class="sxs-lookup"><span data-stu-id="1e52e-150">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="1e52e-151">他們也能夠隱藏和顯示內容透過學習路徑來傳遞網頁組件。</span><span class="sxs-lookup"><span data-stu-id="1e52e-151">They also have the ability to hide and show content delivered through the learning pathways Web part.</span></span> <span data-ttu-id="1e52e-152">此外，他們必須能夠建置自訂播放清單，並將它們指派給自訂的子類別。</span><span class="sxs-lookup"><span data-stu-id="1e52e-152">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="1e52e-153">從 SharePoint**設定**] 功能表中，按一下 [**網站權限**]。</span><span class="sxs-lookup"><span data-stu-id="1e52e-153">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="1e52e-154">按一下 [**進階權限設定**。</span><span class="sxs-lookup"><span data-stu-id="1e52e-154">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="1e52e-155">按一下 [ **Microsoft 365 學習路徑擁有者**。</span><span class="sxs-lookup"><span data-stu-id="1e52e-155">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="1e52e-156">按一下 [**新增** > **將使用者新增到這個群組**，然後新增您想要做為擁有者的人員。</span><span class="sxs-lookup"><span data-stu-id="1e52e-156">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="1e52e-157">在共用郵件中，將連結新增至[瀏覽網站](custom_exploresite.md)，然後按一下 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="1e52e-157">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="1e52e-158">後續步驟</span><span class="sxs-lookup"><span data-stu-id="1e52e-158">Next Steps</span></span>
- <span data-ttu-id="1e52e-159">瀏覽網站和網頁組件中所提供的[預設的內容](custom_exploresite.md)。</span><span class="sxs-lookup"><span data-stu-id="1e52e-159">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
