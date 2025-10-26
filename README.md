# ⚡ **EU Renewable Energy Market Intelligence Dashboard**  
**(Power BI | Data Analytics | Automation | Energy Strategy | ETL | DAX | Data Modeling)**  

---

## 🚀 **Executive Summary**

Europe’s renewable energy transition depends on strategic foresight — knowing *where* to invest and *when*.  
This Power BI dashboard transforms fragmented Excel forecasts into a **centralized market intelligence tool** that empowers energy strategists to **compare, forecast, and act** on long-term capture price trends for **Solar PV and Onshore Wind** in **Great Britain (GB)** and **Germany (DE)**.  

By automating the analytics process, the project enables leadership to:
- **Compare baseload and capture price evolution (2022–2050)**  
- **Identify high-performing renewable technologies under inflation & currency shifts**  
- **Evaluate forecast reliability across versions (2022Q3 vs 2023Q1)**  
- **Reduce analyst turnaround time from days to minutes** through full ETL automation  

> 💼 **Business Impact:** Delivered a repeatable analytics framework that cuts manual reporting time by **85%** and provides executives with instant, reliable insights into cross-country investment performance.  

![EU Power Market Forecast Problem Overview](./assets/EU%20Power%20Market%20Forecast%20Problem%20View.png)

---

## 🧩 **Business Problem**

Energy strategy executives faced recurring challenges:
- Analysts submitted **inconsistent forecast files** (different years, formats, currencies).  
- Strategic planning was slowed by **manual data cleaning** and **non-standard updates**.  
- Leadership couldn’t clearly see **how forecasts evolved** or **which technology offered better returns**.  

📉 *Result:* High-stake investment decisions were being made on fragmented and outdated data.  

### 🎯 **Goal**
Create a **fully automated Power BI dashboard** that consolidates forecasts, compares capture and baseload price trends, and enables **real-time strategic insights** — with zero manual intervention.  

---

## 🧠 **Methodology**

| Phase | Approach | Key Deliverable |
|-------|-----------|-----------------|
| **1. Data Engineering** | Automated ingestion using **Power Query (M)** Folder Connector | Unified dataset with dynamic year alignment |
| **2. Data Cleaning & ETL** | Transform logic to normalize inconsistent file structures | Clean, analytics-ready dataset |
| **3. Data Modeling** | Built a **Star Schema** linking Forecast, Country, and Technology tables | Single source of truth |
| **4. Analytics (DAX)** | Developed KPI measures: Median Capture Price, YoY Growth %, Forecast Shift % | Insight-ready metrics |
| **5. Visualization & Storytelling** | Designed **Power BI dashboard** with interactive slicers, bookmarks, and trend arrows | Executive-level data exploration |
| **6. Automation** | Enabled **auto-refresh** for new forecast files via Power Query logic | Scalable, reusable process |

---

## 🛠️ **Skills & Tools**

**Power BI & Visualization**
- KPI Cards, Trend Arrows (UNICHAR), Conditional Formatting  
- Drill-through Analysis, Bookmarks, Interactive Dashboards  

**Power Query (M)**
- Folder Connector ETL Automation  
- Query Staging to Resolve `Formula.Firewall`  
- Dynamic Year Extraction for Irregular Data  

**DAX**
- `PERCENTILEX.INC()` for Median Calculations  
- YoY Change and Forecast Shift Measures  
- Inflation & FX Conversion Logic  

**Data Engineering**
- Modular ETL Workflow  
- Scalable File Management via Folder Connector  

**Tech Stack**
> Power BI Desktop • Power Query (M) • DAX • Excel/CSV • GitHub  

---

## 📊 **Results & Recommendations**

| Metric | Insight | Business Impact |
|---------|----------|----------------|
| **Baseload Prices** | GB (€67→€70) vs DE (€66→€81) | GB stabilizes faster, DE shows volatility — plan price hedging |
| **Capture Prices** | Solar PV (GB) €50→€62 ↑ ; Onshore Wind (DE) €53→€57 ↑ | Solar PV outperforms long-term |
| **Correlation** | Solar PV & Generation (–0.89), Wind (–0.82) | Higher generation = lower price → adjust PPA terms |
| **Forecast Shift** | Q3 2022 → Q1 2023 (+8% PV, +6% Wind) | Build internal forecast validation pipeline |

> 💡 *Recommendation:* Prioritize long-term **Solar PV investments post-2029** in GB and enhance DE’s **grid resilience** for wind expansion.

---

## 🔄 **Next Steps**

- 🌍 **Expand** to include France, Netherlands, and Spain  
- 🧠 **Integrate ML Forecasting** using Python or Azure ML  
- ⚙️ **Automate Refresh** with Power BI Service + Gateway  
- 🪞 **Scenario Simulations** using “What-If” parameters  
- 🧾 **Data Limitations:** Current inputs are analyst-based; integrating real-time market feeds will enhance accuracy  

---

## 📚 **Learning Highlights**

- Solved **Formula.Firewall** errors through staged queries  
- Created **modular ETL pipelines** with flexible file ingestion  
- Designed DAX-based **median capture price measures**  
- Delivered **executive-ready visuals** with dynamic storytelling  

---

## 🖼️ **Dashboard Preview**

![EU Power Market Forecast](./assets/EU%20Power%20Market%20Forecast.png)

[▶️ **View Full Interactive Dashboard (PDF)**](./Energy%20Project%20Dashboard.pdf)

---

## 🎨 **Project Presentation (PowerPoint)**

![Presentation1](./assets/EU%20Power%20Market%20Forecast%20Report%20.png)

[📂 **Open Full Presentation**](./Presentation1.pptx)

---

## 👤 **Author**

**Kuku Faruq Olabiyi**  
_Data Analytics | Power BI | Business Intelligence | Data Storytelling_  
📧 **kukuolabiyi04@gmail.com**  
💼 [LinkedIn](https://www.linkedin.com/in/faruqkukuolabiyi)  
🐙 [GitHub](https://github.com/iexcelwithdata)
