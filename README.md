# Adventure Works Sales Analytics Project

## Project Overview

This repository contains the complete **Adventure Works Sales Analytics Project** created using:

- Microsoft Excel
- MySQL / SQL
- Microsoft Power BI
- Tableau

The project follows an end-to-end analytics workflow:

**Data Preparation → Data Modeling → Analysis → Visualization → Dashboard → Business Insights**

Adventure Works Cycles is used as the project dataset. The analysis focuses on sales, profit, production cost, products, customers, regions and time.

---

## Files Included

### 1. `Adventure work.csv`
Raw / consolidated project data used as a source for analysis and data preparation.

### 2. `Adventure_Works_project.xlsx`
Excel project workbook used for data preparation, pivot analysis and dashboard creation.

The Excel dashboard covers:
- Year-wise Sales
- Month-wise Sales
- Region Sales
- Sales vs Production Cost
- Total Sales
- Total Profit
- Total Orders
- Best Selling Product
- Top Sales Region
- Year / Month / Quarter / Region filters

### 3. `Adventure_work_project.pbix`
Microsoft Power BI project file.

The Power BI workflow is:

**Power Query → Data Model → DAX → Interactive Dashboard → Business Insights**

Dashboard areas include:
- Total Sales
- Total Profit
- Total Orders
- Profit Margin
- Year-wise Sales
- Regional Performance
- Quarter-wise Sales
- Top 10 Products
- Sales vs Production Cost

### 4. `Adventure Works Final PPT Group 4.pptx`
Final project presentation for Group 4.

The presentation contains:
- Project overview
- Data preparation
- Data modeling
- Excel dashboard
- Power BI dashboard
- Tableau dashboard
- SQL queries
- Key insights
- Overall project report

### 5. `Adventure_Works_SQL_Queries_Q0_Q13.sql`
MySQL SQL query file containing the project's SQL analysis sections from Q0 to Q13.

Main SQL topics:
- Union of sales tables
- Product name lookup
- Customer name and Unit Price lookup
- Date columns from OrderDateKey
- Sales Amount calculation
- Production Cost calculation
- Profit calculation
- Month-wise Sales
- Year-wise Sales
- Quarter-wise Sales
- Sales vs Production Cost
- KPI development
- Overall report

### 6. `FactInternetSales.xlsx`
Adventure Works fact sales data.

### 7. `Fact_Internet_Sales_New.xlsx`
Additional / new Internet Sales fact data used with the main sales table.

### 8. `Dimcustomer.xlsx`
Customer dimension data used for customer-level analysis and customer lookup.

### 9. `DimDate.xlsx`
Date dimension data used for time-based analysis.

### 10. `DimProduct.xlsx`
Product dimension data used for product names and product-level analysis.

### 11. `DimProductCategory.xlsx`
Product category dimension used for category-level analysis.

### 12. `DimProductSubCategory.xlsx`
Product subcategory dimension used for detailed product classification.

### 13. `DimSalesterritory.xlsx`
Sales territory dimension used for regional / territory analysis.

---

## Data Model

The project uses a star-schema style model.

### Fact Table

**FactInternetSales**

Main sales transaction information.

### Dimension Tables

- DimCustomer
- DimProduct
- DimDate
- DimSalesTerritory
- DimProductCategory
- DimProductSubCategory

Conceptually:

```text
                 DimCustomer
                      |
                      |
DimDate ---- FactInternetSales ---- DimProduct
                      |
                      |
              DimSalesTerritory
                      |
              DimProductSubCategory
                      |
               DimProductCategory
```

---

## Excel Analysis

Excel was used for:

1. Data preparation
2. Pivot table analysis
3. Charts
4. Slicers
5. Interactive dashboard
6. Business insights

### Main Visualizations

- Year-wise Sales → Column / Bar Chart
- Month-wise Sales → Line Chart
- Region Sales → Pie Chart
- Sales vs Production Cost → Combination Chart

---

## SQL Analysis

The SQL section contains Q0–Q13.

### Q0 — Union of Sales Tables
Combines the two sales sources for analysis.

### Q1 — Lookup Product Name
Uses product information to bring the product name into the sales analysis.

