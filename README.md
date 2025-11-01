
# 📘 Global eCommerce Sales Dataset – README

## Overview

This dataset contains 100,000 synthetic eCommerce transactions from various countries, designed specifically for use in Power BI, Excel, Tableau, or any BI tool. It's clean, realistic, and includes enough dimensions to build a rich, interactive dashboard.

It simulates 3 years of global sales and includes details like product categories, customer segments, profit, returns, and more.

---

## File Details

- **Filename:** `global_ecommerce_data.csv`
- **Size:** ~10 MB
- **Rows:** 100,000
- **Format:** CSV
- **Data Type:** Synthetic (not real, generated for training and demo purposes)

---

## Column Descriptions

| Column Name       | Description |
|-------------------|-------------|
| `OrderID`         | Unique ID for each transaction |
| `CustomerID`      | Unique identifier for the customer |
| `Country`         | Country where the order was placed |
| `OrderDate`       | Date of the order in YYYY-MM-DD format |
| `Category`        | Product category (e.g., Electronics, Clothing) |
| `SubCategory`     | More specific product type |
| `ProductName`     | Name of the product sold |
| `Quantity`        | Number of items purchased |
| `UnitPrice`       | Price per unit (in USD) |
| `Discount`        | Discount applied (range from 0 to 0.2) |
| `TotalSales`      | Revenue after discount = Quantity × UnitPrice × (1 - Discount) |
| `PaymentMethod`   | Method used to pay (e.g., PayPal, Credit Card) |
| `CustomerSegment` | Type of customer (Consumer, Corporate, Small Business) |
| `ShippingCost`    | Cost of delivery |
| `Profit`          | Final profit = TotalSales - Cost of Goods - Shipping |
| `OrderPriority`   | Priority level (High, Medium, Low) |
| `Returned`        | Whether the item was returned (Yes/No) |

---

## Suggested Visuals (for Power BI)

- **KPI Cards:** Total Sales, Profit, Profit Margin (%)
- **Line Chart:** Monthly sales trends
- **Pie/Donut Charts:** Sales by Category, Country, and Payment Method
- **Bar Charts:** Top-selling Products, Segments, or Countries
- **Treemap:** Sales by Category & Subcategory
- **Slicers:** Filter by Year, Month, Segment, and Country

---

## Sample DAX Measures

```DAX
Total Sales = SUM(Sales[TotalSales])
Total Profit = SUM(Sales[Profit])
Profit % = DIVIDE([Total Profit], [Total Sales], 0)
```

Format `Profit %` as a percentage with 1–2 decimal places.

---

## Use Cases

- Power BI dashboard development
- DAX and time-intelligence practice
- Data storytelling projects
- Mock executive reporting
- BI interview preparation

---

## Notes

- This data is **completely synthetic** and safe for public use.
- It’s built to help analysts, students, and data enthusiasts sharpen their visualization and reporting skills.
