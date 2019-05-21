---
author: pkrebs
ms.author: pkrebs
title: 建立 SharePoint 網頁的播放清單
ms.date: 02/10/2019
description: 建立 SharePoint 網頁的播放清單
ms.openlocfilehash: 97ef3e7fd37b11011afcc0738245f364a71f5112
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247533"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="ad01a-103">建立 SharePoint 網頁的自訂播放清單</span><span class="sxs-lookup"><span data-stu-id="ad01a-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="ad01a-104">學習路徑的獨特功能的其中一個已建立組合的資產從 Microsoft 和您所建立的 SharePoint 資產的播放清單的能力。</span><span class="sxs-lookup"><span data-stu-id="ad01a-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="ad01a-105">在這個範例中，我們會建立 SharePoint 頁面遲建立播放清單。</span><span class="sxs-lookup"><span data-stu-id="ad01a-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="ad01a-106">建立 SharePoint 網頁的播放清單的能力提供各種建置使用可以從 Microsoft 或貴組織的網頁組件頁面的機會。</span><span class="sxs-lookup"><span data-stu-id="ad01a-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="ad01a-107">例如，播放清單可以包含與內嵌視訊 YouTube，從 SharePoint] 頁面上或從 Office 365 表單或內嵌的 Power BI 報表內建的表單。</span><span class="sxs-lookup"><span data-stu-id="ad01a-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="ad01a-108">在這個範例中，我們將顯示您如何建置與內嵌網頁組件和文字網頁組件的頁面。</span><span class="sxs-lookup"><span data-stu-id="ad01a-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="ad01a-109">建立自訂播放清單的 SharePoint 頁面</span><span class="sxs-lookup"><span data-stu-id="ad01a-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="ad01a-110">按一下 [SharePoint**齒輪**圖示，，然後按一下 [**新增工作] 頁面**。</span><span class="sxs-lookup"><span data-stu-id="ad01a-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="ad01a-111">按一下左側的 [] 頁面上的 [**新增新區段 （+）** ，然後按一下 [版面配置] 區段中的 [**兩個資料行**。</span><span class="sxs-lookup"><span data-stu-id="ad01a-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="ad01a-112">在左邊的欄中，按一下 [+]，然後按一下 [**內嵌]** 網頁組件。</span><span class="sxs-lookup"><span data-stu-id="ad01a-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="ad01a-113">在右邊的欄中，按一下 [+]，然後按一下 [**文字**網頁組件。</span><span class="sxs-lookup"><span data-stu-id="ad01a-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="ad01a-114">您的頁面看起來應該像這樣。</span><span class="sxs-lookup"><span data-stu-id="ad01a-114">Your page should look like this.</span></span>

![cg pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="ad01a-116">從 YouTube 加入影片和文字</span><span class="sxs-lookup"><span data-stu-id="ad01a-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="ad01a-117">在瀏覽器中，移至 YouTube。</span><span class="sxs-lookup"><span data-stu-id="ad01a-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="ad01a-118">本範例中，搜尋 「 什麼是 Office 365-Microsoft 的最佳生產力的應用程式 」。</span><span class="sxs-lookup"><span data-stu-id="ad01a-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="ad01a-119">按一下 [視訊播放、 暫停它，然後以滑鼠右鍵按一下它。</span><span class="sxs-lookup"><span data-stu-id="ad01a-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="ad01a-120">按一下 [**複製內嵌程式碼**，然後回到 [SharePoint] 頁面。</span><span class="sxs-lookup"><span data-stu-id="ad01a-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="ad01a-121">**內嵌**網頁組件中，按一下 [**新增內嵌程式碼**，然後從 YouTube 視訊中加入程式碼。</span><span class="sxs-lookup"><span data-stu-id="ad01a-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="ad01a-122">返回 [YouTube] 頁面，然後複製影片的**描述**文字。</span><span class="sxs-lookup"><span data-stu-id="ad01a-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="ad01a-123">返回 [SharePoint] 頁面上，選取**文字**網頁組件，然後從 YouTube 視訊複製的文字。</span><span class="sxs-lookup"><span data-stu-id="ad01a-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="ad01a-124">標題區域中的 [SharePoint] 頁面上，選取 [**編輯網頁組件**] 圖示，然後命名 「 自訂播放清單簡介 」 頁面。</span><span class="sxs-lookup"><span data-stu-id="ad01a-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="ad01a-125">**版面配置**，選取 [**純文字**，然後關閉**標題區域**屬性] 窗格中。</span><span class="sxs-lookup"><span data-stu-id="ad01a-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="ad01a-126">[] 頁面上現在看起來應該如下所示。</span><span class="sxs-lookup"><span data-stu-id="ad01a-126">The page should now look something like the following.</span></span> 

![cg pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="ad01a-128">發佈頁面</span><span class="sxs-lookup"><span data-stu-id="ad01a-128">Publish the page</span></span>

- <span data-ttu-id="ad01a-129">選取 [**發佈**] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="ad01a-129">Select the **Publish** button.</span></span> <span data-ttu-id="ad01a-130">您現在可以將此 SharePoint 頁面新增至自訂播放清單。</span><span class="sxs-lookup"><span data-stu-id="ad01a-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 