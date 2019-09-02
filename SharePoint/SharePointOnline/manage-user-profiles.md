---
title: "Manage user profiles in the SharePoint admin center"
ms.reviewer: 
ms.author: kaarins
author: kaarins
manager: pamgreen
audience: Admin
ms.topic: article
f1_keywords:
- 'ViewUserProfiles'
- 'SPOTAMgUserProfiles'
ms.service: sharepoint-online
localization_priority: Normal
ms.collection:  
- Strat_SP_admin
- M365-collaboration
search.appverid:
- SPO160
- MOE150
- BSA160
- GSP150
- MET150
ms.assetid: 494bec9c-6654-41f0-920f-f7f937ea9723
description: "Learn how to use the SharePoint admin center to create and edit custom user properties, add and remove admins on OneDrive accounts, manage audiences, and disable OneDrive creation."
---

# Manage user profiles in the SharePoint admin center

This article is for global admins and SharePoint admins in Office 365. 

- If you're running SharePoint Server, see [Administer the User Profile service in SharePoint Server](/SharePoint/administration/user-profile-service-administration). 
  
- If you're not an admin, see [View and update your profile in Office Delve](https://support.office.com/article/4e84343b-eedf-45a1-aeb9-8627ccca14ba) for info about changing your profile. 
  
Most organizations don't need to change any user profile settings in the SharePoint admin center. For the organizations that do need to work with user profile settings, this article describes the most common tasks.
  
## Create and edit custom user properties
<a name="customuserproperties"> </a>

In Office 365, identity is managed by Azure Active Directory. For info about this, see [Understanding Office 365 identity and Azure Active Directory](/office365/enterprise/about-office-365-identity). SharePoint Online receives this profile information. If you need to store additional info about your users, you can create custom properties in the SharePoint admin center. For info about doing this, see [Add and edit user profile properties in SharePoint Online](add-and-edit-user-profile-properties.md).
  
> [!NOTE]
> Instead of creating user sub-types in the SharePoint admin center, we recommend using the Microsoft 365 admin center to [Compare groups](/office365/admin/create-groups/compare-groups) or using the Azure AD admin center to [create groups with dynamic membership](/azure/active-directory/users-groups-roles/groups-dynamic-membership). 
  
## Add and remove admins for a user's OneDrive
<a name="addremoveadmins"> </a>

Follow these steps to transfer ownership of a OneDrive to a different user, or give a user full control over another user's OneDrive.
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  
    
2. In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If the classic SharePoint admin center appears, select **Open it now** at the top of the page to open the new SharePoint admin center.
      
3. In the left pane, select **Classic features**.
 
4. Under **User profiles**, select **Open**. 
    
5. Under **People**, select **Manage User Profiles**.
    
    ![The Manage User Profiles link on the user profiles page](media/de423783-b0dd-4742-a937-c634936f0dca.PNG)
  
6. Enter the user's name and select **Find**.
    
7. Right-click the user, and then select **Manage site collection owners**.
    
8. Add and remove admins for the OneDrive, and then select **OK**.
    
    ![Manage the owners of a OneDrive](media/120f7c8c-262f-4a41-a484-e830c662f534.png)
  
For info about automatically transferring ownership of OneDrive to a user's manager when the user account is marked for deletion, see [Set up access delegation](/onedrive/retention-and-deletion).
  
## Manage audiences
<a name="manageaudiences"> </a>

Audiences let you customize content on pages so that it appears only to particular people based on their:
  
- Membership in a distribution list or security group
    
- Location in the reporting structure or public info in the user profile
    
For example, you can display a navigational link to only people in a particular geographic location. For info about using audiences, see [Target content to specific audiences](https://support.office.com/article/33d84cb6-14ed-4e53-a426-74c38ea32293).

> [!NOTE]
> Only sites that use classic templates can be customized based on audience. <br>Audiences are not a security feature. They help you deliver relevant content to specific groups of people, but don't prevent content from being available to anyone with the appropriate permissions. 

To add, edit, or delete an audience or an audience rule, go to the Manage Audiences page:
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  
    
2. In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If this opens the new SharePoint admin center, select **Classic SharePoint admin center** in the left pane.
      
3. In the left pane, select **User profiles**. 
    
4. Under **People**, select **Manage Audiences**.
    
    ![The Manage Audiences link on the user profiles page](media/5d94f074-ce73-4b11-a415-027e1b65b547.PNG)
  
    Creating a new audience:
    
    ![Creating a new audience](media/8396cb6b-5426-40e0-9024-126bca6e8cc9.PNG)
  
    Creating a new rule for the audience:
    
    ![Creating rules for a new audience](media/deafdd2d-4770-4344-87af-9dd1c1e6d7c4.PNG)
  
Audiences compile approximately weekly, and you can only view audience members after the audience compiles. The user profiles page shows the number of audiences, the number of uncompiled audiences, and the compilation status and time.
  
## Disable OneDrive creation for some users
<a name="disableonedrivecreation"> </a>

If some users are licensed to use OneDrive, but you don't want them to create a OneDrive (perhaps for regulatory reasons), you can prevent them from doing so. 

> [!NOTE]
> If a user already created a OneDrive, changing the following setting won't delete it. 
  
1. Sign in to https://admin.microsoft.com as a global or SharePoint admin. (If you see a message that you don't have permission to access the page, you don't have Office 365 administrator permissions in your organization.)
    
    > [!NOTE]
    > If you have Office 365 Germany, sign in at https://portal.office.de. If you have Office 365 operated by 21Vianet (China), sign in at https://login.partner.microsoftonline.cn/. Then select the Admin tile to open the admin center.  

In the left pane, under **Admin centers**, select **SharePoint**. (You might need to select **Show all** to see the list of admin centers.) If the classic SharePoint admin center appears, select **Open it now** at the top of the page to open the new SharePoint admin center.
      
2. In the left pane, select **Classic features**.
 
3. Under **User profiles**, select **Open**. 

4. Under **People**, select **Manage User Permissions**.
    
    ![The Manage User Permissions link on the user profiles page](media/946e0564-2e7d-40a6-8603-cc3534a557be.PNG)
  
5. By default, "Everyone except external users" has permission to "Create Personal Site" (which includes creating a OneDrive and saving user data such as followed and frequent sites). Remove that group and add specific groups to allow only a subset of licensed users to create a OneDrive.
    
    ![The permissions dialog box for controlling who can create a OneDrive](media/a23b4ec4-7862-4fd4-895a-983fed62c24d.png)

> [!NOTE]
> The **Disable OneDrive** check box has no effect. Use the "Create Personal Site" check box to specify the security groups that have permission to create a OneDrive.  
  
6. Select **OK**.
    

