---
title: "Configure settings for the SharePoint Store"
ms.reviewer: 
ms.author: kaarins
author: kaarins
manager: pamgreen
audience: Admin
ms.topic: article
ms.service: sharepoint-online
localization_priority: Normal
search.appverid:
- SPO160
- MET150
ms.assetid: 6b806fb8-9295-441d-b954-07009021dc48
description: "Learn how to allow or prevent users from getting apps from the SharePoint Store, and how to manage app requests."
---

# Configure settings for the SharePoint Store

The SharePoint Store is an Internet-based service that offers apps for Office, SharePoint, Exchange, Access, and Project. Site users can access the SharePoint Store directly from a SharePoint Online site in order to browse for and buy third-party apps. If a SharePoint Online environment has been configured to prevent users from getting apps from the SharePoint Store, users can still browse for and request apps. These requests are added to the App Requests list in the App Catalog.
  
For more information about the SharePoint Store, see [Office Store and SharePoint Store Terms of Use](https://support.office.com/article/64c7f343-16b5-40bb-b39f-66c9d1c4d405).
  
For more information about how to buy apps, see [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43).
  
## Specify whether users can get apps from the SharePoint Store
<a name="__top"> </a>

By default, SharePoint Online is configured to allow users to get or request apps from the SharePoint Store. The option to change this setting will not be enabled if you have not yet created an App Catalog site. For information about how to create an App Catalog site, see [Use the App Catalog to make custom business apps available for your SharePoint Online environment](use-app-catalog.md).
  
Even if you choose not to allow users to buy apps from the SharePoint Store, they will still be able to browse the SharePoint Store and request apps.
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  
    
2. In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If the classic SharePoint admin center appears, select **Open it now** at the top of the page to open the new SharePoint admin center. 

3. In the left pane of the new SharePoint admin center, select **Classic features**.     

4. Under **Apps**, select **Open**, and then select **Configure Store Settings**.
    
5. Next to **App Purchases**, do one of the following:
    
  - Select **Yes** if you want users to be able to get free, trial, or paid third-party apps from the SharePoint store. 
    
  - Select **No** if you do not want users to be able to get third-party apps. 
    
## View or manage app requests
<a name="__top"> </a>

When users request an app, they are requesting that an admin buys that app on their behalf. In an app request, users can request a specific number of licenses, and they can provide a business justification for why they need the app. App requests are saved to the App Requests list in the App Catalog site.
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  
    
2. In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If the classic SharePoint admin center appears, select **Open it now** at the top of the page to open the new SharePoint admin center. 

3. In the left pane of the new SharePoint admin center, select **Classic features**.     

4. Under **Apps**, select **Open**, and then select **Configure Store Settings**.
    
5. Next to App Requests, select the link **Select here to view app requests**.
    
6. In the App Requests list, select a request, and then select the **Edit** button.
    
7. In the **Status** list, do one of the following: 
    
  - To approve the request, select **Approved**. If you approve the app request and you want to purchase the app immediately, select the link next to **View App Details**. The app details page in the SharePoint store will open in another tab in your browser, and you can follow the steps to purchase the app. For more information about buying apps, see [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43). Note that the app must be purchased from the store before it will be available for the end user in their site.
    
  - To decline the request, select **Declined**.
    
8. On the app request form, add any comments in the **Approvers Comments** field, and then select **Save**.
    
9. Once the status has been changed to **Approved,** if the app wasn't purchased during the approval process above, the global admin or SharePoint admin will need to go to the SharePoint Store and acquire the app in order to make it available for the end user. See [Buy an app from the SharePoint Store](https://support.office.com/article/dd98e50e-d3db-4ecb-9bb7-82b189822d43).
    
Site users who request apps can view their requests by going to **Settings** \> **Add an app** \> **Your Requests**.
  
## Specify whether to allow apps for Office to start in documents
<a name="__top"> </a>

Documents stored on sites may contain apps for Office from several sources. You can specify whether or not you want to allow these apps to work when documents are opened in the browser.
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  
 
2. In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If the classic SharePoint admin center appears, select **Open it now** at the top of the page to open the new SharePoint admin center. 

3. In the left pane of the new SharePoint admin center, select **Classic features**.     

4. Under **Apps**, select **Open**, and then select **Configure Store Settings**.
 
5. Next to Apps for Office from the Store, do one of the following:
    
  - Select **Yes** if you want to allow apps for Office to start when documents are opened in the browser. 
    
  - Select **No** if you do not want to allow apps for Office to start when documents are opened in the browser. 
    

