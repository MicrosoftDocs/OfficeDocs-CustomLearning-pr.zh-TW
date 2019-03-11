---
author: pkrebs
ms.author: pkrebs
title: 佈建自訂學習網站
ms.date: 02/10/2019
description: 佈建 SharePoint 佈建引擎透過 Office 365 網站自訂學習
ms.openlocfilehash: 83d76d2d12e9dfc0f39ef55c58443cb3fda2a2d9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523586"
---
# <a name="provision-custom-learning"></a>佈建自訂學習

SharePoint Online 佈建服務時，Office 365 租用戶系統管理員可以啟動簡單按幾下的佈建程序。 佈建服務是佈建自訂學習建議的方式。 它是快速又簡單，而且只需幾分鐘開始程序。 開始之前與佈建服務，但請確定您已符合佈建的必要條件。

## <a name="prerequisites"></a>必要條件
 
若要成功設定自訂學習與[SharePoint Online 佈建服務](https://provisioning.sharepointpnp.com)的佈建服務，執行佈建的人員必須符合下列先決條件： 
 
- 佈建自訂學習的人員必須是租用戶 Administratorof 租用戶會佈建自訂學習。  
- 租用戶應用程式目錄必須能夠使用中的 SharePoint 系統管理中心的 [應用程式] 選項。 如果您的組織沒有 SharePoint 租用戶應用程式目錄，請參閱[SharePoint Online 的文件](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog)建立一個。  
- 佈建自訂學習的人員必須是租用戶應用程式目錄網站集合擁有人。 如果佈建自訂學習人員不是網站集合擁有人的應用程式目錄[完成這些指示](addappadmin.md)，並繼續執行。 

### <a name="to-provision-custom-learning"></a>若要佈建自訂學習

1. 移至 [ http://provisioning.sharepointpnp.com ，並從 [首頁] 頁面的右上角的 [**登入**。  使用認證登入您要安裝網站範本已設定目標租用戶。

![pnphome.png](media/inst_signin.png)

2. 清除**同意代表您的組織**，然後選取 [**接受**]。

![在](media/inst_perms.png)

3. 從解決方案庫中選取**自訂學習運作的 Office 365** 。

![在](media/inst_select.png)

4. 從 [解決方案] 首頁上選取 [**新增至您的租用戶**

![inst_select.png](media/inst_add.png)

5. 完成安裝適當地佈建的 [資訊] 頁面上的欄位。 在最低限度下輸入想要取得以佈建到網站佈建程序與目的地 URL 的相關通知的電子郵件地址。  
> [!NOTE]
> 讓您網站的目的地 URL 至員工，例如 「 / 網站/MyTraining 」 或 「 / teams/LearnOffice365 「 易記的某個項目。

![inst_options.png](media/inst_options.png)

6. 選取 [**佈建**時安裝自訂學習到您的租用戶環境準備就緒]。  佈建程序需要 15 分鐘。 將會透過 （若要在佈建] 頁面所輸入的通知電子郵件地址） 的電子郵件通知您該網站時可供存取。

> [!IMPORTANT]
> 租用戶系統管理員佈建自訂學習網站必須移至網站，並再開啟 [CustomLearningAdmin.aspx 初始化自訂學習系統屬性。 現階段，租用戶系統管理員也應該將指派擁有者至網站。 

## <a name="validate-provisioning-success"></a>驗證佈建成功

佈建完成時，租用戶系統管理員會收到一封電子郵件從 PnP 佈建服務。 系統管理員可以將連結複製到提供的電子郵件中的網站，然後依照 [移至網站的指示。 或者，租用戶系統管理員可以瀏覽至 [<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx。 這會初始化為其第一次使用設定自訂學習 CustomConfig 清單項目。 第一次開啟此頁面上的人員必須是租用戶系統管理員、 網站集合管理員或網站擁有者。 您應該會看到看起來像這樣的頁面： 

## <a name="add-owners-to-site"></a>將擁有者新增至網站
租用戶系統管理員，也不太可能您要自訂網站，讓您將需要指派至網站的擁有者的人。 讓他們可以修改網站頁面並 rebrand 網站擁有人在網站上擁有系統管理權限。 他們也能夠隱藏和顯示內容傳遞到自訂學習網頁組件。 他們也必須建立自訂播放清單，並將它們指派給自訂的子類別的能力。  

1. 從 SharePoint**設定**] 功能表中，按一下 [**網站權限**]。
2. 按一下 [**進階權限設定**。
3. 按一下 [**自訂學習 for Office 365 擁有者**。
4. 按一下 [**新增** > **將使用者新增到這個群組**，新增您想要擁有者的人員，然後按一下 [**共用**。

8. 按一下**下列**選項中的右上角的頁面追蹤網站。  

### <a name="next-steps"></a>後續步驟
- 瀏覽網頁組件中包含[預設的內容](sitecontent.md)。
