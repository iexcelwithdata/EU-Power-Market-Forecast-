# ⚡ EU Renewable Energy Forecast Dashboard (Power BI)
Interactive Power BI dashboard for EU renewable energy capture price forecasts


![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?logo=powerbi)  
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)  
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)  

## 📖 Scenario

Laura is a director for strategic planning and development at a European renewable energy firm assisted by two excellent analysts named Aaron and Brian. The duo provides her with power market forecasts for their respective markets. Aaron is covering Great Britain (GB) and Brian is responsible for Germany (DE). Both are on holiday and will not return until after Oktoberfest.

Laura has an urgent analysis to perform within a few days. She knows you are a great data analyst working in another department and has reached out to you for help. She has placed Aaron and Brian’s Excel spreadsheets in a Dropbox folder, containing forecasts on generation capacity, power generation, wholesale, and capture prices etc. from Q3 2022 and Q1 2023. She wants you to help make sense of the data and draw some insights for her work.

Laura is particularly interested in the following for the 2023–2050 period:

How do wholesale power prices (baseload) compare between GB and DE, and can the generation mix explain the difference?

From a capture price perspective, which technology offers better potential between solar PV in GB and onshore wind in DE?

In the long run, is there a relationship between capture prices and power generation output (GWh) for solar PV and onshore wind in DE?

Did Aaron change his forecast for solar PV and onshore wind capture prices between Q3 2022 and Q1 2023? If so, how significant is the shift and what could possibly explain that?

Laura also provided key assumptions:

GBP-EUR exchange rate: 1.164 (2022), 1.161 (2023), 1.158 (2024–2050).

Annual inflation rate: 6.87% (DE, 2022) and 9.06% (GB, 2022).

Finally, as a strategist, she wants to avoid similar hassles in future. She’d like a process where she can swap in new Excel spreadsheets (different quarters) and have Power BI update automatically.

You also discussed the task with another analyst colleague who suggested considering the following:

Centralized Data Approach – future-proofing via a data lake/warehouse.

Data Transformation (ETL) – clean, filter, and structure Excel data for analysis.

Data Visualization – build interactive Power BI dashboards with slicers for quarters, years, and currencies.

Automation – enable automatic refresh when new files are added.

User-Friendly Interface – give Laura control over filters and parameters.

Documentation & Training – ensure Laura can reuse the workflow independently.s.  

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

