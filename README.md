# 🏨 OYO Hotels — Revenue & Occupancy Analytics

A real-world case study Power BI project analyzing OYO's hotel performance across 15 Indian cities, 325 properties and 12 months of simulated data based on OYO's public business reports.

---

## 📊 Dashboard Preview
📄 [View Full Dashboard PDF](screenshots/oyo-dashboard.pdf)

---

## Business Context
OYO Rooms is India's largest hospitality company operating budget to premium hotels across 35+ cities. This project simulates the work of a BA in OYO's Revenue Management team — analyzing occupancy rates, RevPAR, and city-level performance to identify underperforming properties and recommend pricing strategies.

---

## Business Questions Answered
1. Which cities generate the most revenue for OYO?
2. What percentage of properties are meeting the 75% occupancy target?
3. Which property types have the highest RevPAR?
4. How does occupancy vary seasonally across cities?
5. Which cities have the highest cancellation rates?

---

## Key Insights
| # | Insight |
|---|---------|
| 1 | Mumbai leads revenue at ₹40M+ — Tier 1 cities drive 60%+ of total revenue |
| 2 | Only 36.78% of properties achieve High occupancy — 25% are Low performers |
| 3 | Goa has highest RevPAR despite fewer properties — premium seasonal pricing works |
| 4 | Average occupancy of 70.18% is below OYO's 75% target |
| 5 | 15.10% avg cancellation rate is high — needs dynamic pricing intervention |

---

## Tools & Stack
- **Power BI Desktop** — 3-page interactive dashboard
- **Power Query** — data transformation and calculated columns
- **DAX** — 6 business measures
- **Python (Pandas, NumPy)** — realistic dataset generation
- **Data simulated** based on OYO public reports and hospitality industry benchmarks

---

## DAX Measures
| Measure | Purpose |
|---------|---------|
| Total Revenue | SUM of all property revenue |
| Avg Occupancy Rate | Average occupancy % across properties |
| Avg RevPAR | Revenue Per Available Room |
| Avg Customer Rating | Average guest rating |
| Total Properties | Distinct property count |
| Avg Cancellation Rate | Average booking cancellation % |

---

## Dashboard Pages
| Page | Contents |
|------|---------|
| Executive Overview | KPI cards, revenue by city, occupancy distribution |
| City & Property Analysis | Property type performance, city comparisons |
| Seasonal Trends | Monthly patterns, peak seasons, Goa vs other cities |

---

## BA Deliverables
- 📄 [Business Requirements Document](docs/BRD.md)
- 📊 [Insights & Recommendations Report](docs/insights_report.md)

---

## Dataset
Simulated dataset of 3,900 records across 325 properties and 15 Indian cities — generated using Python based on OYO's public business reports and hospitality industry benchmarks.

---

## Author
**Lincy DCosta** — BE AI & Data Science, Fr. CRCE Mumbai  
[GitHub](https://github.com/lincy1405)