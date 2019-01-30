# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="1fc61-101">安裝學習方案網頁組件的自訂</span><span class="sxs-lookup"><span data-stu-id="1fc61-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="1fc61-102">租用戶全安裝必要條件</span><span class="sxs-lookup"><span data-stu-id="1fc61-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="1fc61-p101">若要安裝自訂學習網頁組件整個承租人必須 Office 365 管理權限。 如果您沒有這些權限您可以使用 Office 365 系統管理員或安裝個別的網站集合的網頁組件。</span><span class="sxs-lookup"><span data-stu-id="1fc61-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="1fc61-105">您或 Office 365 系統管理員必須已安裝並設定整個租用戶的[應用程式目錄](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant)或[網站集合的應用程式目錄](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)網頁組件會收到。]</span><span class="sxs-lookup"><span data-stu-id="1fc61-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="1fc61-p102">我們支援 SharePoint Online 僅。網頁組件中不支援任何版本的 SharePoint 內部部署上進行安裝。</span><span class="sxs-lookup"><span data-stu-id="1fc61-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="1fc61-108">將自訂學習網頁組件新增至您的租用戶</span><span class="sxs-lookup"><span data-stu-id="1fc61-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="1fc61-p103">下載自訂學習網頁組件並將它儲存到本機磁碟。 此檔案命名為"ms-自訂-learning.sppkg"。 未變更的名稱或檔案的尾碼。</span><span class="sxs-lookup"><span data-stu-id="1fc61-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="1fc61-112">您的租用戶的瀏覽至 [ [Office 365 系統入口網站](https://admin.microsoft.com/AdminPortal/Home#/homepage)</span><span class="sxs-lookup"><span data-stu-id="1fc61-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="1fc61-p104">左導覽列中選取 [Admin 中心、 SharePoint]。如此會開啟新] 索引標籤中，在 SharePoint 系統管理中心中選取 [應用程式、 應用程式目錄、 SharePoint 相關應用程式</span><span class="sxs-lookup"><span data-stu-id="1fc61-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="1fc61-115">選取 [上傳網頁組件並選擇您下載的"ms-自訂-learning.sppkg"檔案</span><span class="sxs-lookup"><span data-stu-id="1fc61-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="1fc61-116">此租用戶全安裝的核取方塊旁邊"使此解決方案可在組織中所有置於桌"。</span><span class="sxs-lookup"><span data-stu-id="1fc61-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![部署方案](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="1fc61-118">將客戶學習網頁組件新增至 SharePoint Online 頁面</span><span class="sxs-lookup"><span data-stu-id="1fc61-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="1fc61-p105">自訂學習已安裝在您的租用戶之後您可以新增網頁組件至 SharePoint 頁面。當您執行時，突然是您可以使用 Office 365 訓練。</span><span class="sxs-lookup"><span data-stu-id="1fc61-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="1fc61-121">全形欄版面配置中新增自訂學習網頁組件：</span><span class="sxs-lookup"><span data-stu-id="1fc61-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint 頁面版面配置](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="1fc61-p106">在 [SharePoint] 頁面上，選取 [新增區段，然後選取全形欄。 您會看到下列提示：</span><span class="sxs-lookup"><span data-stu-id="1fc61-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="1fc61-p107">選取 [Microsoft Learning。 您現在應該會看到下列：</span><span class="sxs-lookup"><span data-stu-id="1fc61-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![學習網頁組件的自訂](media/clo365addwebpart.png)

 <span data-ttu-id="1fc61-129">您現在可以按一下 [並排顯示來探索解決方案所含的預設的內容。</span><span class="sxs-lookup"><span data-stu-id="1fc61-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="1fc61-130">後續步驟</span><span class="sxs-lookup"><span data-stu-id="1fc61-130">Next Steps</span></span>
- <span data-ttu-id="1fc61-131">探索網頁組件中所包含的[預設內容](webpartcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="1fc61-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="1fc61-132">[自訂](customization.md)您的組織的訓練經驗。</span><span class="sxs-lookup"><span data-stu-id="1fc61-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="1fc61-133">[磁碟機採用](driveadoption.md)的訓練解決方案。</span><span class="sxs-lookup"><span data-stu-id="1fc61-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

