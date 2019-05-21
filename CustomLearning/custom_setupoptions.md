---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 學習路徑安裝程式選項
ms.date: 02/11/2019
description: 自訂學習設定安裝選項
ms.openlocfilehash: bef8e513d9126defc4b4f73acc6e07fc060044aa
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247688"
---
# <a name="learning-pathways-setup-options"></a><span data-ttu-id="4c526-103">學習路徑安裝程式選項</span><span class="sxs-lookup"><span data-stu-id="4c526-103">Learning pathways setup options</span></span>
<span data-ttu-id="4c526-104">學習路徑提供的彈性來設定解決方案，以幾種不同的方式。</span><span class="sxs-lookup"><span data-stu-id="4c526-104">Learning pathways provides the flexibility to set up the solution in a couple different ways.</span></span> <span data-ttu-id="4c526-105">下列各節將概述可用的選項。</span><span class="sxs-lookup"><span data-stu-id="4c526-105">The following sections outline the options available.</span></span>

## <a name="recommended---sharepoint-online-provisioning-service-setup"></a><span data-ttu-id="4c526-106">建議的 SharePoint Online 的佈建服務安裝</span><span class="sxs-lookup"><span data-stu-id="4c526-106">Recommended - SharePoint Online Provisioning Service Setup</span></span> 
<span data-ttu-id="4c526-107">SharePoint Online 佈建服務提供最快，最簡單，建議的方法，以便設定自訂學習。</span><span class="sxs-lookup"><span data-stu-id="4c526-107">The SharePoint Online Provisioning Service provides the fastest, easiest, and recommended method for setting up Custom Learning.</span></span> <span data-ttu-id="4c526-108">與 SharePoint Online 佈建服務，為 Office 365 租用戶系統管理員登入至服務、 建立幾個選項，並且按一下 [**新增] 以租用戶**佈建自訂學習網站及自訂學習網頁組件。</span><span class="sxs-lookup"><span data-stu-id="4c526-108">With the SharePoint Online Provisioning Service, an Office 365 tenant admin signs into the service, makes a few choices, and clicks **Add to Tenant** to provision the Custom Learning Site and the Custom Learning Web part.</span></span> <span data-ttu-id="4c526-109">佈建完成時，租用戶系統管理員會收到網站已準備好一封電子郵件。</span><span class="sxs-lookup"><span data-stu-id="4c526-109">When provisioning is done, the Tenant Admin receives an email that the site is ready to go.</span></span> 

- <span data-ttu-id="4c526-110">若要開始使用 SharePoint 佈建服務，請移至[與 PnP 佈建服務的佈建](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="4c526-110">To get started with the SharePoint Provisioning Service, go to [Provision with the PnP Provisioning Service](custom_provision.md)</span></span>   

## <a name="stand-alone-learning-pathways-web-part-setup"></a><span data-ttu-id="4c526-111">獨立單獨學習路徑網頁組件設定</span><span class="sxs-lookup"><span data-stu-id="4c526-111">Stand alone learning pathways web part setup</span></span>
<span data-ttu-id="4c526-112">已建立的 SharePoint Online 新式通訊訓練入口網站的公司，學習路徑提供手動安裝至現有的 SharePoint Online 網站學習路徑網頁組件的 Microsoft 365 的選項。</span><span class="sxs-lookup"><span data-stu-id="4c526-112">For organizations that already have an established SharePoint Online modern communication training portal, learning pathways provides the option to manually install the Microsoft 365 learning pathways web part into an existing SharePoint Online site.</span></span> <span data-ttu-id="4c526-113">請注意網站必須新式的 SharePoint Online 網站。</span><span class="sxs-lookup"><span data-stu-id="4c526-113">Note that the site must be a modern SharePoint Online site.</span></span> <span data-ttu-id="4c526-114">此方法需要租用戶系統管理員權限和使用 Windows PowerShell 或 SharePoint Online 管理命令介面的經驗。</span><span class="sxs-lookup"><span data-stu-id="4c526-114">This method requires Tenant Admin permissions and experience with Windows PowerShell or the SharePoint Online Management Shell.</span></span> <span data-ttu-id="4c526-115">請注意，此方法需要更多技術的專業知識然後 SharePoint Online 佈建服務安裝程式。</span><span class="sxs-lookup"><span data-stu-id="4c526-115">Note that this method requires more technical expertise then the SharePoint Online Provisioning Service setup.</span></span>

- <span data-ttu-id="4c526-116">手動網頁組件的安裝指示，請參閱 < 請參閱<b0>手動安裝的網頁組件</b0>。</span><span class="sxs-lookup"><span data-stu-id="4c526-116">For Manual web part installation instructions, see see [Manually install the web part](custom_manualsetup.md).</span></span> 

## <a name="update-learning-pathways"></a><span data-ttu-id="4c526-117">學習路徑的更新</span><span class="sxs-lookup"><span data-stu-id="4c526-117">Update learning pathways</span></span>
<span data-ttu-id="4c526-118">已安裝更早版本的 Microsoft 365 學習路徑，先前的 Office 365，稱為 「 自訂學習使用 SharePoint Online 佈建服務的組織可以使用最新版本更新解決方案。</span><span class="sxs-lookup"><span data-stu-id="4c526-118">Organizations that have used the SharePoint Online Provisioning Service to install earlier versions of Microsoft 365 learning pathways, previously called Custom Learning for Office 365,can update the solution to the latest version.</span></span> <span data-ttu-id="4c526-119">如需如何檢查部署解決方案，以及如何更新方案時，指示的最新版本對版本的指示，請參閱[讀我檔案](https://github.com/pnp/custom-learning-office-365/blob/master/README.md)的 「 更新方案 」 區段。</span><span class="sxs-lookup"><span data-stu-id="4c526-119">For instructions on how to check the version deployed against the most recent version of the solution, along with instructions on how to update the solution, see the "Updating the solution" section of the [ReadMe file](https://github.com/pnp/custom-learning-office-365/blob/master/README.md).</span></span>

### <a name="next-steps---provision-microsoft-365-learning-pathwayscustomprovisionmd"></a><span data-ttu-id="4c526-120">接下來的步驟-[佈建 Microsoft 365 學習路徑](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="4c526-120">Next Steps - [Provision Microsoft 365 learning pathways](custom_provision.md)</span></span>
