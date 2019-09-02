---
title: "Migrate to SharePoint Online"
ms.reviewer: 
ms.author: jhendr
author: JoanneHendrickson
manager: pamgreen
audience: ITPro
ms.topic: conceptual
ms.prod: sharepoint-server-itpro
localization_priority: Normal
search.appverid: MET150
msCollection: 
- SPMigration
- M365-collaboration
description: "Moving to SharePoint Online?"
---

# Migrate to SharePoint Online and OneDrive

Moving to SharePoint Online or OneDrive for Business?
  
There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move. 
  
## What is SharePoint Online?

A component of your Office 365 enterprise subscription, SharePoint Online (SPO) is a cloud based collaboration platform that lets you and your organization store, organize, and share data and easily communicate with each other. With SPO, you can share common resources and applications on portals, search to discover information and expertise across your organization, and stay in the know with personalized news in SharePoint home and the SharePoint mobile apps.
  
## Planning your move to SharePoint online

The method you select to move your data depends on a number of factors including the amount of data and the size. What data do you want or need to move? Where is the content currently stored? Taking the time to plan your migration, including taking an inventory and assessment of your data, is key to a successful migration. 

### Migration scenario guides

Most migrations fall into regular phases as described below. Proven success factors for migration include planning, assessing and remediating, preparing your target environment, migrating and onboarding your users.  See our migration guides to assist you in planning your migration.

- [Box to OneDrive Migration Guide](https://docs.microsoft.com/en-us/sharepointmigration/box-to-onedrive-and-sharepoint-migration-guide)
- [MySites to OneDrive Migration Guide](https://docs.microsoft.com/en-us/sharepointmigration/mysites-to-onedrive-migration-guide)
- [File share to OneDrive and SharePoint Migration Guide](https://docs.microsoft.com/en-us/sharepointmigration/fileshare-to-odsp-migration-guide)
- [SharePoint Server team sites Migration Guide](https://docs.microsoft.com/en-us/sharepointmigration/sp-teams-sites-migration-guide)


## Assess your data ##

  Use the SharePoint Assessment and Identity Management tool for SharePoint 2013 and 2010 servers to assist in migration to SharePoint online.

  Go here to download: <a href="https://www.microsoft.com/en-us/download/details.aspx?id=53598">SharePoint Migration Assessment Tool</a>.

## Microsoft FastTrack services 
Microsoft FastTrack services can help you get started with your migration to the cloud. To learn more, go to <a href="https://fasttrack.microsoft.com/about"> Microsoft FastTrack.</a> 

## Ways to move your data

|**Method**|**Description**|
|:-----|:-----|
|SharePoint Migration Tool|The SharePoint Migration Tool (SPMT) can easily migrate your files from SharePoint on-premises document libraries, lists or regular files shares.</br>Download either the current release or the latest public preview: </br></br>[SharePoint Migration Tool (current release)](http://spmtreleasescus.blob.core.windows.net/install/default.htm) or </br>[SharePoint Migration Tool Public Preview V3.0.104.3](https://spmtreleasescus.blob.core.windows.net/betainstall/default.htm)|
|PowerShell|To use the PowerShell version of the SPMT, see [Migrate to SharePoint Online using PowerShell](https://docs.microsoft.com/en-us/sharepointmigration/overview-spmt-ps-cmdlets).|
|OneDrive sync client  <br/> |After installing the OneDrive Sync client, you can drag and drop files to a folder on the computer and the content will automatically sync with either OneDrive or SharePoint Online.  <br/> |
|Manual upload  <br/> |Uploading files one at a time from the SharePoint Online tenant. <br/> |
   
>[!Note]
>When you migrate your content to SharePoint Online or OneDrive using the SPMT or the Migration API, you are copying the files.  Your source files are not deleted.