### Q2 — Lookup Customer Name & Unit Price
Adds customer information and unit price.

### Q3 — Date Columns from OrderDateKey
Creates / derives date-related information such as year, month and quarter.

### Q4 — Sales Amount
Calculates sales amount using unit price, order quantity and discount information.

### Q5 — Production Cost
Calculates production cost using product standard cost and order quantity.

### Q6 — Profit Calculation
Calculates profit from sales and production cost.

### Q7 & Q9 — Month and Sales Table
Creates month-wise sales analysis.

### Q8 — Year-wise Sales
Analyzes annual sales performance.

### Q10 — Quarter-wise Sales
Analyzes quarterly sales performance.

### Q11 — Sales vs Production Cost
Compares sales against production cost.

### Q12 — KPI Development
Develops key performance indicators.

### Q13 — Overall Report
Provides the overall sales analysis report.

---

## Power BI

Power BI was used for:

- Power Query data cleaning
- Data modeling
- DAX calculations
- KPI cards
- Charts
- Slicers
- Interactive dashboard
- Business insights

### Dashboard KPIs

The final presentation reports:

- Total Sales: **29.36M**
- Total Profit: **12.08M**
- Total Orders: **60.40K**
- Profit Margin: **41.15%**
- Average Order Value: **486.09**

---

## Tableau

Tableau was used for:

- Calculated fields
- Filters
- Interactive visualizations
- Year-wise sales
- Month-wise sales
- Quarter-wise sales
- Regional sales
- Sales vs Product Cost

Filters shown in the project:
- Year
- Region
- Month
- Quarter

---

## Key Business Insights

According to the final project presentation:

### Peak Year
**2013** recorded the highest annual sales at approximately **16.4M**.

### Top Region
**Southwest** led regional performance. The presentation also identifies **Australia** as the strongest international market by sales.

### Top Product
**Mountain-200 Black (42)** was the best-selling product at approximately **1.37M**.

### Top Customer
**Jordan Turner** led customer purchases at approximately **16.0K**.

### Quarterly Performance
**Q4** consistently delivered the strongest quarterly sales, indicating a year-end seasonal effect.

### Sales vs Cost
Production cost remained below sales across the period, supporting an overall margin of approximately **41%**.

---

## Tools & Skills

### Excel
- Data Preparation
- Pivot Tables
- Charts
- Slicers
- Dashboarding

### SQL / MySQL
- SELECT
- WHERE
- JOIN
- UNION / UNION ALL
- GROUP BY
- Aggregations
- Date functions
- Calculated fields
- Business analysis queries

### Power BI
- Power Query
- Data Modeling
- DAX
- KPI Cards
- Slicers
- Interactive Dashboards

### Tableau
- Calculated Fields
- Filters
- Charts
- Interactive Dashboards
- Business Visualization

---

## Project Workflow

```text
Raw Data
   ↓
Data Cleaning & Preparation
   ↓
Excel / Power Query
   ↓
Data Modeling
   ↓
SQL Analysis
   ↓
Power BI & Tableau Visualization
   ↓
Interactive Dashboards
   ↓
Business Insights & Final Report
```

---

## How to Use the Project Files

### For Excel
Open:

`Adventure_Works_project.xlsx`

Review the cleaned data, pivot tables, charts, slicers and dashboard.

### For SQL
Open:

`Adventure_Works_SQL_Queries_Q0_Q13.sql`

in MySQL Workbench.

Run the queries after the required Adventure Works tables/data have been imported into the database.

### For Power BI
Open:

`Adventure_work_project.pbix`

in Power BI Desktop.

Review the data model, Power Query steps, DAX measures and dashboard.

### For Tableau
Use the prepared Adventure Works data to recreate / review the Tableau visualizations included in the final project workflow.

### For Presentation
Open:

`Adventure Works Final PPT Group 4.pptx`

to view the final project presentation and summarized findings.

---

## Project Outcome

The Adventure Works project demonstrates an end-to-end data analytics workflow using **Excel, SQL, Power BI and Tableau**, transforming sales data into dashboards and business insights across products, customers, regions and time.

**Project:** Adventure Works Sales Analytics  
**Group:** Group 4  
**Year:** 2026
# Author
Anuradha Hasnabade
