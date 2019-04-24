---
author: pkrebs
ms.author: pkrebs
title: 獨立單獨的網頁組件設定
ms.date: 02/10/2019
description: 了解 Office 365 手動網頁組件設定的自訂
ms.openlocfilehash: 8bf6292518c36eda74a49f9968c8e0559fcf8320
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055056"
---
# <a name="stand-alone-web-part-setup"></a>獨立單獨的網頁組件設定

自訂學習提供手動、 突顯單獨網頁組件安裝程式已建立 SharePoint Online 新式通訊網站專用於訓練，這些組織或，只想要設定在自己的自訂學習網頁組件通訊網站。 請注意，手動設定需要使用 Windows PowerShell 與 SharePoint Online 管理命令介面的體驗。 手動設定為，如下所示的自訂學習網頁組件的步驟：

- 驗證您已符合所有必要條件。
- 在您 Office 365 租用戶的應用程式目錄中安裝 customlearning.sppkg 檔案。
- 佈建/識別做為 Office 365 首頁網站的自訂學習新式通訊網站。
- 執行 PowerShell 指令碼，將會使用適當的成品，取決於自訂學習設定您的租用戶。
- 瀏覽至 [CustomLearningAdmin.aspx 網站] 頁面上載入系統管理網頁組件，以初始化自訂的內容設定。

> [!NOTE]
> 如果您要尋找的快速，簡單的方法來設定自訂學習，請參閱 <<c0>佈建自訂學習。

## <a name="prerequisites"></a>必要條件
若要確保成功的手動安裝程式自訂學習網頁組件，必須符合下列必要條件。 

- 您必須已安裝並設定為全租用戶應用程式目錄。 請參閱[設定您的 Office 365 租用戶](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)和遵循 [建立應用程式目錄網站] 區段。 
- 如果已提供您的全租用戶應用程式目錄將需要有它才能完成此安裝程序上傳套件的權限帳戶的存取權。 通常這是具有 SharePoint 系統管理員角色的帳戶。 
- 如果具有該角色的帳戶未運作，移至 SharePoint 系統管理中心和應用程式目錄網站集合及其中一個記錄檔中的尋找網站集合管理員為下列其中一個網站集合管理員，或新增 SharePoint 系統管理員帳戶會失敗，網站集合管理員。 
- 您也必須是 SharePoint 租用戶管理員帳戶的存取權

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>步驟 1-取得從 GitHub 的網頁組件套件和安裝指令碼
安裝程序的一部分，您需要自訂學習網頁組件套件和 PowerShell 安裝指令碼。

- 移[自訂學習 GitHub 儲存機制](https://github.com/pnp/custom-learning-office-365)。
- 按一下 [**下載**] 來將網頁組件套件和指令碼儲存到本機磁碟機。 您會使用指令碼和網頁組件套件中稍後的步驟，此程序。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步驟 2-上傳至租用戶應用程式目錄的網頁組件
若要設定自訂學習運作的 Office 365，您 customlearning.sppkg 檔案上傳至全租用戶應用程式目錄，並將它部署。 請如需如何將應用程式新增至應用程式目錄的詳細指示，參閱[使用應用程式目錄]，以讓 SharePoint Online 環境適用的自訂商務應用程式](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>步驟 3-佈建/識別新式通訊網站
識別現有的 SharePoint 通訊網站或是佈建一個新 SharePoint Online 租用戶中。 如需有關如何佈建通訊網站請參閱[建立通訊網站在 SharePoint Online 中](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)，並遵循步驟來建立通訊網站。

## <a name="step-4---add-the-custom-learning-for-office-365-app-to-the-site"></a>步驟 4-新增至網站的 Office 365 應用程式自訂學習

1. 從 SharePoint 網站上，按一下 [系統] 功能表，然後按一下 [**新增應用程式**。 
2. 在**您的應用程式**下, 按一下 [**從 Your Organization**，，，然後按一下 [**自訂學習運作的 Office 365**。 

## <a name="step-5---set-permissions-for-the-site"></a>步驟 5-設定網站的權限
請確定下列權限設定的網站：
- **網站集合管理員或擁有者群組之一部分**的初始化設定為其第一次使用的自訂學習 CustomConfig 清單項目所需的權限。 
- **成員群組**管理自訂學習，包括 [隱藏] 和 [顯示內容和管理自訂播放清單所需的權限
- **訪客 」 群組**-檢視網站內容所需的權限。 

## <a name="step-6--execute-powershell-configuration-script"></a>步驟 6-執行 PowerShell 設定指令碼
PowerShell 指令碼`CustomLearningConfiguration.ps1`是包含您想要執行建立解決方案使用的三個[租用戶屬性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 除了指令碼會建立兩個[單一的組件應用程式頁面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)網站頁面] 程式庫以裝載在已知位置上的系統管理員和使用者網頁組件。

1. 如果您已經尚未下載 SharePoint Online 管理命令介面，請立即下載。 請參閱[SharePoint Online 管理命令介面下載](https://go.microsoft.com/fwlink/p/?LinkId=255251)。
2. 您可能需要將 PowerShell 執行原則，以執行指令碼。 如需詳細資訊，請參閱 <<c0>關於執行原則。
3. 執行`CustomLearningConfiguration.ps1`指令碼。 除了您的租用戶系統管理員認證，指令碼會提示您輸入您的租用戶名稱和網站名稱。 考慮您網站的 URL，如下列範例會`https://contoso.sharepoint.com/sites/O365CL`、`contoso`是租用戶名稱和`O365CL`為網站名稱。 

### <a name="disabling-telemetry-collection"></a>停用遙測集合
此解決方案的一部分包含匿名的遙測追蹤選擇] 中，預設設定為 [開啟。 如果您正在執行手動安裝，且您想要開啟遙測關閉追蹤，請變更`CustomlearningConfiguration.ps1`$optInTelemetry 變數設 $false 並執行指令碼的指令碼。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>驗證成功佈建並初始化 CustomConfig 清單

成功執行的 PowerShell 指令碼之後，您瀏覽至網站，初始化**CustomConfig**清單項目，如其第一次使用，會設定自訂學習，驗證網站正常運作。

- 請移至 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 開啟**CustomLearningAdmin.aspx**初始化設定為第一次使用的自訂學習**CustomConfig**清單項目。 您應該會看到看起來像這樣的頁面：

![cg adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>將擁有者新增至網站
租用戶系統管理員，也不太可能您要自訂網站，讓您將需要指派至網站的幾個擁有者的人。 讓他們可以修改網站頁面並 rebrand 網站擁有人在網站上擁有系統管理權限。 他們也能夠隱藏和顯示內容傳遞到自訂學習網頁組件。 此外，他們必須能夠建置自訂播放清單，並將它們指派給自訂的子類別。  

1. 從 SharePoint**設定**] 功能表中，按一下 [**網站權限**]。
2. 按一下 [**進階權限設定**。
3. 按一下 [**自訂學習 for Office 365 擁有者**。
4. 按一下 [**新增** > **將使用者新增到這個群組**，然後新增您想要做為擁有者的人員。 
5. 在共用郵件中，將連結新增至[瀏覽網站](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore)，然後按一下 [**共用**]。

### <a name="next-steps"></a>後續步驟
- [自訂](custom_overview.md)您組織的訓練體驗。

