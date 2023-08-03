---
title: "Relationship Mesh template"
description: "Learn how to use Microsoft Graph Data Connect to take required actions to manage and improve the interactions at various stages in a customer engagement life cycle."
author: "rimisra2"
ms.localizationpriority: high
ms.prod: "data-connect"
---

# Relationship Mesh template 

Building strong relationships with customers is especially important to improve customer retention, loyalty, and revenue. Gaining insights into the strength of relationships with customers and their key contacts enables your teams to take required actions to manage and improve the interactions at various stages in a customer engagement life cycle. 

This template enables you to create a Relationship Mesh solution that shows how well your sales team is connected to your key accounts and how they interact with each contact at each account. 
 
## Key use cases 
- Integrate customer/seller relationship data from various systems together into a single view with actionable insights at the area and individual account level.  
- Minimize customer churn, increase loyalty, and generate more revenue in every account.  
- Programmatically manage and improve customer interactions at each stage of the sales cycle. 
- Get visibility into your accounts and establish clear next steps. 
- Define ruleset to calculate the connectivity score between internal and external contacts.  
- Gain timely analytics and insights that help improve relationships between sellers with high priority accounts. 
- Establish a detailed view of relationship event tracking and a checklist to make it actionable.  

## Microsoft Graph Data Connect data sets 
- Outlook emails **(BasicDataSet_v0.Message_v1)** 
- Outlook calendar events **(BasicDataSet_v0.CalendarView_v0)** 

## CRM data  
- Contacts 
- Accounts 
- Opportunities  
- Employees 

## Power BI dashboards 
With the prepackaged business logic, you can calculate connectivity scores between your sellers and customer contacts based on CRM, email communication, and meeting data. This dashboard shows you a summary of all high priority accounts and their connectivity scores. The dashboard also includes accounts that need attention, accounts in good standing, and the shortest and longest gaps since the last activity.

![An image that shows the relationship mesh intro dashboard](images/data-connect-templates-mesh-intro.png)

The **Detail dashboard** includes actionable insights both at organizational level and at an individual account level, so you can refine your search by industries, sectors, sellers, tiers and transaction size. The dashboard also shows the network of sellers and external contacts, the top contacts at an account, the top relationship touchpoints, the interactions, an event tracker, and the list of prospecting checklist. 
![An image that shows the relationship mesh detail accounts dashboard](images/data-connect-templates-mesh-account.png)
