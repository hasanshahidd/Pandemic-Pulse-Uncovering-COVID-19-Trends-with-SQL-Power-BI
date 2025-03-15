<h1 align="center">🦠 Pandemic Pulse: Uncovering COVID-19 Trends with SQL & Power BI 📊</h1>

<p align="center">
  <img src="covid/image/DALL·E 2025-03-15 11.43.41 - A digital banner for 'Pandemic Pulse_ Health Trends & Insights'. The background features a global map with highlighted health trend zones. A modern da.webp" alt="Pandemic Pulse Banner"/>
</p>

---

## 🚀 Project Overview

COVID-19 has transformed the world, and data analytics plays a crucial role in understanding its impact. **Pandemic Pulse** is a comprehensive data analysis project that leverages:
- **SQL (PostgreSQL)** for data extraction, transformation, and querying.
- **Power BI** for dynamic, interactive visualizations.
- **Excel** for initial data storage and cleaning.

This project explores **global COVID-19 trends** with a deep dive into **cases, deaths, and vaccinations** across different regions.  
It showcases my expertise in **data analytics, dashboarding, and performance-driven storytelling** using SQL and Power BI.

---

## 🌍 Dataset Source & Scope

📂 **Dataset:** [Our World in Data - COVID-19](https://ourworldindata.org/covid-deaths)  
📈 **Key Focus Areas:**  
- **Total Cases, Deaths & Vaccinations** (Globally)  
- **Trends Over Time** (Yearly, Quarterly & Monthly)  
- **Vaccination Coverage & Case Fatality Rates**  

---

## 🛠 Tools & Technologies Used

<p align="left">
  <a href="https://www.postgresql.org/" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="PostgreSQL" width="50" height="50"/>
  </a>
  <a href="https://powerbi.microsoft.com/" target="_blank">
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/fb/PowerBI_Logo.svg" alt="PowerBI" width="50" height="50"/>
  </a>
  <a href="https://www.microsoft.com/en-us/microsoft-365/excel" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/excel/excel-original.svg" alt="Excel" width="50" height="50"/>
  </a>
</p>

- **Excel** – Initial data cleaning & preprocessing  
- **PostgreSQL** – SQL queries for data transformation & insights  
- **Power BI** – Data visualization, dashboards & reports  

---

## 🏗️ Data Processing Steps

🔹 **Excel (Data Preprocessing & Cleaning)**  
✔ Removed unnecessary columns  
✔ Filtered out inconsistencies & missing data  

🔹 **SQL (Data Transformation & Analysis)**  
✔ Imported CSV dataset into **PostgreSQL**  
✔ Applied **SELECT, GROUP BY, HAVING, WINDOW FUNCTIONS, CTEs & VIEWS**  
✔ Derived meaningful KPIs for deeper insights  

🔹 **Power BI (Dashboard & Visualizations)**  
✔ Integrated **PostgreSQL queries** into Power BI  
✔ Built **interactive & dynamic dashboards**  
✔ Created **DAX measures & calculated columns** for additional insights  

![Power BI Dashboard](covid/image/Screenshot%202025-03-15%20113944.png)

---

## 📊 Key Insights  

Here are five key areas explored in this project:  

### 🟢 1. Global Overview  
- Displays **Total Cases, Deaths & Vaccinations**  
- Includes **Yearly, Quarterly & Monthly** breakdowns  

### 🔵 2. Global Cases & Deaths Trends  
- **Line charts** for trends over time  
- **Stacked bar charts** for comparisons  
- Dynamic **slicers & drill-downs**  

### 🟡 3. Vaccination Progress  
- **% Population Vaccinated** worldwide  
- Comparison of **Vaccination Rate vs Death Rate**  

### 🔴 4. Pandemic Impact Analysis  
- Understanding **wave patterns**  
- Death rate fluctuations over time  

### 🟣 5. Final Summary & Future Trends  
- Predictive insights for future pandemic management  
- Lessons learned from global data  

---

## 🔥 SQL Queries & Analytical Approach  

I performed **advanced SQL queries** to extract meaningful insights from the dataset.  
Some key queries included:

```sql
-- Total Global COVID-19 Cases Over Time
SELECT EXTRACT(YEAR FROM date) AS Year, 
       SUM(new_cases) AS Total_Cases
FROM covid_data
GROUP BY Year
ORDER BY Year;
