<h1 align="center">🟡 Blinkit Sales Dashboard</h1>
<h3 align="center">SQL | Excel | Power BI</h3>

<p align="center">
  <img src="blinkit_main_dashboard.png" alt="Blinkit Dashboard Overview" width="85%" style="border-radius:15px;box-shadow:0 0 10px rgba(0,0,0,0.2);"/>
</p>

---

## 🧠 Project Overview  
The **Blinkit Sales Dashboard** is a complete **data analytics and visualization project** integrating **SQL, Excel, and Power BI**.  
It provides an in-depth analysis of sales trends, outlet performance, and customer preferences — helping the company make informed business decisions.

🔹 **Goal:** Build an automated pipeline from SQL to Excel to Power BI  
🔹 **Focus Areas:** Data Cleaning, KPI Creation, and Interactive Visualization  
🔹 **Outcome:** A dynamic dashboard enabling outlet-level performance monitoring  

---

## 🧰 Tools & Technologies Used  
| Tool | Purpose |
|------|----------|
| 🧮 **SQL** | Data extraction, cleaning & KPI generation |
| 📗 **Excel** | Data validation, pivot analysis & dashboarding |
| 📊 **Power BI** | Interactive dashboards & advanced data visualization |
| ⚙️ **Power Query** | Data transformation & automated refresh |

---

## ⚙️ Project Workflow  

### 🧩 Step 1: SQL – Data Cleaning & KPI Generation  
<p align="center">
  <img src="blinkit_sql_cleaning.png" alt="SQL Data Cleaning" width="85%" style="border-radius:15px;box-shadow:0 0 10px rgba(0,0,0,0.2);"/>
</p>

✅ Removed duplicates, nulls, and inconsistent categories  
✅ Created KPIs: `Total Sales`, `Average Rating`, `Outlet Performance`  
✅ Standardized item categories and outlet metadata  

**Sample Query**
```sql
SELECT Outlet_Type, 
       SUM(Total_Sales) AS Total_Sales, 
       AVG(Total_Sales) AS Avg_Sales, 
       COUNT(*) AS Items_Sold, 
       AVG(Rating) AS Avg_Rating
FROM blinkit_sales
GROUP BY Outlet_Type;
