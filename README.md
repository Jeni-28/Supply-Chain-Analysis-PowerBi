# Supply Chain Analysis using Power BI

## Project Overview

This project focuses on analyzing supply chain data to evaluate business performance across sales, inventory, delivery, and product quality. The objective is to identify inefficiencies, uncover business insights, and support data-driven decision-making through interactive Power BI dashboards.

The dashboard provides a comprehensive view of supply chain operations and helps businesses improve efficiency, inventory planning, logistics management, and supplier performance.

---

## Business Objectives

- Analyze product-wise sales and revenue performance
- Evaluate inventory and stock management efficiency
- Monitor delivery performance using shipping and lead times
- Assess supplier quality and defect rates
- Generate actionable business recommendations

---

## Tools & Technologies

- Power BI
- MySQL Database
- phpMyAdmin
- CSV Dataset
- DAX Measures
- Data Modeling & Visualization

---

## Dataset Information

The dataset contains supply chain-related information including:

- Product Type
- SKU
- Price
- Revenue Generated
- Products Sold
- Stock Levels
- Availability
- Shipping Time
- Lead Time
- Supplier Information
- Manufacturing Cost
- Defect Rate
- Inspection Results
- Transportation Mode
- Shipping Cost

---

## Data Preparation

### Data Cleaning
- Imported CSV dataset into Power BI
- Validated and cleaned data
- Split data into:
  - Supply Chain Data
  - Supplier Performance Data

### Calculated Column
```DAX
Stock Status =
IF([Stock Levels] < 30, "Low Stock", "Sufficient Stock")
```

### Measures

```DAX
Total Revenue = SUM('Supply Chain Data'[Revenue Generated])

Total Products Sold = SUM('Supply Chain Data'[Number of products sold])

Average Shipping Time = AVERAGE('Supply Chain Data'[Shipping times])

Average Defect Rate = AVERAGE('Supplier Performance Data'[Defect rates])
```

---

## Dashboard Pages

### 1. Overview Dashboard
Provides a high-level summary of:

- Revenue Performance
- Product Sales
- Revenue by Location
- Shipping Cost Distribution
- Product Category Analysis

### 2. Sales Analysis
Focuses on:

- Revenue by Product Type
- Revenue by Location
- Top Performing SKUs
- Sales vs Revenue Relationship

### 3. Inventory Analysis
Focuses on:

- Stock Availability
- Low Stock Monitoring
- Product-wise Stock Levels
- Order Quantity Analysis

### 4. Delivery Analysis
Focuses on:

- Shipping Time Analysis
- Lead Time Analysis
- Carrier Performance
- Transportation Mode Comparison

### 5. Quality Analysis
Focuses on:

- Supplier Performance
- Manufacturing Cost Analysis
- Defect Rate Monitoring
- Inspection Results

---

## Key Insights

### Sales Performance
- Skincare products generate the highest sales and revenue.
- Top-performing SKUs contribute significantly to total revenue.
- Mumbai and Kolkata are the strongest-performing locations.

### Inventory Performance
- 76% of products have sufficient stock levels.
- 24% of products fall under low-stock categories.
- Skincare products have the highest demand.

### Delivery Performance
- Cosmetics products experience the highest shipping time.
- Road transport is the fastest transportation mode.
- Sea transport is the most economical option.

### Quality Performance
- Supplier B has the lowest defect rate.
- Supplier C has the highest defect rate.
- Higher manufacturing costs do not necessarily indicate better quality.

---

## Business Recommendations

- Increase focus on high-performing skincare products.
- Improve inventory planning for high-demand items.
- Optimize logistics costs and delivery efficiency.
- Reduce dependency on suppliers with high defect rates.
- Strengthen quality inspection processes.

---

## Challenges Faced

- Supplier naming inconsistencies prevented relationship creation between tables.
- Learning and implementing DAX calculations.
- Data preparation and dashboard design.

---

## Project Outcome

The project successfully demonstrates how Power BI can be used to analyze supply chain operations and transform raw data into meaningful business insights. The dashboard helps stakeholders monitor performance, identify inefficiencies, and make informed decisions.

---

## Dashboard Preview

### Overview Dashboard
(Add Screenshot Here)

### Sales Dashboard
(Add Screenshot Here)

### Inventory Dashboard
(Add Screenshot Here)

### Delivery Dashboard
(Add Screenshot Here)

### Quality Dashboard
(Add Screenshot Here)

---

## Author

**Jenihelan M**

MCA Student | Data Analyst Aspirant

Skills:
- Power BI
- SQL
- Python
- Excel
- Data Analytics
