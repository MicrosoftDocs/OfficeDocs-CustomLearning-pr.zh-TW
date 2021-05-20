---
author: pkrebs
ms.author: pkrebs
title: 手動安裝教學路徑
ms.date: 02/18/2019
manager: bpardi
description: 手動安裝教學路徑
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575968"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a><span data-ttu-id="1219a-103">手動安裝及設定 Office 365 的自訂學習</span><span class="sxs-lookup"><span data-stu-id="1219a-103">Manually installing and configuring Custom Learning for Office 365</span></span>

<span data-ttu-id="1219a-104">Microsoft 自訂學習網頁元件是使用[SharePoint 架構](/sharepoint/dev/spfx/sharepoint-framework-overview)版本1.7.1 進行組建。</span><span class="sxs-lookup"><span data-stu-id="1219a-104">The Microsoft Custom Learning Web Part is build using the [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.</span></span>

<span data-ttu-id="1219a-105">若要手動安裝和設定網頁元件和網站集合，您必須完成下列步驟：</span><span class="sxs-lookup"><span data-stu-id="1219a-105">To manually install and configure the web part and site collection, you will need to complete the following steps:</span></span>

1. <span data-ttu-id="1219a-106">確認您已符合所有必要條件。</span><span class="sxs-lookup"><span data-stu-id="1219a-106">Validate that you have met all the prerequisites.</span></span>
1. <span data-ttu-id="1219a-107">在 Office 365 租使用者應用程式目錄中安裝 customlearning sppkg 檔案。</span><span class="sxs-lookup"><span data-stu-id="1219a-107">Install the customlearning.sppkg file in your Office 365 Tenant App Catalog.</span></span>
1. <span data-ttu-id="1219a-108">布建/識別現代化的通訊網站，以充當 Office 365 主網站的自訂教學。</span><span class="sxs-lookup"><span data-stu-id="1219a-108">Provision/Identify a modern communication site to act as your Custom Learning for Office 365 home site.</span></span>
1. <span data-ttu-id="1219a-109">執行 PowerShell 腳本，它會使用自訂學習依據的適當工件來設定您的租使用者。</span><span class="sxs-lookup"><span data-stu-id="1219a-109">Execute a PowerShell script that will configure your tenant with the appropriate artifacts that Custom Learning depends on.</span></span>
1. <span data-ttu-id="1219a-110">流覽至 CustomLearningAdmin 中的 [.aspx 網站] 頁面，載入管理網頁元件以初始化自訂內容設定。</span><span class="sxs-lookup"><span data-stu-id="1219a-110">Navigate to the CustomLearningAdmin.aspx site page to load the admin web part to initialize the custom content configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1219a-111">必要條件</span><span class="sxs-lookup"><span data-stu-id="1219a-111">Prerequisites</span></span>

<span data-ttu-id="1219a-112">您必須已設定並設定整個租使用者型應用程式目錄。</span><span class="sxs-lookup"><span data-stu-id="1219a-112">You must have set up and configured the tenant-wide App Catalog.</span></span> <span data-ttu-id="1219a-113">請參閱[設定您的 Office 365 租使用者](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)，並遵循 [建立應用程式目錄網站] 區段。</span><span class="sxs-lookup"><span data-stu-id="1219a-113">See [Set up your Office 365 tenant](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) and follow the Create app catalog site section.</span></span> <span data-ttu-id="1219a-114">如果您已布建整個租使用者的應用程式目錄，您將需要存取權將套件上傳至其的帳戶，才可完成此設定程式。</span><span class="sxs-lookup"><span data-stu-id="1219a-114">If your tenant-wide App Catalog has already been provisioned, you will need access to an account that has rights to upload a package to it to complete this setup process.</span></span> <span data-ttu-id="1219a-115">一般來說，此帳戶具有「SharePoint 系統管理員」角色。</span><span class="sxs-lookup"><span data-stu-id="1219a-115">Generally this account has the SharePoint administrator role.</span></span> <span data-ttu-id="1219a-116">若具有該角色的帳戶無法運作，請移至 SharePoint 系統管理中心，並尋找應用程式目錄網站集合的網站集合管理員，並以其中一個網站集合管理員身分登入，或新增網站集合管理員失敗的 SharePoint 系統管理員帳戶。</span><span class="sxs-lookup"><span data-stu-id="1219a-116">If an account with that role does not work, go to the SharePoint admin center and find the Site Collection Administrators for the app catalog site collection and either log in as one of the Site Collection Administrators, or add the SharePoint administrator account that failed to the Site Collection Administrators.</span></span> <span data-ttu-id="1219a-117">您也需要存取屬於 SharePoint 租使用者管理員的帳戶。</span><span class="sxs-lookup"><span data-stu-id="1219a-117">You will also need access to an account that is a SharePoint Tenant Admin.</span></span>

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a><span data-ttu-id="1219a-118">將網頁元件 Upload 至租使用者應用程式目錄</span><span class="sxs-lookup"><span data-stu-id="1219a-118">Upload the web part to the Tenant App Catalog</span></span>

<span data-ttu-id="1219a-119">若要設定 Office 365 的自訂教學，請將 customlearning sppkg 檔案上傳至整個租使用者應用程式目錄並加以部署。</span><span class="sxs-lookup"><span data-stu-id="1219a-119">To set up Custom Learning for Office 365, you upload the customlearning.sppkg file to the tenant-wide App Catalog and deploy it.</span></span> <span data-ttu-id="1219a-120">如需如何將應用程式新增至應用程式目錄的詳細指示，請參閱[Use the App Catalog for the SharePoint Online 環境可使用自訂商務應用程式](/sharepoint/use-app-catalog)。</span><span class="sxs-lookup"><span data-stu-id="1219a-120">See [Use the App Catalog to make custom business apps available for your SharePoint Online environment](/sharepoint/use-app-catalog) for detailed instructions on how to add an app to the app catalog.</span></span>

## <a name="provisionidentify-modern-communication-site"></a><span data-ttu-id="1219a-121">布建/識別新式通訊網站</span><span class="sxs-lookup"><span data-stu-id="1219a-121">Provision/Identify Modern Communication Site</span></span>

<span data-ttu-id="1219a-122">請識別現有的 SharePoint 通訊網站，或在您的 SharePoint Online 租使用者中布建新的網站。</span><span class="sxs-lookup"><span data-stu-id="1219a-122">Either identify an existing SharePoint communication site or provision a new one in your SharePoint Online tenant.</span></span> <span data-ttu-id="1219a-123">如需如何布建通訊網站的詳細資訊，請參閱[在 SharePoint Online 中建立通訊網站](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)，並遵循步驟來建立通訊網站。</span><span class="sxs-lookup"><span data-stu-id="1219a-123">For more information about how to provision a communication site, see [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) and follow the steps to create a communication site.</span></span>

## <a name="set-permissions-for-the-site"></a><span data-ttu-id="1219a-124">設定網站的許可權</span><span class="sxs-lookup"><span data-stu-id="1219a-124">Set permissions for the site</span></span>

<span data-ttu-id="1219a-125">您將會想要新增的每個人都應該能夠在訪客群組中查看內容，以及應該能夠將自訂播放清單管理至 Members 群組的所有人。</span><span class="sxs-lookup"><span data-stu-id="1219a-125">You will want to add everyone who should be able to view content to the Visitors group and everyone who should be able to administer custom playlists to the Members group.</span></span> <span data-ttu-id="1219a-126">若要在使用者第一次必須是網站集合管理員或擁有者群組的一部分時設定自訂學習的網站。</span><span class="sxs-lookup"><span data-stu-id="1219a-126">To configure the site for Custom Learning the first time the user must be either a site collection administrator or part of the Owners group.</span></span>

<span data-ttu-id="1219a-127">將 Office 365 應用程式的自訂學習新增至網站集合。</span><span class="sxs-lookup"><span data-stu-id="1219a-127">Add Custom Learning for Office 365 App to the site collection.</span></span>

## <a name="execute-powershell-configuration-script"></a><span data-ttu-id="1219a-128">執行 PowerShell 設定腳本</span><span class="sxs-lookup"><span data-stu-id="1219a-128">Execute PowerShell Configuration Script</span></span>

<span data-ttu-id="1219a-129">您必須執行 PowerShell 腳本 `CustomLearningConfiguration.ps1` ，才能建立解決方案所使用的三個 [租使用者屬性](/sharepoint/dev/spfx/tenant-properties) 。</span><span class="sxs-lookup"><span data-stu-id="1219a-129">A PowerShell script `CustomLearningConfiguration.ps1` is included that you will need to execute to create three [tenant properties](/sharepoint/dev/spfx/tenant-properties) that the solution uses.</span></span> <span data-ttu-id="1219a-130">此外，腳本會在網站頁面庫中建立兩個 [單一元件應用程式頁面](/sharepoint/dev/spfx/web-parts/single-part-app-pages) ，以裝載系統管理員和使用者網頁元件的已知位置。</span><span class="sxs-lookup"><span data-stu-id="1219a-130">In addition, the script creates two [single part app pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in the site pages library to host the admin and user web parts at a known location.</span></span>

### <a name="disabling-telemetry-collection"></a><span data-ttu-id="1219a-131">停用遙測集合</span><span class="sxs-lookup"><span data-stu-id="1219a-131">Disabling Telemetry Collection</span></span>

<span data-ttu-id="1219a-132">此解決方案的一部分包含匿名遙測追蹤加入宣告，其預設為 [開啟]。</span><span class="sxs-lookup"><span data-stu-id="1219a-132">Part of this solution includes anonymized telemetry tracking opt-in, which by default is set to on.</span></span> <span data-ttu-id="1219a-133">如果您正在執行手動安裝，而您想要關閉遙測追蹤，請變更腳本， `CustomlearningConfiguration.ps1` 以設定 $false 的 $optInTelemetry 變數。</span><span class="sxs-lookup"><span data-stu-id="1219a-133">If you are performing a manual install and you would like to turn telemetry tracking off, change the `CustomlearningConfiguration.ps1` script to set the $optInTelemetry variable to $false.</span></span>

<span data-ttu-id="1219a-134">如果您未執行手動安裝，且想要關閉遙測追蹤功能，當執行時，會包含另一個腳本，以 `TelemetryOptOut.ps1` 停用遙測追蹤。</span><span class="sxs-lookup"><span data-stu-id="1219a-134">If you are not performing a manual install and would like to turn telemetry tracking off, a separate script `TelemetryOptOut.ps1` has been included that when run will disable telemetry tracking.</span></span>

## <a name="initialize-web-part-custom-configuration"></a><span data-ttu-id="1219a-135">初始化網頁元件的自訂設定</span><span class="sxs-lookup"><span data-stu-id="1219a-135">Initialize web part custom configuration</span></span>

<span data-ttu-id="1219a-136">成功執行 PowerShell 腳本後，請流覽至 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。</span><span class="sxs-lookup"><span data-stu-id="1219a-136">After the PowerShell script is successfully run, navigate to `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="1219a-137">這會初始化 CustomConfig 清單專案，以設定第一次使用的自訂學習。</span><span class="sxs-lookup"><span data-stu-id="1219a-137">This initializes the CustomConfig list item that sets up custom learning for its first use.</span></span>

<span data-ttu-id="1219a-138">設定現在已完成，您可以使用 Office 365 的自訂學習來向前移動。</span><span class="sxs-lookup"><span data-stu-id="1219a-138">The configuration is now complete and you can move forward with using Custom Learning for Office 365.</span></span> <span data-ttu-id="1219a-139">如需詳細資訊，請參閱使用者檔。</span><span class="sxs-lookup"><span data-stu-id="1219a-139">See the user documentation for more information.</span></span>
