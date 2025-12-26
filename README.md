# 🛒 E-commerce Sales Analysis  
A Data Analytics Project using Python, SQL & Visualization

## 📌 Project Overview
This project analyzes sales data from an e-commerce business to uncover insights about customer behavior, geographic performance, and monthly sales trends.  
Multiple CSV datasets were merged, cleaned, and transformed to extract meaningful insights and build visualizations.

---

## 🎯 Objectives
- Perform **ETL (Extract, Transform, Load)** on raw e-commerce sales data  
- Store & query structured data using **SQL**
- Analyze **sales patterns, regional performance, and customer distribution**
- Visualize insights using **Matplotlib & Seaborn**

---

## 🛠️ Technologies Used
| Component | Technology |
|----------|------------|
| Programming | Python |
| Data Processing | Pandas |
| Database / Querying | SQL |
| Visualizations | Matplotlib, Seaborn |
| File Format | CSV |

---

## 📂 Dataset
- **7 CSV files** representing different sales-related data sources  
- After ETL processing, structured into a tabular format for SQL querying

---

## 🚀 ETL Process
1. **Extract** – Loaded all CSV files into Pandas  
2. **Transform** –  
   - Cleaned missing values  
   - Formatted date & categorical columns  
   - Merged datasets into a unified structure  
3. **Load** – Exported processed data for SQL querying

---

## 📊 Key Insights Generated
| Insight Type | Description |
|--------------|-------------|
| **Monthly Sales Trend** | Identified peak revenue months |
| **Top Performing States** | Ranked states by total sales |
| **Customer Distribution** | Visualized number of customers by region |

---

## 📈 Visualizations
- 📅 **Monthly Sales Trend (Bar Chart)**
- 🌍 **Sales Contribution by State (Horizontal Bar Chart)**
- 👥 **Customer Count by Region (Pie Chart / Bar Chart)**

> *Visualizations help measure seasonality, regional demand, and business growth opportunities.*

---

## 📎 Example SQL Queries
```sql
-- Top 5 states by total sales
SELECT state, SUM(amount) AS total_sales
FROM ecommerce_sales
GROUP BY state
ORDER BY total_sales DESC
LIMIT 5;

-- Monthly revenue trend
SELECT monthname(order_date) AS month, SUM(amount) AS revenue
FROM ecommerce_sales
GROUP BY month
ORDER BY revenue DESC;
```

## Results

✔ Monthly sales patterns showed seasonal demand peaks
✔ Top states contributed majority of revenue
✔ Customer distribution was uneven, guiding marketing opportunities
