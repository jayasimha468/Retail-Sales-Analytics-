# Retail Sales Analytics | Python, SQL & Business Insights

## Project Overview

An end-to-end Retail Sales Analytics project focused on evaluating sales performance, profitability, discount patterns, product categories, regional performance, customer segments, and shipping methods.

This project uses Python for data cleaning and Exploratory Data Analysis (EDA), and SQLite with SQL for business-focused analysis. The objective is to transform raw retail data into meaningful business insights and actionable recommendations.

## Business Objectives

- Analyze overall sales and profit performance.
- Identify profitable and loss-making product categories and subcategories.
- Evaluate the relationship between discounts and profitability.
- Compare sales and profit performance across regions and states.
- Analyze customer segment performance.
- Evaluate shipping mode performance.
- Generate data-driven business recommendations.

## Tech Stack

- **Programming:** Python
- **Data Analysis:** Pandas
- **Database:** SQLite
- **Query Language:** SQL
- **Environment:** Jupyter Notebook

## Project Structure

```text
Retail-Sales-Analytics/
│
├── Enterprise_Retail_Sales_Analytics.ipynb
├── Retail_Sales_SQL_Analysis_Final.ipynb
├── retail_cleaned.csv
└── README.md
```

## Analysis Performed

### Python Analysis

- Data cleaning and duplicate removal
- Exploratory Data Analysis (EDA)
- KPI calculation
- Category and subcategory performance analysis
- Regional sales and profit analysis
- Discount and profitability analysis
- Shipping mode analysis
- Business insights and recommendations

### SQL Analysis

- Data loading and SQLite database creation
- SELECT, WHERE, ORDER BY and LIMIT
- Aggregate functions: SUM(), COUNT(), AVG()
- GROUP BY and HAVING
- CASE WHEN statements
- Subqueries
- INNER JOIN
- Window functions: RANK()
- Category-wise and subcategory-wise analysis
- Region-wise, state-wise and segment-wise analysis
- Discount impact and loss-making transaction analysis

## Key Business Findings

1. **Technology** generated the highest total profit of $145,455.66.
2. **Furniture** recorded the lowest profit margin at 2.49%, despite generating $741,306.50 in sales.
3. **Office Supplies** had the highest number of loss-making records (885).
4. Higher discount levels were associated with negative aggregate profits in this dataset.
5. The **West region** recorded the highest total sales ($725,255.74) and total profit ($108,330.15).
6. The **Consumer segment** generated the highest total sales, while Home Office had the highest average profit per record.
7. **California** recorded the highest total sales and total profit among the analyzed states.

## Business Recommendations

- Review pricing and discount strategies for Furniture.
- Investigate loss-making transactions in Office Supplies.
- Monitor high-discount transactions to protect profit margins.
- Maintain the strong profitability of Technology products.
- Evaluate regional and state-level performance to identify growth opportunities.
- Monitor average profit across customer segments.

## Dataset

The project uses the Sample Superstore retail sales dataset, containing 9,977 records and 14 columns, including sales, profit, quantity, discount, product category, region, customer segment, and shipping information.

**Note:** The dataset does not contain order dates or customer identifiers. Therefore, time-based and customer-level analysis was not performed.

## Conclusion

This project demonstrates practical data analytics skills using Python, Pandas, SQLite, and SQL. It covers data cleaning, exploratory analysis, SQL querying, business performance evaluation, and the extraction of actionable insights from retail sales data.vvv
