---
author: karuanag
ms.author: karuanag
title: 自訂和共用播放清單
ms.date: 02/10/2019
description: 從現有內容或新的 SharePoint 頁面建立自訂播放清單
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233805"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="dbf9f-103">自訂和共用播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="dbf9f-104">建立播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-104">Create a Playlist</span></span>

<span data-ttu-id="dbf9f-105">播放清單是「資產」的 compliation。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="dbf9f-106">「資產」是 Microsoft 訓練內容的 SharePoint 頁面或現有專案。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="dbf9f-107">當您建立播放清單時，您會選取同時為您的使用者建立學習路徑的資產。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="dbf9f-108">新增 SharePoint 頁面的好處是，您可以使用組織中所主控的 YouTube 影片或影片，來建立 SharePoint 頁面。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="dbf9f-109">您也可以使用表單或其他 Office 365 內容來建立頁面。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="dbf9f-110">步驟1：建立播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="dbf9f-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="dbf9f-111">在此範例中，我們將先建立 SharePoint 頁面以新增至播放清單。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="dbf9f-112">我們將使用 YouTube 的「影片網頁元件」和「文字網頁元件」來建立頁面。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="dbf9f-113">這些指示假設您正在使用 SharePoint 線上服務。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="dbf9f-114">建立新的頁面</span><span class="sxs-lookup"><span data-stu-id="dbf9f-114">Create a new page</span></span>
1.  <span data-ttu-id="dbf9f-115">在 [新增 > 網站] 頁面上，選取 [設定] 功能表 > 網站內容 > 網站 > 頁面]。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="dbf9f-116">在 [標題] 區域中，輸入 [使用小組] 命令框</span><span class="sxs-lookup"><span data-stu-id="dbf9f-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="dbf9f-117">選取 [新增新的區段]，然後選取兩欄。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-117">Select the Add a new section, and then select Two Columns.</span></span>

