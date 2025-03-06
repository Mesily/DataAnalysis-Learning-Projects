# Data_Analysis-Learning-Projects
---
I am a graduate of Economics with a strong passion for data analysis, continuously expanding my skills through self-learning. My journey in data analytics has enabled me to explore and apply advanced techniques, as demonstrated in my practice projects. While I have made significant progress, I am still learning and refining my expertise in data visualization, statistical modeling, and business intelligence. I am proficient in the use of Microsoft-Excel, Power BI, and SQL. My works reflect my commitment to using data-driven insights to solve real-world challenges.

## Project Title: Under-Five Child Mortality Rate
---
[Project Overview](#project-overview)

[Data Source](#data-source)

[Tools](#tools)

[Data Cleaning and Preparation](#data-cleaning-and-preparation)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis and Transformation](#data-analysis-and-transformation)

[Data Visualization and Reporting](#data-visualization-and-reporting) 

[Conclusion](#conclusion)

### Project Overview:
---
I analyzed child mortality data from an open-source dataset compiled by Gapminder, covering 15,073 records from 1751 to 2021 across 192 UN countries. Based on historical developments in medicine and public health, I used the IFS function in Excel to categorize the timeline into five distinct eras: Pre-Scientific Medicine Era (1751–1879), Early Medical Science & Public Health Era (1880–1953), Pre-Intervention Era (1954–1979), Global Health Revolution Era (1980–2000), and Advanced Healthcare & Digital Health Era (2001–2021). These categorizations were guided by reports from WHO, UNICEF, and the World Bank, which highlight key advancements such as scientific medicine, expanded vaccination programs, immunization initiatives, the Millennium Development Goals (MDGs), and digital health technologies.
Using Pivot Tables and Charts in Microsoft Excel, I observed a steady decline in child mortality rates as healthcare systems evolved over time. Additionally, I identified war-ridden countries based on external research using Google search results on nations with ongoing or historical conflicts. I then applied the IFS function in Excel to tag each country as either "war-ridden" or "not war-ridden." Further analysis of selected war-ridden countries—such as Sudan, Somalia, Syria, Myanmar, and Afghanistan—showed that despite prolonged conflicts, under-five mortality rates generally declined. This underscores the crucial role of medical advancements and global health interventions in improving child survival rates, even in crisis settings.
In conclusion, the steady reduction in under-five mortality is largely attributed to advancements in scientific medicine, public health policies, and digital health solutions. With the integration of artificial intelligence and modern technology, global healthcare continues to improve, emphasizing the importance of data-driven policies and sustained health interventions.

### Data Source:
---
This is an open-source dataset compiled by Gapminder, using data from sources such as the World Bank and the UN [https://ourworldindata.org/grapher/child-mortality?time=earliest..latest].

### Tools:
- Power BI
  1. for data cleaning and preparation
  2. for confirmation of data quality
     
- Microsoft Excel
  1. for data analysis and transformation
  2. for Data visualization

### Data Cleaning and Preparation
At the data cleaning and preparation stage, I did the following:
- Data loading and inspection
- Data formating
- The original dataset contained 16,739 records across 237 countries and areas. Using Power BI, I refined it to 15,073 records, focusing on 192 countries recognized by the United Nations. Liechtenstein was not included in the original dataset.

### Exploratory Data Analysis
This involves exploring the data to answer the following questions:
1. What is the total number of countries analysed?
2. What is the trend of the World's child mortality rate on the avaerage?
3. What is the trend of Child mortality rate of 5 war-ridden countries on the avaerage?

### Data Analysis and Transformation
This includes major formulas used:
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
```Excel
=IFS(
A2="Afghanistan","War-ridden",
A2="Somalia","War-ridden",
A2="Syria","War-ridden",
A2="Sudan","War-ridden",A2="Myanmar","War-ridden",
A2<>"Afghanistan"<>"Somalia"<>"Syria"<>"Sudan"<>"Myanmar","Not War-ridden"
)
```

### Data Visualization and Reporting
Pivot tables and pivot charts are used to represent my findings as below.

![Pivot Chart - Mortality-rate](https://github.com/user-attachments/assets/d36695f6-8982-47ef-8562-399e5adaf84e)


![Pivot table - child-mortality-rate](https://github.com/user-attachments/assets/d30c6a5a-e383-44f1-b3a9-422bac577229)



### Conclusion
Across 192 countries between 1751 and 2021, there has been a downward trend in the world's under-5 child mortality rate. War-ridden countries, regardless of prolonged wars or conflicts have also shown continous down trend on the average. These steady decline in child mortality rate are highly attributed to the evolvement of healthcare systems over time.








