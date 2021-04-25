---
author: karuanag
ms.author: karuanag
manager: alexb
title: 自訂和共用播放清單
ms.date: 02/10/2019
description: 從現有內容或新的 SharePoint 頁面建立自訂播放清單
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000209"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="74ab3-103">自訂和共用播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="74ab3-104">建立播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-104">Create a Playlist</span></span>

<span data-ttu-id="74ab3-105">播放清單是「資產」的 compliation。</span><span class="sxs-lookup"><span data-stu-id="74ab3-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="74ab3-106">「資產」是 Microsoft 訓練內容的 SharePoint 頁面或現有專案。</span><span class="sxs-lookup"><span data-stu-id="74ab3-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="74ab3-107">當您建立播放清單時，您會選取同時為您的使用者建立學習路徑的資產。</span><span class="sxs-lookup"><span data-stu-id="74ab3-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="74ab3-108">新增 SharePoint 頁面的好處是，您可以使用組織中所主控的 YouTube 影片或影片，來建立 SharePoint 頁面。</span><span class="sxs-lookup"><span data-stu-id="74ab3-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="74ab3-109">您也可以使用表單或其他 Office 365 內容來建立頁面。</span><span class="sxs-lookup"><span data-stu-id="74ab3-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="74ab3-110">步驟1：建立播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="74ab3-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="74ab3-111">在此範例中，我們將先建立 SharePoint 頁面以新增至播放清單。</span><span class="sxs-lookup"><span data-stu-id="74ab3-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="74ab3-112">我們將使用 YouTube 的「影片網頁元件」和「文字網頁元件」來建立頁面。</span><span class="sxs-lookup"><span data-stu-id="74ab3-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="74ab3-113">這些指示假設您正在使用 SharePoint 線上服務。</span><span class="sxs-lookup"><span data-stu-id="74ab3-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="74ab3-114">建立新的頁面</span><span class="sxs-lookup"><span data-stu-id="74ab3-114">Create a new page</span></span>
1.  <span data-ttu-id="74ab3-115">在 [新增 > 網站] 頁面上，選取 [設定] 功能表 > 網站內容 > 網站 > 頁面]。</span><span class="sxs-lookup"><span data-stu-id="74ab3-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="74ab3-116">在 [標題] 區域中，輸入 [使用小組] 命令框</span><span class="sxs-lookup"><span data-stu-id="74ab3-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="74ab3-117">選取 [新增新的區段]，然後選取兩欄。</span><span class="sxs-lookup"><span data-stu-id="74ab3-117">Select the Add a new section, and then select Two Columns.</span></span>

