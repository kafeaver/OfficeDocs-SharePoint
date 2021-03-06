---
title: "Integrate a new Yammer network into SharePoint Server 2013"
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
ms.date: 3/8/2018
ms.audience: ITPro
ms.topic: article
ms.prod: sharepoint-server-itpro
localization_priority: Normal
ms.assetid: 6485e76d-9c52-40eb-ae0f-4e00c321c7d8
description: "Summary: Learn how to integrate a new Yammer Enterprise network into an existing SharePoint Server 2013 environment."
---

# Integrate a new Yammer network into SharePoint Server 2013

 **Summary:** Learn how to integrate a new Yammer Enterprise network into an existing SharePoint Server 2013 environment. 
  
This scenario describes the prerequisites and recommended steps to integrate a new Yammer Enterprise network together with your existing SharePoint Server 2013 environment.
  
## Scenario prerequisites

For this scenario, we assume that:
  
- You have SharePoint Server 2013 SP1 or later installed.
    
- You don't use the SharePoint Server 2013 Newsfeed social feature.
    
- You use Active Directory Domain Services (AD DS) as your identity provider and Active Directory Federation Services (AD FS) 2.0 for identity federation.
    
- You are ready to use a Yammer Enterprise network.
    
## Step 1: Purchase Yammer Enterprise

Yammer Enterprise is included in many Office 365 plans, which means that you might already have a license for the service. 
  
## Step 2: Create your Yammer network

We recommend that you [create one single, central Yammer network](https://go.microsoft.com/fwlink/p/?LinkId=524341). This makes collaboration among all employees easier, and you can invite users from other domains to the primary domain as guests. A single network also provides centralized administration, which guarantees consistency across things like policy implementation and management, feature rollout, and scheduled maintenance. If all employees are in one location or are dispersed but share a common email address, use a single Yammer network.
  
When you set up your network, [Enforce Office 365 identity for Yammer users](http://technet.microsoft.com/library/008f940b-6bec-47fc-bcc6-9c6133467562%28Office.14%29.aspx).
  
For information about how users are managed in Yammer Enterprise, see [Manage Yammer users across their life cycle from Office 365](http://technet.microsoft.com/library/6c4c8fff-6444-404a-bffc-f9da0bcc3039%28Office.14%29.aspx).
  
## Step 3: Set up directory synchronization

Office 365 uses Azure Active Directory for identity management, and Yammer Enterprise can be set up to enforce Office 365 identity. If you're using an on-premises directory, in order to manage users in one place, you need to sync your on-premises directory with Azure Active Directory by using Azure Active Directory Connect. 
  
For more information, see [Plan for directory synchronization for Office 365](http://technet.microsoft.com/library/d3577c90-dda5-45ca-afb0-370d2889b10f%28Office.14%29.aspx) and [Integrate your on-premises directories with Azure Active Directory](https://go.microsoft.com/fwlink/p/?LinkId=869669).
  
## Step 4: Disable default SharePoint Server 2013 social features

After you set up directory synchronization, [disable the default SharePoint Server 2013 social features](hide-sharepoint-server-2013-social-features.md).
  
If your organization wants to upgrade and migrate to SharePoint Server 2013, see the following articles:
  
- [Overview of the upgrade process to SharePoint Server 2016](../upgrade-and-update/overview-of-the-upgrade-process.md)
    
- [Upgrade to SharePoint Server 2016](../upgrade-and-update/upgrade-to-sharepoint-server-2016.md)
    
## Step 5: Use Yammer Embed

After you disable the default SharePoint Server 2013 social features, you should [use the Yammer embed widget](add-the-yammer-embed-widget-to-a-sharepoint-page.md) to include Yammer feeds on SharePoint pages. 
  
## See also

#### Concepts

[Integrate Yammer with on-premises SharePoint 2013 environments](integrate-yammer-with-on-premises-sharepoint-2013-environments.md)
  
[Social scenarios with Yammer and SharePoint Server 2013](social-scenarios-with-yammer-and-sharepoint-server-2013.md)
#### Other Resources

[Manage Yammer users across their life cycle from Office 365](http://technet.microsoft.com/library/6c4c8fff-6444-404a-bffc-f9da0bcc3039%28Office.14%29.aspx)

