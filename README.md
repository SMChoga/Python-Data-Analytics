# Multi-Dataset Analysis Using Python: Insights into Education, Economy, Sales, and Demographics

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaning/preparation)
- [Data Analysis](#data-analysis)
- [Results/Findings](#results-findings)
- [References](#references)

### Project Overview
This project utilizes real-world datasets to practice and demonstrate data manipulation, statistical analysis, and data visualization skills using Python's pandas and matplotlib libraries. Key datasets include student performance scores, global GDP data, supermarket sales, and global population statistics. The project explores student academic performance patterns, economic and demographic trends, and consumer behavior through pivot tables and various chart types.

### Data Source
- StudentsPerformance.csv
- gdp.csv
- supermarket_sales.csv
- population_total.csv

### Tools
Python for data analysis

### Data Cleaning/Preparation
- Assigned a new column (language score) and populated it with randomly generated integer values between 1 and 100.
- Removed missing values from population data using dropna().
- Sorted exam scores by subject, and selected the top 100 students based on language performance.

### Data Analysis
Include interesting code/features worked with
```sql
Select distinct industry
From layoffs_stage2
Order by 1;

Select dem.company, dem.industry, sal.company, sal.industry
 From layoffs_stage2 dem
   Inner Join layoffs_stage2 sal
     On dem.company = sal.company
       Where (dem.industry = '' or dem.industry IS Null)
		  And sal.industry IS NOT Null
             ;

Update layoffs_stage2 dem
  Inner Join layoffs_stage2 sal
     On dem.company = sal.company
       Set dem.industry = sal.company
       Where (dem.industry = '' or dem.industry IS Null)
		  And sal.industry IS NOT Null
               ;
```

### Results/Findings
The analysis results are summarized as follows:
- Average scores across math, reading, and writing were distributed fairly evenly with some gender-based trends.
- Parents’ education levels varied widely, potentially indicating different socioeconomic backgrounds.
- Males and females had different performance distributions across subjects.
- GDP per capita and population charts showed steep rises in India and China compared to Brazil and Indonesia.
- The supermarket dataset showed gender-based purchasing behavior differences in product lines and total sales.


### References
[Alex the Analyst - YouTube Channel](https://www.youtube.com/watch?v=OT1RErkfLNQ&list=PL9PrwgRNlv62OiqVlASto1N4cAQRg60dr&index=22&pp=gAQBiAQB)








