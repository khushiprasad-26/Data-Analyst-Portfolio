# 📦 Supply Chain Dashboard | Power BI

## 📌 Project Overview

This project is an interactive **Supply Chain Analytics Dashboard developed using Microsoft Power BI**.

The dashboard provides a comprehensive view of **sales, inventory, products, customers, stores, and geographical performance**. It transforms raw supply chain data into meaningful KPIs and visual insights that can support business decision-making.

The project focuses on understanding inventory levels, sales performance, customer distribution, product information, and supply chain activity across different locations and time periods.

---

## 🎯 Project Objectives

The main objectives of this project were to:

- Monitor overall sales and inventory performance
- Analyze product and inventory information
- Understand sales distribution across different states
- Analyze customer and store performance
- Track supply chain activity over time
- Identify important business KPIs
- Compare inventory and sales-related metrics
- Create an interactive dashboard for business users
- Present complex supply chain data in an easy-to-understand format

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Data Cleaning & Transformation**
- **Data Modeling**
- **Data Visualization**
- **KPI Development**
- **Interactive Dashboard Design**

---

## 📊 Dashboard Components

The dashboard contains multiple interactive visualizations, including:

### 🔹 KPI Cards

Important metrics are presented through KPI cards to provide a quick overview of business performance.

Examples include:

- Inventory-related KPIs
- Sales-related KPIs
- Product metrics
- Business performance indicators

### 🔹 Sales Analysis

The dashboard analyzes sales performance using different dimensions such as:

- State
- Customer
- Product
- Store
- Time period

### 🔹 Inventory Analysis

Inventory data is analyzed to understand:

- Available inventory
- Product-level inventory
- Inventory adjustments
- Inventory distribution
- Changes in inventory over time

### 🔹 Geographical Analysis

A map visualization is used to analyze business performance across different **states and geographical locations**.

This helps identify regions with stronger sales activity and understand geographical distribution.

### 🔹 Product Analysis

The dashboard provides product-level analysis to understand:

- Product availability
- Product pricing
- Inventory
- Sales contribution

### 🔹 Customer Analysis

Customer information is used to analyze:

- Customer locations
- Customer distribution
- Sales activity by region

### 🔹 Store Analysis

Store-level information helps evaluate business activity across different stores and locations.

---

## 🗂️ Data Model

The Power BI report uses multiple related tables, including:

```text
Calendar
   │
   ├── Sales
   │
   └── Inventory

Customer
   │
   └── Sales

Product
   │
   ├── Sales
   │
   └── Inventory

Store
   │
   └── Sales

States Master
   │
   └── Geographical Analysis
```

### Main Tables

- `F_POS_SALES_Modified3` — Sales transaction data
- `F_INVENTORY_ADJUSTED9` — Inventory and inventory adjustment data
- `D_PRODUCT7` — Product information
- `D_Customer5` — Customer information
- `D_STORE8` — Store information
- `D_States_Master1` — State/geographical information
- `Calendar4` — Date and time analysis

---

## 🔄 Data Preparation Workflow

The project followed a structured data analytics workflow:

```text
Raw Data
    ↓
Data Cleaning
    ↓
Power Query Transformation
    ↓
Data Modeling
    ↓
Relationships
    ↓
DAX Measures
    ↓
KPI Creation
    ↓
Data Visualization
    ↓
Interactive Dashboard
    ↓
Business Insights
```

---

## 📈 Key Business Questions

The dashboard was designed to answer questions such as:

- What is the overall sales performance?
- What is the current inventory situation?
- Which products contribute significantly to the business?
- How are sales distributed across different states?
- Where are customers located?
- How does sales performance change over time?
- What are the major inventory adjustments?
- Which stores and regions show stronger business activity?

---

## ⚠️ Data Quality Challenge

One of the important challenges identified during the project was **data inconsistency between Total Cost and its individual components**.

In some records, the following did not always reconcile:

```text
Procurement Cost + Transportation Cost ≠ Total Cost
```

This occurred because the `Total Cost` value was pre-calculated in the source data and some records contained missing or rounded values.

### 🔧 Solution

To address this issue:

1. Cross-checked the individual cost components.
2. Created calculated fields to validate the cost logic.
3. Identified records where the values did not match.
4. Investigated the differences.
5. Used business assumptions to determine the appropriate interpretation of the data.

This helped improve confidence in the analysis and demonstrated the importance of **data validation before building business dashboards**.

---

## 💡 Business Insights

The dashboard can help organizations:

- Monitor supply chain performance
- Identify inventory-related issues
- Understand regional sales patterns
- Analyze product performance
- Track customer distribution
- Compare store-level activity
- Make more informed inventory and sales decisions

---

## 🎨 Dashboard Features

The Power BI dashboard includes:

- 📌 KPI Cards
- 🗺️ Geographical Map
- 📊 Bar & Column Charts
- 📈 Trend Analysis
- 🍩 Donut/Pie Charts
- 🎛️ Interactive Slicers
- 🔍 Dynamic Filtering
- 📦 Inventory Analysis
- 🛒 Sales Analysis

Users can interact with the dashboard by selecting different filters and dimensions to explore the data dynamically.

---

## 📁 Project Structure

```text
Supply-Chain-Dashboard/
│
├── Supply Chain Dashboard.pbix
│
├── README.md
│
└── Dashboard/
    └── Supply Chain Dashboard Screenshot
```

---

## 🚀 Project Outcome

This project strengthened my practical experience in **Power BI, Power Query, DAX, data modeling, data validation, KPI development, and dashboard design**.

More importantly, it helped me understand how raw supply chain data can be transformed into an interactive analytical solution that provides actionable business insights.





**#PowerBI #DataAnalytics #DataAnalyst #SupplyChainAnalytics #BusinessIntelligence #DataVisualization #Dashboard #DAX #PowerQuery #GitHub**
