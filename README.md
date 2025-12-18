# APRA-Banking-System-Analytics
End-to-end analysis of the Australian banking system using APRA data, focusing on balance sheet structure, funding dynamics, and institutional comparison via Power BI.

# APRA Banking System Analytics (Power BI)

## Overview
This project analyses the Australian banking system using publicly available APRA monthly statistics.

The dashboard focuses on:
- balance sheet scale
- funding dynamics
- institutional concentration
- loan portfolio structure

across time and institutions. Risk and asset quality metrics were intentionally excluded to maintain analytical clarity and focus on balance sheet structure.

The project demonstrates end-to-end finance analytics capability, from data modelling and KPI design to executive-level insight generation.

---

## Business Questions
- How has the size of the Australian banking system evolved over time?
- Is lending growth supported by stable funding growth?
- How concentrated is the system across major institutions?
- How do funding profiles and loan portfolios differ across banks?
- How does an individual bank evolve relative to system trends?

---

## Dashboard Structure

### Page 1 — System Overview
**Summary:**  
The dashboard shows a system transitioning from growth to consolidation, with lending constrained by funding availability and persistent housing concentration.

**Key insights:**
- System asset growth is slowing amid tighter credit conditions  
- Loan expansion is increasingly constrained by deposit growth  
- Housing remains the dominant exposure across the system  
- Funding gaps remain contained, indicating conservative liquidity management  

---

### Page 2 — Institution Comparison
**Summary:**  
Page 2 shows a highly concentrated banking system where large institutions benefit from scale and stable funding, while smaller banks exhibit more diverse funding profiles and loan portfolio strategies.

**Key insights:**
- System assets are concentrated among a small number of large institutions  
- Larger banks show more balanced loan-to-deposit profiles  
- Funding strategies vary meaningfully even among similarly sized banks  
- Loan portfolio composition reflects distinct strategic positioning  

Users can drill through from this page to view institution-level trends.

---

### Page 3 — Bank Deep Dive
**Summary:**  
Page 3 provides an institution-level time-series view of balance sheet growth, funding alignment, and portfolio structure.

**Interpretation guidance:**
- Alignment between loan and deposit growth indicates funding discipline  
- Divergence may signal increased liquidity risk  
- Portfolio stability suggests incremental strategy rather than abrupt repositioning  
- Trends should be interpreted relative to system conditions and peers  

---

## Key KPIs Implemented
A deliberately limited and consistent core KPI set is used across all pages:

- **Scale:** Total Assets, Total Loans, Total Deposits  
- **Growth:** Loan Growth (YoY), Deposit Growth (YoY)  
- **Funding:** Loan-to-Deposit Ratio, Funding Gap  
- **Composition:** Housing, Business, and Other Loan Shares  

The same measures are reused across system, peer, and institution-level views to ensure comparability.

---

## Data & Methodology
- **Source:** APRA Monthly Authorised Deposit-taking Institution Statistics  
- **Period:** March 2019 – October 2025  
- **Granularity:** One record per institution per month (resident-only)

The data model follows a star schema with separate Date, Institution, and Financial fact tables. Metrics are used as reported by APRA to avoid reconciliation issues arising from definitional changes over time.

---

## Assumptions & Limitations
- On-balance-sheet data only  
- No adjustment for mergers, restructures, or accounting changes  
- Analysis is descriptive, not predictive  
- Interpretations depend on selected institution and reporting period  

---

## Documentation

- 📄 **Executive Insights Report:**  
  [APRA_Banking_System_Insights_Report.pdf](APRA_Banking_System_Insights_Report.pdf)

- 📘 **Data Model Design:**  
  [Data Model Document.pdf](Doc/Data%20Model%20Document.pdf)

---

## Tools Used
- Power BI (DAX, data modelling, visualisation)
- SQL
- Python (optional data preparation)
- Excel
