---
author: pkrebs
ms.author: pkrebs
title: 隱藏及顯示技術
ms.date: 05/20/2019
description: 如何隱藏及顯示技術
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 7e4b2c6df2784fae592dd2b80dd0c17b437454e7
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310327"
---
# <a name="hide-and-show-technology"></a><span data-ttu-id="0c5a5-103">隱藏和顯示技術</span><span class="sxs-lookup"><span data-stu-id="0c5a5-103">Hide and show Technology</span></span>

<span data-ttu-id="0c5a5-104">在某些情況下，您可能會想要隱藏組織不支援之技術的內容。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-104">In some cases, you’ll want to hide content for a technology that’s not supported in your organization.</span></span> <span data-ttu-id="0c5a5-105">隱藏技術功能的設計是為了避免技術出現在整個網頁元件中。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-105">The Hide Technology feature is designed to prevent technology from appearing throughout the Web part.</span></span> <span data-ttu-id="0c5a5-106">它提供更廣泛的隱藏及顯示內容的方式，而不是依子類別或播放清單隱藏內容。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-106">It offers a broader way to hide and show content than hiding it by subcategory or playlist.</span></span> <span data-ttu-id="0c5a5-107">例如，您可以隱藏 Yammer 子類別，但是 Yammer 可能仍會顯示在某些案例播放清單中，例如「連線您的組織使用 Yammer]。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-107">For example, you can hide a Yammer subcategory, but Yammer may still show up in certain scenario playlists such as "Connect your organization with Yammer".</span></span> <span data-ttu-id="0c5a5-108">若要確定特定技術的內容未公開給使用者，請依技術加以隱藏。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-108">To ensure content for a specific technology is not exposed to end users, hide it by Technology.</span></span> 

## <a name="hide-a-technology"></a><span data-ttu-id="0c5a5-109">隱藏技術</span><span class="sxs-lookup"><span data-stu-id="0c5a5-109">Hide a Technology</span></span>

1. <span data-ttu-id="0c5a5-110">在 [Microsoft 365 學習路徑]**首頁** 上，按一下 **建議的播放清單** 磚。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-110">From the Microsoft 365 learning pathways **Home** page, click the **Recommended playlists** tile.</span></span>
2. <span data-ttu-id="0c5a5-111">從自訂學習網頁元件中，選取 [ **Aministration** ] 圖示。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-111">From the Custom Learning Web part, select the **Aministration** icon.</span></span>
3. <span data-ttu-id="0c5a5-112">在 [ **管理** ] 頁面右上方的下拉式清單方塊中，選取 [ **技術**]。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-112">In the dropdown list box in the upper-right section of the **Administration** page, select **Technology**.</span></span>
<span data-ttu-id="0c5a5-113">在此範例中，按一下頁面左窗格中的 [ **Yammer** ]，然後按一下 [Yammer] 旁邊的 eyeball。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-113">For this example, click **Yammer** in the left pane of the page, then click the eyeball next to Yammer.</span></span>  

![[範例] 視窗會顯示標示為圖示的技術類別，以隱藏該圖示。](media/cg-hidetech.png)

### <a name="verify-the-playlist-is-hidden"></a><span data-ttu-id="0c5a5-115">確認播放清單已隱藏</span><span class="sxs-lookup"><span data-stu-id="0c5a5-115">Verify the playlist is hidden</span></span>
- <span data-ttu-id="0c5a5-116">若要確認 **Yammer** 的技術是隱藏的，請選取 [瀏覽器] 索引標籤，並載入 **建議的播放清單** 頁面，然後重新整理頁面。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-116">To verify **Yammer** technology is hidden, select the browser tab with the **Recommended playlists** page loaded, and then refresh the page.</span></span> <span data-ttu-id="0c5a5-117">您會注意到 **組織使用 Yammer** 播放清單的連線已隱藏。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-117">You'll notice that the **Connect your organization with Yammer** playlist is hidden.</span></span> 

![範例視窗顯示隱藏的技術不再列出。](media/cg-hidetechrefresh.png)

## <a name="unhide-a-technology"></a><span data-ttu-id="0c5a5-119">取消隱藏技術</span><span class="sxs-lookup"><span data-stu-id="0c5a5-119">Unhide a Technology</span></span>

- <span data-ttu-id="0c5a5-120">在 [ **管理** ] 頁面上，選取技術，然後為隱藏的技術選取 eyeball 以取消隱藏。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-120">From the **Administration** page, select a technology, then select the eyeball for the hidden technology to unhide it.</span></span> <span data-ttu-id="0c5a5-121">在此範例中，會取消隱藏 **Yammer** 技術。</span><span class="sxs-lookup"><span data-stu-id="0c5a5-121">For this example, unhide the **Yammer** technology.</span></span> 