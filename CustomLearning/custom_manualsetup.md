---
author: pkrebs
ms.author: pkrebs
title: 學習路徑手動設定
ms.date: 07/06/2020
description: Microsoft 365 學習路徑手動設定
ms.service: sharepoint online
ms.openlocfilehash: 511b4e5d7d251a1e3fbffcefb01d4ba1f139e5a1
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2021
ms.locfileid: "51163070"
---
# <a name="learning-pathways-manual-setup"></a>學習路徑手動設定

Microsoft 365 教學路徑為需要支援下列其中一種案例的組織提供手動設定： 

- 您的組織具有專用於訓練的 SharePoint 線上新式通訊網站，且您想要將學習路徑新增至該網站。 在此情況下，尚未在網站上設定「學習路徑」網頁元件。

- 您想要在其中一個組織的 SharePoint 通訊網站中，安裝多種語言支援的學習路徑。 該網站的預設語言不是英文，也就是學習路徑所支援的語言之一。 以下是學習路徑支援的語言：

- 英文
- 簡體中文
- 法文
- 德文
- 義大利文 (義大利)
- 日本 (日本) 
- 葡萄牙文 (巴西) 
- 俄文 (俄文) 
- 西班牙文

手動設定學習路徑需要使用 Windows PowerShell 和 SharePoint 線上管理命令介面。 以下是手動設定學習路徑的步驟概述： 

- 確認您已符合所有必要條件。
- 檢查網站的預設語言設定。 若確定，請繼續手動安裝。 如果您需要不同的預設語言設定，則需要建立新的網站。 
- 在 SharePoint 租使用者應用程式目錄中安裝 customlearning sppkg 檔案。
- 布建/識別現代化的通訊網站，以充當您的 Microsoft 365 教學路徑主網站。
- 執行 PowerShell 腳本，它會將您的租使用者設定為教學路徑所依據的工件。
- 流覽至 CustomLearningAdmin 中的 [.aspx 網站] 頁面，載入管理網頁元件以初始化自訂內容設定。

## <a name="prerequisites"></a>必要條件
為了確保成功手動設定「學習路徑」網頁元件，必須符合下列必要條件。 

- 您必須已設定並設定整個租使用者型應用程式目錄。 請參閱 [設定您的 Office 365 租使用者](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) ，並遵循「建立應用程式目錄」網站一節。 
- 如果您已布建整個租使用者的應用程式目錄，您必須存取具有上傳套件之許可權的帳戶。 一般來說，此帳戶具有 SharePoint 系統管理員角色。 
- 若具有該角色的帳戶不能運作，請移至 SharePoint 系統管理中心，並尋找應用程式目錄網站集合的網站集合管理員，並以其中一個網站集合管理員身分登入，或新增網站集合管理員失敗的 SharePoint 系統管理員帳戶。 
- 您也需要存取屬於 SharePoint 租使用者管理員的帳戶。

## <a name="step-1---check-your-language-settings"></a>步驟 1-檢查您的語言設定
作為手動安裝程式的第一步，請檢查您的網站語言設定。 可能的選項如下：

### <a name="option-1---you-dont-want-multilingual-support"></a>選項 1-您不想要多語言支援
如果您不想要對網站進行多語言支援，請確定已關閉該功能。
1.  在 SharePoint 通訊網站上，選取 [**設定**  >  **網站資訊**]。請查看 [  >  **所有網站設定**]  >  **語言設定**。 
2.  將 [ **允許翻譯成多種語言的頁面和新聞** ] 設定為 [ **關閉**]。
3.  按一下 **[儲存]**。 
4.  繼續進行步驟2。

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>選項 2-您想要多語言支援，並使用預設語言確定
SharePoint 通訊網站具有預設語言。 預設語言會決定您用來查看學習路徑的語言，包括「學習路徑管理」頁面。 在初次建立網站時設定預設語言設定，此後便無法變更。 在使用手動設定 Continueing 之前，請先確定您是使用目標網站的預設語言。

