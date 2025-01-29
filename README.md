# Dynamic Retail Dashboard in Excel  

## Overview  
The **Dynamic Retail Dashboard** is an interactive Excel-based analytics tool designed to provide deep insights into retail data. By leveraging **Power Query**, **Pivot Tables**, and **dynamic visualizations**, this dashboard enables businesses to monitor key performance indicators (KPIs), analyze trends, and make data-driven decisions.  

This project helps answer critical business questions such as:  
- What are the total sales, profit, and order trends over time?  
- Which product categories and subcategories drive the most revenue?  
- How do sales vary across different countries and regions?  
- What is the impact of returned orders on overall profitability?  

---

## Features & Functionalities  
- **Key Performance Indicators (KPIs)** – Displays Total Sales, Profit, Order Count, and Profit Margin dynamically.  
- **Sales & Profit Trends** – Visualizes performance across different time periods.  
- **Category & Segment-Wise Analysis** – Identifies profitable product categories and sales distribution.  
- **Geographical Sales Insights** – Highlights top-performing countries with heatmaps.  
- **Top & Bottom Subcategories** – Showcases the best and least-performing product segments.  
- **Dynamic Filters & Slicers** – Enhances interactivity for deeper data exploration.  

---

## Dataset Breakdown  
The dashboard utilizes multiple datasets to generate insights:  

### Orders Data  
The Orders table contains details of customer orders, including product, shipping, and financial metrics.

**Sample Data:**
| Order ID       | Returned | Order Date   | Ship Date   | Ship Mode       | Customer Name   | Segment    | Country         | Market | Sales   | Profit   | Discount |
|----------------|----------|--------------|-------------|-----------------|-----------------|------------|-----------------|--------|---------|----------|----------|
| CA-2012-124891 | No       | 31-07-2020   | 31-07-2020  | Same Day        | Rick Hansen     | Consumer   | United States   | US     | 2309.65 | 762.18   | 0        |
| IN-2013-77878  | Yes      | 05-02-2021   | 07-02-2021  | Second Class    | Justin Ritter   | Corporate  | Australia       | APAC   | 3709.40 | -288.77  | 0.1      |
| IN-2013-71249  | No       | 17-10-2021   | 18-10-2021  | First Class     | Craig Reiter    | Consumer   | Australia       | APAC   | 5175.17 | 919.97   | 0.1      |

### Returns Data
Tracks orders that have been returned, along with the associated markets.

**Sample Data:**
| Returned | Order ID         | Market         |
|----------|------------------|----------------|
| Yes      | MX-2013-168137   | LATAM          |
| Yes      | US-2011-165316   | LATAM          |
| Yes      | ES-2013-1525878  | EU             |
| Yes      | CA-2013-118311   | United States  |

### 3. **People Table**
Contains details about sales representatives and their respective regions.

**Sample Data:**
| Person              | Region          |
|---------------------|-----------------|
| Anna Andreadi       | Central         |
| Chuck Magee         | South           |
| Kelly Williams      | East            |
| Matt Collister      | West            |
| Deborah Brumfield   | Africa          |

---

## How the Dashboard Works  

### 1. KPI Metrics for Business Overview  
-  **Objective:** Calculate and display Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

   **Steps:**
   1. Import the **Orders Table** into Excel using Power Query.
   2. Create calculated columns for:
      - `Profit Margin` = `Profit / Sales`.
      - `Total Orders` = Count of `Order ID`.
   3. Use Excel formulas to calculate:
      - `Total Sales` = `=SUM(Sales)`.
      - `Total Profit` = `=SUM(Profit)`.
      - `Total Quantity` = `=SUM(Quantity)`.
   4. Build a dynamic KPI table and use symbols to enhance visual appeal (e.g., 💰 for Total Sales).
 

![Screenshot 2025-01-29 143520](https://github.com/user-attachments/assets/f1574be2-3e17-400d-a6fa-c76c80103160)

---
### 2. Trend Analysis for Sales & Profit  
- Uses a **Scatter Plot** to display sales and profit patterns over time.  
- Includes **slicers** to filter by **market, segment, and region**.


![Screenshot 2025-01-29 143608](https://github.com/user-attachments/assets/72f0dfdc-e70c-4474-b794-2ff870326f8f)

---
### 3. Product Category Performance  
- **Bar charts** rank categories by profitability.  
- Allows filtering by **region or time period** for in-depth analysis.


![Screenshot 2025-01-29 143530](https://github.com/user-attachments/assets/d5318e8f-989e-4c7e-9259-5a4b899f0069)

---
### 4. Geographical Sales Distribution  
- **Heatmaps** and **Geographic Maps** visualize country-wise sales.  
- Helps businesses identify their strongest and weakest markets.


![Screenshot 2025-01-29 143547](https://github.com/user-attachments/assets/aa691d02-b229-41a8-8f96-a9e7bb28d8a8)

---
### 5. Customer Segment Analysis  
- Uses a **Pie Chart** to display sales distribution among customer segments.  
- Helps tailor marketing strategies based on customer demographics.


![Screenshot 2025-01-29 143541](https://github.com/user-attachments/assets/92051f07-efce-451a-a156-6a6a14b1de17)

---
### 6. Identifying Top & Bottom Performing Subcategories  
- **Column Charts** rank the **top 5** and **bottom 5** subcategories by revenue.  
- Provides insights for inventory management and promotional strategies.


![Screenshot 2025-01-29 143553](https://github.com/user-attachments/assets/5bbcc9bd-4f13-41d6-9a25-961620f2feb5)

![Screenshot 2025-01-29 143600](https://github.com/user-attachments/assets/ea8c85b7-20c7-4e73-89e6-fe65bd167f22)

---
### 7. Yearly Sales Trends & Forecasting  
- A **dynamic Line Chart** highlights sales growth patterns across multiple years.  
- Helps predict future sales based on historical trends.


![Screenshot 2025-01-29 143619](https://github.com/user-attachments/assets/0b1e2ca1-0a52-4d13-81ac-b8bea9659bf1)

---

## Future Enhancements  
- **Return Rate Analysis** – Investigate return patterns by product category.  
- **Customer Profitability Analysis** – Identify most and least profitable customers.  
- **Market-Wise Insights** – Compare sales trends across different retail markets.  
- **Advanced Power BI Integration** – Upgrade to Power BI for deeper analytics.  

---

## Why This Dashboard Matters  
This Excel dashboard is a **powerful business intelligence tool** that empowers retail managers to:  
- Track sales performance in real time.  
- Optimize inventory and pricing strategies.  
- Enhance decision-making through interactive insights.  

---

## Installation & Usage  
1. **Download the Excel File** from this repository.  
2. Ensure **Excel Power Query** is enabled for automated data transformation.  
3. Use **slicers and filters** to explore dynamic insights.  
4. Modify the dataset to analyze custom retail data.  

---

## Visuals  
### **Dashboard Overview**  
![Retail Dashboard Screenshot](https://github.com/user-attachments/assets/94b3c272-0cf3-4a75-9740-fdd99ac34c34)

---
