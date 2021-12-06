# PowerBI-ProcessDashboard
The project is aimed at understanding the process performance of our Sales Process

Context
A fictitious company (Felsh) sells a majority of its products with the help of door-to-door sales agents
called “Energy Officers” or “EOs”. The Felsh Direct Channel has a distributed supply chain with thousands of
EOs carrying stock to the field at any given time. The stocks are sold in the field when the solar lights are paid
with a deposit by the customers. We use our call centre’s to support Energy Officers by verifying the customer
information and product installation.

The Task
Felsh would like to better understand the process performance of our Sales Process.
Please analyze this process to determine the following:

Overall and stage-wise turnaround time:
- Define both an overall SLA and an SLA for each stage in the process based on the topperforming quartile of completed sales cases
- Determine the monthly overall and stage-wise turnaround time

Process failure:
Determine the 1st time success rate of the overall process
- Determine ‘any time’ success rate of the overall process (which includes all successful installations even if there was an initial failure)
- At which stages does the process fail most often?

Area level performance:
- Show the above process failure and SLA performance area-wise. What insights are you able to get from looking at these areas that should be communicated to sales managers to improve overall performance?

Agent-wise performance
- Conduct a deep dive on top 20 performing agents [in terms of overall sales & TAT]. What insights are you able to get from looking at these agents, that should be communicated to sales managers to improve overall process performance?

Process Improvements
- Based on what you have learned about the process in conducting this analysis, what overall improvements would you suggest to the process designer and the call centre team?

IV. Data Sets [attached]
1. PA_PE_Exercises_SalesDataDump
2. PA_PE_Exercise_EO’sList

The column details in the file PA_PE_Exercises_SalesDataDump are as follows:
1. Country - The country in which that Prospect is created.
2. Created At - The prospect stage creation time.
3. Prospect ID - The unique key to identify a prospect.
4. User ID- The ID of the Energy Officer who is pursuing the prospect.
5. Status - This will define the current stage of prospect.
6. Ticket ID - This is referred as the ticket data which is created on zendesk
7. Approved - This will specify whether that stage was approved or not.
8. Attempt - This will provide the attempt number usually it is for the Installation Verification process.

The Sales Process can be identified using Status which is in following order for each prospect:
I. Prospect [beginning of process]
II. Pre Approved Prospect
III. Three way call
IV. Installation Pending
V. Installed
VI. Installation Reattempt (in case if installed stage is rejected)
VII. Installation Verified [end of process]

The column details in the file PA_PE_Exercise_EO’sList are as follows:
1. User ID - the ID of the Energy Officer
2. Current Area - The area in which that user is created.
3. Country - The country in which that user is created.