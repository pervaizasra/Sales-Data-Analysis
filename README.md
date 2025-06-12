# Sales-Data-Analysis

# 🛒 Superstore Sales Analysis — End-to-End Data Analytics Project

![Power BI Dashboard](https://github.com/yourusername/superstore-sales-analysis/assets/dashboard-preview.png) <!-- Replace with actual image link -->

## 📌 Project Overview

This project showcases a full data analysis pipeline using a global Superstore sales dataset. The process includes data cleaning with Python, exploratory data analysis (EDA), and building an interactive dashboard using Power BI to visualize sales, profit, customer behavior, and shipping performance.

---

## 📂 Dataset Overview

The dataset contains **51,290** records and **21** columns, with transactional sales data including:

- `order_id`, `order_date`, `ship_date`
- `customer_name`, `segment`, `region`, `country`
- `product_name`, `category`, `sales`, `profit`, `discount`
- `order_priority`, `shipping_cost`

---

## 🔧 Phase 1: Data Cleaning (Python - Pandas)

| Step                           | Description                                |
|-------------------------------|--------------------------------------------|
| ✅ Missing Values             | Confirmed no nulls in dataset              |
| ✅ Duplicate Removal          | Removed repeated `order_id`s               |
| ✅ Type Conversion            | Converted dates to `datetime`              |
| ✅ New Features               | Extracted `order_month`, `order_year`      |
| ✅ Shipping Delay             | Created `shipping_delay_days` (ship - order) |

Cleaned data exported to `cleaned_superstore_data.csv` for Power BI.

---

## 📊 Phase 2: Exploratory Data Analysis (EDA)

Conducted using **Seaborn**, **Matplotlib**, and **Plotly**:

### 🕒 Time Trends
- Sales trend shows growth over years with Q4 spikes.
- Monthly breakdown reveals seasonal peaks.

### 👤 Customer Behavior
- Top 10 customers contribute to over 20% of revenue.
- Consumer segment dominates overall sales volume.

### 🌍 Geographic Insights
- US and India lead in sales.
- Some regions have high sales but negative profit → optimization needed.

### 🚚 Shipping Performance
- Avg delay: ~2.9 days.
- Most orders use Standard Class shipping.

---

## 📈 Phase 3: Power BI Dashboard (5 Pages)

📁 File: [`Sales Analysis.pbit`](./Sales%20Analysis.pbit)

| Page               | Visualizations Included                                  |
|--------------------|-----------------------------------------------------------|
| Executive Summary  | KPI cards, sales trend line, profit by region, map view   |
| Time-Based Trends  | Monthly sales & orders, YoY growth                        |
| Customer Insights  | Top customers, segment pie chart, orders by market        |
| Regional Insights  | Tree map, bar chart, map: sales by country                |
| Shipping Insights  | Shipping delay analysis, mode distribution, segment view  |

⚙️ Built using DAX measures like:
- `Total Sales`, `Total Profit`, `Orders Count`
- `Avg Shipping Delay`, `YoY Sales Growth %`, `Customer Sales`

---

## 📦 Tools Used

- **Python**: Pandas, Seaborn, Plotly, Matplotlib
- **Power BI**: DAX, Data Modeling, Visualization
- **Jupyter Notebook**: Cleaning, EDA
- **Excel/CSV**: Data export for BI

---

## 📁 Project Structure

```
├── SuperStore_Analysis.ipynb       # Python notebook for cleaning + EDA
├── Sales Analysis.pbit             # Power BI template file
├── cleaned_superstore_data.csv     # Exported dataset for Power BI
├── README.md                       # Project documentation
└── assets/
    └── dashboard-preview.png       # Screenshots for GitHub README
```

---

## ✅ Key Takeaways

- Majority of sales come from **Consumer segment** and **Q4 months**.
- Top 10 customers are vital for profitability → Retarget campaigns.
- Shipping delays are consistent → Consider optimization or faster options.
- High sales ≠ high profit → Investigate loss-making regions.

---

## 📌 Next Steps (Optional Enhancements)

- Predictive modeling using `Prophet`, `ARIMA`, or `LSTM`
- Customer segmentation (KMeans, DBSCAN)
- Real-time dashboard deployment via Power BI Service

---

## 🌐 Author

**Asra Pervaiz**  
Data Analyst | Aviation + Business Intelligence | Power BI, Python, SQL  
[LinkedIn](https://www.linkedin.com/in/asra-pervaiz) • [Portfolio](https://yourportfolio.com) • [Email](mailto:your.email@example.com)

---
