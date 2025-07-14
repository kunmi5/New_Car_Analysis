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
 


