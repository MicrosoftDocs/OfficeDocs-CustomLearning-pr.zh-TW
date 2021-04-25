---
author: pkrebs
ms.author: pkrebs
title: 疑難排解 Microsoft 365 學習路徑
ms.date: 02/10/2019
description: 深入瞭解如何疑難排解 Microsoft 365 教學路徑
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000299"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>疑難排解 Microsoft 365 教學路徑

以下是 Microsoft 365 教學路徑或 SharePoint 線上布建服務可能發生之問題的疑難排解提示。

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>如何知道您是否有承租人系統管理員許可權

登入 SharePoint 線上布建服務，以及布建自訂學習要求承租人系統管理員許可權。 如果您遇到 SharePoint 線上布建服務的登入問題，請確定您已被指派全域系統管理員角色。 自訂學習解決方案需要租使用者系統管理員許可權，否則稱為 Office 365 全域系統管理員角色。 以下是判斷您是否已被指派全域系統管理員角色的方法。

1.  登入 Office.com。
2.  按一下 [**管理**]
3.  在 [**使用者**] 底下，選取 [作用中 **使用者**]
4.  搜尋您的名稱
5.  按一下搜尋結果中的名稱。 您應該會看到全域管理員的角色。
![列出您的角色以及授權、群組成員資格及其他資訊的範例頁面。](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>如果您沒有全域系統管理員角色
- 尋找組織中的全域系統管理員，讓該人員登入服務，或讓他們為您指派全域系統管理員角色。

## <a name="tenant-app-catalog-troubleshooting"></a>租使用者應用程式目錄疑難排解
自訂學習需要在目標租使用者中布建應用程式目錄。 建立應用程式目錄需要全域管理員許可權。 以下是常見應用程式目錄問題的疑難排解步驟：

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>如何知道您是否有租使用者應用程式目錄 
針對初學者，請確定您具有全域管理員許可權。 請參閱上述租使用者管理員許可權的步驟。

1. 從 Office 365，按一下 [**管理**]，按一下展開箭號 >，然後按一下 [**顯示所有** 系統  >  **管理中心**]  >  **SharePoint**。
2. 按一下 [**傳統系統管理員 SharePoint 中心**  >  **應用**  >  **程式] 應用程式目錄**。
3. 在 [ **應用程式**] 底下，您應該會看到一個貼上標題為「 **散佈應用程式 SharePoint**。 如果您看到的是磚，表示您有租使用者應用程式目錄。 請參閱 how **to 確定您的網站 Colllection ...** ] 區段。 如果您看不到所需的磚，您將需要為您的租使用者建立承租人應用程式目錄。 請參閱 **如何建立租使用者應用程式目錄** 一節。

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>如何確保您是租使用者應用程式目錄上的網站集合擁有者 
若要布建 Microsoft 365 學習路徑，您必須是租使用者應用程式目錄上的網站集合擁有者。 以下是判斷您是否為擁有者的方式。

1. 從 Office 365，按一下 [**管理**]，按一下展開箭號 >，然後按一下 [**顯示所有** 系統  >  **管理中心**]  >  **SharePoint**。
2. 按一下 [ **傳統 Admin SharePoint Center**]，然後選取 **應用程式目錄**。
3. 選取 [ **擁有** 者]，然後確定您是網站集合擁有者。 它看起來應該像這樣。
![管理系統管理員頁面。](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>如何建立租使用者應用程式目錄（若有的話） 
1. 使用您的 SharePoint 線上系統管理員帳戶登入 Office 365。
2. 按一下 [ **管理**]。
3. 在 [系統 **管理中心**] 底下，按一下 [ **SharePoint**]。 
4. 按一下 [**應用**  >  **程式應用程式目錄**]。
5. 按一下 [ **建立新的應用程式目錄網站**]，然後按一下 **[確定]**。 
6.  輸入應用程式目錄的資訊。 您可能想要包含一個以上的系統管理員。 下列範例所示。  
![用於輸入新應用程式目錄資訊的表單。](media/cg-appcatalogfinish.png)

7.  這樣就完成了。 您已經完成。 但在您進入自訂教學之前，您至少需要等候30分鐘，確定應用程式目錄建立已完成。 

> [!IMPORTANT]
> 在建立承租人應用程式目錄之後，請至少等候30分鐘，再提供自訂學習。 這可確保應用程式目錄布建程式在 SharePoint 內完成。 