# Car Sales Dashboard (Power BI + Python/SQL)

## 📌 Overview

An interactive car sales performance dashboard analyzing YTD sales, pricing trends, and dealer/company performance across the US. Data was sourced from Kaggle, cleaned and processed using Python and SQL, then visualized in Power BI for business reporting.

## 🎯 Business Problem

Sales leadership needed a consolidated view of car sales performance — tracking revenue trends, pricing shifts, top-performing companies/dealers, and regional sales distribution — to support data-driven decision making and identify growth opportunities across markets.

## 🛠️ Tools & Skills Used

- **Python & SQL** — data cleaning, transformation, and preprocessing
- **Power BI** — interactive dashboard design, DAX measures, KPI cards, drill-down/detail views
- **Data Visualization** — trend analysis, donut charts, geo-mapping, ranked tables

## 📊 Dataset

Car Sales dataset (Kaggle) — transactional-level car sales records including Car ID, Date, Customer Name, Dealer Name, Company, Color, Body Style, Model, and Total Sales value.

## 🔍 Key Features

### Overview Dashboard

- **YTD KPIs with MTD Comparison:**
  * YTD Total Sales: **$69.0M** (↑23.60% YoY) | MTD Total Sales: $52.87M
  * YTD Average Price: **$27.98K** (↓0.84% YoY) | MTD Avg Price: $28.26K
  * YTD Cars Sold: **2.6K units** (↑19.77% YoY) | MTD Cars Sold: 1.87K units
- **YTD Sales Weekly Trend:** Line chart tracking weekly sales fluctuation across the year, ranging from $1.0M to $14.4M per week
- **Sales by Body Style:** Donut chart breakdown across SUV, Sedan, Hatchback, Passenger, and Hardtop categories
- **Sales by Color:** Donut chart showing customer color preference distribution (Pale White, Black, Red)
- **Geo Analysis:** Interactive US map showing cars sold and average price by dealer region (covering regions like Austin, Janesville, Middletown, Scottsdale, Greenville)
- **Company-wise Sales Ranking:** Table ranking companies by YTD Total Sales and % contribution to overall revenue — Chevrolet (7.30%), Ford (6.81%), Dodge (6.74%) lead the pack

<!-- TODO before publishing: recheck the YoY figures in Power BI. Sales +23.6% does not reconcile with units +19.77% and average price -0.84% (that combination gives roughly +19%). -->

### Details Page

- **Transaction-level drill-down** with 17,557+ individual sales records
- Fields include Car ID, Date, Customer Name, Dealer Name, Company, Color, Model, and Total Sales per transaction
- Enables granular auditing of any individual sale behind the summary KPIs

## 💡 Key Insights

- **Growth is volume-led, not price-led:** YTD sales and units sold are both up strongly year over year while average price is roughly flat, so revenue growth comes from selling more cars rather than raising prices
- Chevrolet, Ford, and Dodge lead with **~20.85%** of YTD revenue combined; the remaining ~79% is spread across other manufacturers, so there is no single-brand dependency
- Weekly sales show high volatility (ranging $1M–$14.4M), suggesting seasonal or promotional demand spikes worth investigating further
- Pale White and Black are the most preferred car colors among customers, which could inform inventory and manufacturing planning

## 📁 Files

- `car_sales_overview.png` — Dashboard overview page (KPIs, trends, segmentation, geo-map, company rankings)
- `car_sales_details.png` — Transaction-level detail/drill-down page
