# Olist_Data_Analysis
An end-to-end data analysis of the Olist E-Commerce dataset using SQL for data extraction and Power BI for interactive visualization, focusing on sales trends, logistical bottlenecks, and customer satisfaction.


# 🛒 Olist E-Commerce Analytics Dashboard

## 📌 Project Overview
This project is an end-to-end data analysis of the **Brazilian E-Commerce Public Dataset by Olist** (provided via Kaggle). The objective of this case study is to extract actionable business insights from over 100,000 orders to improve platform profitability and operational efficiency. 

The analysis is broken down into three core business pillars:
1. **Sales Performance:** Evaluating revenue trends and category profitability.
2. **Logistical Efficiency:** Identifying geographical bottlenecks and SLA compliance.
3. **Customer Behavior:** Determining the critical factors that influence customer satisfaction and review scores.

## 🛠️ Tech Stack
* **Database Management:** MS SQL Server (SSMS)
* **Data Manipulation & Querying:** T-SQL (CTEs, Window Functions, Aggregate Functions, Complex JOINs)
* **Data Visualization & BI:** Power BI 
* **Design & UI:** Canva (Custom Dashboard Backgrounds)

## 📊 Dashboard Highlights

### 1. Sales Performance
* Tracks the monthly revenue trajectory across 2016-2018.
* Identifies high-value product categories (e.g., *Health & Beauty*, *Watches & Gifts*).
* Monitors the Average Order Value (AOV) to gauge consumer purchasing habits.

### 2. Logistical Efficiency
* Features an SLA Compliance monitor (On-Time vs. Late deliveries).
* Utilizes geographical mapping to highlight extreme delivery bottlenecks in Northern Brazilian states (RR, AP, AM).
* Tracks the overall platform average delivery lead time.

### 3. Customer Behavior
* Proves the "Speed-to-Satisfaction" correlation, showing a direct link between delivery lead times and 1-star vs. 5-star reviews.
* Highlights the highest and lowest-rated product categories to assist with vendor quality control.

## 💡 Key Business Insights
1. **The Q4 Revenue Spike:** The platform experiences massive seasonal growth in November (Black Friday), necessitating scaled logistics and warehouse capacity in Q4.
2. **The Northern Bottleneck:** While the platform has a healthy 93.2% on-time delivery rate, customers in remote states (Roraima, Amapá) experience 25+ day wait times. 
3. **The Root Cause of Bad Reviews:** Slow shipping is the primary driver of 1-star reviews. 5-star reviews average 10 days for delivery, while 1-star reviews stretch to 20+ days. 
4. **Strategic Recommendation:** Olist must pivot from national couriers to localized 3PL (Third-Party Logistics) partners in the extreme North to reduce lead times and improve overall customer lifetime value.

## ⚙️ Methodology & Data Architecture
To ensure high dashboard performance, a two-step approach was utilized:
* **Pre-Aggregation:** Instead of relying on a complex Star Schema in Power BI, heavy data transformations and metric calculations (e.g., running totals, date differences) were executed directly in SQL Server.
* **Data Integrity:** Missing values (NULLs) in critical fields like delivery dates were deliberately converted to "Unknown" rather than deleted, ensuring total revenue and order volume metrics were not artificially skewed.

## 🚀 How to Explore This Project
1. **SQL Scripts:** Navigate to the `/SQL_Queries` folder to view the raw T-SQL code used for data extraction and cleaning.
2. **Power BI Dashboard:** Download the `Olist_Dashboard.pbix` file and open it in Power BI Desktop to interact with the slicers and visuals.
3. **Executive Report:** View the `Case_Study_Report.pdf` for the full business presentation and strategic recommendations.

## 👨‍💻 Author
**John Carlo Ablay**
* **Role:** Aspiring Data Analyst
* **LinkedIn:** [Insert your LinkedIn URL here]
* **Portfolio:** [Insert your Portfolio URL here]
