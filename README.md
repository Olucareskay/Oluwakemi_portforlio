# FUSION MART SALES PERFORMANCE ANALYSIS

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Explanatory Data Analysis](#explanatory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

### Project Overview

This data analysis project aims to providean analytical view of sales trends, key performance indicators (KPIs), and business insights. This analysis helps to assist in monitoring sales performance across different branches, product lines, and sales agents. It is also interactive, allowing users to filter data dynamically using an interactive dashboard.

### Data Sources

The data was sourced from Fusion Mart’s sales records, including transactional details such as date of sale, product type, branch, total revenue, and customer feedback. The primary sources included CSV/Excel files, SQL databases, and Power BI reports.
### Tools

- Excel (.xlsx) – Used for data collection, preprocessing, and preliminary analysis like cleaning. [Download here](https://microsoft.com)
- SQL Databases – Used to store and retrieve structured sales data. [Download here](https://mysql.com)
- Power BI (.pbix) – Used for data visualization and interactive dashboard creation. [Download here](https://microsoft.com)

### Data Cleaning
Before analysis, the raw data was cleaned and processed using the following techniques:
-	Handling missing values by filling gaps with appropriate estimates or removing incomplete records.
-	Standardizing column names for consistency.
-	Removing duplicate entries to ensure data integrity.
-	Filtering out anomalies and outliers in sales figures.
-	Ensuring correct data types for each field (e.g., dates, numerical values).

  ### Explanatory Data Analysis

 This involves sales performance data to answer key questions, such as :
 - What is the overall sales?
 - Which products are top sellers?
 - What are the peak sales period?
 - What were the main drivers of sales growth in the last quarter?
 - How does sales performance compare across different branches and product lines?
 - What impact did discounts and promotions have on sales?
 - Are there any seasonal trends that affect revenue fluctuations?
 - Which sales agents contributed the most to revenue generation?
 - What strategies can be implemented to improve underperforming areas?

   ### Data Analysis

   The data was analyzed using various techniques to extract meaningful insights like:
   Key analytical methods using PowerBI included:
-	Descriptive statistics to summarize sales performance (e.g., total revenue, average order value).
-	Trend analysis to identify sales patterns over different time periods.
-	Comparative analysis across different branches and product lines.
-	Correlation analysis to understand relationships between factors (e.g., promotions and sales growth).
-	Profitability assessment to determine which products generated the most profit.

Some interesting codes are:
   ```sql
   SELECT * FROM Customer_Details;
   SELECT * FROM Sales_Details;
   SELECT C.Invoice_ID, C.Name, C.City, C.Customer_Type, C.Gender, 
       S.Sales_Agent, S.Branch, S.Product_Line, S.Unit_Price, S.Quantity, S.COGS, S.Tax_5, 
       S.Order_Date, S.Time, S.Payment, S.Shipment_Date, S.Rating, S.Days_to_Ship
   FROM Customer_Details C
   JOIN Sales_Details S ON C.Invoice_ID = S.Invoice_ID;
  ```

### Results

The following KPIs provide an overview of Fusion Mart’s sales performance:
-	Total Sales: $306,100
-	Total Profit: $43,620
-	Number of Customers: 100 unique customers
-	Product Lines Count: 6 different product categories
-	Average Customer Rating: 6.97

The analysis are summarized a follows:
- Top Performers: Gina ($87,500), Sarah ($86,900), and Benny ($69,800)
-	Low Performers: Ian ($12,500) and Raul ($19,800)
- Best-selling Products: Food and beverages ($53,471) and Electronics ($51,750)  
-	Least-selling Products: Health and Beauty ($46,851) and Fashion ($51,134)
-	Top Performing Branch:  Naypytaw ($105,300) which is Branch C
-	Low Performing Branch:  Mandalay ($99,660) which is Branch B
-	Peak Sales Months: January ($110,168.50) and March ($103,343)
-	Lowest Sales Month: February ($92,589)

### Recommendations

- The management team can use this data to provide incentives to high-performing agents and offer additional training to those who need support.
- Optimize inventory based on product sales trends.
-	Enhance promotional campaigns during low-sales months.
-	Improve data-driven decision-making through continuous analytics monitoring.
  
### Limitations

- Some records were incomplete informations which was affecting accuracy.
- The analysis was performed within a limited time frame, which restricted deeper insights.

### References

1. Data Science for Business" by Provost & Fawcett
2. Salesforce Blog:https://www.salesforce.com/blog/
   









