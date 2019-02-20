---
author: pkrebs
ms.author: pkrebs
title: 建立 SharePoint 頁面的 [播放清單
ms.date: 02/10/2019
description: 建立 SharePoint 頁面的 [播放清單
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103688"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="58ae7-103">建立自訂播放清單 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="58ae7-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="58ae7-p101">其中一個自訂學習的唯一功能已建立從資產 Microsoft 和您建立的 SharePoint 資產組合的播放清單的功能。在這個範例中，我們將建立 SharePoint 頁面之前建立播放清單。能夠建立播放清單從 SharePoint 頁面提供各種機會來建立可從 Microsoft 或組織的網頁組件頁面。例如，播放清單可以包含內嵌影片 YouTube、 SharePoint 頁面或 Office 365 表單或內嵌的 Power BI 報表所構成的表單。在這個範例中，我們將顯示您如何建置含有內嵌網頁組件和文字網頁組件的頁面。</span><span class="sxs-lookup"><span data-stu-id="58ae7-p101">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create. In this example, we’ll create a SharePoint page in advance of creating a playlist. The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization. For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report. In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="58ae7-109">建立自訂的播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="58ae7-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="58ae7-110">按一下 SharePoint**齒輪**圖示，然後再按一下 [**新增工作] 頁面**。</span><span class="sxs-lookup"><span data-stu-id="58ae7-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="58ae7-111">按一下 [**新增新區段 （+）** ] 頁面的左端上和版面配置] 區段中 [**兩欄**。</span><span class="sxs-lookup"><span data-stu-id="58ae7-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="58ae7-112">在 [左] 欄中，按一下 [+] 和 [**內嵌]** 網頁組件。</span><span class="sxs-lookup"><span data-stu-id="58ae7-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="58ae7-p102">在右邊的欄中，按一下 [+] 和 [**文字**網頁組件。您的頁面行會類似。</span><span class="sxs-lookup"><span data-stu-id="58ae7-p102">In the right column, click +, and then click the **Text** web part. Your page should look like this.</span></span>

![cg pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="58ae7-116">從 YouTube 新增視訊及文字</span><span class="sxs-lookup"><span data-stu-id="58ae7-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="58ae7-p103">在瀏覽器中移至 YouTube。此範例中，如搜尋 「 什麼是 Office 365-Microsoft 的最佳產能應用程式 」。</span><span class="sxs-lookup"><span data-stu-id="58ae7-p103">In your browser, go to YouTube. For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="58ae7-119">按一下 [在播放、 暫停，然後以滑鼠右鍵按一下它視訊。</span><span class="sxs-lookup"><span data-stu-id="58ae7-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="58ae7-120">按一下 [**複製內嵌程式碼**，然後回到 [SharePoint] 頁面。</span><span class="sxs-lookup"><span data-stu-id="58ae7-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="58ae7-121">**Embed**網頁組件] 中按一下 [**新增內嵌程式碼**，然後新增程式碼從 YouTube 影片。</span><span class="sxs-lookup"><span data-stu-id="58ae7-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="58ae7-122">返回 YouTube 頁面並複製影片的**描述**文字。</span><span class="sxs-lookup"><span data-stu-id="58ae7-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="58ae7-123">回到 [SharePoint] 頁面上，選取**文字**的網頁組件，然後複製 YouTube 影片的文字。</span><span class="sxs-lookup"><span data-stu-id="58ae7-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="58ae7-124">在 [SharePoint] 頁面的 [標題] 區域中選取 [**編輯網頁組件**] 圖示，並再命名"自訂播放清單 Introduction"] 頁面。</span><span class="sxs-lookup"><span data-stu-id="58ae7-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="58ae7-p104">針對**版面配置**，選取 [**純文字**，然後關閉**標題區域**內容窗格。頁面現在看起來應類似如下的某個項目。</span><span class="sxs-lookup"><span data-stu-id="58ae7-p104">For **Layout**, select **Plain**, then close **Title Region** properties pane. The page should now look something like the following.</span></span> 

![cg pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="58ae7-128">發佈頁面</span><span class="sxs-lookup"><span data-stu-id="58ae7-128">Publish the page</span></span>

- <span data-ttu-id="58ae7-p105">選取 [**發佈**] 按鈕。現在您已經準備好將此 SharePoint] 頁面上新增至您的自訂播放清單。</span><span class="sxs-lookup"><span data-stu-id="58ae7-p105">Select the **Publish** button. Now you're ready to add this SharePoint page to your custom playlist.</span></span> 