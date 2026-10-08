# Supply Chain & Inventory Analytics

## 📌 Project Overview

This project analyzes supply chain and inventory data to identify inventory inefficiencies, reorder requirements, supplier performance, warehouse trends, and high-value SKUs.

The project combines **MySQL** for data analysis and **Power BI** for interactive dashboard development.

The objective is to help businesses make better inventory decisions by identifying:

- Inventory value concentration
- Overstocked inventory
- High-risk inventory
- Reorder requirements
- Supplier performance
- Warehouse and regional performance
- High-value and slow-moving SKUs
- ABC inventory classification

---

## 🛠️ Tools & Technologies

- **MySQL** — Data cleaning validation and SQL analysis
- **Power BI** — Interactive dashboard and visualization
- **SQL** — Aggregations, filtering, CASE statements, CTEs and window functions
- **Excel/CSV** — Source dataset
- **GitHub** — Project documentation and version control

---

## 📊 Dataset

The dataset contains **91,250 inventory records** covering:

- SKUs
- Inventory levels
- Inventory value
- Units sold
- Days of inventory
- Suppliers
- Supplier lead time
- Warehouses
- Regions
- Inventory status
- Reorder risk
- Stockout indicators

---

# 📈 Power BI Dashboard

The Power BI report contains four analytical pages.

## 1. Supply Chain & Inventory Overview

Key metrics:

- Total Inventory Value
- Total Units Sold
- Average Inventory Level
- Average Days of Inventory

The page also provides analysis by:

- Region
- Warehouse
- Inventory Status
- SKU

---

## 2. Inventory Risk & Reorder Analysis

This page focuses on inventory risk and replenishment requirements.

Key metrics include:

- Reorder Required
- High Risk Records
- Overstock Records
- Average Days of Inventory

Additional analysis:

- Reorder risk distribution
- Top SKUs requiring reorder
- Inventory status by region
- Inventory status by warehouse

---

## 3. Supplier Performance Analysis

This page evaluates supplier performance using:

- Average Supplier Lead Time
- Inventory Value by Supplier
- Average Days of Inventory by Supplier
- Reorder Requirements by Supplier

A supplier comparison table provides:

- Average lead time
- Inventory value
- Average inventory days
- Reorder records

---

## 4. ABC & Inventory Efficiency Analysis

This page identifies inventory concentration and efficiency.

Analysis includes:

- Top SKUs by inventory value
- Top SKUs by days of inventory
- Inventory Value vs Days of Inventory
- Inventory Status Distribution
- ABC inventory classification
- SKU-level ABC analysis

---

# 🔍 Key Findings

### Inventory

- **91,250 records** were analyzed.
- Total inventory value is approximately **525.24M**.
- Average inventory level is approximately **471.52**.
- Average inventory coverage is approximately **45.13 days**.

### Reorder Risk

- **5,041 records (5.52%)** require reordering.
- **86,209 records (94.48%)** have sufficient stock.

### Inventory Status

- Approximately **57.86K records** are classified as Healthy.
- Approximately **31.78K records** are classified as Overstock.
- **719 records** are classified as High Risk.
- **892 records** have No Forecast Demand.

### Supplier Performance

- Average supplier lead time is approximately **7.98 days**.
- Supplier performance varies across lead time, inventory value and reorder requirements.

### SKU Efficiency

Some SKUs have significantly higher inventory coverage than others.

For example:

- **SKU_5** has approximately **98 days** of inventory.
- **SKU_7** has approximately **76 days**.
- **SKU_3** has approximately **72 days**.

These SKUs may require further investigation for potential slow-moving or excess inventory.

---

# 💡 Business Recommendations

Based on the analysis:

### 1. Reduce Overstock

Investigate SKUs with very high Days of Inventory to reduce excess working capital.

### 2. Prioritize Reorder Requirements

Focus replenishment activities on the **5.52% of records requiring reorder**.

### 3. Monitor High-Risk Inventory

The **719 high-risk records** should be reviewed regularly to prevent potential stock availability problems.

### 4. Improve Supplier Management

Compare supplier lead times and reorder requirements to identify opportunities for supplier optimization.

### 5. Focus on High-Value SKUs

Use ABC classification to prioritize inventory management efforts toward high-value SKUs.

### 6. Improve Forecasting

Records classified as **No Forecast Demand** should be investigated to improve demand forecasting and inventory planning.

---

# 📂 Project Structure

```text
Supply-Chain-Inventory-Analytics/
│
├── Data/
│   └── cleaned/
│       └── supply_chain_cleaned.csv
│
├── SQL/
│   └── supply_chain_analysis.sql
│
├── PowerBI/
│   └── Supply_Inventory.pbix
│
├── Screenshots/
│   ├── dashboard_overview.png
│   ├── inventory_risk.png
│   ├── supplier_performance.png
│   └── abc_inventory_analysis.png
│
└── README.md