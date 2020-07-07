---
author: pkrebs
ms.author: pkrebs
title: 學習路徑的設定選項
ms.date: 07/16/2020
description: 學習路徑的設定選項
ms.openlocfilehash: 1434a06fbe5f374de7b2f2e4fa471a8eda5ac871
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.contentlocale: zh-TW
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043215"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>多語系學習路徑的設定選項
隨著 SharePoint 線上通訊網站的多語系功能的發行，教學途徑現在可支援多種語言。 您可以根據組織的需求，以不同類型的方式設定學習路徑。 為了協助您決定組織的最佳路徑，我們已概述設定選項。 

## <a name="new-install-scenarios"></a>新安裝案例
「新的安裝案例」會說明使用 Microsoft 365 的「查閱書」服務安裝新的學習路徑實例的選項。 

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>案例1：我們尚未安裝學習路徑，需要學習路徑的多語系支援 
若尚未安裝學習路徑，且需要多種語言，您可以使用 Microsoft 365 的「查詢」服務，安裝具有九種語言支援的新學習路徑方案。 英文將會是預設的語言，而且無法變更。 
- 若要布建新的學習路徑方案，以英文做為網站的預設語言，請參閱布建[新的學習路徑解決方案](custom_provision.md)。

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>案例2：我們已安裝教學路徑，但目前並未使用它，也沒有對網站或播放清單進行任何自訂 
如果您已安裝學習路徑，但未主動使用它，或是尚未對網站或播放清單進行任何自訂，您可以使用 Microsoft 365 的 [查詢] [考察書] 服務，安裝具有九種語言支援的新方案。 英文將會是預設的語言，而且無法變更。 
- 若要布建新的學習路徑方案，以英文做為網站的預設語言，請參閱布建[新的學習路徑解決方案](custom_provision.md)。

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>案例3：尚未安裝學習路徑，也不需要多語言支援 
若尚未安裝學習路徑，而且不需要多語系支援，您可以從 Microsoft 365 的「查閱書」服務安裝。 英文將會是預設的語言。 安裝之後，您必須關閉多語言支援。 
- 若要布建沒有多語系支援的新學習路徑方案，請參閱布建[新的學習路徑解決方案](custom_provision.md)。

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>更新學習路徑（使用網頁元件上傳）案例
如果您已安裝現有的學習路徑版本，您可以將 [學習路徑] 網頁元件上傳至 SharePoint 的應用程式目錄，以啟用多語系支援。 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>案例1：我們需要升級現有的學習路徑版本，但不需要多語言支援
您可以更新沒有多語言支援的學習路徑版本4.0。 透過更新，您會收到一些新功能，包括自訂播放清單和子類別的影像選取器。 

- 若要更新沒有多語系支援的現有學習路徑方案，請參閱[更新學習路徑中的多語系支援](custom_update.md)。 無多語系支援的升級程式與多語系支援相同，但步驟較少。 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>案例2：我們需要升級為多語言支援，且網站集合的預設語言為預設語言
學習路徑版本4會支援網站集合中的多語系頁面。 除了多種語言支援之外，您還可以取得一些新功能，包括自訂播放清單和子類別的影像選取器。 
- 若要更新現有的學習路徑網站多語系支援，請參閱[更新學習路徑中的多語系支援](custom_update.md)。 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>使用手動安裝更新學習路徑以進行多語言支援 
下列概述使用手動安裝「學習路徑」網頁元件，將現有學習路徑的實例更新為版本4.0 多語系版本的案例。 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>案例1：我們需要多語言支援，且網站集合的預設語言不是我們的預設語言–沒有自訂內容 
學習路徑版本4.0 將支援此案例。 不過，此案例假設您在現有的網站上沒有自訂的內容或播放清單。 在此案例中，您可以使用您的預設語言來建立新的 SharePoint 線上通訊網站、上傳網頁元件，然後使用 PowerShell 腳本手動設定學習路徑。 
- 若要使用您的預設語言，設定多語言支援的學習路徑，請參閱[多語言支援的手動安裝學習路徑](custom_manualsetup.md)。

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>案例2：我們需要多語言支援，且網站集合的預設語言並非我們的預設語言–此外我們有自訂內容 
在此案例中，您可以使用您的預設語言來建立新的 SharePoint 線上通訊網站、上傳網頁元件，然後使用 PowerShell 腳本手動設定學習路徑。 

依照上述步驟重新建立學習路徑網站後，您必須移動**CustomPlaylists**清單和**CustomAssets**清單的內容。 您也可以選擇性地移動實際自訂資產的自訂頁面，如果這些頁面位於現有的學習路徑網站中，您也可以將它刪除。 由於**CustomPlaylists**清單中的所有專案，此工作可能會很困難，因為**CustomAssets**清單中的清單專案識別碼會隱藏在每個播放清單專案的 JSONData 欄位中。 因此，只要將**CustomPlaylists**清單的內容從一個網站移至另一個網站，將會不夠。 此外， **CustomAssets**清單會在清單專案的 [JSONData] 欄位中包含自訂資產頁面的絕對 URL。 若資產未移動，且網站未重新命名（因而將絕對 URL 變更為資產頁面），則**CustomAssets**可以保留。 不過，您必須手動修正專案。 由於這種遷移類型的複雜度，我們建議您考慮登記我們的一個學習路徑合作夥伴，以協助您進行這項轉換。
- 若要使用您的預設語言，設定多語言支援的學習路徑，請參閱[多語言支援的手動安裝學習路徑](custom_manualsetup.md)。