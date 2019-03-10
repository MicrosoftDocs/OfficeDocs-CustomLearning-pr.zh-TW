---
author: pkrebs
ms.author: pkrebs
title: 獨立單獨的網頁組件設定
ms.date: 02/10/2019
description: 了解 Office 365 手動網頁組件設定的自訂
ms.openlocfilehash: 650e6c12ebe8ca7fedc6edc107b5822c48ead99a
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411873"
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

## <a name="step-4---set-permissions-for-the-site"></a>步驟 4-設定網站的權限
請確定下列權限設定的網站：
- **網站集合管理員或擁有者群組之一部分**的初始化設定為其第一次使用的自訂學習 CustomConfig 清單項目所需的權限。 
- **成員群組**管理自訂學習，包括 [隱藏] 和 [顯示內容和管理自訂播放清單所需的權限
- **訪客 」 群組**-檢視網站內容所需的權限。 

## <a name="step-5--execute-powershell-configuration-script"></a>步驟 5-執行 PowerShell 設定指令碼
PowerShell 指令碼`CustomLearningConfiguration.ps1`是包含您想要執行建立解決方案使用的三個[租用戶屬性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 除了指令碼會建立兩個[單一的組件應用程式頁面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)網站頁面] 程式庫以裝載在已知位置上的系統管理員和使用者網頁組件。

### <a name="disabling-telemetry-collection"></a>停用遙測集合
此解決方案的一部分包含匿名的遙測追蹤選擇] 中，預設設定為 [開啟。 如果您正在執行手動安裝，且您想要開啟遙測關閉追蹤，請變更`CustomlearningConfiguration.ps1`$optInTelemetry 變數設為 $false 指令碼。

如果您未執行手動安裝，並可能會想要開啟另一個指令碼關閉追蹤的遙測`TelemetryOptOut.ps1`已包含執行時，會停用遙測追蹤。

## <a name="step-6---initialize-web-part-custom-configuration"></a>步驟 6-Initialize 網頁組件自訂設定
成功執行的 PowerShell 指令碼之後，瀏覽至`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 這會初始化為其第一次使用設定自訂學習**CustomConfig**清單項目。

設定現已完成。 若要深入了解如何調整您的環境自訂學習網站和網頁組件，請參閱 < <b0>Customize 訓練體驗</b0>。

### <a name="next-steps"></a>後續步驟
- [自訂](custom_overview.md)您組織的訓練體驗。