![兩欄新增](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="dbf9f-119">在左框中，選取 [新增網頁元件]，然後選取 [內嵌]。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="dbf9f-120">在網頁瀏覽器中，移至此 URL https://youtu.be/wYrRCRphrp0 並取得影片的內嵌程式碼。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="dbf9f-121">在 [SharePoint 網頁元件] 中，選取 [新增內嵌程式碼]，然後將其貼到 [嵌入] 方塊中。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="dbf9f-122">在右側方塊中，選取 [新增網頁元件]，然後選取 [文字]。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="dbf9f-123">在網頁瀏覽器中，移至此 URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 並複製 Try！</span><span class="sxs-lookup"><span data-stu-id="dbf9f-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="dbf9f-124">頁面上的指示，並將其貼到 [文字] 網頁元件。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="dbf9f-125">您的頁面看起來應該如下所示。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-125">Your page should look like the following.</span></span> 

![內嵌頁面](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="dbf9f-127">按一下 [ **發佈**]，然後複製頁面的 URL，並將它貼到 [記事本] 中。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="dbf9f-128">步驟2：建立播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="dbf9f-129">流覽至網站體驗中的 [ **自訂學習管理** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="dbf9f-130">![custom_admin.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="dbf9f-131">確定已選取**類別**</span><span class="sxs-lookup"><span data-stu-id="dbf9f-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="dbf9f-132">按一下您想要顯示新播放清單的類別</span><span class="sxs-lookup"><span data-stu-id="dbf9f-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="dbf9f-133">在類別名稱旁邊，按一下加號符號 ![custom_addplay.png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="dbf9f-134">請填入下列範例中所示的值，然後選取 [ **建立**]。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="dbf9f-135">![custom_details.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="dbf9f-136">播放清單的**標題**-顯示名稱</span><span class="sxs-lookup"><span data-stu-id="dbf9f-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="dbf9f-137">**Description** -所學內容的相關資訊</span><span class="sxs-lookup"><span data-stu-id="dbf9f-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="dbf9f-138">**類別** -根據初始選取範圍預先選取</span><span class="sxs-lookup"><span data-stu-id="dbf9f-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="dbf9f-139">**Sub Category** -根據您的初始選取專案預先選取</span><span class="sxs-lookup"><span data-stu-id="dbf9f-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="dbf9f-140">**技術** -如果適用的話，選取</span><span class="sxs-lookup"><span data-stu-id="dbf9f-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="dbf9f-141">**層級** -初級、Intermidate 或 Advanced</span><span class="sxs-lookup"><span data-stu-id="dbf9f-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="dbf9f-142">**物件** -這可讓您根據 Microsoft 所提供之角色的預先定義清單來設定內容目標。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="dbf9f-143">按一下 [**儲存詳細資料**]</span><span class="sxs-lookup"><span data-stu-id="dbf9f-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="dbf9f-144">您可以自訂播放清單的圖示影像。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="dbf9f-145">按一下圖像圖示，然後插入先前上傳之圖像的 URL。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="dbf9f-146">請確定圖像位於自訂的教學網站集合中，或是所有使用者都可以存取該檔案的另一個位置。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="dbf9f-147">![custom_image.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="dbf9f-148">步驟3：將資產新增至播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="dbf9f-149">在這個步驟中，您將會從 Microsoft 新增現有的資產，以及您建立至播放清單的 SharePoint 頁面。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="dbf9f-150">儲存您的播放清單詳細資料後，您就可以使用搜尋現有的資產。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="dbf9f-151">**在任何搜尋字詞中輸入** ，以查看其他播放清單中提供的預先定義的資產清單。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="dbf9f-152">**按一下資產名稱** ，將其包含在新的播放清單中。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="dbf9f-153">![custom_slist.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="dbf9f-154">您也可以新增先前建立的 SharePoint 頁面，也可以在體驗中從頭開始建立。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="dbf9f-155">按一下 [播放清單資源] 對話方塊中的 [ **新增資產** ] 選項</span><span class="sxs-lookup"><span data-stu-id="dbf9f-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="dbf9f-156">將您的資產命名為 **職稱**。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-156">Give your asset a **Title**.</span></span> <span data-ttu-id="dbf9f-157">輸入後，其他選項會顯示 ![custom_newpage.png](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="dbf9f-158">您現在可以在 SharePoint Online 中建立新資產頁面，或在現有頁面的 URL 中輸入，以將其新增至您的自訂播放清單。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="dbf9f-159">[**類別**]、[**子類別**] 及 [**技術**] 欄位會根據您先前的選取範圍，預先填入此播放清單。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="dbf9f-160">針對此個別資產進行適當的層級和物件的選擇。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="dbf9f-161">按一下 [ **儲存資產** ]，將其新增至自訂播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="dbf9f-162">重複這些步驟，搜尋或新增個別頁面，直到完成播放清單為止。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="dbf9f-163">按一下 [ **關閉播放清單** 以儲存]</span><span class="sxs-lookup"><span data-stu-id="dbf9f-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="dbf9f-164">具有此內容的播放清單現在可在任何安裝/內嵌自訂學習 webpart 的地方使用。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="dbf9f-165">如果您在關閉播放清單後犯了錯誤，您可以按一下播放清單名稱旁邊的 X，將其從類別中刪除。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="dbf9f-166">考慮事項</span><span class="sxs-lookup"><span data-stu-id="dbf9f-166">Things to Think About</span></span>

<span data-ttu-id="dbf9f-167">自訂播放清單可用來協助您的使用者使用各種任務。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="dbf9f-168">您是否有下班時間的要求表單？</span><span class="sxs-lookup"><span data-stu-id="dbf9f-168">Do you have a time off request form?</span></span>  <span data-ttu-id="dbf9f-169">要求硬體設備的表單？</span><span class="sxs-lookup"><span data-stu-id="dbf9f-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="dbf9f-170">任何現有的訓練資產都可以設計成經驗。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="dbf9f-171">共用播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-171">Share Playlists</span></span>

1. <span data-ttu-id="dbf9f-172">流覽至 webpart 或網站體驗中的任何播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="dbf9f-173">在左上角會看到三個圖示</span><span class="sxs-lookup"><span data-stu-id="dbf9f-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="dbf9f-174">按一下代表連結的圖示</span><span class="sxs-lookup"><span data-stu-id="dbf9f-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="dbf9f-175">將 URL 複製到播放清單</span><span class="sxs-lookup"><span data-stu-id="dbf9f-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="dbf9f-176">![share.png](media/share.png) 此 URL 現在可以插入網站導航或在其他通訊中使用，以直接將員工直接加入該播放清單。</span><span class="sxs-lookup"><span data-stu-id="dbf9f-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="dbf9f-177">後續步驟- [磁片磁碟機採用](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="dbf9f-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
