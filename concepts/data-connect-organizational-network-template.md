---
title: "Microsoft Graph Data Connect Organizational Network template"
description: "Use this template to harness information flows and team connectivity to unlock productivity, innovation, employee engagement and organizational change."
author: "rimisra2"
ms.localizationpriority: high
ms.prod: "data-connect"
---

# Microsoft Graph Data Connect Organizational Network template

The purpose of organizational network analysis (ONA) is to harness information flows and team connectivity to unlock productivity, innovation, employee engagement and organizational change. This solution template enables customers to leverage ONA metrics from Microsoft 365 data and analyze the networks within. 

## Microsoft Graph Data Connect data sets 
- Azure Active Directory users **(BasicDataSet_v0.User_v1)**
- Teams chats **(BasicDataSet_v0.TeamChat_v1)** 
- Outlook emails **(BasicDataSet_v0.Message_v1)** 
- Outlook calendar items **(BasicDataSet_v0.CalendarView_v0)** 

## GitHub tutorial

The [Information Oversharing GitHub resources](https://github.com/microsoftgraph/dataconnect-solutions/tree/main/solutions/ona) helps organizations harness information flows and team connectivity to unlock productivity, innovation, employee engagement, and organizational change.

## Key use cases 
- Harness information flows and team connectivity to unlock productivity, innovation, employee engagement and organizational change.  
- Evaluate information flows capturing the betweenness of nodes and their probability to be on the information flow between two people.  
- Identify potential gatekeepers, change agents, and controllers to remove bottlenecks. 
- Explore influential connections measuring the influence of nodes as being well-connected to others. A high score identifies that the node’s perspective will cascade to others efficiently. 
- Empower inclusive networks by ranking the nodes, based on the number of connections to identify isolated groups that may be lacking information or left apart. 
- Increase return on investement (ROI) by measuring the impact of organizational shifts.  
- Improve organizational efficiency.  
- Predict business outcomes and analyze trends.  
- Understand your team's connectivity patterns. 

## Power BI dashboard 

**Overview page**  
On the Overview page, you can:

- Start analyzing the network graph created from the interactions of the M365 communication data.
- Understand the flow of interactions between departments.
- Glance at the raw data that is populating the graphs.
- Evaluate the number of connections and interactions of the nodes. (Note that there are date and flag filters available for comparison.) 

Each node is based on a person. If a node interacts with another node, then they become a connection. An interaction can be any of the following: 

- One email with 5 or fewer recipients
- One meeting of 5 or fewer attendees
- Eight chat messages (each with 5 or fewer recipients)
 
The blend of interactions is informed by investigations from Microsoft Research (MSR) using statistical insights from U.S.-based Microsoft employees. The two flags available to classify the nodes that can be configured using parameters include the following: 

- Bridge flag: Top 15 percentile bridging index 
- Degree flag: Top 15 percentile degree index 

![An image that shows the overview of the organizational network analysis template](images/data-connect-templates-ona-overview.png)

**Node Analysis page**  
The Node Analysis page provides additional drill-down information of the interactions in the organization and insights on how people prefer to communicate. 
![An image that shows the node analysis page of the organizational network analysis](images/data-connect-templates-ona-communications.png)

**Influence Analysis page**  
Explore influential connections: Measures the influence of nodes as being well-connected to others. This is based on the *Page Rank* of the graph. A high score identifies that the node’s perspective will cascade to others efficiently. How to engage: 

- Identify influencers 
- Explore the profile of the influencers: Title, Department, Country 
- Compare period versus period to analyze consistency 
![An image that shows the influence analysis page of the organizational network analysis](images/data-connect-templates-ona-influence.png)

**Network Size and Breadth page**  
Empower inclusive networks: Rank the nodes based on their number of connections to identify isolated groups that may be lacking information or left apart. 

- Identify siloes and communities that may not be interacting the most.
- Compare period versus period to analyze consistency.
![An image that shows the network size and breadth page of the organizational network analysis](images/data-connect-templates-network.png)

**Bridging Analysis page**  
Evaluate information flow: Measures the connectivity of nodes to detected graph communities. First, graph communities are discovered using label propagation algorithm (LPA). Then, it counts how many communities a node is connected to and normalize by the total number of communities. A node connected to no communities is set to 0. A node connected to all communities is set to 1. 

- Identify key bridges and their departments. 
- Analyze the correlation of bridging and influence.

![An image that shows the bridging analysis page of the organizational network analysis](images/data-connect-templates-ona-bridging.png)
