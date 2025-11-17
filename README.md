# Sales Performance Dashboard – Power BI

This Power BI project analyzes sales performance using a dataset of approximately **10,000 rows**.  
The dashboard provides insights into **Sales, Profit, Orders, Top-performing Regions, Categories, and Customer Segments**.

---

## 📘 Project Overview
The dashboard helps users understand:

- Total Sales & Profit Trend  
- Customer Segmentation  
- Regional Sales Distribution    
- Order Count by Region  
- Category & Sub-Category Performance
- Year by Year Analysis  

This project demonstrates the ability to **clean, model, and visualize data** to extract actionable insights.

---

## 🛠 Tools Used
- **Power BI Desktop**  
- **Power Query** (for data cleaning)  
- **DAX Measures** (for calculations)  
- **CSV Dataset**
      - Name : Sample - Superstore.CSV
      - Resource : Kaggle website   

---

## 🧹 Data Cleaning Steps
- Removed duplicate records  
- Checked for missing values and handled them  
- Standardized date formats  
- Created new columns: Year, Month  
- Calculated Revenue column: `Revenue = Sales*Quantity`  
- Created 10+ DAX measures for analysis  

---

## 📊 Dashboard Features
- **Cards:** Average Sales, Customer Count, Order Count  
- **Order Count by Region:** Donut Vhart  
- **Total Sales by Month:** Line Chart  
- **Total Profit by Sub-Category:** Bar Chart  
- **Total Sales by Product Name:** Bar Chart  
- **Profit Margin by Segment :** Column Chart
- **Total Sales by Category :** Column Chart

---

## 🧮 Key DAX Measures
```DAX
Total Sales = SUM(Sample - Superstore[Sales])
Total Profit = SUM(Sample - Superstore[Profit])
Order Count = DISTINCTCOUNT(Sample - Superstore[OrderID])
Average Sales = AVERAGE(Sample - Superstore[Sales])
Revenue = SUM(Sample - Superstore[Sales]*Sample - Superstore[Discount])
