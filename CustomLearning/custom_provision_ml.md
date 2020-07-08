---
author: pkrebs
ms.author: pkrebs
title: 布建新的教學路徑多語系解決方案
ms.date: 02/10/2019
description: 透過 SharePoint 布建服務布建 Microsoft 365 學習路徑網站
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 6948162d8a96c9a6582484c5f4fc8acad18405a7
ms.sourcegitcommit: f355885fb93d66abf61df535fa704ccdb8df9b64
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/05/2020
ms.locfileid: "45038993"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a>布建新的教學路徑多語系解決方案
在其承租人中未布妥學習路徑的組織，可使用 SharePoint 布建服務，以新增多語系學習路徑方案。 使用此選項，「教學」路徑 SharePoint 範本會轉譯成九種語言，且最少可用於修改。 

> [!IMPORTANT]
> 如果您已在租使用者中布建學習路徑，建議您遵循學習路徑的[更新路徑](custom_update_ml.md)。 如果您在租使用者中的現有實例上安裝學習路徑，則對「學習路徑」網站範本或播放清單所做的任何變更，都可能會遺失。

## <a name="prerequisites-for-multilingual-support"></a>多語系支援的必要條件
 
若要成功設定與布建服務的 Microsoft 365 教學路徑，進行布建的人員必須符合下列先決條件： 
 
