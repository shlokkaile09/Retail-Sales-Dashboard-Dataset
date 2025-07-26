# Retail-Sales-Dashboard-Dataset
# 📊 Retail Sales Dashboard (Excel Mini Project)

## 🚀 Project Overview

This project demonstrates the use of **intermediate to advanced Excel skills** to build a dynamic and interactive dashboard for a fictional retail store. It covers raw data handling, data analysis, visual reporting, and automation tools such as PivotTables and formulas.

---

## 📁 Project Structure

- **Sales_Data**: Raw transactional sales data (500 rows)
- **Analysis**: PivotTable-driven insights and calculations
- **Dashboard**: Visual summary with charts, KPIs, and slicers

---

## 📦 Data Fields

| Column           | Description                          |
|------------------|--------------------------------------|
| Date             | Date of transaction                  |
| Region           | North, South, East, or West          |
| Salesperson      | Name of the salesperson              |
| Product          | Item sold                            |
| Units Sold       | Quantity sold                        |
| Unit Price       | Price per unit                       |
| Total Sales      | `=Units Sold * Unit Price`           |
| Payment Method   | Cash, Card, or Online                |
| Customer Rating  | Customer satisfaction (1 to 5 stars) |

---

## 📊 Features & Techniques Used

### 🧮 Data Preparation
- Converted raw data into an Excel **Table** (`tblSales`)
- Generated calculated columns using formulas

### 🔍 PivotTables (Analysis Sheet)
- **Total Sales by Month**: Grouped dates by month & year
- **Top 5 Salespeople**:
  - Sorted by total sales
  - Filtered top 5 via Value Filter
- **Average Customer Rating by Region**
- **Best-Selling Product** using formulas

### 📈 Dashboard Components
- **KPI Cards**: Total Sales, Avg Rating, Top Product
- **Dynamic Charts**:
  - Bar Chart: Sales by Region
  - Line Chart: Monthly Sales Trend
  - Pie Chart: Payment Method Split
- **Slicers** for Region, Salesperson, Product

---

## 🧠 Formulas Used

### Top 5 Sales Values:
```excel
=LARGE(tblSales[Total Sales], ROW(A1))
