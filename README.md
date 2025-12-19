# ⚡ EU Renewable Energy Market Intelligence  
**Decision Analytics | Energy Strategy | Automated Forecast Intelligence**

---

## 🔑 Executive Outcome

Designed an **automated market intelligence system** that enables energy strategy leaders to **compare renewable investment performance across countries and technologies**, replacing fragmented Excel forecasts with a **single decision-ready source of truth**.

**Impact:**
- Reduced forecast analysis turnaround time by **85%**
- Enabled side-by-side evaluation of **Solar PV vs Onshore Wind** investments in **Great Britain (GB)** and **Germany (DE)** across **2022–2050**
- Made forecast revisions and pricing volatility explicit inputs to long-term investment planning

**Primary Use Cases:**  
Capital allocation, PPA structuring, renewable portfolio strategy

---

## 🧠 Decision Problem

Energy strategy teams lacked clear visibility into:
- How **renewable capture prices evolve relative to baseload prices**
- Whether **forecast revisions materially change investment attractiveness**
- Which renewable technologies remain resilient under inflation and currency effects

As a result, **high-value investment decisions relied on inconsistent, manually prepared analyses**, increasing strategic and financial risk.

---

## 🎯 What I Owned

- Framed the **core analytical questions** guiding investment decisions:
  - Which renewable technology delivers superior long-term capture value?
  - How sensitive are forecasts to revision cycles?
  - Where does price volatility introduce strategic risk?
- Defined the **metric framework** used for executive evaluation
- Built a **fully automated analytics pipeline** to ensure repeatability and scalability

---

## 🧩 Analytical Approach

### Data Engineering
- Automated ingestion of multi-version forecast files using **Power Query Folder Connector**
- Normalized inconsistent structures, currencies, and time horizons

### Data Modeling
- Designed a **star schema** connecting Forecast, Country, and Technology dimensions
- Enabled consistent cross-version and cross-market comparison

### Decision Metrics (DAX)
- Median Capture Price (robust to outliers)
- Year-over-Year Growth (%)
- Forecast Shift (% change between versions)
- Baseload vs Capture Price spread
- Correlation between generation volume and pricing

### Visualization
- Executive-focused Power BI dashboard with trend indicators, slicers, and version comparisons
- Designed for **exploration and decision support**, not static reporting

---

## 📊 Key Findings

| Insight | Strategic Interpretation |
|------|---------------------------|
| **Solar PV (GB)** shows sustained capture price growth (€50 → €62) | Strong long-term investment candidate post-2029 |
| **Germany baseload prices** show higher volatility (€66 → €81) | Requires hedging and grid resilience planning |
| **Generation vs Price correlation (Solar PV: –0.89)** | Higher penetration suppresses prices → impacts PPA design |
| **Forecast revisions (+24% PV)** | Necessitates internal forecast validation pipeline |

---

## 🧭 Strategic Recommendations

- Prioritize **long-term Solar PV investments in Great Britain**
- Strengthen **forecast validation processes** before committing capital
- Incorporate **generation–price sensitivity** into pricing and contract models

---

## ⚙️ Scalability & Automation

- New forecast files integrate automatically with zero manual cleanup
- Metric definitions are reusable across countries and technologies
- Framework supports future **ML-based forecasting** and scenario simulations

---

## 🧠 What This Project Demonstrates

- Ownership of **ambiguous decision problems**
- Ability to design **repeatable analytical systems**
- Comfort operating at the intersection of **strategy, uncertainty, and data**

---

## 📊 Dashboard Preview

![EU Power Market Forecast](./assets/EU%20Power%20Market%20Forecast.png)

[▶️ View Interactive Dashboard (PDF)](./Energy%20Project%20Dashboard.pdf)

---

## 🎨 Executive Presentation

![Presentation Preview](./assets/Powerpoint%20Report.png)

[📂 Open Full Presentation](./assets/EU%20Report.pptx)

---

## 👤 Author

**Faruq Kuku Olabiyi**  
Decision Analytics | Power BI | Energy Strategy  
📧 kukuolabiyi04@gmail.com  
💼 [LinkedIn](https://www.linkedin.com/in/faruqkukuolabiyi)  
🐙 [GitHub](https://github.com/iexcelwithdata)
