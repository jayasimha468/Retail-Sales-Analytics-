# Retail Sales Analytics | Python, SQL & Interactive Dashboard

## 🚀 Live Dashboard

**[View Live Retail Sales Analytics Dashboard](https://2pfarusyhrhi4upvp5oufd.streamlit.app/)**

## Project Overview

An end-to-end Retail Sales Analytics project focused on analyzing sales performance, profitability, discount patterns, product categories, regional performance, customer segments, and shipping methods.

This project uses Python and Pandas for data cleaning and exploratory data analysis, SQLite and SQL for business-focused queries, and Streamlit with Plotly to build an interactive dashboard.

## Business Objectives

- Analyze overall sales and profit performance.
- Identify profitable and loss-making categories and subcategories.
- Evaluate the relationship between discounts and profitability.
- Compare regional and state-level performance.
- Analyze customer segment and shipping mode performance.
- Present business insights through an interactive dashboard.

## Tech Stack

- **Programming:** Python
- **Data Analysis:** Pandas
- **Database:** SQLite
- **Query Language:** SQL
- **Visualization:** Plotly
- **Dashboard:** Streamlit
- **Environment:** Jupyter Notebook
- **Deployment:** Streamlit Community Cloud

## Project Structure

```text
Retail-Sales-Analytics/
│
├── Enterprise_Retail_Sales_Analytics.ipynb
├── Retail_Sales_SQL_Analysis_Final.ipynb
├── retail_cleaned.csv
├── app.py
├── requirements.txt
└── README.md
```

## Analysis Performed

### Python Analysis
- Data cleaning and duplicate removal
- Exploratory Data Analysis (EDA)
- KPI calculations
- Category and subcategory analysis
- Regional sales and profit analysis
- Discount and profitability analysis
- Shipping mode analysis

### SQL Analysis
- SELECT, WHERE, ORDER BY and LIMIT
- Aggregate functions: SUM(), COUNT(), AVG()
- GROUP BY and HAVING
- CASE WHEN statements
- Subqueries
- INNER JOIN
- Window functions: RANK()
- Category, region, state and segment analysis

### Interactive Dashboard
- Total Sales, Total Profit and Profit Margin KPIs
- Category-wise sales visualization
- Region-wise profit visualization
- Discount vs. average profit analysis
- Subcategory performance table
- Loss-making transaction analysis
- Interactive filters for category, region and segment

## Key Business Findings

- Technology generated the highest total profit of $145,455.66.
- Furniture recorded the lowest profit margin at 2.49%.
- Office Supplies had the highest number of loss-making records (885).
- Higher discount levels were associated with negative aggregate profits.
- The West region recorded the highest total sales of $725,255.74.
- Consumer generated the highest total sales among customer segments.
- California recorded the highest total sales and total profit among the analyzed states.

## Dataset

The project uses the Sample Superstore retail sales dataset containing **9,977 records and 14 columns**.

Note: The dataset does not contain order dates or customer identifiers. Therefore, time-based and customer-level analysis was not performed.

## Run the Dashboard Locally

Clone the repository:

```bash
git clone https://github.com/jayasimha468/Retail-Sales-Analytics-.git
cd Retail-Sales-Analytics-
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the Streamlit application:

```bash
streamlit run app.py
```

## Deployment

The interactive dashboard is deployed using **Streamlit Community Cloud**.

**Live URL:** https://2pfarusyhrhi4upvp5oufd.streamlit.app/

## Conclusion

This project demonstrates practical skills in Python, Pandas, SQL, SQLite, data visualization, business analysis, and interactive dashboard development. It transforms retail transaction data into meaningful insights to support business decision-making.
