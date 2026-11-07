# Retail Sales Analytics | Python, SQL & Interactive Dashboard

## 🚀 Live Dashboard

[View Live Retail Sales Analytics Dashboard](https://2pfarusyhrhi4upvp5oufd.streamlit.app/)

## 📌 Project Overview

Retail Sales Analytics is an end-to-end data analytics project focused on analyzing retail business performance and generating meaningful business insights.

The project uses Python and Pandas for data cleaning and exploratory data analysis, SQLite for SQL-based business analysis, and Streamlit with Plotly to build an interactive dashboard.

The objective is to understand sales and profitability, evaluate regional and category performance, identify loss-making areas, and present findings through interactive visualizations.

## 🏗️ Project Architecture

The following architecture diagram illustrates the complete workflow, from raw data processing to dashboard deployment.

![Retail Sales Analytics Project Architecture](architecture.png)

## 🎯 Business Objectives

- Analyze overall sales and profit performance.
- Identify profitable and loss-making product categories.
- Compare sales and profitability across regions.
- Evaluate the relationship between discounts and profitability.
- Analyze customer segments and shipping methods.
- Build an interactive dashboard to communicate business insights.

## 📂 Dataset

- **Dataset:** Sample Superstore
- **Total Records:** 9,977
- **Total Columns:** 14
- **Format:** CSV

### Key Columns

`Ship_Mode`, `Segment`, `Country`, `City`, `State`, `Postal_Code`, `Region`, `Category`, `Sub_Category`, `Sales`, `Quantity`, `Discount`, `Profit`, `Discount_Group`

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data analysis |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| SQLite | SQL-based data analysis |
| SQL | Business queries and aggregations |
| Plotly | Interactive visualizations |
| Streamlit | Dashboard development |
| Git & GitHub | Version control and project hosting |

## 🔄 Project Workflow

### 1. Data Cleaning and Preparation
- Loaded the retail dataset using Pandas.
- Inspected data types and dataset structure.
- Checked for missing values and duplicate records.
- Removed duplicate records.
- Prepared the cleaned dataset for analysis.

### 2. Exploratory Data Analysis (EDA)
- Analyzed sales and profit distribution.
- Compared category and subcategory performance.
- Evaluated regional sales and profitability.
- Examined customer segments and shipping methods.
- Investigated discount patterns and their association with profit.

### 3. SQL Analysis Using SQLite

Performed business-focused SQL analysis using:

- SELECT, WHERE and ORDER BY
- Aggregate functions: SUM, AVG and COUNT
- GROUP BY and HAVING
- CASE WHEN statements
- Subqueries
- INNER JOIN
- Window functions such as RANK()

### 4. Interactive Dashboard Development

Developed an interactive dashboard using Streamlit and Plotly with:

- Total Sales, Total Profit and Profit Margin KPI cards.
- Category-wise sales analysis.
- Region-wise profitability analysis.
- Discount versus average profit visualization.
- Subcategory performance analysis.
- Loss-making records analysis.
- Interactive filters for Category, Region and Segment.
- Filtered dataset exploration.

### 5. Deployment

Deployed the dashboard using Streamlit Community Cloud.

**Live Dashboard:** https://2pfarusyhrhi4upvp5oufd.streamlit.app/

## 📊 Key Business Insights

| Metric | Result |
|---|---:|
| Total Sales | $2,296,195.81 |
| Total Profit | $286,242.20 |
| Total Records | 9,977 |
| Profit Margin | 12.47% |
| Loss-Making Records | 1,869 |
| Total Loss | -$156,113.56 |

### Important Findings

- Technology generated the highest category-level profit.
- The West region recorded the highest regional sales and profit.
- Furniture had a relatively low profit margin compared with other categories.
- Tables, Bookcases and Supplies were among the loss-making subcategories.
- Higher discount levels were associated with lower profitability in the analyzed data.

**Note:** These findings describe observed patterns in the dataset and do not establish causation.

## 📁 Project Structure

```text
Retail-Sales-Analytics/
│
├── Enterprise_Retail_Sales_Analytics.ipynb
├── Retail_Sales_SQL_Analysis_Final.ipynb
├── app.py
├── requirements.txt
├── retail_cleaned.csv
├── architecture.png
└── README.md
```

## ▶️ Run the Project Locally

### Step 1: Clone the Repository

```bash
git clone https://github.com/jayasimha468/Retail-Sales-Analytics-.git
```

### Step 2: Navigate to the Project Folder

```bash
cd Retail-Sales-Analytics-
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Streamlit Dashboard

```bash
streamlit run app.py
```

The dashboard will open in your browser.

## 📌 Project Links

- **Live Dashboard:** https://2pfarusyhrhi4upvp5oufd.streamlit.app/
- **GitHub Repository:** https://github.com/jayasimha468/Retail-Sales-Analytics-

## 👨‍💻 Author

**Jayasimha Obulam** 

B.Tech – Artificial Intelligence and Machine Learning

**Technical Areas:** Python | SQL | Data Analytics | Data Visualization | Machine Learning

---

*This project demonstrates practical skills in data cleaning, exploratory data analysis, SQL querying, business intelligence, interactive dashboard development, and deployment.*
