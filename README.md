# Data_Analysis-Learning-Projects
---
This is where I documented my projects while self-learning Data Analysis

## Project Title: Under-Five Child Mortality Rate
---
[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools](#tools)

[Data Cleaning and Preparation](#data-cleaning-and-preparation)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis](#data-analysis)

### Project Overview:
---
I analyzed child mortality data from an open-source dataset compiled by Gapminder, covering 16,739 records from 1751 to 2021 across 237 countries. Based on historical developments in medicine and public health, I used the IFS function in Excel to categorize the timeline into five distinct eras: Pre-Scientific Medicine Era (1751–1879), Early Medical Science & Public Health Era (1880–1953), Pre-Intervention Era (1954–1979), Global Health Revolution Era (1980–2000), and Advanced Healthcare & Digital Health Era (2001–2021). These categorizations were guided by reports from WHO, UNICEF, and the World Bank, which highlight key advancements such as scientific medicine, expanded vaccination programs, immunization initiatives, the Millennium Development Goals (MDGs), and digital health technologies.
Using Pivot Tables and Charts in Microsoft Excel, I observed a steady decline in child mortality rates as healthcare systems evolved over time. Additionally, I identified war-ridden countries based on external research using Google search results on nations with ongoing or historical conflicts. I then applied the IFS function in Excel to tag each country as either "war-ridden" or "not war-ridden." Further analysis of selected war-ridden countries—such as Sudan, Somalia, Syria, Myanmar, and Afghanistan—showed that despite prolonged conflicts, under-five mortality rates generally declined. This underscores the crucial role of medical advancements and global health interventions in improving child survival rates, even in crisis settings.
In conclusion, the steady reduction in under-five mortality is largely attributed to advancements in scientific medicine, public health policies, and digital health solutions. With the integration of artificial intelligence and modern technology, global healthcare continues to improve, emphasizing the importance of data-driven policies and sustained health interventions.

### Data Sources:
---
This is an open-source dataset compiled by Gapminder, using data from sources such as the World Bank and the UN [https://ourworldindata.org/grapher/child-mortality?time=earliest..latest].

### Tools:
- Microsoft Excel
  1. for data cleaning and preparation
  2. for data analysis and transformation
  3. for Data visualization

### Data Cleaning and Preparation
In the initial phase of the data cleaning and preparation, I did the following:
- Data loading and inspection
- Data formating
- Missing data were intentionally ignored since they were empty year data showing the absence of records for certain countries in such years.


### Exploratory Data Analysis (EDA)
EDA involved exploring the data to answer the following questions:
1. What is the total number of countries analysed
2. What is the trend of the World's child mortality rate on the avaerage
3. What is the trend of Child mortality rate of 5 war-ridden countries on the avaerage

### Data Analysis
This includes the some basic lines of code, queries and DAX expressions used
E.g
```Excel
=IFS(
    AND(C2>=1751, C2<=1879), "Pre-Scientific Medicine Era",
    AND(C2>=1880, C2<=1953), "Early Medical Science & Public Health Era",
    AND(C2>=1954, C2<=1979), "Pre-Intervention Era",
    AND(C2>=1980, C2<=2000), "Global Health Revolution Era",
    AND(C2>=2001, C2<=2021), "Advanced Healthcare & Digital Health Era",
    OR(C2<1751, C2>2021), "Unknown"
)
```

|S/No|Description|Amount|
|----|-----------|------|
|1|Sales Volume at Aba|10,000|
|2|number of new employees|8|
|3|Average Revenue for the month|25,000|

