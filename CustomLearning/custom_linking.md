---
author: pkrebs
ms.author: pkrebs
title: 連結至學習資產的自訂
ms.date: 02/15/2019
description: 如何自訂學習資產的連結
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056145"
---
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="e3926-103">連結至自訂學習內容</span><span class="sxs-lookup"><span data-stu-id="e3926-103">Link to Custom Learning content</span></span>

<span data-ttu-id="e3926-104">使用自訂學習，有兩種方式可連結至內容：</span><span class="sxs-lookup"><span data-stu-id="e3926-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="e3926-105">連結至裝載您要顯示的內容篩選網頁組件頁面。</span><span class="sxs-lookup"><span data-stu-id="e3926-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="e3926-106">直接連結至網頁組件的執行個體</span><span class="sxs-lookup"><span data-stu-id="e3926-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="e3926-107">連結至頁面</span><span class="sxs-lookup"><span data-stu-id="e3926-107">Link to a page</span></span>

<span data-ttu-id="e3926-108">如果您建立新頁面，且學習體驗自訂學習網頁組件，您可以連結] 頁面上設定為顯示內容的網頁組件與您想要顯示。</span><span class="sxs-lookup"><span data-stu-id="e3926-108">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="e3926-109">在前一個區段中，我們會討論如何在頁面上顯示 Excel 播放清單。</span><span class="sxs-lookup"><span data-stu-id="e3926-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="e3926-110">您現在可以編輯連結] 頁面上的 [首頁] 頁面。</span><span class="sxs-lookup"><span data-stu-id="e3926-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="e3926-111">從 [首頁] 頁面上，按一下 [**編輯**]。</span><span class="sxs-lookup"><span data-stu-id="e3926-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="e3926-112">按一下 [**編輯詳細資料**中下列其中一個 [首頁] 磚。</span><span class="sxs-lookup"><span data-stu-id="e3926-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="e3926-113">在這個範例中，我們可以編輯 [**建議播放清單**] 磚。</span><span class="sxs-lookup"><span data-stu-id="e3926-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="e3926-114">在 [**連結**] 按一下 [**變更**]。</span><span class="sxs-lookup"><span data-stu-id="e3926-114">Under **Link**, click **Change**.</span></span>

![cg linktopage.png](media/cg-linktopage.png)

4. <span data-ttu-id="e3926-116">按一下 [**網站**]，然後**網站頁面**，按一下您想要連結到的頁面，然後按一下 [**開啟**。</span><span class="sxs-lookup"><span data-stu-id="e3926-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="e3926-117">在這個範例中，我們會連結至前一節所述**建立-您對擁有-experience.aspx**頁面。</span><span class="sxs-lookup"><span data-stu-id="e3926-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="e3926-118">關閉 Hero 內容] 窗格，按一下 [**發佈**]，然後測試連結。</span><span class="sxs-lookup"><span data-stu-id="e3926-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="e3926-119">連結至自訂學習網頁組件</span><span class="sxs-lookup"><span data-stu-id="e3926-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="e3926-120">自訂學習可讓您、 系統管理員，則使用者，能夠連結至含有網頁組件頁面的網頁組件獨立於執行個體。</span><span class="sxs-lookup"><span data-stu-id="e3926-120">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="e3926-121">您可以對它共用複製的連結，從其他頁面。</span><span class="sxs-lookup"><span data-stu-id="e3926-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="e3926-122">[複製] 連結，按下時，顯示 [CustomLLearningViewer.aspx] 頁面上的自訂學習網頁組件執行個體。</span><span class="sxs-lookup"><span data-stu-id="e3926-122">The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="e3926-123">讓我們看看範例。</span><span class="sxs-lookup"><span data-stu-id="e3926-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="e3926-124">從 [首頁] 頁面上，按一下 [ **Office 365 訓練**。</span><span class="sxs-lookup"><span data-stu-id="e3926-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="e3926-125">按一下 [ **Microsoft Teams**、，然後按一下 [ **Microsoft Teams 的簡介**。</span><span class="sxs-lookup"><span data-stu-id="e3926-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="e3926-126">按一下 [**複製**] 圖示。</span><span class="sxs-lookup"><span data-stu-id="e3926-126">Click the **Copy** icon.</span></span>

![cg linktowebpart.png](media/cg-linktowebpart.png)

4. <span data-ttu-id="e3926-128">從 [自訂學習] 功能表按一下 [Home 鍵。</span><span class="sxs-lookup"><span data-stu-id="e3926-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="e3926-129">在瀏覽器網址列中貼上複製的 URL，然後按 ENTER。</span><span class="sxs-lookup"><span data-stu-id="e3926-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="e3926-130">下圖所示，連結移至 [CustomLearningViewer.aspx] 頁面上，而且會顯示 [複製] 連結中的參數為基礎的內容。</span><span class="sxs-lookup"><span data-stu-id="e3926-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![cg linktowebpartviewer.png](media/cg-linktowebpartviewer.png)

