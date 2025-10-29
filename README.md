# 🟡 Blinkit Sales Dashboard – SQL, Excel & Power BI

![Main Dashboard Overview](blinkit_main_dashboard.png)

### 📊 Project Overview  
The **Blinkit Sales Dashboard** is a complete end-to-end data analytics project developed using **SQL**, **Excel**, and **Power BI**.  
It focuses on cleaning and analyzing Blinkit’s sales data to identify performance trends, top outlets, and customer preferences.  
The project delivers business insights through **automated data processing** and **interactive dashboards**.

---

## 🧰 Tools & Technologies Used  
- **SQL** – Data cleaning, transformation, and KPI creation  
- **Excel** – Data validation, pivot analysis, and initial dashboard  
- **Power BI** – Data modeling, visualization, and business insights  
- **Power Query** – Automated data connection and refresh  

---

## ⚙️ Project Workflow  

### 🧮 1. SQL – Data Cleaning & KPI Generation  
![SQL Data Cleaning](blinkit_sql_cleaning.png)

- Cleaned and standardized raw Blinkit sales data.  
- Removed duplicate and inconsistent records for accurate reporting.  
- Created KPIs using SQL aggregate functions such as:  
  - `SUM(Total_Sales)` → Total Sales  
  - `AVG(Rating)` → Average Rating  
  - `COUNT(Item_Identifier)` → Total Items Sold  
- Prepared analysis-ready data for Excel and Power BI integration.  

**Example SQL Query:**
```sql
SELECT 
  Outlet_Type, 
  SUM(Total_Sales) AS Total_Sales, 
  AVG(Total_Sales) AS Avg_Sales, 
  COUNT(*) AS No_Of_Items, 
  AVG(Rating) AS Avg_Rating
FROM blinkit_sales
GROUP BY Outlet_Type;
