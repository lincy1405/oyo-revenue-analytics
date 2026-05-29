# Business Requirements Document (BRD)
## OYO Hotels — Revenue & Occupancy Analytics

**Document Version:** 1.0  
**Prepared By:** Lincy DCosta  
**Date:** May 2026  
**Status:** Final

---

## 1. Project Overview
This project analyzes OYO's hotel performance across 15 Indian cities to evaluate occupancy rates, revenue per available room (RevPAR), and property-level performance. The goal is to identify underperforming properties and recommend data-driven pricing and operational strategies.

---

## 2. Business Objectives
- Monitor occupancy performance against OYO's 75% target
- Identify top and bottom performing cities and properties
- Analyze seasonal demand patterns across cities
- Recommend pricing strategies to improve RevPAR
- Reduce cancellation rates through targeted interventions

---

## 3. Stakeholders
| Stakeholder | Role | Interest |
|-------------|------|----------|
| Revenue Manager | Primary User | RevPAR, pricing optimization |
| City Operations Head | Primary User | City-level occupancy performance |
| Property Managers | Secondary User | Individual property metrics |
| CFO | Secondary User | Overall revenue and profitability |

---

## 4. Scope
**In Scope:**
- 325 properties across 15 Indian cities
- 12 months of occupancy and revenue data
- City tier analysis (Tier 1, 2, 3)
- Property type performance (OYO Rooms, Townhouse, Flagship, Capital O, Palette)
- Seasonal trend analysis

**Out of Scope:**
- Individual booking level analysis
- Customer demographics
- Competitor benchmarking
- Real-time data integration

---

## 5. Functional Requirements
| ID | Requirement |
|----|-------------|
| FR1 | Dashboard shall display Total Revenue, Avg Occupancy, RevPAR, Rating, Properties and Cancellation Rate as KPIs |
| FR2 | System shall classify properties as High, Medium or Low occupancy |
| FR3 | System shall show revenue and occupancy by city |
| FR4 | System shall analyze performance by property type |
| FR5 | System shall show monthly seasonal trends |
| FR6 | System shall allow filtering by City Tier and Property Type |

---

## 6. Non-Functional Requirements
| ID | Requirement |
|----|-------------|
| NFR1 | Dashboard shall be interactive with cross-filtering |
| NFR2 | All DAX measures shall be reusable across pages |
| NFR3 | Report shall be exportable as PDF |
| NFR4 | Dataset shall be reproducible via Python script |

---

## 7. Data Requirements
| Field | Type | Description |
|-------|------|-------------|
| Property_ID | Text | Unique property identifier |
| City | Text | City where property is located |
| City_Tier | Integer | 1 = Metro, 2 = Tier 2, 3 = Tier 3 |
| Property_Type | Text | OYO Rooms, Townhouse, Flagship etc |
| Total_Rooms | Integer | Number of rooms in property |
| Base_Price | Float | Base room price in INR |
| Month | Text | Month of performance data |
| Occupancy_Rate | Float | % of rooms occupied |
| Revenue | Float | Total monthly revenue |
| RevPAR | Float | Revenue per available room |
| Customer_Rating | Float | Average guest rating (1-5) |
| Cancellation_Rate | Float | % of bookings cancelled |
| Occupancy_Status | Text | High/Medium/Low classification |

---

## 8. Assumptions & Constraints
- Data is simulated based on OYO public reports and hospitality benchmarks
- High occupancy = 75%+, Medium = 50-74%, Low = below 50%
- All revenue figures are in Indian Rupees (INR)
- Seasonal factors are based on Indian travel patterns