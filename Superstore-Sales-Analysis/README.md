# 📊 Superstore Sales Analysis – Power BI Project

## 📁 Project File
**File:** `Superstore_sales_analysis.pbix`

This project presents an interactive Power BI dashboard built to analyze four years of Superstore sales data. It uncovers insights on regional performance, product profitability, customer behavior, and time-based trends using clean, professional visuals and DAX-based KPIs.

---

## 🎯 Objectives

- Identify top-performing and underperforming product categories and regions.
- Track sales and profit trends across time using drill-down and dynamic filters.
- Provide detailed drillthrough analysis by segment, category, and geography.
- Create a visually intuitive report suitable for executive decision-making.

---

## 🚀 Dashboard Pages & Features

### 🔹 Page 1 – Overview
- ✅ KPI Cards: Total Sales, Total Profit, Total Orders, Average Order Value, Total Customers.
- 📈 Line Chart: Monthly trend of sales and profit with drill-down via date hierarchy.
- 🔝 Bar Chart: Top 5 sub-categories by profit or sales using TopN filter.
- 🌍 Filled Map: State-level profit heatmap with conditional formatting.

### 🔹 Category Page – Drillthrough Details
- 🔍 Drillthrough-enabled by selecting a specific `State`, `Category`, or `Customer Segment`.
- 📥 Filtered views show granular-level performance tied to the selected item.
- 🔁 Back button included for user-friendly navigation.

---

## 💡 Key Visual Elements & DAX Measures

| Metric | Formula |
|--------|---------|
| **Average Order Value** | `= SUM(Sales) / DISTINCTCOUNT(Order ID)` |
| **Previous 6 Months Sales** | `= CALCULATE(SUM(Sales), DATESINPERIOD(Order Date, MAX(Order Date), -6, MONTH))` |

Other elements:
- Dynamic date hierarchy
- Slicers for Category and Segment
- Conditional formatting on maps
- Custom `YearMonth` column for accurate time-axis sorting

---

## 🗺️ Geographic Insights

- Filled map shows profit by state, color-scaled using conditional formatting.
- Cities and customer segments analyzed using stacked bar and column charts.

---

## 📈 Data Trends

- 📊 Seasonal spikes in December (holiday sales)
- 🚨 Losses in Central region despite high sales
- 🥇 Technology category outperforms others in profitability

---

## 📦 Dataset

- Source: [Kaggle - Sales Forecasting Dataset](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)
- Contains:
  - `Order ID`, `Order Date`, `Customer ID`, `Region`, `State`, `City`
  - `Category`, `Sub-Category`, `Sales`, `Profit`, `Quantity`, `Discount`

---

## 🛠 Tools Used

- **Power BI Desktop**
- DAX (Data Analysis Expressions)
- Date hierarchies and drillthrough filters
- Conditional formatting for visual enhancement

---

## 📘 How to Use

1. Open `Superstore_sales_analysis.pbix` in Power BI Desktop.
2. Explore Page 1 for high-level KPIs and top-performing segments.
3. Select any state or category → Right-click or use the drillthrough button → Navigate to Page 2/5.
4. Use slicers or hierarchy buttons to drill down into time-based trends.
5. Hover over maps or bars to view detailed tooltips.

---


## 📄 License

This is a personal project built for educational demonstration purposes.

---

## 🙋‍♂️ Author

**Soumya Reddy**  
Graduate Student | Data Analyst  
[LinkedIn](https://www.linkedin.com/in/soumyab04/)
[Email](soumyabaddham@gmail.com)

