# 🍕 Pizza Sales Analysis & Dashboard  

This project analyzes pizza sales data to uncover business insights using **SQL (SSMS)** and **Excel (Pivot Tables, Pivot Charts, Dashboards)**. The aim is to calculate key KPIs, identify sales patterns, and present findings in a professional format.  

---

## 🔎 Problem Statement  
The objective was to evaluate sales performance of a pizza store by analyzing historical data. The goal was to:  
- Identify key performance indicators (KPIs).  
- Analyze sales trends over time (daily, weekly, hourly).  
- Examine sales contribution by pizza category and size.  
- Discover best and worst-selling products.  
- Build a dashboard for **quick, visual decision-making**.  

---

## 🔑 Project Highlights  
- **KPI Calculation (SQL):** Designed queries to compute Total Revenue, Total Orders, Average Order Value, Pizzas Sold, and Avg. Pizzas per Order.  
- **Trend Analysis:** Evaluated customer ordering behavior by day of the week and hour of the day.  
- **Category & Size Breakdown:** Analyzed sales distribution across categories (Classic, Veggie, Supreme, Chicken) and pizza sizes.  
- **Product Performance:** Identified **Top 5 best sellers** and **Bottom 5 underperformers**.  
- **Dashboard:** Built an interactive Excel dashboard summarizing insights with Pivot Tables & Charts.  
- **Reporting:** Documented findings in a professional Word report with visualizations and recommendations.  

---

## 📊 Tools & Technologies  
- **SQL (SSMS):** Data extraction, KPI generation, and sales analysis queries.  
- **Excel:** Pivot Tables, Pivot Charts, and interactive dashboard design.  
- **MS Word:** Documentation of business insights and reporting.  

---

## 📈 Key Insights  
- 💰 **Revenue:** Generated **$817K+** from ~21,000 orders.  
- 🍕 **Pizzas Sold:** Over **49,000 pizzas** sold, with Classic & Supreme categories leading sales.  
- 📆 **Daily Trends:** Highest orders placed on **Fridays and weekends**.  
- ⏰ **Hourly Trends:** Peak sales during **lunch (12–2 PM)** and **dinner (6–8 PM)** hours.  
- 🥇 **Top Performers:** Best-selling pizzas drove a significant share of revenue.  
- 🥴 **Underperformers:** Bottom 5 pizzas had minimal contribution, highlighting opportunities for menu optimization.  

---

## 📂 Project Structure  
/Pizza-Sales-Analysis
├── pizza_sales.xlsx # Dataset + Pivot Table Dashboard
├── SQL_Queries.docx # SQL queries for KPIs and analysis
├── Sales_Report.docx # Professional report with findings
└── README.md # Documentation

--


---

## 🛠️ SQL Query Examples  

**1. Total Revenue**  
```sql
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

SELECT DATENAME(DW, order_date) AS order_day, 
       COUNT(DISTINCT order_id) AS total_orders 
FROM pizza_sales
GROUP BY DATENAME(DW, order_date);

SELECT TOP 5 pizza_name, SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold DESC;
```

--

 ## 📌 Outcomes  
- Built an **end-to-end analytics pipeline**: Data → SQL Queries → Excel Dashboard → Word Report.  
- Delivered insights into customer ordering behavior, product performance, and sales trends.  
- Showcased practical skills in **SQL, Excel visualization, and business analysis**.  
- Demonstrated ability to turn raw data into **actionable insights** for decision-making.  

---

## 🚀 Learning & Takeaways  
- Strengthened SQL skills for business-focused queries and KPI tracking.  
- Learned to build interactive dashboards in Excel using Pivot Tables & Charts.  
- Practiced presenting technical findings in a clear, business-friendly report.  
- Demonstrated the value of combining **data analytics and visualization** for retail decision-making.  

