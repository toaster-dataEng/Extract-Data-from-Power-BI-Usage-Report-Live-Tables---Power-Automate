# Extract-Data-from-Power-BI-Usage-Report-Live-Tables---Power-Automate
Extract Data from Power BI Usage Report Live Tables - Power Automate - Save to Excel as separate sheet

Connections: 
Excel Online (Business) 
Power BI (DX Query) 
Tenant Sharepoint  

Tool: Power Automate

Objective:
The tool aims to automatically / programmatically extract data from the LIVE Power BI Usage Report to be able to archive data historically. PBI Usage report generally has limit of upto 90days, hence this solution. The extracted data is then saved into an excel file which tables are separated on each worksheet. This worksheets shuold automatically recognized upon data import from PBI Desktop app as separate tables along with their data.

1st part of the flow: Setup recurrence. Content. Extract Dates Dimension
![image](https://github.com/user-attachments/assets/3b913523-bbbf-43ad-80a0-448d16c12449)


2nd part of the flow: Report Views

![image](https://github.com/user-attachments/assets/6a64976f-f292-4a71-bdf1-c6cae1903b2b)


3rd part of the flow: Reports

![image](https://github.com/user-attachments/assets/d6167cb7-58d7-427c-9ea5-ffa591fad7a6)


4th part of the flow: Users

![image](https://github.com/user-attachments/assets/b3b6c0a5-a024-4950-928a-509c0a0d345e)


5th part of the flow: Workspace Reports

![image](https://github.com/user-attachments/assets/36531c75-ce25-46f5-b4ce-26a7c7a00ee0)


6th part of the flow: Workspace Views

![image](https://github.com/user-attachments/assets/4c85ed29-84b8-4847-aa44-5112c9242425)


7th part of the flow: Report Pages

![image](https://github.com/user-attachments/assets/e9e8df4e-3b63-4316-aca0-9fa17b84c064)


8th part of the flow: Report Load Times

![image](https://github.com/user-attachments/assets/da1789fc-3b6e-4524-896e-74571cc81814)


9th part of the flow: Model Measures

![image](https://github.com/user-attachments/assets/2fcfe22c-4dc1-47d5-8970-8def9f9c4cf7)

Highlevel steps to get the DAX query:
Open Power BI Desktop > Open Usage Report Semantic Model > Click Table Visual > 
Identify Table Fields you want to extract > Click each field > Table should filled up >
Click VIEW Tab > Performance Analyzer > Hit Start Recording > On the Table Visual, Click on Analyze this Visual on the bottom >
At the Performance Analyzer tab > Expand the + sign after you clicked 'Analyze this visual' > Then Copy Query

Code to insert CSV to excel workbook:
https://learn.microsoft.com/en-us/office/dev/scripts/resources/samples/convert-csv









