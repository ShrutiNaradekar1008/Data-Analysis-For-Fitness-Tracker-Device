# End-to-End Data Analysis Project

## Objective
Utilizing the Fitbit Fitness Tracker Data, identify some trends in smart device usage, how these trends can be applied to Bellabeat’s customers and how they can help influence Bellabeat’s marketing strategy.

## Dataset
- Source: Kaggle – **https://www.kaggle.com/datasets/arashnic/fitbit**

## Workflow
1. Data cleaning using **Excel**
2. Data analysis using **SQL in Google BigQuery**
3. Data validation using **R**
4. Data visualization using **Tableau**

## Data Cleaning (Excel)
Performed the following steps:
- Removed duplicate records
- Handled missing values
- Standardized date and categorical formats
- Verified column data types

## SQL Analysis (BigQuery)
### First I categorized people based on count of tracker utilizaton throuout the data period(04-12-2016 to 05-12-2016).
```SQL
SELECT
  ID AS PEOPLE,
  COUNT(ID) AS COUNT_OF_UTILIZATION,
  CASE
  WHEN COUNT(ID) BETWEEN 25 AND 31 THEN 'ACTIVE_USER'
  WHEN COUNT(ID) BETWEEN 15 AND 24 THEN 'MODERATE_USERS'
  ELSE 'LIGHT_USERS'
  END AS TYPE_OF_USER
FROM 
  `bellabeat-project-108.Final_Dataset.dailyactivity_merged`
GROUP BY ID
ORDER BY COUNT_OF_UTILIZATION DESC

### Analyzed the pattern of time spent by users
```SQL
SELECT 
  DAY,
  AVG(VERYACTIVEMINUTES) AS AVG_OF_VERYACTIVEMINUTES,
  AVG(FAIRLYACTIVEMINUTES) AS AVG_OF_FAILYACTIVEMINUTES,
  AVG(LIGHTLYACTIVEMINUTES) AS AVG_OF_LIGHTLYACTIVEMINUTES,
  AVG(SEDENTARYMINUTES) AS AVG_OF_SEDENTARYMINUTES
 FROM 
 `bellabeat-project-108.Final_Dataset.weekdays_activity` 
 GROUP BY DAY



## Visualization (Tableau)


Dashboard screenshots are available in `tableau/` folder.  
Tableau Public Link: **[paste your Tableau link here]**

## Key Insights
- Insight 1: **[example: Sales peak during Q4 months]**
- Insight 2: **[example: Category A contributes highest revenue]**
- Insight 3: **[example: Customer retention is lower in region X]**

## Tools Used
- Excel  
- SQL (Google BigQuery)  
- R  
- Tableau  

## How to Reproduce This Analysis
1. Download dataset from Kaggle
2. Perform cleaning steps as described above
3. Upload cleaned data to BigQuery and run SQL scripts from `sql/`
4. Run R validation script from `r_validation/`
5. Build dashboard using Tableau
