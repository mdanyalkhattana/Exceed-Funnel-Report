
# EXCEED Funnel Report Dashboard

## Overview

The **EXCEED Funnel Report Dashboard** is a professional Power BI project designed to provide end-to-end analysis of the **sales funnel**, tracking leads from initial contact to finalized sales.

The dashboard enables businesses to **monitor lead progression, evaluate conversion rates, and identify bottlenecks** in the sales process, supporting data-driven decision-making and strategic planning.

---

## Main Focus

* Analyze the **full lead-to-sale journey**, from initial lead generation to invoicing and exceeded targets.
* Identify **critical drop-off points** in the funnel to optimize sales processes.
* Provide **actionable insights** for sales and marketing teams to increase conversion efficiency.

---


## Key Features

* **Funnel Visualization**: Shows progression of leads through stages – Leads → Quotes → Invoiced → Exceeded/Cancelled.
* **Dynamic KPIs**: Real-time insights for conversion rates, sales performance, and target achievement.
* **Time-Based Analysis**: Daily, weekly, monthly, and quarterly trends to track performance over time.
* **Interactive Filters**: Independent slicers for visual-specific analysis without affecting other reports.
* **Gap Analysis**: Highlights where leads are being lost, enabling targeted interventions.

---

## Tools & Technologies

* **Power BI** – Dashboard development and visualization
* **DAX (Data Analysis Expressions)** – Advanced calculations and measures
* **Excel / SQL** – Data preparation and cleaning
* **GitHub** – Version control and portfolio showcase

---

## Data Preparation & Modeling

* Standardized and cleaned raw sales and leads data.
* Created **date tables** for advanced time intelligence.
* Designed **independent measures** to maintain accurate totals and avoid conflicts between table and visual-level data.
* Applied DAX logic to **handle negative values and missing data**, ensuring clean and reliable metrics.

---

## Example Measures

```DAX
## Carry Forward =
VAR SAVEVALUE = ('public dimlead'[Leads with Quotes] - [##Invoiced1]) - [## Cancelled]
RETURN IF(SAVEVALUE < 0, 0, SAVEVALUE)
```

```DAX
Date_Table = CALENDAR(MIN(Sales[Date]), MAX(Sales[Date]))
```

* Measures enable **precise lead-to-sales tracking** and **independent visual analysis**.

---

## Dashboard Screenshots

<img width="1259" height="723" alt="image" src="https://github.com/user-attachments/assets/87751822-f58d-43e7-b6dc-aa38471c3ebe" />


---

## Project Structure

```text
EXCEED-Funnel-Dashboard/
│
├─ README.md
├─ Exceedfunnelreport.pbix       # Power BI file
├─ Data/
│   └─ data.xlsx        
├─ pdf of dashboard/
│   

---



**Muhammad Danyal ** – Data Analyst & Power BI Developer


