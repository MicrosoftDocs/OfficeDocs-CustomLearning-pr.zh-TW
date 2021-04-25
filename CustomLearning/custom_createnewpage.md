---
author: pkrebs
ms.author: pkrebs
title: 建立播放清單的 SharePoint 頁面
ms.date: 02/10/2019
description: 建立播放清單的 SharePoint 頁面
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999084"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>建立自訂播放清單的 SharePoint 頁面

學習路徑的其中一個獨特功能是建立播放清單，這些播放清單是由 Microsoft 的資產和您所建立的 SharePoint 資產所組成。 在此範例中，我們會在建立播放清單之前建立 SharePoint 頁面。 從 SharePoint 頁面建立播放清單的功能，提供各種機會，可使用 Microsoft 或您組織中提供的網頁元件來建立頁面。 例如，播放清單可以包含從 YouTube 中內嵌影片的 SharePoint 頁面，或是從 Office 365 表單或內嵌的 Power BI 報表內建的表單。 在此範例中，我們將示範如何使用 [內嵌網頁元件] 和 [文字] 網頁元件建立頁面。  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>建立自訂播放清單的 SharePoint 頁面

1. 按一下 SharePoint **齒輪** 圖示，然後按一下 [ **新增頁面**]。
2. 在頁面的左側，按一下 [ **新增新的區段 (+)** ]，然後按一下 [ **兩欄** ] 以進行區段版面配置。
3. 在左側欄中，按一下 [+]，然後按一下 [ **嵌入** 網頁元件]。 
4. 在右列中，按一下 [+]，然後按一下 [ **文字** ] 網頁元件。 您的頁面看起來應該像這樣。

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>從 YouTube 新增影片和文字

1. 在您的瀏覽器中，移至 YouTube。 在此範例中，請搜尋「什麼是 Office 365 – Microsoft 的最佳生產力應用程式」。
2. 按一下影片以播放它，然後暫停它，然後在其上按一下滑鼠右鍵。 
3. 按一下 [ **複製內嵌程式碼**]，然後回到 [SharePoint] 頁面。 
4. 按一下 [**嵌入** 網頁元件] 中的 [**新增內嵌程式碼**]，然後從 YouTube 影片新增程式碼。
5. 回到 YouTube 頁面，然後複製影片的 **描述** 文字。 
6. 回到 [SharePoint] 頁面上，選取 [ **文字** ] 網頁元件，然後複製 YouTube 影片中的文字。
7. 選取 [SharePoint] 頁面的 [標題] 區域中的 [ **編輯網頁元件** ] 圖示，然後將頁面命名為「自訂播放清單簡介」。 
8. 若為 **Layout**，請選取 [ **普通**]，然後關閉 [ **標題區域** 內容] 窗格。 頁面現在應該如下所示。 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>發行頁面

- 選取 [ **發佈** ] 按鈕。 現在，您已準備好將此 SharePoint 頁面新增至自訂播放清單。 