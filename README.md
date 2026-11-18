# 📊 ClipKart – E-commerce Sales Performance Analysis

An interactive Power BI dashboard designed to analyze e-commerce sales performance, identify top-performing products, evaluate regional performance, and understand revenue distribution across product categories.

## 📌 Project Overview

This project focuses on analyzing e-commerce sales data to uncover meaningful business insights through data visualization and business intelligence.

Using Microsoft Power BI, I developed an interactive dashboard that helps understand overall revenue performance, order distribution, product performance, and geographical sales patterns.

The dashboard transforms raw sales data into meaningful visual insights that can support business decision-making.

## 🎯 Business Objectives

The main objectives of this project are:

- Analyze overall revenue and order performance.
- Identify the highest revenue-generating products.
- Compare sales performance across different cities.
- Understand revenue contribution by product category.
- Calculate average order value.
- Identify trends and patterns in sales performance.

## 🛠️ Tools & Technologies

- **Microsoft Power BI** – Dashboard development and data visualization.
- **Power Query** – Data cleaning and transformation.
- **DAX** – Creating calculated measures and business KPIs.
- **Microsoft Excel** – Dataset storage and initial data handling.
- **SQL** – Data querying and analysis.

## 📂 Dataset Information

The dataset contains the following columns:

| Column | Description |
|---|---|
| Category | Product category |
| City | City where the order was recorded |
| Date | Order date |
| OrderID | Unique order identifier |
| Price | Product price |
| Product | Product name |
| Quantity | Number of units purchased |
| Revenue | Revenue generated |

## 📈 Dashboard Features

### 1. Key Performance Indicators (KPIs)

The dashboard includes:

- Total Revenue
- Total Orders
- Regions Covered
- Average Order Value

### 2. Sales Performance Analysis

- **Total Revenue by Category:** Understand revenue contribution across product categories.
- **Top Performing Cities:** Compare revenue generated across different cities.
- **Top Revenue Products:** Identify products generating the highest revenue.
- **Revenue by Products:** Compare revenue performance across individual products.

### 3. Business Analysis

The dashboard helps answer important business questions:

1. How much total revenue has the business generated?
2. Which product categories contribute the most revenue?
3. Which cities generate the highest revenue?
4. Which products generate the highest revenue?
5. What is the average order value?
6. How is revenue distributed across different product categories?

## 📊 Dashboard Preview

![ClipKart Sales Performance Dashboard](images/dashboard.png)

## 🧮 DAX Measures

Some of the key measures used in the dashboard:

**Total Revenue**
```dax
Total Revenue =
SUM(Sales[Revenue])
```

**Total Orders**
```dax
Total Orders =
DISTINCTCOUNT(Sales[OrderID])
```

**Average Order Value**
```dax
Average Order Value =
DIVIDE(
    [Total Revenue],
    [Total Orders],
    0
)
```

**Total Products**
```dax
Total Products =
DISTINCTCOUNT(Sales[Product])
```

**Total Units Sold**
```dax
Total Units Sold =
SUM(Sales[Quantity])
```

*Note: Replace `Sales` with the actual table name used in your Power BI model.*

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Building interactive dashboards using Power BI.
- Creating DAX measures for business KPIs.
- Working with different visualization techniques.
- Analyzing product and geographical sales performance.
- Understanding how businesses use data to make informed decisions.
- Designing dashboards with a focus on usability and business requirements.

## 📁 Project Structure

```text
ClipKart-Sales-Analysis/
│
├── Dataset/
│   └── ecommerce_data.xlsx
│
├── PowerBI/
│   └── ClipKart_Dashboard.pbix
│
├── images/
│   └── dashboard.png
│
└── README.md
```

## 🚀 Conclusion

The ClipKart Sales Performance Dashboard demonstrates how raw e-commerce data can be transformed into meaningful business insights using Power BI.

This project represents my practical learning in data analytics, business intelligence, data visualization, and DAX.

---

**Created as part of my Data Analytics learning journey.**
