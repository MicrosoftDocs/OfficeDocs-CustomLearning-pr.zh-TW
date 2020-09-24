---
author: karuanag
ms.author: karuanag
title: 自訂和共用播放清單
ms.date: 02/10/2019
description: 從現有內容或新的 SharePoint 頁面建立自訂播放清單
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233805"
---
# <a name="customize-and-share-playlists"></a>自訂和共用播放清單

## <a name="create-a-playlist"></a>建立播放清單

播放清單是「資產」的 compliation。 「資產」是 Microsoft 訓練內容的 SharePoint 頁面或現有專案。 當您建立播放清單時，您會選取同時為您的使用者建立學習路徑的資產。  

新增 SharePoint 頁面的好處是，您可以使用組織中所主控的 YouTube 影片或影片，來建立 SharePoint 頁面。 您也可以使用表單或其他 Office 365 內容來建立頁面。  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>步驟1：建立播放清單的 SharePoint 頁面
在此範例中，我們將先建立 SharePoint 頁面以新增至播放清單。 我們將使用 YouTube 的「影片網頁元件」和「文字網頁元件」來建立頁面。  這些指示假設您正在使用 SharePoint 線上服務。 

#### <a name="create-a-new-page"></a>建立新的頁面
1.  在 [新增 > 網站] 頁面上，選取 [設定] 功能表 > 網站內容 > 網站 > 頁面]。
2.  在 [標題] 區域中，輸入 [使用小組] 命令框
3.  選取 [新增新的區段]，然後選取兩欄。

![兩欄新增](media/clo365addtwocolumn.png)

4.  在左框中，選取 [新增網頁元件]，然後選取 [內嵌]。 
5.  在網頁瀏覽器中，移至此 URL https://youtu.be/wYrRCRphrp0 並取得影片的內嵌程式碼。 
6.  在 [SharePoint 網頁元件] 中，選取 [新增內嵌程式碼]，然後將其貼到 [嵌入] 方塊中。 
7.  在右側方塊中，選取 [新增網頁元件]，然後選取 [文字]。 
8.  在網頁瀏覽器中，移至此 URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 並複製 Try！ 頁面上的指示，並將其貼到 [文字] 網頁元件。 您的頁面看起來應該如下所示。 

![內嵌頁面](media/clo365teamscommandbox.png)

9.  按一下 [ **發佈**]，然後複製頁面的 URL，並將它貼到 [記事本] 中。

#### <a name="step-2-create-the-playlist"></a>步驟2：建立播放清單

1. 流覽至網站體驗中的 [ **自訂學習管理** ] 頁面。
![custom_admin.png](media/custom_admin.png)
1. 確定已選取**類別** 
1. 按一下您想要顯示新播放清單的類別
1. 在類別名稱旁邊，按一下加號符號 ![custom_addplay.png](media/custom_addplay.png)

1. 請填入下列範例中所示的值，然後選取 [ **建立**]。 
![custom_details.png](media/custom_details.png)
- 播放清單的**標題**-顯示名稱
- **Description** -所學內容的相關資訊
- **類別** -根據初始選取範圍預先選取
- **Sub Category** -根據您的初始選取專案預先選取
- **技術** -如果適用的話，選取
- **層級** -初級、Intermidate 或 Advanced
- **物件** -這可讓您根據 Microsoft 所提供之角色的預先定義清單來設定內容目標。

6. 按一下 [**儲存詳細資料**]

> [!TIP]
> 您可以自訂播放清單的圖示影像。  按一下圖像圖示，然後插入先前上傳之圖像的 URL。  請確定圖像位於自訂的教學網站集合中，或是所有使用者都可以存取該檔案的另一個位置。  
![custom_image.png](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>步驟3：將資產新增至播放清單
在這個步驟中，您將會從 Microsoft 新增現有的資產，以及您建立至播放清單的 SharePoint 頁面。 

1. 儲存您的播放清單詳細資料後，您就可以使用搜尋現有的資產。
1. **在任何搜尋字詞中輸入** ，以查看其他播放清單中提供的預先定義的資產清單。 **按一下資產名稱** ，將其包含在新的播放清單中。
![custom_slist.png](media/custom_slist.png)

您也可以新增先前建立的 SharePoint 頁面，也可以在體驗中從頭開始建立。

1. 按一下 [播放清單資源] 對話方塊中的 [ **新增資產** ] 選項
1. 將您的資產命名為 **職稱**。 輸入後，其他選項會顯示 ![custom_newpage.png](media/custom_newpage.png)
1. 您現在可以在 SharePoint Online 中建立新資產頁面，或在現有頁面的 URL 中輸入，以將其新增至您的自訂播放清單。 
1. [**類別**]、[**子類別**] 及 [**技術**] 欄位會根據您先前的選取範圍，預先填入此播放清單。
1. 針對此個別資產進行適當的層級和物件的選擇。  
1. 按一下 [ **儲存資產** ]，將其新增至自訂播放清單
1. 重複這些步驟，搜尋或新增個別頁面，直到完成播放清單為止。 
1. 按一下 [ **關閉播放清單** 以儲存]

具有此內容的播放清單現在可在任何安裝/內嵌自訂學習 webpart 的地方使用。 

> [!NOTE]
> 如果您在關閉播放清單後犯了錯誤，您可以按一下播放清單名稱旁邊的 X，將其從類別中刪除。  

#### <a name="things-to-think-about"></a>考慮事項

自訂播放清單可用來協助您的使用者使用各種任務。  您是否有下班時間的要求表單？  要求硬體設備的表單？  任何現有的訓練資產都可以設計成經驗。  

## <a name="share-playlists"></a>共用播放清單

1. 流覽至 webpart 或網站體驗中的任何播放清單
1. 在左上角會看到三個圖示
1. 按一下代表連結的圖示
1. 將 URL 複製到播放清單

![share.png](media/share.png) 此 URL 現在可以插入網站導航或在其他通訊中使用，以直接將員工直接加入該播放清單。 

### <a name="next-steps---drive-adoption"></a>後續步驟- [磁片磁碟機採用](driveadoption.md)
