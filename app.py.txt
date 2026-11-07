
import streamlit as st
import pandas as pd
import plotly.express as px
from pathlib import Path

st.set_page_config(
    page_title="Retail Sales Analytics",
    page_icon="📊",
    layout="wide"
)

@st.cache_data
def load_data():
    file_path = Path(__file__).parent / "retail_cleaned.csv"
    return pd.read_csv(file_path)

df = load_data()

st.title("📊 Retail Sales Analytics Dashboard")
st.write("Retail Sales Analysis using Python, Pandas and SQL.")

st.sidebar.header("Dashboard Filters")

categories = st.sidebar.multiselect(
    "Category",
    df["Category"].unique(),
    default=list(df["Category"].unique())
)

regions = st.sidebar.multiselect(
    "Region",
    df["Region"].unique(),
    default=list(df["Region"].unique())
)

segments = st.sidebar.multiselect(
    "Segment",
    df["Segment"].unique(),
    default=list(df["Segment"].unique())
)

filtered_df = df[
    df["Category"].isin(categories)
    & df["Region"].isin(regions)
    & df["Segment"].isin(segments)
]

if filtered_df.empty:
    st.warning("No data available for selected filters.")
    st.stop()

total_sales = filtered_df["Sales"].sum()
total_profit = filtered_df["Profit"].sum()
total_records = len(filtered_df)
profit_margin = (
    total_profit / total_sales * 100
    if total_sales != 0 else 0
)

col1, col2, col3, col4 = st.columns(4)

col1.metric("Total Sales", f"${total_sales:,.2f}")
col2.metric("Total Profit", f"${total_profit:,.2f}")
col3.metric("Total Records", f"{total_records:,}")
col4.metric("Profit Margin", f"{profit_margin:.2f}%")

st.divider()

left, right = st.columns(2)

category_sales = (
    filtered_df.groupby("Category", as_index=False)
    .agg(Total_Sales=("Sales", "sum"))
)

with left:
    st.subheader("Sales by Category")
    fig = px.bar(
        category_sales,
        x="Category",
        y="Total_Sales",
        color="Category"
    )
    st.plotly_chart(fig, use_container_width=True)

region_profit = (
    filtered_df.groupby("Region", as_index=False)
    .agg(Total_Profit=("Profit", "sum"))
)

with right:
    st.subheader("Profit by Region")
    fig = px.bar(
        region_profit,
        x="Region",
        y="Total_Profit",
        color="Region"
    )
    st.plotly_chart(fig, use_container_width=True)

st.subheader("Discount vs Average Profit")

discount_analysis = (
    filtered_df.groupby("Discount", as_index=False)
    .agg(Average_Profit=("Profit", "mean"))
)

fig = px.line(
    discount_analysis,
    x="Discount",
    y="Average_Profit",
    markers=True
)
st.plotly_chart(fig, use_container_width=True)

st.subheader("Subcategory Performance")

subcategory = (
    filtered_df.groupby("Sub_Category", as_index=False)
    .agg(
        Total_Sales=("Sales", "sum"),
        Total_Profit=("Profit", "sum")
    )
    .sort_values("Total_Profit", ascending=False)
)

st.dataframe(subcategory, use_container_width=True)

st.subheader("Loss Analysis")

loss_records = filtered_df[filtered_df["Profit"] < 0]

col1, col2 = st.columns(2)
col1.metric("Loss Records", len(loss_records))
col2.metric(
    "Total Loss",
    f"${loss_records['Profit'].sum():,.2f}"
)

with st.expander("View Dataset"):
    st.dataframe(filtered_df, use_container_width=True)

st.caption("Retail Sales Analytics | Python | Pandas | Plotly | Streamlit")
