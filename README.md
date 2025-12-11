# 🌍 World Energy Consumption Analysis using MySQL

This project analyzes **global energy consumption trends** across multiple countries and years using **MySQL**.  
It reveals insights on renewable vs non-renewable usage, regional consumption patterns, and long-term sustainability indicators.

---

## 📌 Project Overview
The goal of this analysis is to understand:

- Global energy consumption patterns  
- Regional differences in energy usage  
- Trends in renewable vs non-renewable energy  
- High-consumption countries and factors influencing growth  
- Year-over-year change in global demand  

---

## 🗂 Dataset Information
The dataset includes:

- **Countries:** 190+  
- **Years:** 1965–2020  
- **Attributes:** Energy consumption, population, renewable share, fossil fuel usage, etc.

> *Dataset Source:* Public energy statistics (BP, OWID, Kaggle)

---

## 🛠️ Tools & Technologies Used
- **MySQL** (Core analysis)
- **SQL Queries** (Joins, CTEs, Window Functions, Aggregations)
- **Python / Power BI** *(Optional for visualization if used)*

---

## 🔍 SQL Techniques Used
This project demonstrates strong SQL proficiency, including:

- INNER / LEFT Joins  
- Subqueries  
- Common Table Expressions (CTEs)  
- Window Functions (ROW_NUMBER, RANK, LEAD, LAG)  
- Grouping & Aggregation  
- Trend Analysis Queries  
- Data Cleaning using SQL  

---

## 📊 Key Insights Generated
- Countries with the **highest renewable energy adoption**  
- Countries with the **fastest-growing consumption**  
- **Top 10 high-consumption** energy consumers  
- Long-term shifts from **non-renewable → renewable energy**  
- Region-wise energy distribution patterns  
- Year-over-year growth in global demand  

---

## 🧠 Sample SQL Queries

### ▶ Top 10 Countries by Total Energy Consumption
```sql
SELECT country, SUM(energy_consumption) AS total_consumption
FROM energy_data
GROUP BY country
ORDER BY total_consumption DESC
LIMIT 10;
