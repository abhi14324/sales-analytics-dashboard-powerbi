
# Project Title

A brief description of what this project does and who it's for

# Sales Analytics Dashboard using Power BI

## Project Overview

This project is an interactive **Sales Analytics Dashboard** built using **Power BI** to analyze business sales performance across products, cities, promotions, and time periods.
The dashboard converts raw transactional sales data into meaningful business insights that help identify top-performing products, weak-performing products, profitability patterns, and sales trends.

---

## Project Objective

The main objective of this dashboard is to:

* Identify **Top 5 and Bottom 5 products** by sales, profit, and quantity sold
* Analyze **sales trends over time**
* Study the relationship between **sales and profit**
* Compare sales performance between **two user-selected periods**
* Analyze **promotion category discounts**
* Track **city-wise sales distribution**
* Provide detailed transaction-level analysis using filters

---

## Tools and Technologies Used

* **Power BI** – Dashboard development and visualization
* **DAX (Data Analysis Expressions)** – Measures and calculations
* **Data Modeling** – Star schema relationships

---

## Data Model

The dashboard follows a **star schema data model**.

### Tables Used

* Fact Table
* Customer Dimension Table
* Product Dimension Table
* Promotion Dimension Table
* Measure Table
* Date Table 1
* Date Table 2 

### Key Fields

* Order ID
* Customer ID
* Product ID
* Sales
* Profit
* Quantity
* Discount
* Promotion Category
* City
* Date

---

## Dashboard Pages

### 1. Top and Bottom 5 Analysis

This page shows:

* Top 5 products by sales
* Bottom 5 products by sales
* Top 5 products by quantity sold
* Bottom 5 products by quantity sold
* Top 5 products by profit
* Bottom 5 products by profit

---

### 2. Overview Dashboard

This page includes:

* Sales by city
* Total order count
* Promotion category discount analysis
* Sales vs profit relationship
* Sales trend over time

---

### 3. Comparison Dashboard

This page allows users to compare:

* Sales between two selected periods
* Profit between two selected periods
* Quantity sold between two selected periods

---

### 4. Interactive Filter Analysis

Users can interact using:

* Date filters
* Product filters
* Customer filters
* Promotion filters

---

### 5. Transaction Table View

Detailed transaction-level reporting includes:

* Order ID
* Customer ID
* Date
* Discount
* Net Sales
* Profit
* Units Sold

### Page 6: Filter Analysis Page
Additional filters help users focus on specific business segments.


---

## Power BI Service Deployment

The dashboard was developed in **Power BI Desktop** and published to **Power BI Service** for cloud-based access and report sharing.

### Deployment Benefits

* Online dashboard accessibility
* Browser-based report viewing
* Easy sharing with stakeholders
* Centralized cloud reporting

This deployment demonstrates practical understanding of dashboard publishing and report delivery in a business environment.
 
## Live Dashboard

Power BI Service Link: https://app.powerbi.com/groups/b9cc1061-396a-4d50-8f0e-50d72ef5750c/reports/4b3dcc0d-6d05-46be-9109-ad91a278eb6b/43d5e75bef3e436978fa?experience=power-bi



--- 

## Key Business Insights

* Apple iPhone 14 generated highest sales and profit
* Tupperware Lunch Box showed lowest sales performance
* Weekend Flash Sale provided highest average discount
* Metro cities contributed major sales volume
* Sales and profit show a strong positive relationship

---

## Business Value

This dashboard helps businesses:

* Identify profitable products
* Detect weak-performing products
* Optimize promotion strategy
* Monitor regional sales performance
* Support pricing and inventory decisions

---

## Sample Measures Used

```DAX
Quantity Sold = CALCULATE(SUM('Fact Table'[Units Sold]),ALL('Date Table 1'), USERELATIONSHIP('Date Table 2'[Date],'Fact Table'[Date (dd/mm/yyyy)]))


Sum of Net Sales = CALCULATE(SUM('Fact Table'[Net Sales]),ALL('Date Table 1'), USERELATIONSHIP('Date Table 2'[Date],'Fact Table'[Date (dd/mm/yyyy)]))


Total Profit = CALCULATE(SUM('Fact Table'[Profit]), ALL('Date Table 1') , USERELATIONSHIP('Date Table 2'[Date] , 'Fact Table'[Date (dd/mm/yyyy)]))
```

## Future Improvements

* Add forecasting analysis
* Add dynamic KPI indicators
* Add drill-through reports
* Add advanced DAX calculations

---

## Project Files

* Sales Dashboard Power BI file (.pbix)
* Dataset
* Screenshots
* Documentation

---

## Author

**Abhishek Kumar**
