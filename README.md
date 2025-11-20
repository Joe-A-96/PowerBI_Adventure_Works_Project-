# Power BI Dashboard — Project Overview

## About the Project
This repository contains a Power BI report developed to provide insights into a sample sales dataset  
The project demonstrates end-to-end data analytics skills—from data preparation and interactive visualization.

## Objectives
- Deliver meaningful insights through clean, interactive visuals  
- Build a robust data model to support accurate and fast calculations  
- Apply analytical logic to identify trends and performance drivers  
- Present a professional, user-friendly dashboard for business use  

# Skills Demonstrated

## Data Modeling
- Designing fact and dimension tables  
- Building star schemas  
- Establishing relationships and cardinality  
- Optimizing data model performance  

## Power Query (M Language)
- Data cleaning and transformation (merging, appending, grouping)  
- Handling missing values, data types, and normalization  
- Creating reusable transformation steps  
- Building parameterized queries (optional)  

## Data Visualization and UX Design
- Creating interactive dashboards  
- Using slicers, drill-downs, tooltips, and bookmarks  
- Designing consistent layouts  
- Applying best practices in color usage and readability  

## Analytics and Insights
- Identifying trends, seasonality, and anomalies  
- Performance comparisons (YoY, QoQ, MOM)  
- Segmentation and categorical analysis  
- Extracting business-focused insights  

## Sample DAX Highlights
```DAX
Total Sales = SUM('Sales'[Sales Amount])

Sales YTD = TOTALYTD([Total Sales], 'Calendar'[Date])

YoY Growth % =
VAR CurrentYear = [Total Sales]
VAR LastYear    = CALCULATE([Total Sales], DATEADD('Calendar'[Date], -1, YEAR))
RETURN DIVIDE(CurrentYear - LastYear, LastYear)

```
**Link to my Dashboard**
[Link to my Dashboard](https://app.powerbi.com/links/TgtjT6yu9g?ctid=3ea7c128-c601-4479-a003-e14d00c0b5cb&pbi_source=linkShare&bookmarkGuid=82b37e37-0573-4733-895c-57efcfa7a365)
