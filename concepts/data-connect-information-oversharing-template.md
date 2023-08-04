---
title: "Microsoft Graph Data Connect Information Oversharing template"
description: "Use this template to determine whether sensitive data was mistakenly leaked or if employees intentionally shared confidential information with malicious intent."
author: "rimisra2"
ms.localizationpriority: high
ms.prod: "data-connect"
---

# Microsoft Graph Data Connect Information Oversharing template

Information oversharing is a security and compliance use case powered by our newly available SharePoint datasets. This template helps you validate if sensitive data was mistakenly leaked or if employees intentionally shared confidential information with malicious intent. 

## GitHub tutorial

The [Information Oversharing GitHub resources](https://github.com/microsoftgraph/dataconnect-solutions/tree/main/solutions/information-oversharing) helps organizations analyze how secure their SharePoint sites are, maintain information boundaries, and establish new rules based on how sensitive data is managed and classified.

## Key use cases 
- Monitor the sharing landscape and craft customer tenant policies.  
- Protect confidential client data, maintain constant compliance.  
- Scale your machine learning model with the increased volume of email data.  
- Understand risky behaviors and usage and promote employee behaviors.  
- Create monthly tenant policy adoption reports and month over month sharing trends reports.  
- Identify malicious actors and protect confidential data.  
- Set terms to watch for leakage, and categorize and assign severity levels.  
- Allow customers to better understand how secure your SharePoint is. 
- Maintain information boundaries. 
- Establish new rules based on how sensitive data is managed and classified. 
 

## Microsoft Graph Data Connect data sets  
- Microsoft groups **(BasicDataSet_v0.GroupMembers_v0)** 
- Microsoft groups **(BasicDataSet_v0.GroupDetails_v0)** 
- Microsoft groups **(BasicDataSet_v0.GroupOwners_v0)** 
- OneDrive and SharePoint Online **(DocumentSharingDataset_v0_Preview)**
- OneDrive and SharePoint Online **(SharePointSitesDataset_v0_Preview)**
- OneDrive and SharePoint Online **(SharePointGroupsDataset_v0_Preview)**

## Power BI dashboard 

**Sharing details**  
![An image that shows the sharing details of the oversharing dashboard](images/data-connect-templates-oversharing-sharing.png)

**Sharing by item type**
![An image that shows the sharing by item type of the oversharing dashboard](images/data-connect-templates-oversharing-items.png)

**Sharing by role definition**
![An image that shows the sharing by role definition of the oversharing dashboard](images/data-connect-templates-oversharing-roles.png)

**Sharing by file extension**
![An image that shows the sharing by file extension of the oversharing dashboard](images/data-connect-templates-oversharing-extensions.png)

**External sharing**
![An image that shows the external sharing of the oversharing dashboard](images/data-connect-templates-oversharing-external.png)
