---
author: pkrebs
ms.author: pkrebs
title: 布建新的教學路徑多語系網站
ms.date: 02/10/2019
description: 透過 SharePoint 布建服務布建 Microsoft 365 學習路徑網站
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: ca565a113056a915cfc780568ca36777bbf8f5bb
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699025"
---
# <a name="provision-a-new-learning-pathways-multilingual-site"></a><span data-ttu-id="ac829-103">布建新的教學路徑多語系網站</span><span class="sxs-lookup"><span data-stu-id="ac829-103">Provision a new learning pathways multilingual site</span></span>
<span data-ttu-id="ac829-104">未在其承租人中布建學習路徑的組織，可將多語系學習路徑方案新增至其租使用者。</span><span class="sxs-lookup"><span data-stu-id="ac829-104">Organizations that that don’t have learning pathways already provisioned in their tenant can add the multilingual learning pathways solution to their tenant.</span></span> <span data-ttu-id="ac829-105">使用此選項，「教學」路徑 SharePoint 範本會轉譯成九種語言，且最少可用於修改。</span><span class="sxs-lookup"><span data-stu-id="ac829-105">With this option, the learning pathways SharePoint template is translated into nine languages and can be used with a minimum of modification.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ac829-106">如果您已在租使用者中布建學習路徑，建議您遵循學習路徑的[更新路徑](custom_update_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="ac829-106">If you already have learning pathways provisioned in your tenant, it's recommended that you follow the [update path](custom_update_ml.md) for learning pathways.</span></span> <span data-ttu-id="ac829-107">如果您在租使用者中的現有實例上安裝學習路徑，則對「學習路徑」網站範本或播放清單所做的任何變更，都可能會遺失。</span><span class="sxs-lookup"><span data-stu-id="ac829-107">If you install learning pathways over an existing instance in your tenant, any changes made to the the learning pathways site template or playlists may be lost.</span></span>

## <a name="prerequisites-for-multilingual-support"></a><span data-ttu-id="ac829-108">多語系支援的必要條件</span><span class="sxs-lookup"><span data-stu-id="ac829-108">Prerequisites for multilingual support</span></span>
 
