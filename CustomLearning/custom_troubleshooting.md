---
author: pkrebs
ms.author: pkrebs
title: 疑難排解自訂學習
ms.date: 02/10/2019
description: 了解如何疑難排解自訂學習
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055082"
---
# <a name="troubleshoot-custom-learning"></a>疑難排解自訂學習

在這裡進行疑難排解時可能發生的問題秘訣與自訂學習 for Office 365 或 SharePoint Online 佈建服務。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>如何知道您是否擁有租用戶系統管理員權限

登入 SharePoint Online 佈建服務和佈建自訂學習需要租用戶系統管理員權限。 如果您急需登入 SharePoint Online 佈建服務的問題，請確定您已獲指派全域系統管理員角色。 自訂學習解決方案需要租用戶系統管理員權限，又稱為 Office 365 全域系統管理員角色。 以下是如何判斷是否您已獲指派全域系統管理員角色。

1.  登入 Office.com。
2.  按一下 [**系統管理**
3.  [**使用者**] 下方選取 [**作用中使用者**
4.  搜尋您的名稱
5.  按一下您在搜尋結果中的名稱。 全域系統管理員應該會看到您的角色。

![cg globaladminrole.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>如果您沒有全域系統管理員角色
- 尋找組織中的全域系統管理員和擁有該登入服務，或已將其指派給您的全域系統管理員角色的人員。

## <a name="tenant-app-catalog-troubleshooting"></a>疑難排解的租用戶應用程式目錄
自訂學習需要應用程式目錄]，以目標租用戶中佈建。 建立的應用程式目錄需要全域系統管理員權限。 以下是為一般應用程式目錄問題進行疑難排解步驟：

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>如何知道您是否擁有租用戶應用程式目錄 
首先，請確定您具備全域系統管理員權限。 請參閱上述的租用戶系統管理員權限的步驟。

1. 從 Office 365 中，按一下 [**系統管理員**，請按一下展開箭頭 >，按一下 [**顯示所有** > **系統管理中心** > **SharePoint**。
2. 按一下 [**傳統系統 SharePoint 管理中心** > **apps** > **應用程式目錄**。
3. 在**應用程式**，您應該會看到標題為**Distribute SharePoint 相關應用程式**的磚。 如果您看到磚，您必須租用戶應用程式目錄。 請參閱以下 [**如何確定您是網站 Colllection...** ] 區段。 如果您沒有看到 [您需要建立您的租用戶的租用戶應用程式目錄] 磚。 請參閱 <<c0>如何建立租用戶應用程式目錄] 區段下方。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>如何確保您的租用戶應用程式目錄網站集合擁有人 
若要自訂學習佈建 Office 365，您必須是租用戶應用程式目錄網站集合擁有人。 以下是如何 determin 如果您是擁有者。

1. 從 Office 365 中，按一下 [**系統管理員**，請按一下展開箭頭 >，按一下 [**顯示所有** > **系統管理中心** > **SharePoint**。
2. 按一下 [**傳統系統 SharePoint 管理中心**]，然後選取 [**應用程式目錄**。
3. 選取**擁有者**，並請確定您是網站集合擁有者。 它看起來應該像這樣。
 
![cg sitecollectionowner.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>如何建立租用戶應用程式目錄，如果其中一個不存在 
1. 使用您的 SharePoint Online 系統管理員帳戶登入 Office 365。
2. 按一下 [**系統**]。
3. 在**系統管理中心**中，按一下 [ **SharePoint**]。 
4. 按一下 [**應用程式** > **應用程式目錄**。
5. 按一下 [**建立新的應用程式目錄網站**]，然後按一下 [**確定]**。 
6.  輸入應用程式目錄的資訊。 您可能想要包含一個以上的系統管理員。 下列範例會示範。  

![cg appcatalogfinish.png](media/cg-appcatalogfinish.png)

7.  這樣就完成了。 您已經完成。 但是，您將移至佈建自訂學習之前，您需要等候至少 30 分鐘，以確定應用程式目錄建立完畢。 

> [!IMPORTANT]
> 請等候至少 30 分鐘後再佈建自訂學習建立租用戶應用程式目錄。 這可確保佈建程序的應用程式目錄是 SharePoint 內完成。 