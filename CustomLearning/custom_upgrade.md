---
author: pkrebs
ms.author: pkrebs
title: 自訂學習升級
ms.date: 02/10/2019
description: 了解 Office 365 手動網頁組件設定的自訂
ms.openlocfilehash: 1dd9fd47b608a20ae0b1dc1937e48524547cc938
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543773"
---
# <a name="manual-upgrade-for-custom-learning"></a>手動升級自訂學習

自訂 Office 365 學習提供手動升級程序中更早的試驗已加入的組織。 升級程序，組織可以繼續使用其目前的自訂學習網站，並將新的增強的自訂學習網頁組件新增至其 SharePoint 應用程式目錄]，然後執行 PowerShell 指令碼升級。 以下提供升級程序的概觀： 

- 驗證負責人的上傳新的網頁組件和執行 Powershell 指令碼具有必要權限
- 將網頁組件、 customlearning.sppkg 檔案上傳至您 Office 365 租用戶的應用程式目錄
- 執行 PowerShell 指令碼，將會使用適當的成品所需的自訂學習設定您的租用戶
- 瀏覽至 [CustomLearningAdmin.aspx] 頁面上，以初始化自訂 Ccontent 設定自訂學習網站中。

## <a name="prerequisites"></a>必要條件
若要確保成功升級的自訂學習，必須符合下列必要條件。 

