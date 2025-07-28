Sales Data Analysis – Power BI Project

## 📁 Dataset
- **File Name**: `store data.xlsx`
- **Contents**:
  - `Fact Table`: Main transactional data
  - `Products List`: Product details
  - `Customers`: Customer information
  - `Promotions`: Discount and promotion categories
- **Time Period Covered**: 2020 to 2024

---

## 📌 About the Project
This Power BI project focuses on analyzing a store's sales data from 2020 to 2024. The dataset includes information on:
- Products sold
- Customer details
- Promotional offers used
- Transaction-level sales records

We cleaned the dataset by:
- Changing incorrect data types
- Replacing null values with 0
- Creating relationships between tables using:
  - **One-to-Many Cardinality**:  
    - `Fact Table` columns (foreign keys) joined with primary keys in `Products`, `Promotions`, and `Customers` tables

---

## 🎯 Business Questions Answered

### 1. 🏆 Top/Bottom 5 Products by Sales, Profit, and Quantity Sold
- Used a bar chart with Top N filter.
- **Top Product**: Apple iPhone 14
- **Bottom Product**: Tupperware lunch box

### 2. 📅 Sales Trends Over Time (Daily, Monthly, Quarterly, Annually)
- Observations:
  - **March**: Lowest sales month each year
  - **June**: Average monthly sales
  - **November 2022**: Highest single-month sales

### 3. 📈 Relationship Between Sales and Profit
- Clear **positive linear correlation**:  
  As sales increase, profit increases.

### 4. 📊 Period Comparison of Sales/Profit/Quantity Sold
- Implemented using:
  - **Two date slicers**
  - Measures with `USERELATIONSHIP()` and `ALL()` DAX functions
- Output: Bar charts comparing metrics across two selected periods

### 5. 💸 Average Discount by Promotion Type
- **Highest discounts** observed in **Weekend Sales**
- Average discount value: ₹23,000

### 6. 🧾 Total Number of Orders
- Total Orders: **3,510**

### 7. 🗺️ Sales by City
- **Highest Sales**: Kanpur, Indore, Bhopal, Lucknow  
- **Average Sales**: Patna, Kolkata, Mumbai, Chennai  
- **Lowest Sales**: Bangalore

### 8. 🧮 Detailed Order-Level Metrics with Visual Filters
- Built a dynamic table showing:
  - Sales, Profit, Discount, Net Sales, and more
- Enabled visual filters by:
  - Product
  - Date
  - Customer ID
  - Promotion Categories

---

## 🔧 Tools & Techniques Used
- **Tool**: Power BI Desktop
- **Techniques**:
  - Data cleaning & transformation in Power Query
  - Relationships using primary and foreign keys
  - DAX measures using `CALCULATE`, `USERELATIONSHIP`, `ALL`
  - Slicers and filters for dynamic user interaction
  - Bar/Line charts, Tables, and Cards for visualization

---

## 📌 Conclusion
This dashboard offers actionable insights into product performance, seasonal trends, and promotional impact. It supports custom period comparisons and granular order-level analysis to help businesses make informed decisions.

---

