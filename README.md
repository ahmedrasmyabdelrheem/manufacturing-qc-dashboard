# Manufacturing Quality Control & Production Analytics

## 📌 Project Overview
An end-to-end operational analytics solution designed to monitor garment manufacturing lines, track quality metrics, and reduce scrap rates. 

The project captures shop-floor defect data in real time via digital forms, processes and cleans the data using Power Query, and presents key performance indicators (KPIs) through an interactive Power BI dashboard with scheduled cloud refreshes.

---

## 🎯 Business Problem & Objectives
- **Manual Data Logging:** Reliance on paper inspection logs caused delays in reporting defects.
- **High Scrap Rates:** Lack of real-time visibility into production line performance and machinery downtime.
- **Objective:** Track defect rates across 25,000+ garments, analyze causes across 4 production lines, and provide management with automated daily insights.

---

## 🏗️ Technical Architecture & Pipeline

```text
[Shop-Floor Data Entry]
  - 3 Google Forms deployed across 4 production lines
         ↓
[Cloud Storage & Consolidation]
  - Centralized Google Sheets database
         ↓
[Power Query / ETL Layer]
  - Data cleaning, schema standardization, and appending
         ↓
[Power BI Analytical Layer]
  - Star Schema dimensional model & DAX KPI measures
  - Tracking scrap rates, defects, and downtime stoppages
  - Scheduled 8-hour cloud refresh via Power BI Service
