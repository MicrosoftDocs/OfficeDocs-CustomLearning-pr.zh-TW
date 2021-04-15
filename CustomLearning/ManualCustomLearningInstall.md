---
author: pkrebs
ms.author: pkrebs
title: 手動安裝教學路徑
ms.date: 02/18/2019
manager: bpardi
description: 手動安裝教學路徑
audience: itpro
ms.service: o365-administration
ms.topic: article
ms.openlocfilehash: 212ee8a1517cf79538d4a2d076f60f9382eeaf74
ms.sourcegitcommit: 96ad347dc08694ce2af5a5d42bf1f753d1c30a65
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749311"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>手動安裝及設定 Office 365 的自訂學習

Microsoft 自訂學習網頁元件是使用 [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) 版本1.7.1 建立的。

若要手動安裝和設定網頁元件和網站集合，您必須完成下列步驟：

1. 確認您已符合所有必要條件。
1. 在您的 Office 365 租使用者應用程式目錄中安裝 customlearning sppkg 檔案。
1. 布建/識別現代化的通訊網站，以充當 Office 365 首頁網站的自訂學習。
1. 執行 PowerShell 腳本，它會使用自訂學習依據的適當工件來設定您的租使用者。
1. 流覽至 CustomLearningAdmin 中的 [.aspx 網站] 頁面，載入管理網頁元件以初始化自訂內容設定。

## <a name="prerequisites"></a>必要條件

您必須已設定並設定整個租使用者型應用程式目錄。 請參閱 [設定您的 Office 365 租使用者](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) ，並遵循 [建立應用程式目錄網站] 區段。 如果您已布建整個租使用者的應用程式目錄，您將需要存取權將套件上傳至其的帳戶，才可完成此設定程式。 一般來說，此帳戶具有「SharePoint 系統管理員」角色。 若具有該角色的帳戶無法運作，請移至 SharePoint 系統管理中心，並尋找應用程式目錄網站集合的網站集合管理員，並以其中一個網站集合管理員身分登入，或新增網站集合管理員失敗的 SharePoint 系統管理員帳戶。 您也需要存取屬於 SharePoint 租使用者管理員的帳戶。

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>將網頁元件上傳至租使用者應用程式目錄

若要設定 Office 365 的自訂教學，請將 customlearning 檔案上傳至整個租使用者的應用程式目錄，然後加以部署。 如需如何將應用程式新增至應用程式目錄的詳細指示，請參閱 [Use The App Catalog for the SharePoint Online 環境可使用自訂商務應用程式](/sharepoint/use-app-catalog) 。

## <a name="provisionidentify-modern-communication-site"></a>布建/識別新式通訊網站

請識別現有的 SharePoint 通訊網站，或在您的 SharePoint Online 租使用者中布建新的網站。 如需如何布建通訊網站的詳細資訊，請參閱 [在 SharePoint Online 中建立通訊網站](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) ，並遵循步驟來建立通訊網站。

## <a name="set-permissions-for-the-site"></a>設定網站的許可權

您將會想要新增的每個人都應該能夠在訪客群組中查看內容，以及應該能夠將自訂播放清單管理至 Members 群組的所有人。 若要在使用者第一次必須是網站集合管理員或擁有者群組的一部分時設定自訂學習的網站。

將 Office 365 應用程式的自訂學習新增至網站集合。

## <a name="execute-powershell-configuration-script"></a>執行 PowerShell 設定腳本

您必須執行 PowerShell 腳本 `CustomLearningConfiguration.ps1` ，才能建立解決方案所使用的三個 [租使用者屬性](/sharepoint/dev/spfx/tenant-properties) 。 此外，腳本會在網站頁面庫中建立兩個 [單一元件應用程式頁面](/sharepoint/dev/spfx/web-parts/single-part-app-pages) ，以裝載系統管理員和使用者網頁元件的已知位置。

### <a name="disabling-telemetry-collection"></a>停用遙測集合

此解決方案的一部分包含匿名遙測追蹤加入宣告，其預設為 [開啟]。 如果您正在執行手動安裝，而您想要關閉遙測追蹤，請變更腳本， `CustomlearningConfiguration.ps1` 以設定 $false 的 $optInTelemetry 變數。

如果您未執行手動安裝，且想要關閉遙測追蹤功能，當執行時，會包含另一個腳本，以 `TelemetryOptOut.ps1` 停用遙測追蹤。

## <a name="initialize-web-part-custom-configuration"></a>初始化網頁元件的自訂設定

成功執行 PowerShell 腳本後，請流覽至 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 。 這會初始化 CustomConfig 清單專案，以設定第一次使用的自訂學習。

設定現在已完成，您可以使用 Office 365 的自訂教學進行向前移動。 如需詳細資訊，請參閱使用者檔。
