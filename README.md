# Employee Wellness and Work Preferences Analysis using Power BI

# Table of content
- Introduction
- Objective
- Key Features of the Dashboard
- Tools and Technologies
- Data Analysis
- Data Analysis (DAX)
- Data Visualization
- Project Insights

# Introduction
In today’s rapidly evolving work environment, understanding employee preferences and monitoring wellness are critical for maintaining a productive and satisfied workforce. The shift towards remote work, accelerated by global events, has made it essential for organizations to analyze and adapt to new working patterns. This project, Employee Wellness & Work Preferences Analysis Dashboard, leverages Power BI to provide HR and management teams with comprehensive insights into employee attendance, work-from-home preferences, and overall wellness as indicated by sick leave data.

# Objective
The primary objective of this dashboard is to analyze employee attendance patterns to gain insights into their work preferences, particularly between working from home (WFH) and working from the office, as well as to monitor employee wellness through sick leave (SL) data. The insights derived from this analysis can help HR teams make informed decisions to improve employee satisfaction and overall productivity.

# Key Features of the Dashboard
- Work Preference Visualization:Visual representation of the number of days employees choose to work from home (WFH) compared to working from the office, helping to identify trends in 
  employee work preferences.
- Sick Leave Analysis:plays the total count and percentage of sick leave taken by employees, providing insights into employee wellness and potential health trends.
- Employee Attendance Breakdown: Detailed breakdown of attendance, including WFH days, office presence, and sick leaves, filtered by employee ID and name for personalized insights.
- Performance Indicators: Key Performance Indicators (KPIs) for quick insights into overall attendance, work-from-home trends, and wellness metrics, providing a snapshot of employee 
  engagement and health.

# Tools and Technologies
- Excel
- Microsoft Power BI
- DAX

# Data Analysis
Before creating visualizations, it was essential to prepare and clean the data to ensure accuracy and integrity.
1. Importing Data into Power BI: The data was stored in three different sheets within an Excel file, with each sheet representing a month's data.

2. Using Power Query Editor: The Excel file was imported into Power BI, and the three sheets were loaded into Power Query Editor.
   Step 1: Consolidating Sheets: In Power Query Editor, the three sheets were appended into a single table using the "Append Queries" option. This operation merged the data from all                 three sheets, stacking the rows from each sheet into one consolidated table.

   Step 2: Data Cleaning: The merged table was then cleaned to ensure consistency.
          - Remove Duplicates
          - Handle Missing Values
   
   Step 3: Creating New Columns
           Month Column: A Month column was created by extracting the month from the Date column to facilitate monthly analysis.
           WFH count and SL count column was created to facilitate analysis.

3. Loading the Data for Visualization: After transforming and cleaning the data, it was loaded into the Power BI data model, ready for analysis and visualization.

# Data Analysis (DAX)
Key Measures:
1.Presence % : Create a measure to calculate Presence %.
```
Presence % = DIVIDE([Overall attendance],[Total working Days],0)
```
2. WFH %: Create a measure to calculate WFH %.
```
WFH % = DIVIDE([WFH Count],[Present day],0)
```
3. SL %: Create a measure to calculate sick leave %.
```
SL % = DIVIDE([SL Count],[Total working Days],0)
```

# Data Visualization
![HR Analytics Dashboard](https://github.com/prajaktakadu11/Employee_Wellness_and_Work_Preferences_Analysis-using-Power_BI/blob/main/HR%20analytics%20dashboard.jpeg?raw=true)

# Project Insights
- Work Preferences:
The dashboard revealed that a significant portion of employees preferred WFH during specific months like May and June . This trend could be due to various factors such as weather conditions, or public holidays.

- Employee Wellness:
The analysis showed a spike in sick leaves during certain periods of months or week, indicating potential seasonal illnesses or burnout among employees. This insight could prompt HR to review workload distributions or implement wellness initiatives.

- Attendance Trends:
Certain days of the week showed higher absenteeism, which could be due to weekend fatigue or other external factors. Understanding these patterns could lead to adjustments in work schedules or the implementation of flexible working hours.
