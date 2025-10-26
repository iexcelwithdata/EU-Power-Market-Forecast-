# ⚡ EU Renewable Energy Forecast Dashboard (Power BI)
Interactive Power BI dashboard for EU renewable energy capture price forecasts


## 📖 Scenario

Laura, the director for strategic planning and development at my firm, reached out to me with an urgent request. Her two market analysts, Aaron (GB) and Brian (DE), were on holiday, and she needed an analysis performed within a few days.

She placed their latest Excel spreadsheets in a Dropbox folder, containing forecasts on generation capacity, power generation, wholesale, and capture prices from Q3 2022 and Q1 2023. My task was to make sense of this data and draw key insights for her strategic work



### Laura is particularly interested in the following for the 2023–2050 period:

1.  How do **wholesale power prices (baseload)** compare between Great Britain (GB) and Germany (DE), and how does the generation mix explain the difference?
2.  Which technology offers better long-term potential: **Solar PV in GB** or **Onshore Wind in DE** (from a capture price perspective)?
3.  Is there a relationship between **capture prices and power generation output (GWh)** for solar PV and onshore wind in DE?
4.  Did Aaron significantly change his solar PV and onshore wind capture price forecasts between Q3 2022 and Q1 2023?

#### Laura also provided key assumptions:

1. GBP-EUR exchange rate: 1.164 (2022), 1.161 (2023), 1.158 (2024–2050).

2. Annual inflation rate: 6.87% (DE, 2022) and 9.06% (GB, 2022).

Finally, as a strategist, she wants to avoid similar hassles in future. She’d like a process where she can swap in new Excel spreadsheets (different quarters) and have Power BI update automatically.

I also discussed the task with another analyst colleague who suggested considering the following:

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

---

## 🧮 Data Modeling (DAX)
Key measures developed:  
- **Median Capture Price** (by tech).  
- **Forecast Change %** between the two versions of the dataset.  
- **YoY Growth** with conditional formatting.  
- **Dynamic Arrows** (↑ Green, ↓ Red, → Grey) using `UNICHAR`.    

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
![Main Dashboard](https://github.com/iexcelwithdata/EU-Power-Market-Forecast-/EU-Power-Market-Forecast.png)

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

