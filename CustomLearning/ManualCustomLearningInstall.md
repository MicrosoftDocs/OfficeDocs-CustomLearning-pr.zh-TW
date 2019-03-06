# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>以手動方式安裝和設定自訂學習運作的 Office 365

Microsoft 自訂學習網頁組件是使用[SharePoint 架構](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview)版本 1.7.1 的組建。

若要手動安裝及設定網頁組件和網站集合必須完成下列步驟：

1. 驗證您已符合所有必要條件。
1. 在您 Office 365 租用戶的應用程式目錄中安裝 customlearning.sppkg 檔案。
1. 佈建/識別做為 Office 365 首頁網站的自訂學習新式通訊網站。
1. 執行 PowerShell 指令碼，將會使用適當的成品，取決於自訂學習設定您的租用戶。
1. 瀏覽至 [CustomLearningAdmin.aspx 網站] 頁面上載入系統管理網頁組件，以初始化自訂的內容設定。

## <a name="prerequisites"></a>必要條件

您必須已安裝並設定為全租用戶應用程式目錄。 請參閱[設定您的 Office 365 租用戶](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site)和遵循 [建立應用程式目錄網站] 區段。 如果已提供您的全租用戶應用程式目錄將需要有它才能完成此安裝程序上傳套件的權限帳戶的存取權。 通常這是具有 SharePoint 系統管理員角色的帳戶。 如果具有該角色的帳戶未運作，移至 SharePoint 系統管理中心和應用程式目錄網站集合及其中一個記錄檔中的尋找網站集合管理員為下列其中一個網站集合管理員，或新增 SharePoint 系統管理員帳戶會失敗，網站集合管理員。 您也必須是 SharePoint 租用戶管理員帳戶的存取權

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>將網頁組件上傳至租用戶應用程式目錄

若要設定自訂學習運作的 Office 365，您 customlearning.sppkg 檔案上傳至全租用戶應用程式目錄，並將它部署。 請如需如何將應用程式新增至應用程式目錄的詳細指示，參閱[使用應用程式目錄]，以讓 SharePoint Online 環境適用的自訂商務應用程式](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)。

## <a name="provisionidentify-modern-communication-site"></a>佈建/識別新式通訊網站

識別現有的 SharePoint 通訊網站或是佈建一個新 SharePoint Online 租用戶中。 如需有關如何佈建通訊網站請參閱[建立通訊網站在 SharePoint Online 中](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)，並遵循步驟來建立通訊網站。

## <a name="set-permissions-for-the-site"></a>設定網站的權限

您會想要新增所有人應該能夠瀏覽至 [訪客] 群組的內容與其他人應該能夠管理自訂播放清單至成員群組。 若要自訂學習第一次設定網站使用者必須是網站集合管理員或擁有者群組的一部分。

Office 365 應用程式的自訂學習新增至網站集合中。

## <a name="execute-powershell-configuration-script"></a>執行 PowerShell 設定指令碼

PowerShell 指令碼`CustomLearningConfiguration.ps1`是包含您想要執行建立解決方案使用的三個[租用戶屬性](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties)。 除了指令碼會建立兩個[單一的組件應用程式頁面](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages)網站頁面] 程式庫以裝載在已知位置上的系統管理員和使用者網頁組件。

### <a name="disabling-telemetry-collection"></a>停用遙測集合

此解決方案的一部分包含匿名的遙測追蹤選擇] 中，預設設定為 [開啟。 如果您正在執行手動安裝，且您想要開啟遙測關閉追蹤，請變更`CustomlearningConfiguration.ps1`$optInTelemetry 變數設為 $false 指令碼。

如果您未執行手動安裝，並可能會想要開啟另一個指令碼關閉追蹤的遙測`TelemetryOptOut.ps1`已包含執行時，會停用遙測追蹤。

## <a name="initialize-web-part-custom-configuration"></a>初始化網頁組件自訂設定

成功執行的 PowerShell 指令碼之後，瀏覽至`<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`。 這會初始化會設定為其第一次使用的自訂學習 CustomConfig 清單項目。

現在完成組態時，您可以使用 Office 365 使用自訂學習向前移動。 請參閱如需詳細資訊的使用者文件。