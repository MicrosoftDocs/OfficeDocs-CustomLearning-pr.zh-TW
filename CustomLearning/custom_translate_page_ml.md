---
author: pkrebs
ms.author: pkrebs
title: 轉譯網站頁面
ms.date: 02/10/2019
description: 轉譯網站頁面
ms.openlocfilehash: 32dc0928d12074575c8608cef38e4b4d0e5e5cf3
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699023"
---
# <a name="translate-site-pages"></a><span data-ttu-id="0a815-103">轉譯網站頁面</span><span class="sxs-lookup"><span data-stu-id="0a815-103">Translate site pages</span></span>
<span data-ttu-id="0a815-104">不論您是否已將現有的學習路徑版本更新為版本4.0，或您已布建新的網站，翻譯網站頁面的程式都是相同的。</span><span class="sxs-lookup"><span data-stu-id="0a815-104">Whether you've updated an existing version of learning pathways to version 4.0 or you've provisioned a new site, the process for translating site pages is the same.</span></span> <span data-ttu-id="0a815-105">不過，有一些事項需要注意。</span><span class="sxs-lookup"><span data-stu-id="0a815-105">However, there are a few things to be aware of.</span></span> 
- <span data-ttu-id="0a815-106">當您布建新的教學的多語系4.0 版本時，會將網站頁面翻譯成9種語言。</span><span class="sxs-lookup"><span data-stu-id="0a815-106">When a new learning pathways multilingual 4.0 version is provisioned, the site pages are translated for you into 9 languages.</span></span> 
- <span data-ttu-id="0a815-107">當學習路徑方案更新為多語系4.0 版本時，教學路徑 SharePoint 網站頁面會保持不變。</span><span class="sxs-lookup"><span data-stu-id="0a815-107">When the learning pathways solution is updated to the multilingual 4.0 version, the learning pathways SharePoint site pages remain unchanged.</span></span> <span data-ttu-id="0a815-108">必須手動進行翻譯。</span><span class="sxs-lookup"><span data-stu-id="0a815-108">Translations must be done manually.</span></span> 

<span data-ttu-id="0a815-109">「學習路徑」網站的預設提供下列頁面：</span><span class="sxs-lookup"><span data-stu-id="0a815-109">The learning pathways site, by default, provides the following pages:</span></span>

- <span data-ttu-id="0a815-110">首頁 .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-110">Home.aspx</span></span>
- <span data-ttu-id="0a815-111">Start-with-Six-Simple-Steps .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-111">Start-with-Six-Simple-Steps.aspx</span></span>
- <span data-ttu-id="0a815-112">Get-started-with-Microsoft-365 .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-112">Get-started-with-Microsoft-365.aspx</span></span>
- <span data-ttu-id="0a815-113">Get-started-with-Microsoft-Teams .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-113">Get-started-with-Microsoft-Teams.aspx</span></span>
- <span data-ttu-id="0a815-114">Get-started-with-SharePoint .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-114">Get-started-with-SharePoint.aspx</span></span>
- <span data-ttu-id="0a815-115">Get-started-with-OneDriive .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-115">Get-started-with-OneDriive.aspx</span></span>
- <span data-ttu-id="0a815-116">Ask-questions-and-get-help .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-116">Ask-questions-and-get-help.aspx</span></span>
- <span data-ttu-id="0a815-117">訓練事件-.aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-117">Training events calendar.aspx</span></span>
- <span data-ttu-id="0a815-118">Become-a-Champion .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-118">Become-a-Champion.aspx</span></span>
- <span data-ttu-id="0a815-119">Recommended-Playlists .aspx</span><span class="sxs-lookup"><span data-stu-id="0a815-119">Recommended-Playlists.aspx</span></span>
- <span data-ttu-id="0a815-120">學習路徑管理員成功中心</span><span class="sxs-lookup"><span data-stu-id="0a815-120">Learning pathways Admin Success Center</span></span>

## <a name="create-pages-for-the-languages-you-want"></a><span data-ttu-id="0a815-121">建立所需語言的頁面</span><span class="sxs-lookup"><span data-stu-id="0a815-121">Create pages for the languages you want</span></span>
<span data-ttu-id="0a815-122">一旦您已啟用您的網站的多語系功能，且您已選擇想要使用的語言，即可建立所需的翻譯頁面。</span><span class="sxs-lookup"><span data-stu-id="0a815-122">Once you've enabled your site for multilingual features and you've chosen the languages you want to make available, you can create the translation pages you want.</span></span> <span data-ttu-id="0a815-123">為了協助示範一些重要概念，我們會使用 Microsoft 365 訓練頁面做為範例。</span><span class="sxs-lookup"><span data-stu-id="0a815-123">To help demonstrate some important concepts, we'll use the Microsoft 365 training page as an example.</span></span> <span data-ttu-id="0a815-124">若要執行這項操作，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="0a815-124">To do this:</span></span>