- 您必須設定全租用戶應用程式目錄。 如果您沒有租用戶應用程式目錄，請參閱[設定您的 Office 365 租用戶](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)，和遵循 [建立應用程式目錄網站] 區段。 
- 如果已佈建您的全租用戶應用程式目錄，您必須具有權限，以將套件上傳至該帳戶的存取權。 通常這是具有 SharePoint 系統管理員角色的帳戶。 
- 如果無法使用具有 SharePoint 系統管理員角色的帳戶： 移至 SharePoint 系統管理中心中，選取 [應用程式目錄，按一下 [擁有者，並以下列其中一個網站集合系統管理員身分登入或失敗的 SharePoint 系統管理員帳戶新增至網站集合系統管理員清單。 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>步驟 1-取得從 GitHub 的網頁組件套件和安裝指令碼
安裝程序的一部分，您需要自訂學習網頁組件套件和 PowerShell 安裝指令碼。

1. 移[自訂學習 GitHub 儲存機制](https://github.com/pnp/custom-learning-office-365)。
2. 按一下 [**複製或下載**，然後**下載 ZIP**。   
3. 將**ZIP**檔案儲存到本機磁碟機上的位置。
4. **ZIP**檔案解壓縮本機磁碟機上。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步驟 2-上傳至租用戶應用程式目錄的網頁組件
若要設定自訂學習運作的 Office 365，您 customlearning.sppkg 檔案上傳至全租用戶應用程式目錄，並將它部署。 請如需如何將應用程式新增至應用程式目錄的詳細指示，參閱[使用應用程式目錄]，以讓 SharePoint Online 環境適用的自訂商務應用程式](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

1. 在 Office 365 中，按一下 [**系統**]。
2. 在**系統管理中心**中，按一下 [ **SharePoint**]。
3. 按一下 [**應用程式** > **應用程式目錄** > **SharePoint 的應用程式散發。**
4. 按一下 [**上傳** > **選擇 [檔案]**。
5. 在資料夾中儲存的 ZIP 檔案的位置，選取 [**網頁組件**] 資料夾中，然後再選取**customlearning.sppkg。**
6. 按一下 **[部署]**。

## <a name="step-3---add-the-custom-learning-for-office-365-app-to-the-site"></a>步驟 3-Office 365 應用程式自訂學習新增至網站

1. 從 SharePoint 網站上，按一下 [系統] 功能表，然後按一下 [**新增應用程式**。 
2. 在**您的應用程式**下, 按一下 [**從 Your Organization**，，，然後按一下 [**自訂學習運作的 Office 365**。 

## <a name="step-4---execute-powershell-configuration-script"></a>步驟 4-執行 PowerShell 設定指令碼
PowerShell 指令碼`CustomLearningConfiguration.ps1`是包含從 GitHub 的 ZIP 下載中。 您要執行指令碼，以建立解決方案使用的三個[租用戶屬性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 此外，該指令碼會建立兩個[單一的組件應用程式頁面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)網站頁面] 程式庫以裝載在已知位置上的系統管理員和使用者網頁組件。 這些應用程式頁面是：

- CustomAdministration.aspx
- CustomViewer.aspx

### <a name="to-run-the-powershell-script"></a>若要執行 Powershell 指令碼
- 使用 PowerShell，執行`CustomLearningConfiguration.ps1`指令碼位於從 GitHub ZIP 的 [網頁組件] 資料夾中。 如果成功，您會看到三個索引鍵/值組和**自訂學習系統管理員被停用了..** 命令視窗中。

### <a name="disabling-telemetry-collection"></a>停用遙測集合
自訂學習包含追蹤的匿名的遙測加入確認程序中，預設設定為 [開啟。 如果您想要開啟遙測關閉追蹤，請變更`CustomlearningConfiguration.ps1`指令碼，以設定`$optInTelemetry`變數設定為`$false`。

## <a name="step-5---initialize-web-part-custom-configuration"></a>步驟 5-Initialize 網頁組件自訂設定
成功執行的 PowerShell 指令碼之後，瀏覽至`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 開啟**CustomLearningAdmin.aspx**初始化設定為第一次使用的自訂學習**CustomConfig**清單項目。 您應該會看到看起來像這樣的頁面：

![cg adminapppage.png](media/cg-adminapppage.png)

現在，升級即完成。 若要深入了解如何調整您的環境自訂學習網站和網頁組件，請參閱 < <b0>Customize 訓練體驗</b0>。

## <a name="upgrade-instructions-for-site-owners"></a>升級網站擁有人的指示
自訂 office 365 學習推出了各種不同的網頁組件的增強功能。 [自訂的學習體驗](custom_overview.md)] 區段中的詳細討論使用網頁組件。 現在，網站擁有者應該：  

- 確認 Office 365 網頁組件自訂學習可用。 
- 在網頁上現有的網頁組件取代為新的網頁組件
- 取代任何連結指向舊的網頁組件

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>確認可用的 Office 365 網頁組件自訂學習
1.  從自訂學習網站上，按一下 [**設定**]，然後按一下 [***新增工作] 頁面**。
2.  按一下 [**+** 新增網頁組件，然後選取 [ **Office 365 的自訂學習**網頁組件] 頁面上的圖示。 [] 頁面上現在看起來應該類似下列的圖形：

[cg adminapppage.png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>使用新的網頁組件取代舊的網頁組件
之前取代自訂學習網頁組件，或對網站進行的變更，我們建議您閱讀的[自訂學習體驗](custom_overview.md)文件，因為它說明如何使用新的網頁組件。 

若要升級的自訂學習網站，取代新的網頁組件的網頁組件的現有執行個體。 雖然我們不能是確定已新增網頁組件，先前的試驗指導已將網頁組件新增至下列頁面，所以請尋找來取代這些頁面上的網頁組件：

- Get-啟動-與-Office-365.aspx
- Get-啟動-與-Microsoft-Teams.aspx
- Get-啟動-與-OneDrive.aspx
- Get-啟動-與-SharePoint.aspx

### <a name="replace-existing-links-to-the-web-part"></a>取代現有連結至網頁組件
具有增強功能至新的網頁組件，它們已變更該您連結到播放清單的方式。 升級的一部分，您應該取代任何連結至網頁組件，包括功能表項目，以及在 [首頁] 頁面的連結。 之前取代自訂學習網頁組件，或對網站進行的變更，我們建議您閱讀的[自訂學習體驗](custom_overview.md)文件，因為它說明如何使用新的網頁組件。 

## <a name="recreate-existing-playlists"></a>重新建立現有播放清單 
若要確保播放清單正常運作，任何播放清單已建立與舊版的網頁組件將會需要重新建立。 在刪除之前播放清單，請自訂播放清單和相關聯的資產清單，讓您以新的自訂學習網頁組件輕鬆重建。 製作一份播放清單，然後予以刪除。 若要刪除之前，先製作一份播放清單的內容，您可以使用 JSONData] 欄位。 這樣會使更新版本建立的工作變得更容易。


1. 從自訂學習網站上，按一下 [**設定** > **網站內容**。 
2. 選取 [播放清單、 選取省略符號、 選取 [**編輯**] 然後**JSONData**欄位的內容複製並儲存 [記事本] 或另一個文件以供日後參考。 選取 [**取消**]。
3. 選取 [播放清單，選取省略符號，，然後選取 [**刪除**。
4. 現在，您就可以重新建立新的網頁組件播放清單。
如需自訂學習使用 Office 365 網頁組件的指示，請參閱 [自訂學習 Experience(custom_overview.md)。

### <a name="next-steps"></a>後續步驟
- [自訂](custom_overview.md)您組織的訓練體驗。

