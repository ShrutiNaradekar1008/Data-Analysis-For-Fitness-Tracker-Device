# 📊 End-to-End Data Analysis Project

## 🎯 Objective
The goal of this project is to analyze **[briefly describe dataset, e.g., sales / customer / HR data]**
to identify key trends and insights and present them using an interactive dashboard.

## 📂 Dataset
- Source: Kaggle – **[paste dataset link]**
- Raw data file: `data/raw_dataset.csv`
- Cleaned data file: `data/cleaned_dataset.xlsx`

## 🔄 Workflow
1. Data cleaning using **Excel**
2. Data analysis using **SQL in Google BigQuery**
3. Data validation using **R**
4. Data visualization using **Tableau**

## 🧹 Data Cleaning (Excel)
Performed the following steps:
- Removed duplicate records
- Handled missing values
- Standardized date and categorical formats
- Verified column data types

Cleaned dataset: `data/cleaned_dataset.xlsx`

## 🧮 SQL Analysis (BigQuery)
SQL queries were executed in Google BigQuery to calculate KPIs and analyze trends.

Analysis included:
- Aggregations and grouping
- Category-wise and time-based trends
- Key performance indicators

SQL scripts available in `sql/` folder:
- `bigquery_sales_analysis.sql`
- `kpi_calculations.sql`

## ✅ Data Validation (R)
Validation was performed to ensure data quality after transformation.

Checks included:
- Row count comparison
- Summary statistics verification
- Outlier detection

R script: `r_validation/validation_checks.R`

## 📊 Visualization (Tableau)
An interactive dashboard was created to visualize key insights such as:
- KPI summary
- Trend analysis
- Category or segment comparisons

Dashboard screenshots are available in `tableau/` folder.  
Tableau Public Link: **[paste your Tableau link here]**

## 💡 Key Insights
- Insight 1: **[example: Sales peak during Q4 months]**
- Insight 2: **[example: Category A contributes highest revenue]**
- Insight 3: **[example: Customer retention is lower in region X]**

## 🛠 Tools Used
- Excel  
- SQL (Google BigQuery)  
- R  
- Tableau  

## 📌 How to Reproduce This Analysis
1. Download dataset from Kaggle
2. Perform cleaning steps as described above
3. Upload cleaned data to BigQuery and run SQL scripts from `sql/`
4. Run R validation script from `r_validation/`
5. Build dashboard using Tableau
