# ⚡ EU Renewable Energy Forecast Dashboard (Power BI)
Interactive Power BI dashboard for EU renewable energy capture price forecasts


![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?logo=powerbi)  
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)  
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)  

## 📌 Overview
This repository contains a **Power BI dashboard** designed to analyze and visualize **renewable energy capture price forecasts** for the EU power markets.  
It focuses on **Solar PV, Onshore Wind, and Offshore Wind**, combining data transformation (Power Query), robust data modeling (DAX), and interactive visualization.  

The dashboard enables decision-makers to:  
- Track forecast evolution across quarters.  
- Compare analyst views (Aaron – GB, Brian – DE).  
- Identify year-on-year shifts in capture prices.  
- Visualize technology-specific market insights.  

---

## 🎯 Objectives
- Provide a clear **side-by-side comparison** of renewable capture prices in GB and DE.  
- Track how forecasts evolved between **2022Q3 and 2023Q1**.  
- Deliver interactive slicers (currency, inflation adjustment, forecast version).  
- Create KPI cards with **dynamic arrows (↑ ↓ →)** using DAX & UNICHAR for trend insights.  

---

## 📂 Data Sources
- **Energy Forecasts (2022–2023)**: Raw files from folder connectors.  
- Technologies covered: `Solar PV`, `Onshore Wind`, `Offshore Wind`.  
- Columns include: `Year`, `Quarter`, `Forecast Version`, `Analyst`, `Country`, `Capture Price (£/MWh or €/MWh)`.  

---

## 🔄 Data Transformation (Power Query)
- Automated ingestion of multiple Excel/CSV files via **Folder connector**.  
- Dynamic year extraction logic to handle files with inconsistent starting years.  
- Removed hidden/system files.  
- Applied transformation scripts stored in [`docs/powerquery-m.md`](docs/powerquery-m.md).  

---

## 🧮 Data Modeling (DAX)
Key measures developed:  
- **Average Capture Price** (by tech, country, analyst).  
- **Forecast Change %** between quarters (with ALL() to ignore Forecast Version filter).  
- **YoY Growth** with conditional formatting.  
- **Dynamic Arrows** (↑ Green, ↓ Red, → Grey) using `UNICHAR`.  

👉 Full list available in [`docs/dax-measures.md`](docs/dax-measures.md).  

---

## 📊 Dashboard Features
- **KPI Cards** → capture price changes with trend arrows.  
- **Line Charts** → forecast evolution across years.  
- **Scatter Plots** → technology vs. forecast version insights.  
- **Slicers** → toggle Forecast Version, Currency (GBP/EUR), and Inflation adjustment.  
- **Bookmarks & Drill-through** → for analyst-specific deep dives (Aaron GB, Brian DE).  

---

## 🖼️ Dashboard Preview

### Main Overview Page
![Main Dashboard](assets/dashboard_main.png)

### Analyst Comparison
![Analyst Comparison](assets/dashboard_comparison.png)


*(Replace these placeholders with your actual screenshots in the `/assets/` folder.)*  

---

## ⚙️ How to Use
1. Clone this repo:  
   ```bash
   git clone https://github.com/yourusername/powerbi-energy-forecast-dashboard.git

Open the Power BI file:
- PowerBI_Forecast.pbix
- Refresh data sources (update file paths in Power Query if needed).
- Interact with slicers & visuals to explore insights.

---

---
## 🛠️ Tech Stack

- Power BI Desktop (data modeling & visualization)
- Power Query (M) (ETL & data cleaning)
- DAX (measures & KPIs)
- Excel/CSV (data sources)
- GitHub (project documentation & version control)
---

---
## 📚 Learnings & Challenges

- Solved Formula.Firewall issue in Power Query by staging queries.
- Implemented dynamic year extraction for flexible file ingestion.
- Created custom DAX arrows with UNICHAR + conditional coloring.
- Ensured measures remain independent of Forecast Version slicer.
---

---
## 🚀 Future Improvements

- Automate data refresh with Power BI Service + Gateway.
- Add more countries/technologies as datasets become available.
- Integrate weather and demand data for deeper insights.

---

---
## 👤 Author

Kuku Faruq Olabiyi (Data Analytics)
📧 [kukuolabiyi04@gmail.com]
💼 www.linkedin.com/in/faruqkukuolabiyi
🐙 GitHub
---

---
## 📜 License

This project is licensed under the MIT License – see the LICENSE file for details.
---

