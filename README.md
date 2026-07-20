# 📊 Sales Data Analytics Case Study
## 📖 Overview

This project demonstrates an end-to-end data analytics workflow using **Microsoft Excel, SQL, Power BI, DAX, and Jupyter Notebook**. The objective was to clean raw sales data, perform SQL analysis, build an interactive Power BI dashboard, and document the complete analytics process.

---

## 🎯 Project Objective

The goal of this project was to transform raw sales data into meaningful business insights by applying data cleaning, SQL analysis, data modeling, visualization, and reporting techniques.

---

## 🛠️ Tools & Technologies

- Microsoft Excel
- SQL
- Power BI
- DAX
- Jupyter Notebook

---

## 📂 Project Workflow

### Part 1: Excel Data Cleaning

The raw dataset contained several data quality issues, including:

- Duplicate records
- Inconsistent date formats
- Missing values
- Negative quantity values
- Inconsistent text formatting

### Data Cleaning Steps

- Removed duplicate records
- Standardized date formats
- Corrected text formatting using Excel functions
- Flagged missing values
- Reviewed negative quantity records
- Created a Revenue column
- Built a PivotTable summarizing revenue by Region and Category

---

### Part 2: SQL Analysis

After cleaning the data, it was imported into a SQL table for analysis.

The following SQL queries were performed:

- Total Revenue by Region and Category
- Top-Selling Product per Region using Window Functions
- Month-over-Month Revenue Growth

---

### Part 3: Power BI Dashboard

An interactive Power BI dashboard was created using a Star Schema data model.

### Dashboard Features

- KPI Cards
  - Total Revenue
  - Year-to-Date (YTD) Revenue

- Region-wise Revenue Bar Chart

- Monthly Revenue Trend

- Category Slicer

- DAX Measures

- Row-Level Security (North Manager Role)

---

## 📊 Data Model

A Star Schema was implemented by separating the Sales fact table from the Date dimension table.

This approach improves:

- Query performance
- Data organization
- Time intelligence calculations
- Dashboard scalability

---

## 🔐 Row-Level Security (RLS)

A role named **North Manager** was created to restrict users to viewing only North region data.

Filter used:

```DAX
[Region] = "North"
```

---

## 💡 Key Business Insights

- North generated the highest revenue.
- Revenue performance varied across regions.
- Monthly revenue trends highlighted business performance over time.
- Interactive filters enabled category-level analysis.
- Data cleaning improved the accuracy of reporting and analysis.

---

## 🚀 Skills Demonstrated

- Data Cleaning
- Excel Functions
- PivotTables
- SQL
- SQL Window Functions
- Data Modeling
- DAX
- Power BI
- Dashboard Design
- Row-Level Security (RLS)
- Business Intelligence

---

## 📁 Repository Structure

```
sales-data-analytics-case-study/
│
├── README.md
├── Sales_Data_Analytics_Case_Study.ipynb
├── Sales_Cleaned_Data.xlsx
├── Sales_Dashboard.pbix
│
├── images/
│
└── sql/
    └── sales_queries.sql
```

---

## 📌 Conclusion

This project demonstrates an end-to-end data analytics workflow—from cleaning raw data in Excel to performing SQL analysis and creating an interactive Power BI dashboard. It highlights practical skills in data preparation, querying, visualization, data modeling, and business reporting, making it a comprehensive portfolio project for aspiring Data Analysts.
