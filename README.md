# Supply-chain-insights
---

This case focused on identifying the root causes of delivery delays and service level degradation. The goal is to understand why Lead Time increased, OTD dropped, and where operational improvements can be made.

The project covers data cleaning, exploratory analysis, hypothesis testing, and actionable business recommendations.

**Stack:** Python · pandas  · matplotlib · seaborn

---

## Project Overview

The company is a mid-sized e-commerce business operating in Slovakia, Czechia, Hungary, and Poland.
It manages two warehouses and processes around 2,200 orders per month.

Reported issues:

* increasing number of delays
* growing Lead Time
* declining On-Time Delivery (OTD) and SLA
* logistics costs remain relatively stable

---

## What was done

**1. Data Preparation**
Loaded and cleaned the dataset, fixed date formats, checked for missing values and duplicates.
Lead Time was recalculated due to inconsistencies in the original metric.

**2. Exploratory Data Analysis (EDA)**

* distributions of key metrics (Lead Time, shipping cost, revenue, etc.)
* breakdown by warehouse, route, and country
* comparison before and after the critical date
* identification of trends and anomalies

**3. Operational Analysis**

* Lead Time trends over time
* SLA and OTD comparison before vs after changes
* analysis across combinations: warehouse × route × country × category
* search for operational bottlenecks

**4. Hypothesis Testing**

Three main hypotheses were tested:

* **H1:** Lead Time increased after January 15, 2025, causing OTD decline
* **H2:** A small number of operational combinations drive most delays
* **H3:** The issue is caused by a system-level external factor (process change, vendor, etc.)

**Result:**

* Lead Time increased after January 15
* OTD and SLA declined
* the deterioration affected all segments uniformly
* no specific bottleneck was identified

This indicates a **system-wide issue**, not a localized problem.

---

## Key Findings

| Area        | Finding                               |
| ----------- | ------------------------------------- |
| SLA / OTD   | Consistent decline after Jan 15, 2025 |
| Lead Time   | Increased across all segments         |
| Bottlenecks | No localized bottleneck detected      |
| Issue Type  | Systemic operational degradation      |

---

## Financial Insights

The analysis also revealed profitability issues in certain orders:

* Orders with 1–2 items are rarely profitable
* Orders with 4–6 items have a much higher chance of being profitable
* Even larger orders can be unprofitable if unit price is low
* The main driver is the high share of fixed and logistics costs

**Profitability depends on a combination of:**

* order size
* average price per unit
* cost structure

Increasing average order value is more important than simply increasing item count.

---

## Recommendations

**1. Operations**

* review staffing changes after January 15
* reassess cut-off times
* validate any SLA policy changes
* check for system overload or IT issues (OMS/WMS)

**2. Order Strategy**

* limit discounts for low-volume orders
* introduce a minimum order value for discounts
* apply delivery fees or surcharges for small orders

**3. Increase Average Order Value**

* bundle offers
* cross-selling
* incentives like “add one more item for free shipping”

**4. Cost Structure**

* revisit fixed cost allocation
* shift part of fixed costs toward variable where possible

---

## Conclusion

The performance degradation is systemic rather than localized.
The primary focus should be on identifying operational or process changes introduced after January 15.

At the same time, there is a clear opportunity to improve profitability through better order structure and cost management.
