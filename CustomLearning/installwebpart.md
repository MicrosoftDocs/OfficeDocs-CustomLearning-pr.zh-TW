---
author: karuanag
ms.author: karuanag
title: 安裝學習方案網頁組件的自訂
ms.date: 02/10/2019
description: 自訂學習解決方案的網頁組件的安裝指示
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989684"
---
# <a name="installing-the-custom-learning-solution-webpart"></a>安裝學習方案網頁組件的自訂

## <a name="prerequisites-for-a-tenant-wide-installation"></a>租用戶全安裝必要條件

- 若要安裝自訂學習網頁組件整個承租人必須 Office 365 管理權限。 如果您沒有這些權限您可以使用 Office 365 系統管理員或安裝個別的網站集合的網頁組件。
- 您或 Office 365 系統管理員必須已安裝並設定整個租用戶的[應用程式目錄](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[網站集合的應用程式目錄](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)網頁組件會收到。]
- 我們支援 SharePoint Online 僅。網頁組件中不支援任何版本的 SharePoint 內部部署上進行安裝。

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>將自訂學習網頁組件新增至您的租用戶 

1. 下載自訂學習網頁組件並將它儲存到本機磁碟。 此檔案命名為"ms-自訂-learning.sppkg"。 未變更的名稱或檔案的尾碼。 
2. 您的租用戶的瀏覽至 [ [Office 365 系統入口網站](https://admin.microsoft.com/AdminPortal/Home#/homepage)
3. 左導覽列中選取 [Admin 中心、 SharePoint]。如此會開啟新] 索引標籤中，在 SharePoint 系統管理中心中選取 [應用程式、 應用程式目錄、 SharePoint 相關應用程式 
4. 選取 [上傳網頁組件並選擇您下載的"ms-自訂-learning.sppkg"檔案
5. 此租用戶全安裝的核取方塊旁邊"使此解決方案可在組織中所有置於桌"。  
 
> [!NOTE]
> 安裝網頁組件後您會發現您在 SharePoint Online 中的網頁組件庫中。 **在圖庫中的網頁組件是名為"Microsoft Learning"**

![部署方案](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a>Microsoft Learning 網頁組件新增至 SharePoint Online 頁面

自訂學習已安裝在您的租用戶之後您可以新增網頁組件至 SharePoint 頁面。當您執行 Office 365 和 Windows 10 訓練可供您的網站。

1. 全形欄版面配置中新增自訂學習網頁組件：

![SharePoint 頁面版面配置](media/clo365fullcolumnwidth.png)

2. 在 [SharePoint] 頁面上，選取 [新增區段，然後選取全形欄。 您會看到下列提示：

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. 選取 [Microsoft Learning。 您現在應該會看到下列： 

![學習網頁組件的自訂](media/clo365addwebpart.png)

 您現在可以按一下 [並排顯示來探索解決方案所含的預設的內容。  

### <a name="next-steps"></a>後續步驟
- 探索網頁組件中所包含的[預設內容](webpartcontent.md)。
- [自訂](customization.md)您的組織的訓練經驗。
- [磁碟機採用](driveadoption.md)的訓練解決方案。

