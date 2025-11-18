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
      Name : Sample - Superstore.CSV
      Resource : Kaggle website   

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

---

## 💡 Key Findings and Business Insights
1. 📈 Overall Performance and Growth
- Volume Growth: Order Count and Customer Count saw significant growth, peaking in 2016 and 2017, indicating successful market expansion and customer acquisition.
- Declining Value: Despite high volume, Average Sales per order has declined or stagnated since 2014 ($250.09 in 2014 vs. $230.31 in 2017), suggesting a shift towards smaller transaction sizes.
- Recommendation: Focus marketing efforts on upselling and cross-selling higher-value items to increase the Average Sales value.

2. 💰 Profitability and Categories
- Profit Drivers: Copiers consistently generated the highest total profit, reinforcing the importance of the Technology category.
- Margin Discrepancies: Certain sub-categories (e.g., Appliances, Binders) show low profit margins or even losses within the Consumer segment.
- Recommendation: Conduct a cost-benefit analysis for low-margin products in the Consumer segment, and consider optimizing pricing or reducing operational costs.

3. 🌍 Regional and Segment Performance
- Top Region: The West Region consistently leads with the highest volume of orders (approximately 30-34% of total).
- Highest Margins: The Corporate and Home Office segments consistently display healthier Profit Margins compared to the Consumer segment.
- Recommendation: Implement targeted campaigns to increase order penetration in the South Region, which consistently shows the lowest order count.

4. 📉 Seasonality Trend
- Peak Season: Sales consistently peak in the last quarter (September through December), driven by high demand.
- Off-Season Dip: A sharp and predictable downward trend in sales occurs starting in December/January and continues into the middle of the year (Q1/Q2).
- Recommendation: Utilize this clear seasonality pattern for accurate inventory management and workforce planning, ensuring high stock during Q4 and minimizing holding costs during the early months of the year.

---

## 👤 7. Author and Contact

* **Name:** D.S.Senevirathna
* **GitHub Profile:** [https://github.com/YourGitHubUsername]
* **LinkedIn:** [https://www.linkedin.com/in/YourLinkedInProfile/]
* **Email:** dehemisathsarani184@.com

