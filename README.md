# Pwc_task2_Call_center_trends_Power_BI
PWC Call Center Analysis with Excel and Power BI

<u>Overview</u>

This project focuses on performing comprehensive analysis and visualization of call center data using Excel and Power BI. The goal is to gain valuable insights into call handling performance, customer satisfaction, and operational efficiency.

<u>Table of Contents</u>

<u>[Project Description]</u>
<u>[Key Features]</u>
[Prerequisites]
[Getting Started]
[Usage]
[Data Sources]
[Visualization]
[Creating a Power BI Dashboard]
[Summary]
[Project Description]

Managing and analyzing call center data is crucial for enhancing customer service and optimizing operational processes. This project offers a solution for analyzing call center performance by leveraging the power of Excel and Power BI.

<u>Key Features
Data Preparation: Clean and transform raw call center data for analysis.
Excel Analysis: Perform in-depth analysis and calculations using Excel.
Power BI Visualization: Create interactive and insightful visualizations.
Customer Satisfaction Analysis: Measure and visualize customer satisfaction scores.
Call Handling Efficiency: Analyze and optimize call handling times and performance.
Historical Trends: Identify historical trends and make data-driven decisions.

<u>Prerequisites</u>
Before you begin, ensure you have met the following requirements:

Excel installed on your local machine.
Power BI Desktop for advanced data visualization.
Access to the call center data source (e.g., Excel spreadsheet, database).
Getting Started
To get started with this project, follow these steps:

Clone this repository to your local machine.
Prepare your call center data source (e.g., Excel file) with the required columns.
Open Excel and Power BI to perform data analysis and visualization.
Follow the instructions in the documentation to create visualizations and gain insights.
Usage
Usage
This project can be used for:

Call center performance analysis.
Creating management reports and dashboards.
Identifying areas for improvement in call handling and customer satisfaction.
Making data-driven decisions for call center operations.

Data Sources
The project uses the following data sources:

Call center data in Excel format provided by PWC.

Visualization
![Screenshot 2024-10-03 231102](https://github.com/user-attachments/assets/6e750379-4cb0-425c-ba6a-36fb58c13bf2)

Creating a Power BI Dashboard
To create a dashboard in Power BI for Claire that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset, follow these steps:

Open Power BI Desktop.

Import the cleaned and transformed call center data into Power BI.

Create the following KPIs using DAX formulas:

Overall customer satisfaction
Overall calls answered/abandoned
Calls by time
Average speed of answer
Agent’s performance quadrant (average handle time vs. calls answered)
Design an interactive dashboard with visualizations that showcase these KPIs and metrics creatively.

Add filters, slicers, and drill-through options for Claire to explore the data.

Save and publish the Power BI report to a location accessible by Claire.
DAX Formulas Used
Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1, Sheet1[Answered (Y/N)]="Y"))
DayOfWeek = FORMAT(Sheet1[Date],"dddd")
Resolved (Y) = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="Y"))
MorningCalls = 
CALCULATE(
 COUNTROWS('Sheet1'),
 'Sheet1'[TimePeriod] = "Morning"
) 
Same for other periods

Data Visualization Insights:
Most call satisfaction ratings are 3 and 4.
Average satisfaction rating decreased over three months, peaking in January and dipping in March.
Issue resolution rate was highest in January, dipped in February, and increased in March.
Majority of calls occur in the morning.
Joe has the highest average speed of answer.
Jim has the highest call resolution rate despite slower speed and higher call volume.
Becky has the slowest speed of answer but a higher call resolution rate, ranking 5th.
Martha has the highest speed of answer in the second position.
