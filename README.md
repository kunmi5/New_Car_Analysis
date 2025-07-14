# New_Car_Analysis
This project provides comprehensive information about car sales transactions, including dealer details, customer demographics and vehicle specifications.

---
## Project Overview 
A comprehensive analysis of automotive sales using an interactive dashboard. The dashboard summarizes key metrics such as total sales, transaction types, top-performing dealers, customer behavior, and income distribution trends.
---

## Tools Used
+ Excel for data cleaning and visualization
+ Power BI for visualization
+ SQL for data manipulation
+ Pivot table

---

## SQL queries
_How many category of color._
```sql
select color, count(distinct color)
from new_car_dataset
group by color;
```
_Retrieve the total number per body._
```sql
select body_style, count(*)
from new_car_dataset
group by body_style;
```
_Retrieve total number per transmission._
```sql
select transmission, count(*)
from new_car_dataset
group by transmission;
```
_Retrieve total sales amount for the year 2022._
```sql
select sum(Price)
from new_car_dataset
where year(date) = 2022;
```
_Retrieve sales for 2022 and 2023._
```sql
select sum(Price)
from new_car_dataset
where year(date) in (2022, 2023);
```
_Retrieve average sellingPrice._ 
```sql
select avg(Price)
from new_car_dataset;
```
_Retrieve average selling price for 2022 to 2023._
```sql
select avg(Price)
from new_car_dataset
where year(date) in (2022, 2023);
```
---

### Key Metrics

- **Total Sales:** $671.5M  
- **Top Income Transaction Type:** Auto  
- **Total Cars Sold:** 23,906  
- **Best Selling Model:** Diamante  
- **Most Valuable Customer (MVC):** Emma  
- **Top Performing Dealer by Income:** Progressive Shippers Cooperative Association No  
- **Most Profitable Engine Category:** DoubleÂ‚Â OC

---

## Insights

### 💵 Income & Market Insights

- **Average Income by Gender:**
  - Male: $851,184 (53%)
  - Female: $759,573 (47%)
  - 💡 *Insight:* Male customers have slightly higher average income, which may influence purchasing power or preferences.

- **Market Value by Brand:**
  - Top brands by total market value: **Chevrolet**, **Ford**, **Dodge**
  - Brands like **Mercedes-Benz** and **Oldsmobile** follow behind.

- **Annual Income by Car Body Style:**
  - **SUV** and **Hatchback** styles dominate in terms of income generation.
  - **Passenger** and **Hardtop** styles generate significantly lower income.

### 🌍 Regional & Customer Insights

- **Top Regions by Sales Volume:**
  - Austin leads with **4,135 units sold**
  - Other strong regions include Janesville, Scottsdale, and Pasco

- **Customer Purchase Behavior:**
  - Top 5 customers by purchase amount:
    1. **Louis** – $1.83M  
    2. **Hugo** – $1.92M  
    3. **Paul** – $1.67M  
    4. **Nathan** – $2.01M  
    5. **Emma** – $2.49M (MVC)

- **Monthly Income Trend:**
  - Steady increase over the year with a sharp rise from October to December
  - 💡 *Insight:* Potential seasonality effect or year-end promotional surge

### 🏢 Dealer Performance

- **Top Dealers by Income:**
  - **Progressive Shippers**: $111.97M
  - **Rabun Used Car Sales**: $108.85M
  - Other notable dealers: **Race Car Help**, **Suburban Ford**, **Saab-Belle Dodge**

---

## ✅ Recommendations

### 🔹 For Sales & Marketing Teams
- Focus on **SUV and Hatchback** inventory due to their higher income contribution.
- Leverage seasonal trends—especially **Q4**—for promotional campaigns and new launches.
- Target **Austin, Janesville, and Scottsdale** with region-specific marketing strategies.

### 🔹 For Dealership Strategy
- Analyze **Progressive Shippers** and **Rabun Used Car Sales** practices and replicate high-performing models across underperforming dealers.
- Incentivize dealers with sales commissions based on income performance.

### 🔹 For Customer Relationship Management
- Strengthen loyalty programs targeting high-income customers like **Emma, Nathan, and Louis**.
- Explore gender-based marketing personalization, since males show slightly higher spending.

### 🔹 For Product Development
- Prioritize **best-selling models** like Diamante in production pipelines.
- Assess engine configurations such as **DoubleÂ‚Â OC** for scalability, given high profitability.

---





 


