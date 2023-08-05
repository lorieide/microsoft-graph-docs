---
title: "Microsoft Graph Data Connect Skills Finder and Talent Alignment template"
description: "Use this template to enable engagement managers to build the best suited teams for projects."
author: "rimisra2"
ms.localizationpriority: high
ms.prod: "data-connect"
---

# Microsoft Graph Data Connect Skills Finder and Talent Alignment template

The Skills Finder and Talent Alignment application is a Microsoft Graph Data Connect solution that enables engagement managers to build the best suited teams for projects. Use this template to identify employees who are available who have the best set of skills for the project, as well as the most relevant set of potential skills. 
 
The application processes employee profile and email data from Data Connect and complementary data sources using Azure Data Factory (ADF). It uses this data to build a model based on given queries that contain desired skills or topics of interest, as the most relevant employees are recommended. For each employee, the template provides information from employee profiles, along with inferred information about employees' potential skills, topics of interest, and roles. 

The application's search rules are highly customizable, allowing users to tailor configurations regarding data sources, filters, and search criteria, to best suit their needs. 

## GitHub tutorial

The [Skills Finder and Talent Alignment GitHub resources](https://github.com/microsoftgraph/dataconnect-solutions/tree/main/solutions/projectstaffing) helps organizations build the best suited teams for projects, by identifying employees who are available and have the best set of skills for a project, as well as the most relevant set of potential skills.

## Key use cases 
- Locate subject matter expertise to form teams with the right mix of skills and availability.  
- Enrich Human Resources (HR) data with Microsoft 365 to get insights about skill, capability level, and talent portfolio.  
- Dynamically identify and surface changes in subject matter expertise based on digital exhaust. 
- Get indication of availability and expertise to staff critical projects and high value positions. 
- Leverage analytics to develop data-driven talent strategy to retain and grow your talent over time. 
- Search for relevant employees (by name, skills, and availability or by availability alone) 
- Get relevant information about each recommended employee (employee profile information and inferred information). 
- Provide job opportunities with great skill fit to boost employee satisfaction and retention. 
- Define new teams (creating, adding members, removing members, and exporting team members). 

## Microsoft Graph Data Connect data sets 

- Azure Active Directory users **(BasicDataSet_v0.User_v1)**
- Azure Active Directory managers **(BasicDataSet_v0.Managers)**
- Outlook Emails **(BasicDataSet_v0.Message_v1)** 

## Human resources data:  

- Employee profiles (derived from the systems used in the HR department). 

## Power BI dashboard 

**Search for relevant employees**

Users can search for employees best matching a provided list of search terms. The terms represent skills, responsibilities, technologies, and so on that have been matched or inferred for each employee, based on the provided data sources. 

An example of how a search is performed from the application UI is shown in the image below: 
![An image that shows the talent pool of the skills finder template](images/data-connect-templates-skills-pool.png)

**Search by availability only** 

Users can search for employees without providing any search terms, by setting the availability filter only. By clicking the *Available At* field in the filters section, a calendar view appears. Then users can select the date, starting from which recommended employees must be available. The results are sorted by availability in ascending order (those available are effective immediately first). For identical dates, the results are also sorted alphabetically by name. 
An example of how a search is performed from the application UI is shown in the image below: 
![An image that shows how to search employees by availability](images/data-connect-templates-skills-talent.png)

**Search by skills and availability** 
Users can search for relevant employees and use the availability filter at the same time. In the recommendations list, all the employees have the availability date before or on the date set in the availability filter. This is easier to see when sorting the recommendations by availability. 
![An image that shows how to search employees by skills and availability](images/data-connect-templates-skills-searching.png)

**Search by name** 
The application also gives the option of searching by name. The name does not have to be complete. Users can search by first name, middle name, last name, full name, and so on.
![An image that shows how to search employees by name](images/data-connect-templates-skills-name.png)

**Employee profile information** 
To see more information about an employee from the employee recommendation list or from the team list: 

- Hover over a specific employee in one of these lists. 
- A button with an eye symbol on it will appear on the right side of the employee record. Click the button to search, as shown in the image below:
![An image that shows how to search employee profile information](images/data-connect-templates-skills-profile.png)

A pop-up containing the employee profile appears, as shown in the image below: 
![An image that shows an example of an employee profile](images/data-connect-templates-skills-profileview.png)

**Inferred information** 
By processing the employee profile and email data together with known term correlations from various supported domains, the employee profiles are enriched with inferred data. 
This allows users of the application to find, not only employees who explicitly possess a set of skills or interests, but also the ones which are likely to possess those skills.  It also displays those employees who have the potential to easily learn the desired skills, because they already have a wide range of related abilities. 
The inferred skills and interests are derived from specific domains (taxonomies) and are grouped and displayed. In addition to this information, the application also infers which roles are well suited for a recommended person. 
Below is an example list with several example employees where the roles inferred are underlined. 
![An image that shows how to search employees by the inferred information](images/data-connect-templates-skills-inferred-info.png)

**Search results filtering and sorting** 

Users can create filters to narrow down the search to include employees who match best with the desired characteristics. Search filters can be seen after clicking the icon to the left of the search bar, as shown in the image below. 
![An image that shows how to search employees using filtering and sorting](images/data-connect-templates-skills-filtering.png)

For each filter, the application presents the total list of value options, as shown in the example below.
![An image that shows a list of employee options](images/data-connect-templates-skills-filter-list.png)

Search results can then be sorted by relevance, whereby the search criteria and email search settings dictate the exact order of the recommendations. 

The other sorting option is by availability. This means that employees who match the query best are shown in ascending order of the dates by which they are available to join a new project. The ones who do not have an explicit availability date defined (regarded as available effective immediately) are displayed first. 

The sorting option is below the search bar, as shown in the image below. 
![An image that shows how to find employee skills by relevance](images/data-connect-templates-skills-relevance-sort.png)

**Search term autocomplete and related terms suggestions** 

As a user begins writing search terms in the search bar, the application displays multiple suggestions of known search terms, prefixed with the string that the user typed so far. 
This happens after a short delay from the last keystroke, until the current term is submitted by pressing "Enter". For certain suggested words, the application can also display a list of related term suggestions, as shown in the image below. 
![An image that shows how to search using the autocomplete option and suggestions](images/data-connect-templates-skills-autocomplete.png)

**Use search domains for skills inference and search results matching**

The application supports searching in multiple domains, e.g., Software Engineering, Data Science, Healthcare, Oil and Gas, and so on. The search operation has the option of enabling only the domains that are of interest to the user. The inferred skills differ depending on which domains are enabled. 

For example, if a user searches using the term sensor with the 'Healthcare' domain enabled, the recommendations are as follows: 
![An image that shows how to search by skills inference](images/data-connect-templates-skills-inference.png)

If a user does the same search, but this time with the 'Software Engineering' domain enabled, the skills inferred differ as shown in the image below. 
![An image that shows the search differences using domain options](images/data-connect-templates-skills-differ.png)

**Export search results**

A user can explort the results of a search operation into a file with Excel or CSV format. To do this, the user must click on the highlighted *Export* link right under the search bar, as shown in the image below. Afterwards, a pop-up appears showing how to configure the file name, format, and number of results to export. Only the results pages retrieved so far are then exported as shown in the image below. 
![An image that shows how to export employee search results](images/data-connect-templates-skills-exporting.png)

**Define teams** 

To view the team features, click the icon to the right of the *Search* button, as shown in the image below. 
![An image that shows how to define teams](images/data-connect-templates-skills-teams.png)

**Create a team** 

To create a new team, click the *Create team* button. A pop-up appears, enabling the user to add the name and description of the team, as shown in the image below. 
![An image that shows how to create teams](images/data-connect-templates-skills-creating-teams.png)

**Add members to the team** 

To add an employee to the team, hover over the wanted employee from the list of employees. A plus button appears on the right side of the employee record. Click the plus button, as shown in the image below. 
![An image that shows how to add members to a team](images/data-connect-templates-skills-adding-members.png)

**Remove members from the team** 

To remove an employee from the team, hover over the wanted employee from the list of team members. A button marked with an *X* appears on the right side of the employee description. Click the button, as shown in the image below. 
![An image that shows how to remove members from a team](images/data-connect-templates-skills-removing-members.png)

**Export team members** 

Users can export team members into an Excel or CSV file. To do this, users must click the *Export* button at the bottom of the team members list. A pop-up appears, enabling the users to configure the name and format of the file, as shown in the image below. 

![An image that shows how to export team members](images/data-connect-templates-skills-exporting-members.png)
