---
author: pkrebs
ms.author: pkrebs
title: 更新多語言支援的學習路徑
ms.date: 05/20/2019
description: 更新多語言支援的學習路徑
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000239"
---
# <a name="update-learning-pathways-for-multilingual-support"></a><span data-ttu-id="f4f1c-103">更新多語言支援的學習路徑</span><span class="sxs-lookup"><span data-stu-id="f4f1c-103">Update learning pathways for multilingual support</span></span>
<span data-ttu-id="f4f1c-104">如果您有現有的學習路徑網站，您可以更新它以進行多語言支援。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="f4f1c-105">若要將學習路徑更新為多語系4.0 版本，請將網頁元件套件（customlearning）上傳至 SharePoint 租使用者目錄。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="f4f1c-106">當您更新學習路徑：</span><span class="sxs-lookup"><span data-stu-id="f4f1c-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="f4f1c-107">先前建立的任何自訂播放清單和資產都將維護</span><span class="sxs-lookup"><span data-stu-id="f4f1c-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="f4f1c-108">會維護隱藏或顯示內容的設定</span><span class="sxs-lookup"><span data-stu-id="f4f1c-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="f4f1c-109">學習路徑 SharePoint 範本保持不變</span><span class="sxs-lookup"><span data-stu-id="f4f1c-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="f4f1c-110">學習路徑網站頁面不會轉譯。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="f4f1c-111">您必須手動執行這種工作</span><span class="sxs-lookup"><span data-stu-id="f4f1c-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="f4f1c-112">閱讀學習路徑多語簡介</span><span class="sxs-lookup"><span data-stu-id="f4f1c-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="f4f1c-113">若要瞭解多語系支援如何運作以取得學習路徑，請閱讀 [學習路徑多語言概述](custom_overview_ml.md)) 。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview_ml.md)).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="f4f1c-114">更新的必要條件</span><span class="sxs-lookup"><span data-stu-id="f4f1c-114">Prerequisites to update</span></span>
<span data-ttu-id="f4f1c-115">更新學習路徑之前，必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="f4f1c-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="f4f1c-116">更新學習路徑的人員必須是租使用者應用程式目錄的網站集合擁有者。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="f4f1c-117">如果人員提供的學習路徑不是應用程式目錄的網站集合擁有者，請 [完成這些指示](addappadmin.md) 並繼續。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="f4f1c-118">設定語言設定</span><span class="sxs-lookup"><span data-stu-id="f4f1c-118">Set language settings</span></span> 
<span data-ttu-id="f4f1c-119">在更新學習路徑之前，請先設定網站的語言設定。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="f4f1c-120">若要啟用「學習路徑」網站的多語系支援，您可以將 [ **啟用頁面和新聞] 的 [可轉譯成多種語言** ] 設定為 [ **開啟**]，然後新增您要支援的網站語言。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="f4f1c-121">在 [學習路徑] 網站中，從右上方選取 [ **設定** ]，然後選取 [ **網站資訊**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="f4f1c-122">在 [網站資訊] 窗格的底部，選取 [ **查看所有網站設定**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="f4f1c-123">在 [ **網站管理**] 下，選取 [ **語言設定**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="f4f1c-124">在 [ **讓頁面和新聞可轉譯成多種語言**] 底下，設定切換參數。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="f4f1c-125">針對 multiligual 網站，將切換滑動至 [ **開啟**]，然後繼續進行 [新增語言] 區段。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="f4f1c-126">若為僅供英文使用的網站，請將此開關滑動至 [ **關閉**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="f4f1c-127">新增語言</span><span class="sxs-lookup"><span data-stu-id="f4f1c-127">Add languages</span></span>
<span data-ttu-id="f4f1c-128">學習路徑支援九種語言，您應該只新增您需要的語言。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="f4f1c-129">在本檔中所使用的範例中，會新增義大利文。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="f4f1c-130">在 [ **新增或移除網站語言**] 底下，開始在 [ **選取] 或 [輸入語言**] 中輸入語言名稱，或從下拉式清單中選擇語言。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="f4f1c-131">您可以重複此步驟來新增多種語言。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="f4f1c-132">您可以隨時在網站中新增或移除語言，只要回到此頁面。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="f4f1c-133">指派翻譯員</span><span class="sxs-lookup"><span data-stu-id="f4f1c-133">Assign translators</span></span>
<span data-ttu-id="f4f1c-134">在定義學習路徑的語言設定時，您可以指派翻譯人員。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="f4f1c-135">翻譯員應設定外部語言設定檔。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="f4f1c-136">如需外國語言設定檔的詳細資訊，請參閱 [建立多語言通訊網站、頁面和新聞](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="f4f1c-137">如需支援的語言，請按一下 [ **選取或輸入翻譯工具** ]，然後選取翻譯工具。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="f4f1c-138">更新「學習路徑」網頁元件套件</span><span class="sxs-lookup"><span data-stu-id="f4f1c-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="f4f1c-139">在這個步驟中，您會將「學習路徑4.0」網頁元件上傳至 SharePoint 的應用程式目錄，然後流覽至 [學習路徑管理] 頁面，以啟動更新程式。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="f4f1c-140">上傳網頁元件套件</span><span class="sxs-lookup"><span data-stu-id="f4f1c-140">Upload the web part package</span></span>
1.  <span data-ttu-id="f4f1c-141">移至 [GitHub 自訂學習存放庫](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)，選取 [ **customlearning** ]，然後將其下載至電腦上的本機磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-141">Go to the [GitHub custom learning repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), select **customlearning.sppkg** and then download it to a local drive on your PC.</span></span> 
2.  <span data-ttu-id="f4f1c-142">如果您尚未登入，請使用租用戶系統管理員或網站集合系統管理員帳戶登入您的租用戶。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="f4f1c-143">按一下 [系統 **管理**] [  >  **顯示所有**  >  **SharePoint**  >  **其他功能**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="f4f1c-144">在 [ **應用程式**] 下，按一下 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="f4f1c-145">按一下 [**應用程式目錄**  >  **分配應用程式以供 SharePoint**。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="f4f1c-146">按一下 [**上傳**  >  **選擇** 檔案]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="f4f1c-147">選取您下載的 **customlearning** 檔，按一下 **[確定**  >  **部署**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="f4f1c-148">完成更新</span><span class="sxs-lookup"><span data-stu-id="f4f1c-148">Complete the update</span></span>
1.  <span data-ttu-id="f4f1c-149">從 [學習路徑] 網站的 [**首頁**] 功能表中，選取 [**學習路徑管理**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="f4f1c-150">您會看到提示，詢問您是否要更新。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="f4f1c-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="f4f1c-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="f4f1c-152">按一下 **[開始]**。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-152">Click **Start**.</span></span> 
4. <span data-ttu-id="f4f1c-153">更新完成時，按一下 [ **關閉**]。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="f4f1c-154">後續步驟</span><span class="sxs-lookup"><span data-stu-id="f4f1c-154">Next Steps</span></span>
- <span data-ttu-id="f4f1c-155">探索網站和網頁元件中提供的 [預設內容](custom_exploresite.md) 。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="f4f1c-156">如需翻譯網站頁面的詳細資訊，請參閱 [翻譯網站頁面](custom_translate_page_ml.md)。</span><span class="sxs-lookup"><span data-stu-id="f4f1c-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