1.  <span data-ttu-id="0a815-125">從 [學習路徑]**首頁**，按一下 [ **Microsoft 365 訓練**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-125">From the learning pathways **Home** page, click **Microsoft 365 training**.</span></span>  
2.  <span data-ttu-id="0a815-126">在頂端列上，選取 [**轉譯**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-126">On the top bar, select **Translation**.</span></span>
<span data-ttu-id="0a815-127">![custom_update_ml_transbutton.png](media/custom_update_ml_transbutton.png)</span><span class="sxs-lookup"><span data-stu-id="0a815-127">![custom_update_ml_transbutton.png](media/custom_update_ml_transbutton.png)</span></span>
3. <span data-ttu-id="0a815-128">如果您想要建立頁面以供網站使用的所有語言的翻譯，請選取 [**為所有語言建立**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-128">If you want to create a page for translation in each of all languages available for your site, select **Create for all languages**.</span></span> <span data-ttu-id="0a815-129">否則，請選取 [僅針對您想要的語言**建立**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-129">Otherwise, select **Create** only for the languages you want.</span></span> <span data-ttu-id="0a815-130">在此範例中，我們會選取 [義大利]。</span><span class="sxs-lookup"><span data-stu-id="0a815-130">In this example, we'll select Italian.</span></span>
4.  <span data-ttu-id="0a815-131">按一下 [**查看**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-131">Click **View**.</span></span> <span data-ttu-id="0a815-132">頁面現在可供翻譯。</span><span class="sxs-lookup"><span data-stu-id="0a815-132">The page is now ready for translation.</span></span> 

### <a name="an-important-concept-to-know"></a><span data-ttu-id="0a815-133">知道的重要概念</span><span class="sxs-lookup"><span data-stu-id="0a815-133">An important concept to know</span></span>
<span data-ttu-id="0a815-134">請注意，在下列範例中，頁面已轉譯成義大利文。</span><span class="sxs-lookup"><span data-stu-id="0a815-134">Notice that in the following example, the page has been translated to Italian.</span></span> <span data-ttu-id="0a815-135">但網站標題、導覽和網頁元件仍然會以英文顯示。</span><span class="sxs-lookup"><span data-stu-id="0a815-135">But the Site title, navigation, and web part, still appear in English.</span></span> 

![custom_update_ml_transpgconcept.png](media/custom_update_ml_transpgconcept.png)

 <span data-ttu-id="0a815-137">在以英文設定網站後，以西班牙文為使用者的使用者，會以西班牙文的個人語言手動編輯，並將標題、導覽及頁尾內容翻譯成西班牙文。</span><span class="sxs-lookup"><span data-stu-id="0a815-137">After the site is set up in English, a user with Spanish, for example, as their preferred personal language, manually edits and translates the title, navigation, and footer content into Spanish.</span></span> <span data-ttu-id="0a815-138">以德文做為偏好的個人語言的使用者，對德文的作用相同。</span><span class="sxs-lookup"><span data-stu-id="0a815-138">A user with German as their preferred personal language does the same for German.</span></span> <span data-ttu-id="0a815-139">翻譯內容之後，它會顯示所有慣用語言的使用者。</span><span class="sxs-lookup"><span data-stu-id="0a815-139">Once the content is translated, it will display for all users of those preferred languages.</span></span> <span data-ttu-id="0a815-140">網頁元件會挑選使用者的慣用語言，並顯示以該語言翻譯的內容。</span><span class="sxs-lookup"><span data-stu-id="0a815-140">The Web part picks up the user's preferred language and shows the content translated in that language.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="0a815-141">重要事項：在您建立翻譯頁面後，您必須發佈（或重新發佈）預設的英文語言頁面，以確定：</span><span class="sxs-lookup"><span data-stu-id="0a815-141">Important: After you create the translation pages, you must publish (or republish) the default English-language page to ensure that:</span></span>
- <span data-ttu-id="0a815-142">翻譯頁面會顯示在對應的語言網站中</span><span class="sxs-lookup"><span data-stu-id="0a815-142">Translation pages are shown in the corresponding language site</span></span>
- <span data-ttu-id="0a815-143">翻譯頁面在新聞網頁元件和醒目提示的內容網頁元件中正確顯示</span><span class="sxs-lookup"><span data-stu-id="0a815-143">Translation pages display correctly in the News web part and the Highlighted content web parts</span></span>
- <span data-ttu-id="0a815-144">網站頂端的語言下拉式功能表包含您已啟用的所有語言</span><span class="sxs-lookup"><span data-stu-id="0a815-144">The language dropdown at the top of the site includes all of the languages you've enabled</span></span>
- <span data-ttu-id="0a815-145">翻譯人員會收到轉譯要求的通知。</span><span class="sxs-lookup"><span data-stu-id="0a815-145">Translators are notified of the translation request.</span></span>

## <a name="what-does-a-translator-do"></a><span data-ttu-id="0a815-146">翻譯工具的作用是什麼？</span><span class="sxs-lookup"><span data-stu-id="0a815-146">What does a translator do?</span></span>
<span data-ttu-id="0a815-147">翻譯人員會以手動方式將預設語言頁面的副本轉譯成指定的語言。</span><span class="sxs-lookup"><span data-stu-id="0a815-147">Translators manually translate the copies of the default language page into the language(s) specified.</span></span> <span data-ttu-id="0a815-148">建立頁面的副本時，會以電子郵件通知翻譯人員。</span><span class="sxs-lookup"><span data-stu-id="0a815-148">When the copies of the page(s) are created, translators are notified in email.</span></span> <span data-ttu-id="0a815-149">電子郵件包含預設語言頁面與新建立的翻譯頁面的連結。</span><span class="sxs-lookup"><span data-stu-id="0a815-149">The email includes a link to the default language page and the newly created translation page.</span></span> <span data-ttu-id="0a815-150">翻譯人員將：</span><span class="sxs-lookup"><span data-stu-id="0a815-150">The translator will:</span></span>
1. <span data-ttu-id="0a815-151">選取電子郵件中的 [**開始翻譯**] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="0a815-151">Select the **Start translating** button in the email.</span></span>
2. <span data-ttu-id="0a815-152">在頁面右上方選取 [**編輯**]，然後翻譯內容。</span><span class="sxs-lookup"><span data-stu-id="0a815-152">Select **Edit** on the top right of the page, and translate the content.</span></span>
3. <span data-ttu-id="0a815-153">完成後，請選取 [**儲存為草稿**] （如果您未準備好讓讀者看到此頁面），或者，如果頁面可供在網站上使用該語言的所有人看到，請選取 [**發佈**] 或 [**張貼新聞**]。</span><span class="sxs-lookup"><span data-stu-id="0a815-153">When done, select **Save as draft** (if you're not ready to make it visible to readers)or, if the page is ready to be visible to everyone who is using that language on the site, select **Publish** or **Post news**.</span></span>

<span data-ttu-id="0a815-154">如需翻譯程式的詳細資訊，請參閱[建立多語系通訊網站、頁面和新聞](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。</span><span class="sxs-lookup"><span data-stu-id="0a815-154">For more information about the translation process, see [Create multilingual communication sites, pages, and news](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span> 

## <a name="updating-the-default-language-page"></a><span data-ttu-id="0a815-155">更新預設語言頁面</span><span class="sxs-lookup"><span data-stu-id="0a815-155">Updating the default language page</span></span>
<span data-ttu-id="0a815-156">當 [預設語言] 頁面更新時，必須重新發佈頁面。</span><span class="sxs-lookup"><span data-stu-id="0a815-156">When the default language page is updated, the page must be republished.</span></span> <span data-ttu-id="0a815-157">然後，翻譯頁面的翻譯人員會收到電子郵件通知，表明已進行更新，使其可對個別的翻譯頁面進行更新。</span><span class="sxs-lookup"><span data-stu-id="0a815-157">Then, the translator(s) for the translation pages are notified in email that an update has been made so updates can be made to the individual translation pages.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0a815-158">後續步驟</span><span class="sxs-lookup"><span data-stu-id="0a815-158">Next Steps</span></span>
- [<span data-ttu-id="0a815-159">轉譯自訂播放清單</span><span class="sxs-lookup"><span data-stu-id="0a815-159">Translate custom playlists</span></span>](custom_translate_pl_ml.md)
- [<span data-ttu-id="0a815-160">隱藏及顯示 multiligual 內容</span><span class="sxs-lookup"><span data-stu-id="0a815-160">Hide and show multiligual content</span></span>](custom_translate_pl_ml.md)
