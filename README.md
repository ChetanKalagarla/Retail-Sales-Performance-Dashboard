<div align="center">

# 📊 Power BI Sales Performance Analysis

### 🚀 Retail Sales Intelligence & Business Performance Dashboard

<p>
  <b>Transforming 3 Years of Retail Sales Data into Actionable Business Insights</b>
</p>

<br>

<img src="https://img.shields.io/badge/Power%20BI-Analytics-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
<img src="https://img.shields.io/badge/DAX-Data%20Modeling-1F4E79?style=for-the-badge">
<img src="https://img.shields.io/badge/Power%20Query-ETL-2F5597?style=for-the-badge">
<img src="https://img.shields.io/badge/Business-Intelligence-17365D?style=for-the-badge">

<br><br>

**👨‍💻 Developed by Chetan Kalagarla**

</div>

---

## 📌 Table of Contents

- [📖 Project Overview](#-project-overview)
- [🎯 Business Problem](#-business-problem)
- [💡 Project Objectives](#-project-objectives)
- [🗂️ Dataset & Data Model](#️-dataset--data-model)
- [⚙️ Data Preparation](#️-data-preparation)
- [🧠 DAX & Analytics](#-dax--analytics)
- [📊 Dashboard Pages](#-dashboard-pages)
- [✨ Interactive Features](#-interactive-features)
- [📈 Key Performance Indicators](#-key-performance-indicators)
- [🔍 Top 5 Business Findings](#-top-5-business-findings)
- [⚠️ Key Problems](#️-key-problems)
- [💡 Recommendations](#-recommendations)
- [📁 Repository Structure](#-repository-structure)
- [🛠️ Technology Stack](#️-technology-stack)
- [🚀 How to Use](#-how-to-use)
- [👨‍💻 Author](#-author)

---

# 📖 Project Overview

**Power BI Sales Performance Analysis** is an interactive Business Intelligence solution designed to analyze retail sales performance across **2021, 2022 and 2023**.

The project transforms raw sales data into an interactive dashboard that enables users to analyze:

- 💰 Sales performance
- 📈 Profitability
- 🛒 Orders and quantity
- 📦 Product performance
- 👥 Customer performance
- 🧑‍💼 Salesperson performance
- 🌍 Geographic performance
- 🎯 Budget vs Actual performance
- 📅 Year-over-year trends

The solution uses a **star-schema data model**, Power Query for data preparation, and DAX for business calculations and advanced analytics.

---

# 🎯 Business Problem

The business previously depended on manually prepared reports, making it difficult to:

- Track sales performance efficiently
- Compare performance across years
- Identify profitable products
- Understand customer behavior
- Evaluate salesperson performance
- Compare locations and states
- Monitor budget achievement
- Identify changes in sales trends

### ❓ Key Business Question

> **How is the business performing, where are we generating the most revenue and profit, and where should management focus its attention?**

---

# 💡 Project Objectives

The dashboard was developed to:

| Objective | Purpose |
|---|---|
| 📊 Sales Analysis | Monitor sales across multiple years |
| 💰 Profitability | Analyze profit and gross margin |
| 📦 Product Analysis | Identify high-performing products |
| 👥 Customer Analysis | Understand customer contribution |
| 🧑‍💼 Salesperson Analysis | Compare salesperson performance |
| 🌍 Geographic Analysis | Analyze state and location performance |
| 🎯 Budget Analysis | Compare actual sales with budget |
| 📅 Time Analysis | Analyze monthly, quarterly and yearly trends |
| 🔎 Interactive Analysis | Enable drill-down, drill-through and filtering |

---

# 🗂️ Dataset & Data Model

The project uses a **Star Schema** consisting of a central fact table and multiple dimension tables.

### ⭐ Fact Table

**Fact_Sales**

Contains:

- Order ID
- Product ID
- Location ID
- Sales Person ID
- Customer ID
- Order Date
- Quantity
- Price

### 🔹 Dimension Tables

- `Product_Data`
- `Customer_Data`
- `Location_Data`
- `Salespeople_Data`
- `Date`

### 📅 Supporting Tables

- `Budgeting`
- `Date_Ranges`
- `Sales_2021`
- `Sales_2022`
- `Sales_2023`

The 2021, 2022 and 2023 sales datasets were appended into the final `Fact_Sales` table.

---

# ⚙️ Data Preparation

The data preparation process was performed using **Power Query**.

### 🔄 ETL Process

```text
Raw Sales Data
      │
      ▼
┌───────────────────┐
│  Data Import      │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│ Data Cleaning     │
│ • Data Types      │
│ • Null Checks     │
│ • Duplicates      │
│ • Standardization │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│ Append 2021–2023  │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│    Fact_Sales     │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│ Star Schema Model │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│ DAX Calculations  │
└─────────┬─────────┘
          ▼
┌───────────────────┐
│ Power BI Dashboard│
└───────────────────┘