<span data-ttu-id="ac829-109">若要成功設定與布建服務的 Microsoft 365 教學路徑，進行布建的人員必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="ac829-109">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="ac829-110">提供教學路徑的人員必須是安裝教學路徑的承租人租使用者管理員。</span><span class="sxs-lookup"><span data-stu-id="ac829-110">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="ac829-111">租使用者應用程式目錄必須可在 SharePoint 系統管理中心的 [App] 選項內使用。</span><span class="sxs-lookup"><span data-stu-id="ac829-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="ac829-112">如果您的組織沒有 SharePoint 租使用者應用程式目錄，請參閱[SharePoint 線上檔](https://docs.microsoft.com/sharepoint/use-app-catalog)以建立一個。</span><span class="sxs-lookup"><span data-stu-id="ac829-112">If your organization doesn't have an SharePoint tenant App Catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/sharepoint/use-app-catalog) to create one.</span></span> <span data-ttu-id="ac829-113">在建立應用程式目錄之前，您必須至少等候兩小時之後，再提供學習路徑。</span><span class="sxs-lookup"><span data-stu-id="ac829-113">You must wait at least two hours after creating the App Catalog before provisioning learning pathways.</span></span>  
- <span data-ttu-id="ac829-114">提供教學路徑的人員必須是租使用者應用程式目錄的網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="ac829-114">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="ac829-115">如果人員提供的學習路徑不是應用程式目錄的網站集合擁有者，請[完成這些指示](addappadmin.md)並繼續。</span><span class="sxs-lookup"><span data-stu-id="ac829-115">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a><span data-ttu-id="ac829-116">確定租使用者管理員帳戶未選取語言</span><span class="sxs-lookup"><span data-stu-id="ac829-116">Ensure the Tenant Admin account doesn't have a language selected</span></span>
<span data-ttu-id="ac829-117">在您布建學習路徑之前，請確定租使用者的系統管理員帳戶未選取語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-117">Before you provision learning pathways, ensure that the Admin Account for the tenant doesn't have a language selected.</span></span> <span data-ttu-id="ac829-118">以下說明如何確認系統管理員帳戶未選取語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-118">Here’s how to verify if the Admin account doesn't have a language selected.</span></span> 
1.  <span data-ttu-id="ac829-119">使用 Edge 系統管理設定檔，移至 office.com。</span><span class="sxs-lookup"><span data-stu-id="ac829-119">With your Edge Admin profile, go to office.com.</span></span>
2.  <span data-ttu-id="ac829-120">輸入使用者認證（如有必要）。</span><span class="sxs-lookup"><span data-stu-id="ac829-120">Enter the user credentials (if necessary).</span></span>
3.  <span data-ttu-id="ac829-121">在 Microsoft 365 中，按一下 [**所有應用程式**] > Delve。</span><span class="sxs-lookup"><span data-stu-id="ac829-121">In Microsoft 365, click **All Apps** > Delve.</span></span> 
4.  <span data-ttu-id="ac829-122">按一下 [**我**  >  的**更新設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-122">Click **Me** > **Update Profile**.</span></span>
5.  <span data-ttu-id="ac829-123">向中向左下向下方，按一下 [**如何變更語言和地區設定**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-123">Scroll down the page and click **How can I change language and regional settings**.</span></span>
6.  <span data-ttu-id="ac829-124">按一下 [**這裡**]，然後按一下省略號 **...**。</span><span class="sxs-lookup"><span data-stu-id="ac829-124">Click **here**, and then click the ellipses **...**.</span></span>
7.  <span data-ttu-id="ac829-125">在 [**我的顯示語言**] 底下，您應該會看到**沒有選取語言**。</span><span class="sxs-lookup"><span data-stu-id="ac829-125">Under **My Display Languages**, you should see **No languages selected**.</span></span> <span data-ttu-id="ac829-126">如果已選取語言，請將其取消選取。</span><span class="sxs-lookup"><span data-stu-id="ac829-126">If a language is selected, unselect it.</span></span>

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="ac829-127">提供學習路徑</span><span class="sxs-lookup"><span data-stu-id="ac829-127">To provision learning pathways</span></span>

1. <span data-ttu-id="ac829-128">移至[Microsoft 365 學習路徑方案頁面](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239)。</span><span class="sxs-lookup"><span data-stu-id="ac829-128">Go to the [Microsoft 365 learning pathways solution page](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).</span></span>
2. <span data-ttu-id="ac829-129">按一下 [**新增至您的租使用者**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-129">Click **Add to your tenant**.</span></span> <span data-ttu-id="ac829-130">如果您未登入到您的租使用者，提供服務會要求您提供租使用者系統管理員認證。</span><span class="sxs-lookup"><span data-stu-id="ac829-130">If you aren't signed into to your tenant, the Provisioning Service will ask for your Tenant Admin credentials.</span></span> 
3. <span data-ttu-id="ac829-131">在 [要求的許可權] 對話方塊中，選取 [**代表您的組織同意**]，然後選取 [**接受**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-131">From the Permissions requested dialog box, select **Consent on behalf of your organization** and then select **Accept**.</span></span>

<span data-ttu-id="ac829-132">布建服務需要這些許可權才能建立租使用者應用程式目錄、將應用程式安裝至租使用者應用程式目錄，以及布建網站範本。</span><span class="sxs-lookup"><span data-stu-id="ac829-132">The provisioning service requires these permissions to create the tenant App Catalog, install the application into the tenant App Catalog and provision the site template.</span></span> <span data-ttu-id="ac829-133">您的租使用者沒有整體影響。</span><span class="sxs-lookup"><span data-stu-id="ac829-133">There's no overall impact on your tenant.</span></span> <span data-ttu-id="ac829-134">這些許可權會明確用於解決方案安裝的目的。</span><span class="sxs-lookup"><span data-stu-id="ac829-134">These permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="ac829-135">您必須接受這些許可權，才能繼續安裝。</span><span class="sxs-lookup"><span data-stu-id="ac829-135">You must accept these permissions to continue with the installation.</span></span>

4. <span data-ttu-id="ac829-136">在 [布建資訊] 頁面上，根據您的安裝填寫適當的欄位。</span><span class="sxs-lookup"><span data-stu-id="ac829-136">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="ac829-137">請至少輸入您要取得其布建程式及網站目的地 URL 相關通知的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="ac829-137">At a minimum, enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="ac829-138">將網站的目的地 URL 做為便於員工（如 "/sites/MyTraining" 或 "/teams/LearnMicrosoft365"）的內容。</span><span class="sxs-lookup"><span data-stu-id="ac829-138">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="ac829-140">準備好將學習路徑安裝至您的租使用者**環境時，** 按一下 [布建]。</span><span class="sxs-lookup"><span data-stu-id="ac829-140">Click **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="ac829-141">布建程式最多可能需要15分鐘。</span><span class="sxs-lookup"><span data-stu-id="ac829-141">The provisioning process can take up to 15 minutes.</span></span> <span data-ttu-id="ac829-142">當網站準備好時，您會透過電子郵件通知您。</span><span class="sxs-lookup"><span data-stu-id="ac829-142">You will be notified via email when the site is ready.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ac829-143">布建「學習路徑」網站的承租人管理員必須前往該網站，然後開啟**CustomLearningAdmin**以初始化學習路徑系統管理員屬性。</span><span class="sxs-lookup"><span data-stu-id="ac829-143">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="ac829-144">此時，租使用者管理員也應指派網站的擁有者。</span><span class="sxs-lookup"><span data-stu-id="ac829-144">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="ac829-145">驗證布建成功和初始化 CustomConfig 清單</span><span class="sxs-lookup"><span data-stu-id="ac829-145">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="ac829-146">布建完成時，布建網站的承租人管理員會收到來自 PnP 布建服務的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="ac829-146">When provisioning is complete, the Tenant Admin who provisioned the site receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="ac829-147">電子郵件包含網站的連結。</span><span class="sxs-lookup"><span data-stu-id="ac829-147">The email contains a link to the site.</span></span> <span data-ttu-id="ac829-148">此時，租使用者管理員應該會使用電子郵件中提供的連結前往網站，並設定網站以供第一次使用：</span><span class="sxs-lookup"><span data-stu-id="ac829-148">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="ac829-149">請移至 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。</span><span class="sxs-lookup"><span data-stu-id="ac829-149">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="ac829-150">開啟**CustomLearningAdmin**會初始化**CustomConfig**清單專案，以設定第一次使用的學習路徑。</span><span class="sxs-lookup"><span data-stu-id="ac829-150">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="ac829-151">您應該會看到如下所示的頁面：</span><span class="sxs-lookup"><span data-stu-id="ac829-151">You should see a page that looks like this:</span></span>

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="ac829-153">將擁有者新增至網站</span><span class="sxs-lookup"><span data-stu-id="ac829-153">Add Owners to Site</span></span>
<span data-ttu-id="ac829-154">作為租使用者系統管理員，您不太可能是自訂網站的人員，所以您必須將少數擁有者指派給網站。</span><span class="sxs-lookup"><span data-stu-id="ac829-154">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="ac829-155">擁有者具有網站的管理許可權，可供使用者修改網站頁面及才能重塑網站。</span><span class="sxs-lookup"><span data-stu-id="ac829-155">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="ac829-156">他們也可以隱藏及顯示內容，以及建立自訂的播放清單和子類別。</span><span class="sxs-lookup"><span data-stu-id="ac829-156">They also have the ability to hide and show content and build custom playlist and subcategories.</span></span>  

1. <span data-ttu-id="ac829-157">在 [SharePoint**設定**] 功能表中，按一下 [**網站許可權**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-157">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="ac829-158">按一下 [**高級許可權設定**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-158">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="ac829-159">按一下 [ **Microsoft 365 學習路徑擁有**者]。</span><span class="sxs-lookup"><span data-stu-id="ac829-159">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="ac829-160">按一下 [**新增**  >  **使用者至此群組**]，然後新增您想要成為擁有者的人員。</span><span class="sxs-lookup"><span data-stu-id="ac829-160">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="ac829-161">在 [共用郵件] 中新增[流覽網站的](custom_exploresite.md)連結，然後按一下 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-161">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

## <a name="add-translators-to-the-site"></a><span data-ttu-id="ac829-162">將翻譯人員新增至網站</span><span class="sxs-lookup"><span data-stu-id="ac829-162">Add translators to the site</span></span>
<span data-ttu-id="ac829-163">翻譯人員需要網站的成員許可權或更高的許可權。</span><span class="sxs-lookup"><span data-stu-id="ac829-163">Translators require member permissions or higher on the site.</span></span> 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a><span data-ttu-id="ac829-164">選擇在網站上使用多種語言的選項</span><span class="sxs-lookup"><span data-stu-id="ac829-164">Choose options for using multiple languages on the site</span></span>
<span data-ttu-id="ac829-165">SharePoint 布建服務以九種語言建立學習路徑網站。</span><span class="sxs-lookup"><span data-stu-id="ac829-165">The SharePoint Provisioning Service creates the Learning Pathways site in nine languages.</span></span> <span data-ttu-id="ac829-166">適用的建議如下：</span><span class="sxs-lookup"><span data-stu-id="ac829-166">The following recommendations apply:</span></span>
- <span data-ttu-id="ac829-167">關閉您不想要支援的語言</span><span class="sxs-lookup"><span data-stu-id="ac829-167">Turn off the languages you don’t want to support</span></span>
- <span data-ttu-id="ac829-168">如果您不支援多語系網站，請關閉 [多語言] 功能。</span><span class="sxs-lookup"><span data-stu-id="ac829-168">If you are not supporting a multilingual site, turn off the multi-lingual feature.</span></span> 

### <a name="remove-languages-you-dont-want-to-support"></a><span data-ttu-id="ac829-169">移除不想要支援的語言</span><span class="sxs-lookup"><span data-stu-id="ac829-169">Remove languages you don’t want to support</span></span>
<span data-ttu-id="ac829-170">針對選擇只支援一種語言的組織，除了預設英文語言之外，我們建議移除不支援的語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-170">For organizations that choose to support only one language, in addition to the default English language, we recommend removing languages that aren’t supported.</span></span> 
1. <span data-ttu-id="ac829-171">從 [學習路徑] 網站中，選取頁面右上角的 [**設定**]，然後選取 [**網站資訊**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-171">From the Learning Pathways site, select **Settings** from the top-right of the page, and then select **Site information**.</span></span>
2. <span data-ttu-id="ac829-172">在 [網站資訊] 窗格的底部，選取 [**查看所有網站設定**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-172">At the bottom of the site information pane, select **View all site settings**.</span></span>
3. <span data-ttu-id="ac829-173">在 [**網站管理**] 下，選取 [**語言設定**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-173">Under **Site Administration**, select **Language settings**.</span></span>
4. <span data-ttu-id="ac829-174">在 [**讓頁面和新聞轉譯成多種語言**] 底下，將開關滑動至 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-174">Under **Enable pages and news to be translated into multiple languages**, slide the toggle to **On**.</span></span> <span data-ttu-id="ac829-175">預設值應為 On。</span><span class="sxs-lookup"><span data-stu-id="ac829-175">It should be On by default.</span></span>
5. <span data-ttu-id="ac829-176">在 [新增或移除網站語言] 底下，按一下 [**移除**]，移除網站不需要的語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-176">Under Add or remove site languages, click **Remove** to remove the languages you don't need for the site.</span></span> <span data-ttu-id="ac829-177">下列會顯示 [語言設定] 頁面的範例，除了預設英文語言之外，還會顯示網站支援的義大利文。</span><span class="sxs-lookup"><span data-stu-id="ac829-177">The following shows an example of the Language Settings page to show Italian supported for the site, in addition to the default English language.</span></span>

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> <span data-ttu-id="ac829-179">移除語言時，不能移除預設的英文語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-179">When removing languages you cannot remove the default English language.</span></span> 

### <a name="assign-translators"></a><span data-ttu-id="ac829-180">指派翻譯員</span><span class="sxs-lookup"><span data-stu-id="ac829-180">Assign translators</span></span>
<span data-ttu-id="ac829-181">如果您想要翻譯頁面，可選擇為每種語言指派一或多個翻譯人員（網站的預設語言除外）。</span><span class="sxs-lookup"><span data-stu-id="ac829-181">If you're going to translate pages, optionally assign one or more translators for each language (except the site default language).</span></span> 
- <span data-ttu-id="ac829-182">在 [**翻譯人員**] 欄中，開始輸入您想要成為翻譯人員的名稱，然後從清單中選取名稱。</span><span class="sxs-lookup"><span data-stu-id="ac829-182">In the **Translator** column, start typing the name of a person you want to be a translator, and then select the name from the list.</span></span> 

> [!NOTE]
> <span data-ttu-id="ac829-183">您組織的 Active Directory 中的任何人都可以指派成翻譯工具。</span><span class="sxs-lookup"><span data-stu-id="ac829-183">Anyone in your organization's Active Directory can be assigned as a translator.</span></span> <span data-ttu-id="ac829-184">指派為翻譯人員的人員不會自動獲得適當的許可權。</span><span class="sxs-lookup"><span data-stu-id="ac829-184">People assigned as translators will not automatically be given appropriate permissions.</span></span> <span data-ttu-id="ac829-185">當沒有網站的「編輯」許可權的人員嘗試存取網站時，會將其導向至可要求存取的網頁。</span><span class="sxs-lookup"><span data-stu-id="ac829-185">When someone without edit permissions to a site tries to access the site, they will be directed to a web page where they can request access.</span></span>

## <a name="turn-off-multilingual-support"></a><span data-ttu-id="ac829-186">關閉多語言支援</span><span class="sxs-lookup"><span data-stu-id="ac829-186">Turn off multilingual support</span></span>
<span data-ttu-id="ac829-187">例如，如果您不想要使用多語系網站，則建議您關閉多語系功能。</span><span class="sxs-lookup"><span data-stu-id="ac829-187">If you don’t want a multilingual site, for example, you want an English-only site, it’s recommended that you turn off the multilingual feature.</span></span> 
- <span data-ttu-id="ac829-188">在 [**允許翻譯頁面和新聞**] 底下，選取 [**關閉**]。</span><span class="sxs-lookup"><span data-stu-id="ac829-188">Under **Enable pages and news to be translated**, select **Off**.</span></span> 

### <a name="add-languages"></a><span data-ttu-id="ac829-189">新增語言</span><span class="sxs-lookup"><span data-stu-id="ac829-189">Add languages</span></span>
<span data-ttu-id="ac829-190">學習路徑支援9種語言，但建議您只新增您必須用來支援「學習路徑」網站的語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-190">Learning pathways supports 9 languages, but it’s recommended that you add only the languages you need to support for the learning pathways site.</span></span> <span data-ttu-id="ac829-191">您可以在任何時候新增語言則。</span><span class="sxs-lookup"><span data-stu-id="ac829-191">You can add langauges at any time.</span></span> 
- <span data-ttu-id="ac829-192">在 [**新增或移除網站語言**] 底下，開始在 [**選取] 或 [輸入語言**] 中輸入語言名稱，或從下拉式清單中選擇語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-192">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="ac829-193">您可以重複此步驟來新增多種語言。</span><span class="sxs-lookup"><span data-stu-id="ac829-193">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="ac829-194">您可以隨時在網站中新增或移除語言，只要回到此頁面。</span><span class="sxs-lookup"><span data-stu-id="ac829-194">You can add or remove languages from your site at any time by going back to this page.</span></span>



