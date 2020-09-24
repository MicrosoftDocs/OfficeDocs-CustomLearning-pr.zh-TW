---
author: pkrebs
ms.author: pkrebs
title: 自訂學習路徑
ms.date: 02/18/2019
description: 自訂學習路徑
ms.service: sharepoint online
ms.openlocfilehash: 56027e48917cbdeeb2187f87497f3281fff3c23a
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234225"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="69436-103">自訂學習路徑</span><span class="sxs-lookup"><span data-stu-id="69436-103">Customize learning pathways</span></span>

<span data-ttu-id="69436-104">Microsoft 365 教學路徑提供各種方式，可讓您自訂群組織的內容。</span><span class="sxs-lookup"><span data-stu-id="69436-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="69436-105">例如，您可以：</span><span class="sxs-lookup"><span data-stu-id="69436-105">For example, you can:</span></span>  
- <span data-ttu-id="69436-106">修改教學路徑 SharePoint 網站-變更網站名稱、徽標和使用者。</span><span class="sxs-lookup"><span data-stu-id="69436-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="69436-107">修改 [提問] 和 [取得協助] 頁面，以建立您自己的説明中心。</span><span class="sxs-lookup"><span data-stu-id="69436-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="69436-108">隱藏或顯示內容，以反映組織中支援的服務或功能</span><span class="sxs-lookup"><span data-stu-id="69436-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="69436-109">專為使用者的需求建立自訂的播放清單和子類別</span><span class="sxs-lookup"><span data-stu-id="69436-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="69436-110">組建具有篩選內容的登陸頁面以支援商務成果，例如促進 Microsoft 團隊的採用、Outlook 行動性，或與 Microsoft 365 的共同作業。</span><span class="sxs-lookup"><span data-stu-id="69436-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing.png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="69436-112">需求和許可權</span><span class="sxs-lookup"><span data-stu-id="69436-112">Requirements and Permissions</span></span>

<span data-ttu-id="69436-113">開始使用自訂學習路徑指導之前，請確定您的 SharePoint 租使用者管理員已設定教學路徑。</span><span class="sxs-lookup"><span data-stu-id="69436-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="69436-114">如果您不確定是否已設定，請聯繫 SharePoint 租使用者管理員，確認已布建教學路徑。</span><span class="sxs-lookup"><span data-stu-id="69436-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="69436-115">此外，請務必取得教學路徑 SharePoint 網站的 URL。</span><span class="sxs-lookup"><span data-stu-id="69436-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="69436-116">如果您是租使用者系統管理員，且尚未布建學習路徑，請參閱布建 [學習路徑](custom_provision.md)。</span><span class="sxs-lookup"><span data-stu-id="69436-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="69436-117">提供學習路徑的許可權</span><span class="sxs-lookup"><span data-stu-id="69436-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="69436-118">租使用者系統管理員（也稱為 Office 365 全域系統管理員）</span><span class="sxs-lookup"><span data-stu-id="69436-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="69436-119">具有網站上擁有者權限的 SharePoint 網站集合系統管理員</span><span class="sxs-lookup"><span data-stu-id="69436-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="69436-120">使用學習路徑管理功能的許可權</span><span class="sxs-lookup"><span data-stu-id="69436-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="69436-121">網站集合管理員</span><span class="sxs-lookup"><span data-stu-id="69436-121">Site Collection Administrator</span></span>
- <span data-ttu-id="69436-122">SharePoint 擁有者或成員許可權</span><span class="sxs-lookup"><span data-stu-id="69436-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="69436-123">以使用者身分使用學習路徑網站的許可權</span><span class="sxs-lookup"><span data-stu-id="69436-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="69436-124">Office 365 使用者權限/SharePoint 網站訪客權限或較高</span><span class="sxs-lookup"><span data-stu-id="69436-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="69436-125">開始使用自訂</span><span class="sxs-lookup"><span data-stu-id="69436-125">Get started with customization</span></span>
<span data-ttu-id="69436-126">在您確保具備自訂網站和網頁元件的必要許可權之後，就可以開始使用自訂程式。</span><span class="sxs-lookup"><span data-stu-id="69436-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="69436-127">若要開始，請參閱 [移至 [學習路徑] 網站](custom_goto.md)。</span><span class="sxs-lookup"><span data-stu-id="69436-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>