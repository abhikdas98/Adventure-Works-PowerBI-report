# 🌟 AdventureWorks Power BI Dashboard

![Power BI Banner](assets/banner.png)  
*A full-scale business intelligence dashboard built using the Microsoft AdventureWorks dataset.*

---

## 🧠 Overview
This Power BI dashboard delivers a **comprehensive analysis of sales, profit, and customer performance** for the fictional AdventureWorks company.  
It demonstrates **data modeling, DAX calculations, and storytelling dashboards** — turning raw data into insights for strategic decision-making.

---

## 🎯 Objectives
- 📈 Track company-wide **sales and profit trends**
- 🌍 Compare **regional and product-level performance**
- 👥 Analyze **customer demographics and behavior**
- 🏷️ Identify **top products and sales representatives**
- 📊 Build an **interactive and visually appealing dashboard**

---

## 🗂️ Dataset
| Detail | Description |
|--------|--------------|
| **Source** | Microsoft AdventureWorksDW2022 |
| **Type** | Relational SQL dataset |
| **Fact Table** | FactResellerSales |
| **Dimensions** | DimProduct, DimCustomer, DimDate, DimGeography, DimSalesTerritory |
| **Schema** | Star Schema |

---

## 🧩 Data Model Overview
```

FactResellerSales
│
├── DimProduct
├── DimCustomer
├── DimDate
├── DimGeography
└── DimSalesTerritory

````

---

## 📈 Dashboard Previews

### 🏠 Sales Overview
![Sales Overview](assets/sales-overview.png)
*Shows total sales, profit margin, and YoY growth with dynamic KPIs.*

---

### 🌍 Profit by Region
![Profit by Region](assets/profit-by-region.png)
*Visualizes regional performance using maps and drill-throughs.*

---

### 🚴 Product Performance
![Product Performance](assets/product-performance.png)
*Highlights top products by sales, category, and profitability.*

---

### 👥 Customer Insights
![Customer Insights](assets/customer-insights.png)
*Analyzes customer segmentation, repeat purchase behavior, and demographics.*

---

### 📅 Trend Analysis
![Trend Analysis](assets/trend-analysis.png)
*Displays sales and profit trends across months and years.*

---

## 🧮 Key DAX Measures
```DAX
Total Sales = SUM(FactResellerSales[SalesAmount])

Total Profit = SUM(FactResellerSales[SalesAmount]) - SUM(FactResellerSales[TotalCost])

Profit Margin = DIVIDE([Total Profit], [Total Sales])

YoY Sales Growth = 
    CALCULATE([Total Sales], DATEADD(DimDate[Date], -1, YEAR))
````

---

## 🧰 Tools & Technologies

| Tool                 | Purpose                       |
| -------------------- | ----------------------------- |
| **Power BI Desktop** | Data modeling & visualization |
| **Power Query**      | Data transformation           |
| **SQL Server / CSV** | Data extraction               |
| **DAX**              | Calculated measures and KPIs  |

---

## 🏃 How to Use

1. 📥 **Download or clone** this repository.
2. 🖥️ Install **[Power BI Desktop](https://powerbi.microsoft.com/desktop/)**.
3. 📂 Open the file: `AdventureWorks Report.pbix`.
4. 🧭 Interact with the visuals using filters and slicers to explore insights.

> 💡 *You can add your own datasets or modify visuals to adapt this template for other businesses.*

---

## 🚀 Future Enhancements

* 🔄 Real-time data refresh using Power BI Service
* 🤖 AI-driven insights and anomaly detection
* 🌐 Deploy as a Power BI web app for public sharing
* 📊 Include predictive forecasting using Python integration

---

## 👨‍💻 Author

**Abhik Das**
📍 Data Analyst | BI Developer | Power BI Enthusiast
📧 [LinkedIn](https://www.linkedin.com/in/abhik-das-6430331a5/)
🔗 [GitHub Profile](https://github.com/abhikdas98)

---

## 🏷️ Tags

`#PowerBI` `#DataVisualization` `#BusinessIntelligence` `#AdventureWorks` `#DAX` `#PortfolioProject`

---

## 📢 About This Project

**AdventureWorks Power BI Dashboard** — A complete business intelligence project demonstrating data modeling, visualization, and insights generation.
Ideal for showcasing **Power BI proficiency**, **data storytelling**, and **DAX expertise** in your analytics portfolio.

**Keywords:** Power BI dashboard, sales analytics, business insights, AdventureWorks, DAX, data visualization, analytics portfolio.

---

> ⭐ *If you like this project, give it a star on GitHub — it helps showcase my Power BI work to more people!*
