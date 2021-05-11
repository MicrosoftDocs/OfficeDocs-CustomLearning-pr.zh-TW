---
author: pkrebs
ms.author: pkrebs
title: 管理學習路徑內容更新
ms.date: 10/20/2019
description: 管理學習路徑內容更新
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: c2666ea4805bc5bec3030744e44bc73b03f1865e
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310387"
---
# <a name="manage-learning-pathways-content-updates"></a>管理學習路徑內容更新
Microsoft 365 學習路徑目錄會以季度為基礎進行更新。 目錄內容（即一組 JSON 中繼資料，指向 support.office.com 中主控的學習資產）儲存在組織租使用者內部的全域快取中。 當學習路徑網站集合管理員或擁有者開啟「學習路徑管理」頁面時，會自動更新全域快取。 此外，「學習路徑」全域快取會每24小時更新一次。 更新全域快取時，會自動顯示目錄的內容更新，以供學習路徑使用者。 如果不想讓使用者使用新的內容，則學習路徑管理員可以隱藏子類別或播放清單。

作為學習路徑管理員，您可以使用「學習路徑管理」頁面來隱藏和取消隱藏子類別和播放清單。 如果您不熟悉「學習路徑 admininstration」頁面，請參閱 [Access The Administration 頁面](custom_accessadmin.md)。

## <a name="hide-and-unhide-content-by-category"></a>依類別隱藏和取消隱藏內容
1. 在 [學習路徑] 網站的首頁上，指向 [ **首頁** ] 功能表，然後選取 [ **學習路徑管理**]。
2. 在 [ **Microsoft 365 學習路徑**] 底下，選取子類別。
3. 選取您想要隱藏之子類別或播放清單右側的眼睛。 例如，若要隱藏 **sway** 類別及其所有播放清單，請選取 **Sway** 子類別右側的眼睛。 所有變更都會自動儲存。
4. 若要驗證是否已套用您的變更，請從 [學習路徑] 網站選取功能表中的 [ **Microsoft 365 訓練**]，然後重新整理網頁瀏覽器。
5. 若要取消隱藏內容，請遵循步驟1和2，然後取消選取您想要取消隱藏之內容的紅眼。

## <a name="to-hide-and-unhide-content-by-technology"></a>依技術隱藏和取消隱藏內容
在某些情況下，您可能想要依技術隱藏內容。 例如，您可能想要隱藏所有與 Yammer 相關的內容，包括建議子類別中產品及 Yammer 相關播放清單的 Yammer 播放清單。

1. 在 [學習路徑] 網站的 **首頁** 上，指向 [ **首頁** ] 功能表，然後選取 [ **學習路徑管理**]。
2. 在右上方的下拉式方塊中，選取 [ **技術**]。
3. 在 [ **Microsoft 365 學習路徑**] 底下，選取技術
4. 選取您要隱藏之技術的右側眼睛。 例如，若要隱藏 Yammer 的內容，請在 **Yammer** 技術的右側選取眼睛。 所有變更都會自動儲存。
5. 若要驗證是否已套用您的變更，請從 [學習路徑] 網站選取功能表中的 [ **Microsoft 365 訓練**]，然後重新整理網頁瀏覽器。 您也可以從學習路徑 **首頁** 選取 **建議的播放清單**，並確認您已隱藏之技術的播放清單看不到。

