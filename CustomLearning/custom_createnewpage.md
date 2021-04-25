---
author: pkrebs
ms.author: pkrebs
title: 建立播放清單的 SharePoint 頁面
ms.date: 02/10/2019
description: 建立播放清單的 SharePoint 頁面
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999084"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="d7aef-103">建立自訂播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="d7aef-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="d7aef-104">學習路徑的其中一個獨特功能是建立播放清單，這些播放清單是由 Microsoft 的資產和您所建立的 SharePoint 資產所組成。</span><span class="sxs-lookup"><span data-stu-id="d7aef-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="d7aef-105">在此範例中，我們會在建立播放清單之前建立 SharePoint 頁面。</span><span class="sxs-lookup"><span data-stu-id="d7aef-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="d7aef-106">從 SharePoint 頁面建立播放清單的功能，提供各種機會，可使用 Microsoft 或您組織中提供的網頁元件來建立頁面。</span><span class="sxs-lookup"><span data-stu-id="d7aef-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="d7aef-107">例如，播放清單可以包含從 YouTube 中內嵌影片的 SharePoint 頁面，或是從 Office 365 表單或內嵌的 Power BI 報表內建的表單。</span><span class="sxs-lookup"><span data-stu-id="d7aef-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="d7aef-108">在此範例中，我們將示範如何使用 [內嵌網頁元件] 和 [文字] 網頁元件建立頁面。</span><span class="sxs-lookup"><span data-stu-id="d7aef-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="d7aef-109">建立自訂播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="d7aef-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="d7aef-110">按一下 SharePoint **齒輪** 圖示，然後按一下 [ **新增頁面**]。</span><span class="sxs-lookup"><span data-stu-id="d7aef-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="d7aef-111">在頁面的左側，按一下 [ **新增新的區段 (+)** ]，然後按一下 [ **兩欄** ] 以進行區段版面配置。</span><span class="sxs-lookup"><span data-stu-id="d7aef-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="d7aef-112">在左側欄中，按一下 [+]，然後按一下 [ **嵌入** 網頁元件]。</span><span class="sxs-lookup"><span data-stu-id="d7aef-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="d7aef-113">在右列中，按一下 [+]，然後按一下 [ **文字** ] 網頁元件。</span><span class="sxs-lookup"><span data-stu-id="d7aef-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="d7aef-114">您的頁面看起來應該像這樣。</span><span class="sxs-lookup"><span data-stu-id="d7aef-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="d7aef-116">從 YouTube 新增影片和文字</span><span class="sxs-lookup"><span data-stu-id="d7aef-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="d7aef-117">在您的瀏覽器中，移至 YouTube。</span><span class="sxs-lookup"><span data-stu-id="d7aef-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="d7aef-118">在此範例中，請搜尋「什麼是 Office 365 – Microsoft 的最佳生產力應用程式」。</span><span class="sxs-lookup"><span data-stu-id="d7aef-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="d7aef-119">按一下影片以播放它，然後暫停它，然後在其上按一下滑鼠右鍵。</span><span class="sxs-lookup"><span data-stu-id="d7aef-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="d7aef-120">按一下 [ **複製內嵌程式碼**]，然後回到 [SharePoint] 頁面。</span><span class="sxs-lookup"><span data-stu-id="d7aef-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="d7aef-121">按一下 [**嵌入** 網頁元件] 中的 [**新增內嵌程式碼**]，然後從 YouTube 影片新增程式碼。</span><span class="sxs-lookup"><span data-stu-id="d7aef-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="d7aef-122">回到 YouTube 頁面，然後複製影片的 **描述** 文字。</span><span class="sxs-lookup"><span data-stu-id="d7aef-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="d7aef-123">回到 [SharePoint] 頁面上，選取 [ **文字** ] 網頁元件，然後複製 YouTube 影片中的文字。</span><span class="sxs-lookup"><span data-stu-id="d7aef-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="d7aef-124">選取 [SharePoint] 頁面的 [標題] 區域中的 [ **編輯網頁元件** ] 圖示，然後將頁面命名為「自訂播放清單簡介」。</span><span class="sxs-lookup"><span data-stu-id="d7aef-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="d7aef-125">若為 **Layout**，請選取 [ **普通**]，然後關閉 [ **標題區域** 內容] 窗格。</span><span class="sxs-lookup"><span data-stu-id="d7aef-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="d7aef-126">頁面現在應該如下所示。</span><span class="sxs-lookup"><span data-stu-id="d7aef-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="d7aef-128">發行頁面</span><span class="sxs-lookup"><span data-stu-id="d7aef-128">Publish the page</span></span>

- <span data-ttu-id="d7aef-129">選取 [ **發佈** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="d7aef-129">Select the **Publish** button.</span></span> <span data-ttu-id="d7aef-130">現在，您已準備好將此 SharePoint 頁面新增至自訂播放清單。</span><span class="sxs-lookup"><span data-stu-id="d7aef-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 