# Conversation Lineage template

[Get Started](https://github.com/microsoftgraph/dataconnect-solutions/tree/main/solutions/conversation-lineage)

## Business summary 
Use the Conversation Lineage template to gain insights into an organization's communication patterns by analyzing Microsoft 365 data with Microsoft Graph Data Connect (MGDC). 
This template teaches you the key steps and Azure technologies required to build your own MGDC-based application. By extracting and processing Microsoft 365 data and runnning analytics using Azure Synapse Analytics, you can process both historical data and future data using Azure Synapse triggers. You can also extract sentiment and Natural Language Processing (NLP) entities from conversations using Azure Cognitive Services, enabling you to visualize key insights with PowerBI. 

## Key use cases 
- Integrate Microsoft 365 email conversations with CRM or ticketing information to create a single view with customer sentiment analysis.  
- Leverage the power of conversation patterns to optimize efficient routing. 
- Craft compelling internal email campaigns with proven results.  
- Identify and eliminate bad communication practices.
- Measure changes in an organization’s communication patterns. 
- Reduce redirecting by determining the value that each party brings to the chain of the interaction. 
- Track whether emails are being read and shared using sentiment analysis to gauge reactions. 
- Get a view of the communications sentiment over time.  
- Find the most frequent keywords found in main titles. 
- Get a view of all your emails sent by each department, your top email senders, the total of emails sent, and the count of emails sent externally. 

## MGDC data sets 
- Azure Active Directory users **(BasicDataSet_v0.User_v1)** 
- Teams chats **(BasicDataSet_v0.TeamChat_v1)** 
- Outlook emails **(BasicDataSet_v0.Message_v1)** 
- Outlook calendar items **(BasicDataSet_v0.CalendarView_v0)** 

## PowerBI dashboards 
The **Global Conversation Lineage** dashboard shows overall general sentiment, frequent keywords, and interaction type.
![An image that shows the global conversation lineage dashboard](images/data-connect-templates-conv-lineage.png)

The **Dev 101** report helps you understand the emails sent by each department, your top email senders, the total of emails sent, and the count of emails sent externally. 
![An image that shows the emails by department from the conversation lineage dashboard](images/data-connect-templates-dev101.png)
 
The **Mailing Management** report gives you a view of the top email senders and receivers, all the emails sent to managers and subordinates, and it displays how many emails are read and where the senders are located.  
![An image that shows the mailing management from the conversation lineage dashboard](images/data-connect-templates-mail-management.png)

With the **Are mails actually read** report, you can understand the number of mails read by department, how many emails are read, if there are any pattern to emails not being read and the senders name and location. 
![An image that shows if emails are read from the conversation lineage dashboard](images/data-connect-templates-mails-read.png)

With the **Who interacts with whom?** you can understand the interaction between teams and how frequently those interactions are occurring with each sender. 
![An image that shows who interacts with who from the conversation lineage dashboard](images/data-connect-templates-who-interacts.png)
