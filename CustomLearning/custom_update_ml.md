---
author: pkrebs
ms.author: pkrebs
title: 更新多語言支援的學習路徑
ms.date: 05/20/2019
description: 更新多語言支援的學習路徑
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 37a9b77ee45b8ae1ae4973f171c32de11fb530e1
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: Auto
ms.contentlocale: zh-TW
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031699"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>更新多語言支援的學習路徑
如果您有現有的學習路徑網站，您可以更新它以進行多語言支援。 若要將學習路徑更新為多語系4.0 版本，請將網頁元件套件（customlearning）上傳至 SharePoint 租使用者目錄。 當您更新學習路徑：  

- 先前建立的任何自訂播放清單和資產都將維護
- 會維護隱藏或顯示內容的設定
- 學習路徑 SharePoint 範本保持不變
- 學習路徑網站頁面不會轉譯。 您必須手動執行這種工作

## <a name="read-the-learning-pathways-multilingual-overview"></a>閱讀學習路徑多語簡介
若要瞭解多語系支援如何運作以取得學習路徑，請閱讀[學習路徑多語簡介](custom_overview_ml.md)。 

## <a name="prerequisites-to-update"></a>更新的必要條件
更新學習路徑之前，必須符合下列先決條件：
- 更新學習路徑的人員必須是租使用者應用程式目錄的網站集合擁有者。 如果人員提供的學習路徑不是應用程式目錄的網站集合擁有者，請[完成這些指示](addappadmin.md)並繼續。 

## <a name="set-language-settings"></a>設定語言設定 
在更新學習路徑之前，請先設定網站的語言設定。 若要啟用「學習路徑」網站的多語系支援，您可以將 [**啟用頁面和新聞] 的 [可轉譯成多種語言**] 設定為 [**開啟**]，然後新增您要支援的網站語言。
1.  在 [學習路徑] 網站中，從右上方選取 [**設定**]，然後選取 [**網站資訊**]。
2.  在 [網站資訊] 窗格的底部，選取 [**查看所有網站設定**]。
3.  在 [**網站管理**] 下，選取 [**語言設定**]。
4.  在 [**讓頁面和新聞可轉譯成多種語言**] 底下，設定切換參數。 
- 針對 multiligual 網站，將切換滑動至 [**開啟**]，然後繼續進行 [新增語言] 區段。 
- 若為僅供英文使用的網站，請將此開關滑動至 [**關閉**]。

### <a name="add-languages"></a>新增語言
學習路徑支援九種語言，您應該只新增您需要的語言。 在本檔中所使用的範例中，會新增義大利文。 
- 在 [**新增或移除網站語言**] 底下，開始在 [**選取] 或 [輸入語言**] 中輸入語言名稱，或從下拉式清單中選擇語言。 您可以重複此步驟來新增多種語言。 您可以隨時在網站中新增或移除語言，只要回到此頁面。
 
### <a name="assign-translators"></a>指派翻譯員
在定義學習路徑的語言設定時，您可以指派翻譯人員。 翻譯員應設定外部語言設定檔。 如需外國語言設定檔的詳細資訊，請參閱[建立多語言通訊網站、頁面和新聞](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)。  
- 如需支援的語言，請按一下 [**選取或輸入翻譯工具**]，然後選取翻譯工具。 

## <a name="update-the-learning-pathways-web-part-package"></a>更新「學習路徑」網頁元件套件
在這個步驟中，您會將「學習路徑4.0」網頁元件上傳至 SharePoint 的應用程式目錄，然後流覽至 [學習路徑管理] 頁面，以啟動更新程式。

### <a name="upload-the-web-part-package"></a>上傳網頁元件套件
1.  移至 [小組中的多語系共用位置] 和 [將 customlearning 下載至您電腦上的本機磁片磁碟機] **sppkg** 。 
2.  若尚未登入，請使用租使用者系統管理員或網站集合管理員帳戶登入您的租使用者。 
3.  按一下 [系統**管理**] [  >  **顯示所有**  >  **SharePoint**  >  **其他功能**]。 
4.  在 [**應用程式**] 下，按一下 [**開啟**]。 
5.  按一下 [**應用程式目錄**  >  **分配應用程式以供 SharePoint**。 
6.  按一下 [**上傳**  >  **選擇**檔案]。 
7.  選取您下載的**customlearning**檔，按一下 **[確定**  >  **部署**]。 

### <a name="complete-the-update"></a>完成更新
1.  從 [學習路徑] 網站的 [**首頁**] 功能表中，選取 [**學習路徑管理**]。 
2.  您會看到提示，詢問您是否要更新。 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  按一下 **[開始]**。 
4. 更新完成時，按一下 [**關閉**]。 

### <a name="next-steps"></a>後續步驟
- 探索網站和網頁元件中提供的[預設內容](custom_exploresite.md)。
- 如需翻譯網站頁面的詳細資訊，請參閱[翻譯網站頁面](custom_translate_page_ml.md)。 

