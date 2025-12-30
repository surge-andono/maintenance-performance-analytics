# Maintenance Operational Performance Dataset

## Overview
This dataset represents **simulated maintenance and operational performance data** used for analytics, EDA, and Power BI dashboard development in the *Maintenance Performance Analytics* project.

The data is designed to reflect **realistic maintenance scenarios** commonly found in asset-intensive industries such as mining, manufacturing, and utilities.

---

## Dataset Purpose
This dataset is used to support:
- Exploratory Data Analysis (EDA)
- KPI and measure development
- Star schema data modeling
- Power BI dashboard visualization
- Executive, operational, and RCA analysis

⚠️ **Note:**  
This is a **sample / simulated dataset**, not real production data.

---

## File Information
- **File name:** `maintenance_operational.csv`
- **Format:** CSV
- **Granularity (Grain):**  
  One row represents **one maintenance event for one equipment on a specific date**.

---

## Column Descriptions

| Column Name | Description |
|------------|------------|
| `date` | Date when the maintenance event occurred |
| `equipment_id` | Unique identifier of the equipment |
| `site` | Operational site or plant location |
| `region` | Region where the site is located |
| `downtime_hours` | Total downtime hours caused by the maintenance event |
| `repair_hours` | Total labor hours spent on repair activities |
| `failure_type` | Classification of failure (mechanical, electrical, etc.) |
| `maintenance_cost` | Total maintenance cost associated with the event |
| `work_order_count` | Number of work orders generated for the event |

---

## Analytical Use Cases

This dataset supports the calculation of key maintenance KPIs, including:
- Total Downtime (Hours)
- Total Maintenance Cost
- Total Repair Hours
- Total Work Orders
- MTTR (Mean Time To Repair)
- MTBF (proxy)
- Cost per Work Order
- Cost per Downtime Hour
- Downtime Contribution %
- Downtime MoM %

---

## Data Modeling Notes
- This dataset serves as the **fact table source** (`Fact_MaintenancePerformance`)
- Dimension tables (Date, Equipment, Site, Failure) are derived from this data
- Designed for **star schema** implementation in Power BI

---

## Tools Used
- Power BI
- DAX
- Star Schema Data Modeling

---

## Disclaimer
This dataset is created for **educational, demonstration, and portfolio purposes only**.  
It does not represent actual operational data from any organization.
