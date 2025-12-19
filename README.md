# Flipkart 2024 – E-Commerce Sales & Performance Analysis (Power BI)

## Project Overview
This Power BI project analyzes **Flipkart’s 2024 e-commerce performance** across sales, customers, sellers, and delivery operations.  
The dashboard provides management-level insights into **revenue trends, customer behavior, regional performance, and delivery efficiency** using interactive visualizations.

The objective is to enable **data-driven decision making** through clear KPIs and actionable insights.

---

## Business Objectives
- Analyze overall sales and profit performance
- Identify top-performing categories, brands, and sellers
- Understand customer demographics and regional demand
- Evaluate delivery performance and courier efficiency
- Measure customer retention and repeat purchase behavior

---

## Dataset Information
**Source:** Kaggle – Flipkart Products Dataset  
https://www.kaggle.com/datasets/PromptCloudHQ/flipkart-products

### Tables Used
- **Orders** – Order date, payment method, order status  
- **Order_Items** – Quantity, price, discount, profit  
- **Products** – Category, sub-category, brand  
- **Customers** – Gender, age group, city, state  
- **Sellers** – Seller name, rating, location  
- **Delivery** – Courier, delay days, delivery status  

The tables are connected using keys such as **Order_ID, Customer_ID, and Product_ID** to form a star schema data model.

---

## Data Cleaning & Preparation
- Missing categorical values handled using **mode imputation**
- Duplicate order-item records removed
- Invalid delivery dates removed (Delivery_Date ≥ Order_Date enforced)
- Unrealistic discounts capped between **0–30%**
- Profit values recalculated accordingly

---

## Data Modeling & DAX Calculations

### Calculated Columns
- GrossSales = Price × Quantity  
- DiscountAmount = GrossSales × Discount%  
- NetSales = GrossSales − DiscountAmount  
- ProfitMargin  
- YearMonth (for time-based analysis)
- Delivery delay buckets and on-time flags

### Key Measures
- Total Sales
- Total Profit
- Total Orders
- Average Order Value (AOV)
- Unique Customers
- Repeat Customer Rate
- On-Time Delivery %
- Average Delivery Delay (days)

---

## Dashboard Pages & Insights

### 1️⃣ Sales & Profit Overview
- Total Sales: ₹562M+
- Total Profit: ₹100M+
- Monthly sales and profit trends
- Category-wise and brand-wise performance
- Filterable by region, category, and payment method

### 2️⃣ Customer & Order Insights
- 823 unique customers
- 97% repeat customer rate
- Gender-wise sales distribution
- State-wise sales map highlighting top regions (Delhi, Karnataka)

### 3️⃣ Delivery & Performance Analysis
- On-Time Delivery Rate analysis
- Average delay by courier
- Delay bucket distribution (On-time, 1–2 days, 3–5 days, 6+ days)
- Identification of logistics improvement areas

---

## Tools & Technologies
- **Power BI Desktop**
- **DAX**
- **Data Modeling**
- **Interactive Visualizations**

---

## Files Included
- `Dashboard.pbix` – Editable Power BI dashboard
- `Nalini_Power_BI_END_Term_Project.pdf` – Dashboard presentation


---

## How to View the Dashboard
1. Download the `.pbix` file
2. Open using **Power BI Desktop**
3. Interact with slicers and visuals

---

## Conclusion
The dashboard provides a **holistic view of Flipkart’s business performance**, highlighting:
- Strong revenue growth
- High customer retention
- Efficient delivery operations
- Regional and category-level insights

This project demonstrates practical skills in **Power BI, DAX, data modeling, and business analytics**.

---

## Author
**Nalini Singh**  
Power BI | Data Analytics | Business Intelligence