![兩欄新增](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="74ab3-119">在左框中，選取 [新增網頁元件]，然後選取 [內嵌]。</span><span class="sxs-lookup"><span data-stu-id="74ab3-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="74ab3-120">在網頁瀏覽器中，移至此 URL https://youtu.be/wYrRCRphrp0 並取得影片的內嵌程式碼。</span><span class="sxs-lookup"><span data-stu-id="74ab3-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="74ab3-121">在 [SharePoint 網頁元件] 中，選取 [新增內嵌程式碼]，然後將其貼到 [嵌入] 方塊中。</span><span class="sxs-lookup"><span data-stu-id="74ab3-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="74ab3-122">在右側方塊中，選取 [新增網頁元件]，然後選取 [文字]。</span><span class="sxs-lookup"><span data-stu-id="74ab3-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="74ab3-123">在網頁瀏覽器中，移至此 URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 並複製 Try！</span><span class="sxs-lookup"><span data-stu-id="74ab3-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="74ab3-124">頁面上的指示，並將其貼到 [文字] 網頁元件。</span><span class="sxs-lookup"><span data-stu-id="74ab3-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="74ab3-125">您的頁面看起來應該如下所示。</span><span class="sxs-lookup"><span data-stu-id="74ab3-125">Your page should look like the following.</span></span> 
<span data-ttu-id="74ab3-126">![內嵌頁面](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="74ab3-127">按一下 [ **發佈**]，然後複製頁面的 URL，並將它貼到 [記事本] 中。</span><span class="sxs-lookup"><span data-stu-id="74ab3-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="74ab3-128">步驟2：建立播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="74ab3-129">流覽至網站體驗中的 [ **自訂學習管理** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="74ab3-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="74ab3-130">![您選取自訂學習管理的畫面。](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="74ab3-131">確定已選取 **類別**</span><span class="sxs-lookup"><span data-stu-id="74ab3-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="74ab3-132">按一下您想要顯示新播放清單的類別</span><span class="sxs-lookup"><span data-stu-id="74ab3-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="74ab3-133">在 [類別名稱] 旁邊，按一下 [+ 符號 ![ ] 視窗中的 [類別] 選項，並將加號反白符號。](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="74ab3-134">請填入下列範例中所示的值，然後選取 [ **建立**]。</span><span class="sxs-lookup"><span data-stu-id="74ab3-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="74ab3-135">![您可以在其中輸入播放清單詳細資料的頁面。](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="74ab3-136">播放清單的 **標題**-顯示名稱</span><span class="sxs-lookup"><span data-stu-id="74ab3-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="74ab3-137">**Description** -所學內容的相關資訊</span><span class="sxs-lookup"><span data-stu-id="74ab3-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="74ab3-138">**類別** -根據初始選取範圍預先選取</span><span class="sxs-lookup"><span data-stu-id="74ab3-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="74ab3-139">**Sub Category** -根據您的初始選取專案預先選取</span><span class="sxs-lookup"><span data-stu-id="74ab3-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="74ab3-140">**技術** -如果適用的話，選取</span><span class="sxs-lookup"><span data-stu-id="74ab3-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="74ab3-141">**層級** -初級、Intermidate 或 Advanced</span><span class="sxs-lookup"><span data-stu-id="74ab3-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="74ab3-142">**物件** -這可讓您根據 Microsoft 所提供之角色的預先定義清單來設定內容目標。</span><span class="sxs-lookup"><span data-stu-id="74ab3-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="74ab3-143">按一下 [**儲存詳細資料**]</span><span class="sxs-lookup"><span data-stu-id="74ab3-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="74ab3-144">您可以自訂播放清單的圖示影像。</span><span class="sxs-lookup"><span data-stu-id="74ab3-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="74ab3-145">按一下圖像圖示，然後插入先前上傳之圖像的 URL。</span><span class="sxs-lookup"><span data-stu-id="74ab3-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="74ab3-146">請確定圖像位於自訂的教學網站集合中，或是所有使用者都可以存取該檔案的另一個位置。</span><span class="sxs-lookup"><span data-stu-id="74ab3-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="74ab3-147">![選擇影像視窗。](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="74ab3-148">步驟3：將資產新增至播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="74ab3-149">在這個步驟中，您將會從 Microsoft 新增現有的資產，以及您建立至播放清單的 SharePoint 頁面。</span><span class="sxs-lookup"><span data-stu-id="74ab3-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="74ab3-150">儲存您的播放清單詳細資料後，您就可以使用搜尋現有的資產。</span><span class="sxs-lookup"><span data-stu-id="74ab3-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="74ab3-151">**在任何搜尋字詞中輸入** ，以查看其他播放清單中提供的預先定義的資產清單。</span><span class="sxs-lookup"><span data-stu-id="74ab3-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="74ab3-152">**按一下資產名稱** ，將其包含在新的播放清單中。</span><span class="sxs-lookup"><span data-stu-id="74ab3-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="74ab3-153">![播放清單資產頁面](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="74ab3-154">您也可以新增先前建立的 SharePoint 頁面，也可以在體驗中從頭開始建立。</span><span class="sxs-lookup"><span data-stu-id="74ab3-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="74ab3-155">按一下 [播放清單資源] 對話方塊中的 [ **新增資產** ] 選項。</span><span class="sxs-lookup"><span data-stu-id="74ab3-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="74ab3-156">將您的資產命名為 **職稱**。</span><span class="sxs-lookup"><span data-stu-id="74ab3-156">Give your asset a **Title**.</span></span> <span data-ttu-id="74ab3-157">輸入之後，將會顯示其他選項。</span><span class="sxs-lookup"><span data-stu-id="74ab3-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="74ab3-158">![您可以在其中輸入標題和其他詳細資料的表單。](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="74ab3-159">您現在可以在 SharePoint Online 中建立新資產頁面，或在現有頁面的 URL 中輸入，以將其新增至您的自訂播放清單。</span><span class="sxs-lookup"><span data-stu-id="74ab3-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="74ab3-160">[**類別**]、[**子類別**] 及 [**技術**] 欄位會根據您先前的選取範圍，預先填入此播放清單。</span><span class="sxs-lookup"><span data-stu-id="74ab3-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="74ab3-161">針對此個別資產進行適當的層級和物件的選擇。</span><span class="sxs-lookup"><span data-stu-id="74ab3-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="74ab3-162">按一下 [ **儲存資產** ]，將其新增至自訂播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="74ab3-163">重複這些步驟，搜尋或新增個別頁面，直到完成播放清單為止。</span><span class="sxs-lookup"><span data-stu-id="74ab3-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="74ab3-164">按一下 [ **關閉播放清單** 以儲存]</span><span class="sxs-lookup"><span data-stu-id="74ab3-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="74ab3-165">具有此內容的播放清單現在可在任何安裝/內嵌自訂學習 webpart 的地方使用。</span><span class="sxs-lookup"><span data-stu-id="74ab3-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="74ab3-166">如果您在關閉播放清單後犯了錯誤，您可以按一下播放清單名稱旁邊的 X，將其從類別中刪除。</span><span class="sxs-lookup"><span data-stu-id="74ab3-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="74ab3-167">考慮事項</span><span class="sxs-lookup"><span data-stu-id="74ab3-167">Things to Think About</span></span>

<span data-ttu-id="74ab3-168">自訂播放清單可用來協助您的使用者使用各種任務。</span><span class="sxs-lookup"><span data-stu-id="74ab3-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="74ab3-169">您是否有下班時間的要求表單？</span><span class="sxs-lookup"><span data-stu-id="74ab3-169">Do you have a time off request form?</span></span>  <span data-ttu-id="74ab3-170">要求硬體設備的表單？</span><span class="sxs-lookup"><span data-stu-id="74ab3-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="74ab3-171">任何現有的訓練資產都可以設計成經驗。</span><span class="sxs-lookup"><span data-stu-id="74ab3-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="74ab3-172">共用播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-172">Share Playlists</span></span>

1. <span data-ttu-id="74ab3-173">流覽至 webpart 或網站體驗中的任何播放清單</span><span class="sxs-lookup"><span data-stu-id="74ab3-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="74ab3-174">在左上角會看到三個圖示</span><span class="sxs-lookup"><span data-stu-id="74ab3-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="74ab3-175">按一下代表連結的圖示</span><span class="sxs-lookup"><span data-stu-id="74ab3-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="74ab3-176">將 URL 複製到播放清單 ![ 畫面，您可以在其中按一下 url 旁邊的 [複製]。](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="74ab3-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="74ab3-177">現在可以將此 URL 插入網站導航或利用其他通訊，以直接將員工直接加入該播放清單。</span><span class="sxs-lookup"><span data-stu-id="74ab3-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="74ab3-178">後續步驟- [磁片磁碟機採用](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="74ab3-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