1.  在 SharePoint 通訊網站上，選取 [**設定**  >  **網站資訊**]。請查看 [  >  **所有網站設定**]  >  **語言設定**。 
2.  將 [ **允許翻譯成多種語言的頁面和新聞** ] 設定為 [ **開啟**]。
    - 如果您在 [ **語言**] 底下的 [清單] 上方顯示語言，您可以新增其他語言，然後按一下 [ **儲存**]。 繼續進行步驟2。
    - 如果您想要使用不同的預設語言做為網站的選取專案，您必須以您想要的語言來建立新的 SharePoint 通訊網站。 繼續進行選項3。 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>選項 #3-您想要多語言支援，但想要為網站使用不同的預設語言
使用此選項，您可以使用您想要的預設語言來建立新的 SharePoint 線上通訊網站，然後設定網站的語言設定。 
1.  若要建立新的 SharePoint 通訊網站，請參閱 [在線上 SharePoint 建立通訊網站](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)。 在建立網站時，請務必將語言設為您想要用於學習路徑的預設語言。 
2. 在您建立的網站上，選取 [**設定**  >  **網站資訊**]，以  >  **查看 [所有網站設定**  >  **語言設定**]。 
2.  將 [ **允許翻譯成多種語言的頁面和新聞** ] 設定為 [ **開啟**]。
3. 如有必要，請新增其他語言，然後按一下 [ **儲存**]。 
4. 繼續進行步驟2。 

>!記如果您需要將自訂內容從網站遷移至新建立的網站，請參閱本檔稍後的「遷移自訂內容」一節。 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>步驟 2-從 GitHub 取得網頁元件套件和安裝程式腳本
在設定過程中，您將需要 Microsoft 365 學習路徑網頁元件套件和 PowerShell 安裝程式腳本。