- 提供教學路徑的人員必須是安裝教學路徑的承租人租使用者管理員。  
- 租使用者應用程式目錄必須可在 SharePoint 系統管理中心的 [App] 選項內使用。 如果您的組織沒有 SharePoint 租使用者應用程式目錄，請參閱[SharePoint 線上檔](https://docs.microsoft.com/sharepoint/use-app-catalog)以建立一個。 在建立應用程式目錄之前，您必須至少等候兩小時之後，再提供學習路徑。  
- 提供教學路徑的人員必須是租使用者應用程式目錄的網站集合擁有者。 如果人員提供的學習路徑不是應用程式目錄的網站集合擁有者，請[完成這些指示](addappadmin.md)並繼續。 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a>確定租使用者管理員帳戶未選取語言
在您布建學習路徑之前，請確定租使用者的系統管理員帳戶未選取語言。 以下說明如何確認系統管理員帳戶未選取語言。 
1.  使用 Edge 系統管理設定檔，移至 office.com。
2.  輸入使用者認證（如有必要）。
3.  在 Microsoft 365 中，按一下 [**所有應用程式**] > Delve。 
4.  按一下 [**我**  >  的**更新設定檔**]。
5.  向中向左下向下方，按一下 [**如何變更語言和地區設定**]。
6.  按一下 [**這裡**]，然後按一下省略號 **...**。
7.  在 [**我的顯示語言**] 底下，您應該會看到**沒有選取語言**。 如果已選取語言，請將其取消選取。

### <a name="to-provision-learning-pathways"></a>提供學習路徑

1. 移至[Microsoft 365 學習路徑方案頁面](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239)。
2. 按一下 [**新增至您的租使用者**]。 如果您未登入到您的租使用者，提供服務會要求您提供租使用者系統管理員認證。 
3. 在 [要求的許可權] 對話方塊中，選取 [**代表您的組織同意**]，然後選取 [**接受**]。

布建服務需要這些許可權才能建立租使用者應用程式目錄、將應用程式安裝至租使用者應用程式目錄，以及布建網站範本。 您的租使用者沒有整體影響。 這些許可權會明確用於解決方案安裝的目的。 您必須接受這些許可權，才能繼續安裝。

4. 在 [布建資訊] 頁面上，根據您的安裝填寫適當的欄位。 請至少輸入您要取得其布建程式及網站目的地 URL 相關通知的電子郵件地址。  
> [!NOTE]
> 將網站的目的地 URL 做為便於員工（如 "/sites/MyTraining" 或 "/teams/LearnMicrosoft365"）的內容。

![inst_options.png](media/inst_options.png)

6. 準備好將學習路徑安裝至您的租使用者**環境時，** 按一下 [布建]。  布建程式最多可能需要15分鐘。 當網站準備好時，您會透過電子郵件通知您。 

> [!IMPORTANT]
> 布建「學習路徑」網站的承租人管理員必須前往該網站，然後開啟**CustomLearningAdmin**以初始化學習路徑系統管理員屬性。 此時，租使用者管理員也應指派網站的擁有者。 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>驗證布建成功和初始化 CustomConfig 清單

布建完成時，布建網站的承租人管理員會收到來自 PnP 布建服務的電子郵件。 電子郵件包含網站的連結。 此時，租使用者管理員應該會使用電子郵件中提供的連結前往網站，並設定網站以供第一次使用：

- 請移至 `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`。 開啟**CustomLearningAdmin**會初始化**CustomConfig**清單專案，以設定第一次使用的學習路徑。 您應該會看到如下所示的頁面：

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>將擁有者新增至網站
作為租使用者系統管理員，您不太可能是自訂網站的人員，所以您必須將少數擁有者指派給網站。 擁有者具有網站的管理許可權，可供使用者修改網站頁面及才能重塑網站。 他們也可以隱藏及顯示內容，以及建立自訂的播放清單和子類別。  

1. 在 [SharePoint**設定**] 功能表中，按一下 [**網站許可權**]。
2. 按一下 [**高級許可權設定**]。
3. 按一下 [ **Microsoft 365 學習路徑擁有**者]。
4. 按一下 [**新增**  >  **使用者至此群組**]，然後新增您想要成為擁有者的人員。 
5. 在 [共用郵件] 中新增[流覽網站的](custom_exploresite.md)連結，然後按一下 [**共用**]。

## <a name="add-translators-to-the-site"></a>將翻譯人員新增至網站
如果您將使用該網站的翻譯人員，您可以將許可權指派給他們。 翻譯人員需要成員許可權或更高許可權。 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a>選擇在網站上使用多種語言的選項
SharePoint 布建服務以九種語言建立學習路徑網站。 適用的建議如下：
- 關閉您不想要支援的語言
- 如果您不支援多語系網站，請關閉 [多語言] 功能。 請參閱本主題稍後的「關閉多種語言支援」一節。

### <a name="remove-languages-you-dont-want-to-support"></a>移除不想要支援的語言
針對選擇只支援一種語言的組織，除了預設英文語言之外，我們建議移除不支援的語言。 
1. 從 [學習路徑] 網站中，選取頁面右上角的 [**設定**]，然後選取 [**網站資訊**]。
2. 在 [網站資訊] 窗格的底部，選取 [**查看所有網站設定**]。
3. 在 [**網站管理**] 下，選取 [**語言設定**]。
4. 在 [**讓頁面和新聞轉譯成多種語言**] 底下，將開關滑動至 [**開啟**]。 預設值應為 On。
5. 在 [新增或移除網站語言] 底下，按一下 [**移除**]，移除網站不需要的語言。 下列會顯示 [語言設定] 頁面的範例，除了預設英文語言之外，還會顯示網站支援的義大利文。

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> 移除語言時，不能移除預設的英文語言。 

### <a name="assign-translators"></a>指派翻譯員
如果您想要翻譯頁面，可選擇為每種語言指派一或多個翻譯人員（網站的預設語言除外）。 
- 在 [**翻譯人員**] 欄中，開始輸入您想要成為翻譯人員的名稱，然後從清單中選取名稱。 

> [!NOTE]
> 您組織的 Active Directory 中的任何人都可以指派成翻譯工具。 指派為翻譯人員的人員不會自動獲得適當的許可權。 當沒有網站的「編輯」許可權的人員嘗試存取網站時，會將其導向至可要求存取的網頁。

## <a name="turn-off-multilingual-support"></a>關閉多語言支援
例如，如果您不想要使用多語系網站，則建議您關閉多語系功能。 

1. 從 [學習路徑] 網站中，選取頁面右上角的 [**設定**]，然後選取 [**網站資訊**]。
2. 在 [網站資訊] 窗格的底部，選取 [**查看所有網站設定**]。
3. 在 [**網站管理**] 下，選取 [**語言設定**]。
4. 在 [**讓頁面和新聞轉譯成多種語言**] 底下，將開關滑動至 [**開啟**]。 預設值應為 On。
- 在 [**允許翻譯頁面和新聞**] 底下，選取 [**關閉**]。 

### <a name="add-languages"></a>新增語言
學習路徑支援9種語言，但建議您只新增您必須用來支援「學習路徑」網站的語言。 您可以在任何時候新增語言則。 
- 在 [**新增或移除網站語言**] 底下，開始在 [**選取] 或 [輸入語言**] 中輸入語言名稱，或從下拉式清單中選擇語言。 您可以重複此步驟來新增多種語言。 您可以隨時在網站中新增或移除語言，只要回到此頁面。


