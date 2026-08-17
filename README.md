# Customer Profitability Dashboard | Power BI

An interactive **Customer Profitability Dashboard** developed in Microsoft Power BI to analyze sales performance, profitability, customers, products, and business trends.

The project focuses on transforming raw business data into an interactive analytical dashboard using **Power Query, DAX, data modeling, and Power BI visualizations**.

> **Dataset:** Microsoft Power BI Customer Profitability Sample  
> **Source:** Microsoft Power BI Desktop Samples  
> The dataset used in this project is publicly available and was not created by me. The analysis, data modeling, DAX measures, dashboard design, and visualizations in this repository are part of my work.

---

## 📊 Dashboard Preview

### Overview

![Dashboard Overview](Screenshots/dashboard_overview.png)

### Sales & Profitability Analysis

![Sales Analysis](Screenshots/sales_analysis.png)

### Customer Analysis

![Customer Analysis](Screenshots/customer_analysis.png)

---

## 🎯 Project Objectives

The main objective of this project is to build an interactive dashboard that helps answer questions such as:

- How much revenue is being generated?
- How profitable is the business?
- Which customers generate the most revenue?
- Which customers are the most profitable?
- Which products contribute the most to profitability?
- How does sales performance change over time?
- Which areas of the business require attention?
- What are the major drivers of profit?

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development and visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Calculations and business metrics |
| **Excel** | Source dataset |
| **Star Schema** | Data modeling |

---

## 🗂️ Data Model

The project uses a dimensional data model designed to support interactive analysis.

### Main tables

- **Fact Sales**
  - Revenue
  - Cost
  - Quantity
  - Profit
  - Transaction information

- **Customer Dimension**
  - Customer information
  - Customer segmentation

- **Product Dimension**
  - Product information
  - Product categories

- **Date Dimension**
  - Year
  - Month
  - Quarter
  - Date hierarchy

The model allows the dashboard to analyze business performance across different dimensions such as **time, customer, and product**.

---

## 📈 Key KPIs

The dashboard includes several key performance indicators, including:

- **Total Revenue**
- **Total Cost**
- **Total Profit**
- **Profit Margin**
- **Total Quantity**
- **Average Revenue**
- **Customer Count**
- **Product Count**

These metrics can be dynamically filtered using the dashboard's slicers and visual interactions.

---

## 🧮 DAX Measures

Some of the main calculations used in the dashboard include:

```DAX
Total Revenue =
SUM(Fact_Sales[Revenue])
