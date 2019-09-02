---
title: "Assign roles and permissions to manage term sets"
ms.reviewer: 
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
ms.date: 5/22/2018
audience: End User
ms.topic: article
ms.service: sharepoint-online
localization_priority: Normal
ms.collection:  
- M365-collaboration
search.appverid:
- SPO160
- OSU150
- MET150
ms.assetid: 951216b9-81ac-4850-9ea0-7ad4c45eb231
description: "Learn about the roles for managing metadata term sets on a SharePoint site, and how to assign people to those roles"
---

# Assign roles and permissions to manage term sets

To be able to create or change a term in the Term Store management tool, you must have one of three specific roles: Term Store Administrator, Group Manager, or Contributor. 
  
A Term Store Administrator can do these tasks:
  
- Create or delete term set groups
    
- Add or remove Group Managers or Contributors
    
- Change the working languages for the term store
    
- Any task that a Group Manager or Contributor can do
    
> [!IMPORTANT]
>  You must be a Term Store Administrator to designate additional Term Store Administrators. 
  
To add a Term Store Administrator:
  
1. [Open the Term Store management tool](open-term-store-management-tool.md).
    
2. In the tree view pane on the left, select the taxonomy.
    
3. In the **General** tab of the properties pane, in the **Term Store Administrators** box, type the names of the people who you want to add. You can also click the **Browse** button to find and add users. 
    
4. When you finish adding the names of people who you want to be Term Store Administrators, click **Save**.
    
## Add Group Managers
<a name="__toc332890716"> </a>

A Group Manager can do these tasks:
  
- Add or remove Contributors.
    
- Any task that a Contributor can do
    
> [!IMPORTANT]
>  You must be a Term Store Administrator to add new Group Managers. 
  
To add a Group Manager:
  
1. Go to the site where you want to add a Group Manager.
    
2. [Open the Term Store management tool](open-term-store-management-tool.md).
    
3. In the tree view pane on the left, select the Group for which you want to add a Group Manager. 
    
4. In the **General** tab of the properties pane, in the **Group Managers** box, type the names of the people who you want to add. You can also click the **Browse** button to find and add users. 
    
5. When you finish adding the names of people who you want to be Group Managers, click **Save**.
    
## Add Contributors
<a name="__toc332890717"> </a>

A Contributor can create or change a term set.
  
You must be either a Term Store Administrator or a Group Manager of a specific group to add Contributors to that group.
  
> [!NOTE]
>  The Contributor role in managed metadata differs from a Contributor on a site. 
  
1. Go to the site where you want to add a Contributor.
    
2. [Open the Term Store management tool](open-term-store-management-tool.md).
    
3. In the tree view pane on the left, select the Group to which you want to add a Contributor. 
    
4. In the **General** tab of the properties pane, in the **Contributors** box, type the names of the people who you want to add. You can also click the **Browse** button to find and add users. 
    
5. When you finish adding the names of people who you want to be Contributors, click **Save**.
    
## Managed metadata roles
<a name="__toc332890713"> </a>

The tasks that you can do in the Term Store management tool are determined by the specific role that you're assigned. 
  
> [!NOTE]
>  When you set up a term set, you can designate a group or a person as an Owner, Contact, or Stakeholders for the term set. These labels do not grant any specific permission to work with the term set. Instead, they provide a useful way to track the business owners or stakeholders for a term set. 
  
### Metadata tasks that other site users can perform
<a name="__toc332890714"> </a>

Site users who do not have an assigned role in the Term Store management tool can use terms and terms sets in other ways. 
  
Site users who have at least Contribute permissions on the site can do the following tasks with managed metadata: 
  
- Update values in Managed Metadata columns (if terms sets associated with the columns are open and if the column lets fill-in choices)
    
- Add new terms to a term set when they update the value for a Managed Metadata column
    
- Create new Enterprise Keywords when they update the Enterprise Keywords column for a list or library
    
- Use metadata navigation in lists or libraries to filter the display of items
    
- Use managed terms or Enterprise Keywords in search queries, and then refine search results based on these terms
    
In addition, site users who have appropriate permissions (such as site owners) can create new Managed Metadata columns for lists, libraries, or content types. When they create these columns, they can create new term sets that apply only to the site (previously called "site collection"), and they can manage the terms within these term sets. 
  

  