- 移 [GitHub 存放庫的學習路徑](https://github.com/pnp/custom-learning-office-365)。
- 按一下 [ **下載** ]，將網頁元件套件和腳本儲存至本機磁片磁碟機。 在此程式的後續步驟中，您將會使用腳本和網頁元件套件。

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>步驟 2-將網頁元件上傳至租使用者應用程式目錄
若要設定 Microsoft 365 學習路徑，請將 customlearning 檔案上傳至整個租使用者的應用程式目錄，並加以部署。 如需如何將應用程式新增至應用程式目錄的詳細指示，請參閱 [Use The App Catalog for the SharePoint Online 環境可使用自訂商務應用程式](/sharepoint/use-app-catalog) 。

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>步驟 3-布建/識別現代通訊網站
請識別現有的 SharePoint 通訊網站，或在您的 SharePoint Online 租使用者中布建新的網站。 如需如何布建通訊網站的詳細資訊，請參閱 [在 SharePoint Online 中建立通訊網站](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) ，並遵循步驟來建立通訊網站。

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>步驟 4-將 Microsoft 365 學習路徑應用程式新增至網站

1. 在 SharePoint 網站上，按一下 [系統] 功能表，然後按一下 [ **新增應用程式**]。 
2. 在 [ **您的應用程式**] 下，按一下 **您的組織**，然後按一下 [ **Office 365 的學習路徑**]。 

## <a name="step-5---set-permissions-for-the-site"></a>步驟 5-設定網站的許可權
請確定已為網站設定下列許可權：
- **網站集合管理員或擁有者群組的一部分** -初始化 CustomConfig 清單專案以設定第一次使用的學習路徑時所需的許可權。 
- **Members 群組** -管理學習路徑所需的許可權，包括隱藏及顯示內容，以及管理自訂播放清單
- **訪客群組** -查看網站內容所需的許可權。 

## <a name="step-6--execute-powershell-configuration-script"></a>步驟 6-執行 PowerShell 設定腳本
您必須執行 PowerShell 腳本 `CustomLearningConfiguration.ps1` ，才能建立解決方案所使用的三個 [租使用者屬性](/sharepoint/dev/spfx/tenant-properties) 。 此外，腳本會在網站頁面庫中建立兩個 [單一元件應用程式頁面](/sharepoint/dev/spfx/web-parts/single-part-app-pages) ，以裝載系統管理員和使用者網頁元件的已知位置。

1. 若尚未下載 SharePoint 線上管理命令介面，請立即下載。 請參閱 [SharePoint 線上管理命令介面下載](https://go.microsoft.com/fwlink/p/?LinkId=255251)。
2. 您可能需要設定 PowerShell 執行原則，以執行腳本。 如需詳細資訊，請參閱 [關於執行原則](/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。
3. 執行 `CustomLearningConfiguration.ps1` 腳本。 除了您的租使用者系統管理員認證之外，腳本會提示您輸入租使用者名稱和網站名稱。 考慮網站 URL 的下列範例， `https://contoso.sharepoint.com/sites/O365CL` `contoso` 是租使用者名稱，也就是 `O365CL` 網站名稱。 

### <a name="disabling-telemetry-collection"></a>停用遙測集合
此解決方案的一部分包括匿名遙測追蹤加入宣告，預設為 [開啟]。 如果您正在執行手動安裝，而您想要關閉遙測追蹤，請變更 `CustomlearningConfiguration.ps1` 腳本以設定 $optInTelemetry 變數，以 $false 並執行腳本。

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>驗證布建成功和初始化 CustomConfig 清單

成功執行 PowerShell 腳本後，您會流覽至網站、初始化 **CustomConfig** 清單專案，以設定第一次使用的學習路徑，以及驗證網站是否正常運作。

- 移至`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 開啟 **CustomLearningAdmin.aspx** 來初始化 **CustomConfig** 清單項目，該清單項目會為第一次使用設定學習路徑。 您應該會看到如下所示的頁面：

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>將擁有者新增至網站
作為租使用者系統管理員，您不太可能是自訂網站的人員，所以您必須將少數擁有者指派給網站。 擁有者具有網站的管理許可權，可供使用者修改網站頁面及才能重塑網站。 他們也可以隱藏及顯示透過「學習路徑」網頁元件傳遞的內容。 此外，他們還可以建立自訂的播放清單並將其指派給自訂子類別。  

1. 在 [SharePoint **設定** ] 功能表中，按一下 [ **網站許可權**]。
2. 按一下 [ **高級許可權設定**]。
3. 按一下 [ **Office 365 擁有者的學習路徑**]。
4. 按一下 [**新增**  >  **使用者至此群組**]，然後新增您想要成為擁有者的人員。 
5. 在 [共用郵件] 中新增 [流覽網站的](https://docs.microsoft.com/Office365/CustomLearning/custom_explore) 連結，然後按一下 [ **共用**]。

## <a name="migrate-custom-content"></a>遷移自訂內容
依照上述步驟重新建立學習路徑網站後，您必須移動 **CustomPlaylists** 清單和 **CustomAssets** 清單的內容。 您也可以選擇性地移動實際自訂資產的自訂頁面，如果這些頁面位於現有的學習路徑網站中，您也可以將它刪除。 由於 **CustomPlaylists** 清單中的所有專案，此工作可能會很困難，因為 **CustomAssets** 清單中的清單專案識別碼會隱藏在每個播放清單專案的 JSONData 欄位中。 所以，只要將 **CustomPlaylists** 清單的內容從一個網站移至另一個網站，就無法滿足要求。 此外， **CustomAssets** 清單會在清單專案的 [JSONData] 欄位中包含自訂資產頁面的絕對 URL。 若資產未移動，且未重新命名網站 (因此會將絕對 URL 變更為資產頁面) ，則 **CustomAssets** 可以保留。 不過，您必須手動修正專案。 由於這種遷移類型的複雜度，我們建議您考慮登記我們的一個學習路徑合作夥伴，以協助您進行這項轉換。 

### <a name="next-steps"></a>後續步驟
- 請參閱 [自訂學習路徑](custom_overview.md)。 
- 請參閱 [翻譯網站頁面](custom_translate_page_ml.md)。