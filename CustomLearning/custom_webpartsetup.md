---
author: pkrebs
ms.author: pkrebs
title: 布建自訂學習網站
ms.date: 02/10/2019
description: 透過 SharePoint 布建引擎提供 Office 365 網站的自訂學習
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: f930eba5815366bcefd2730c88a3c2df3f246dd4
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000319"
---
# <a name="provision-custom-learning"></a>提供自訂學習

使用 SharePoint 線上布建服務，Office 365 租使用者管理員只需稍按一次即可啟動布建程式。 布建服務是提供自訂學習的建議方式。 速度很快，而且只需要數分鐘的時間即可開始處理常式。 在開始布建服務之前，請確定您已符合布建的必要條件。

## <a name="prerequisites"></a>了解必要條件
 
若要使用提供服務 [SharePoint 線上](https://provisioning.sharepointpnp.com)布建服務成功設定自訂教學，進行布建的人員必須符合下列先決條件： 
 
- 人員布建的自訂學習必須是租使用者 Administratorof 的承租人，將會布建自訂教學。  
- 租使用者應用程式目錄必須可在 SharePoint 系統管理中心的 [App] 選項內使用。 如果您的組織沒有 SharePoint 租使用者應用程式目錄，請參閱 [SharePoint 線上檔](/sharepoint/use-app-catalog) 以建立一個。  
- 人員布建的自訂學習必須是租使用者應用程式目錄的網站集合擁有者。 如果人員布建自訂學習不是應用程式目錄的網站集合擁有者，請 [完成這些指示](addappadmin.md) 並繼續。 

### <a name="to-provision-custom-learning"></a>提供自訂學習

1. 前往 http://provisioning.sharepointpnp.com 首頁右上角的位置並登 **入** 。  以您計畫安裝網站範本之目標租使用者的認證登入。
![布建服務主頁面。](media/inst_signin.png)

2. 請清除 **您組織的同意** ，然後選取 [ **接受**]。
![同意畫面](media/inst_perms.png)

3. 從方案庫中選取 **Office 365 的自訂學習** 。
![您為 Office 365 選取自訂學習的畫面。](media/inst_select.png)

4. 從解決方案首頁中，選取 [新增 **至您的租** 使用者] 畫面，以 
 ![ 選取 [新增至您的租使用者]。](media/inst_add.png)

5. 請視安裝需要完成填寫佈建資訊頁面上的欄位。 您可以至少輸入您要取得其布建程式及網站目的地 URL 相關通知的電子郵件地址。  
   > [!NOTE]
   > 將網站的目的地 URL 做為便於員工（如 "/sites/MyTraining" 或 "/teams/LearnOffice365"）的內容。

   ![您提供詳細資料的畫面。](media/inst_options.png)

6. 若準備將自訂教學安裝到您的租使用者環境 **，請選取** [布建]。  佈建程序最多會需要 15 分鐘的時間。 網站準備好供存取時，系統會透過電子郵件通知您 (傳送到您在 [佈建] 頁面輸入的通知電子郵件地址)。

> [!IMPORTANT]
> 布建自訂學習網站的承租人管理員必須移至網站，然後開啟 CustomLearningAdmin 以初始化自訂學習管理屬性。 此時，租使用者管理員也應指派網站的擁有者。 

## <a name="validate-provisioning-success"></a>驗證布建成功

布建完成後，租使用者系統管理員會從 PnP 布建服務接收電子郵件。 系統管理員可以複製電子郵件中提供之網站的連結，然後依照指示移至網站。 另外，租使用者管理員可以流覽 <網站集合 URL>/SitePages/CustomLearningAdmin.aspx。 這會初始化 CustomConfig 清單專案，以設定第一次使用的自訂學習。 第一次開啟此頁面的人員必須是承租人管理員、網站集合管理員或網站擁有者。 您應該會看到如下所示的頁面： 

## <a name="add-owners-to-site"></a>將擁有者新增至網站
作為租使用者系統管理員，您不太可能是自訂網站的人員，所以您必須指派網站的擁有者。 擁有者具有網站的管理許可權，可供使用者修改網站頁面及才能重塑網站。 他們也可以隱藏及顯示透過自訂學習網頁元件傳遞的內容。 他們也可以建立自訂的播放清單並將其指派給自訂子類別。  

1. 在 [SharePoint **設定** ] 功能表中，按一下 [ **網站許可權**]。
2. 按一下 [ **高級許可權設定**]。
3. 按一下 [ **自訂學習的 Office 365 擁有** 者]。
4. 按一下 [**新增**  >  **使用者至此群組**]，新增您要擁有者的人員，然後按一下 [**共用**]。

8. 按一下頁面右上角的 **下列** 選項，以追蹤網站。  
