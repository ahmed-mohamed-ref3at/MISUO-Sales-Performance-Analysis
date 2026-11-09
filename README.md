# MISUO Sales Performance Analysis

### Excel Data Cleaning · Pivot Tables · Interactive Sales Dashboard

**Prepared by Ahmed Mohamed Refaat**

A complete, Excel-based sales analysis project focused on converting unstructured order records into an interactive dashboard. The analysis covers recorded sales value, product demand, geographic distribution, sales platforms, customer segments, and delivery performance to support more informed business decisions.

![MISUO Sales Performance Dashboard](images/dashboard.png)

## Project Overview

The project began with a sales workbook containing inconsistent or incomplete information. The data was reviewed and prepared in Microsoft Excel, enriched with analytical fields, summarized with Pivot Tables, and presented through a dashboard with KPI cards, charts, and interactive filters.

**Core business questions**

- How much sales value is recorded, and what is the average selling price?
- Which product categories and colors appear most frequently?
- Which governorates and sales platforms generate the highest order activity?
- What is the split between individual and company customers?
- What do order statuses and delivery-timing indicators reveal?

## Tools & Techniques

- **Microsoft Excel** — data preparation, analysis, and visualization
- **Data Cleaning** — review of missing values, inconsistent labels, dates, and identifiers
- **Feature Engineering** — customer type, governorate, expected/actual delivery durations, and an on-time indicator
- **Pivot Tables** — KPI calculations and grouped summaries
- **Pivot Charts & Slicers** — interactive dashboard visualizations and filtering

## Dataset & Preparation

| Stage | Records | Columns |
| --- | ---: | ---: |
| Original worksheet | 126 | 21 |
| Prepared analysis worksheet | 120 | 24 |

The preparation work addressed incomplete values and inconsistent fields, and organized the final dataset for analysis. The final worksheet includes additional analytical attributes such as:

- **Customer type** — individuals or companies
- **Governorate** — a standardized location field for geographic reporting
- **Expected and actual delivery durations** — measures for comparing delivery timelines
- **On-time flag** — a `1` / `0` indicator used by the dashboard

The original and final Excel workbooks are both included so the input and analytical output can be examined side by side. The final workbook retains the Pivot Tables, charts, and interactive dashboard.

## Dashboard KPIs

| KPI | Dashboard result | How to interpret it |
| --- | ---: | --- |
| **Total Sales** | **EGP 1,252,638.32** | Sum of selling-price values across all 120 analyzed records and statuses |
| **Total Orders** | **120** | Count of analyzed records; **not** a verified count of distinct order IDs |
| **Average Selling Price** | **EGP 10,438.65** | Average selling price across the 120 records |
| **On-Time Delivery** | **36.7%** | 44 of 120 records have an on-time flag of `1` |
| **Best-Selling Category** | **Beds** | 83 records |
| **Most Common Metal Color** | **Black** | 45 of 102 records with a nonblank metal color |

> **Metric note:** “Total Sales” describes recorded selling-price value, not exclusively completed-delivery revenue. The dashboard's on-time percentage uses all 120 rows as its denominator, including rows without a completed delivery. This should not be read as the punctuality rate among delivered orders alone.

## Key Insights

### 1. Product performance

**Beds** are the leading product category, with **83 of 120 records (69.2%)**. Sofas and tables follow with **17 records each**. Black is the most common populated metal-color value (**45 of 102**).

**Business implication:** Review inventory and availability for popular bed categories, while examining demand for other products and colors.

### 2. Geographic concentration

**Cairo** accounts for **56 records (46.7%)**, followed by **Giza** with **24 records (20.0%)**. **11 records** have an unspecified governorate in the dashboard summary.

**Business implication:** Prioritize delivery-capacity monitoring in high-activity areas and improve missing location details when feasible.

### 3. Sales channel activity

**Homezmart** appears on **78 records (65.0%)**, making it the largest platform by analyzed record count. Other platforms can be compared in the included Excel Pivot Tables.

**Business implication:** Compare sales value and fulfillment outcomes by platform before deciding where to increase channel investment.

### 4. Customer segmentation

The analyzed data contains **88 individual-customer records (73.3%)** and **32 company-customer records (26.7%)**.

**Business implication:** Explore whether product preferences, channel use, and delivery needs differ between customer segments.

### 5. Delivery performance

| Order status | Records | Share of analyzed records |
| --- | ---: | ---: |
| Delivered | 96 | 80.0% |
| Failed delivery | 23 | 19.2% |
| Returned | 1 | 0.8% |
| **Total** | **120** | **100%** |

The dashboard's on-time indicator is positive for **44 records**. This highlights an opportunity to analyze delays and to report delivery punctuality separately for records with confirmed delivery dates.

**Business implication:** Investigate recurring delay causes, monitor service levels by area and platform, and make the on-time metric's denominator explicit.

## Analysis Workflow

```text
Raw Excel Data (126 records)
           |
           v
Data Cleaning & Preparation
           |
           v
Feature Engineering (customer, location, delivery fields)
           |
           v
Prepared Analysis Data (120 records)
           |
           v
Pivot Tables & KPI Aggregation
           |
           v
Interactive MISUO Sales Dashboard
           |
           v
Insights & Business Recommendations
```

## Repository Structure

```text
MISUO-Sales-Performance-Analysis/
├── README.md
├── .gitignore
├── data/
│   └── MISUO_Raw_Data.xlsx
├── excel/
│   └── MISUO_Sales_Analysis.xlsx
├── images/
│   └── dashboard.png
└── report/
    ├── MISUO_Sales_Performance_Report.pdf
    └── MISUO_Sales_Performance_Report.pptx
```

## Explore the Project

1. **[View the dashboard](images/dashboard.png)** for a quick overview of the final result.
2. **[Open the Excel analysis workbook](excel/MISUO_Sales_Analysis.xlsx)** in desktop Microsoft Excel to inspect the prepared data, Pivot Tables, charts, and filters.
3. **[Read the full project report](report/MISUO_Sales_Performance_Report.pdf)** for the analysis, visuals, and recommendations.
4. **[Review the raw workbook](data/MISUO_Raw_Data.xlsx)** to compare the source with the prepared analysis file.

The dashboard and its filters are designed for Microsoft Excel; GitHub itself displays a static file preview rather than an interactive Excel dashboard.

## Author

**Ahmed Mohamed Refaat**  
Data Analyst

- **LinkedIn:** [linkedin.com/in/ahmed-mohamed-refaat-642064330](https://www.linkedin.com/in/ahmed-mohamed-refaat-642064330/)
- **Email:** [ahmed5196643@gmail.com](mailto:ahmed5196643@gmail.com)
- **Phone:** +20 122 500 2143
