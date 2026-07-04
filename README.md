# IFRS 9 Expected Credit Loss (ECL) Calculator

![Python](https://img.shields.io/badge/Python-3.8+-blue) ![IFRS9](https://img.shields.io/badge/IFRS9-Compliant-green) ![SAMA](https://img.shields.io/badge/SAMA-Regulatory%20Overlay-red) ![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)

## Overview
An IFRS 9 compliant ECL calculator built on a synthetic 1,000-loan portfolio.
Implements the three-stage impairment model with SAMA regulatory overlays,
sector concentration analysis, stress testing, and a Power BI dashboard —
aligned with GCC banking standards.

---

## Business Problem
Under IFRS 9, banks must provision for expected credit losses across their
entire loan portfolio — not just loans already in default. This project
automates that provisioning process, flags regulatory breaches against
SAMA minimum thresholds, and presents results in a risk committee ready dashboard.

---

## Methodology

```
Synthetic Loan Portfolio (1,000 loans)
           ↓
IFRS 9 Stage Assignment (DPD-based)
           ↓
PD Calculation (12-month vs Lifetime)
           ↓
ECL = PD × LGD × EAD
           ↓
SAMA Regulatory Overlay
           ↓
Sector Concentration Analysis
           ↓
Stress Testing (4 Scenarios)
           ↓
Power BI Dashboard + Excel Report
```

---

## Key Results

| Metric | Value |
|--------|-------|
| Total Portfolio EAD | $187.09M |
| Total ECL (Base Case) | $39.64M |
| SAMA Non-Compliant Loans | 32 |
| Additional Provision Required | $60,147.77 |
| Severe Stress ECL Increase | +31.74% |

---

## IFRS 9 Stage Distribution

| Stage | Loans | Total ECL |
|-------|-------|-----------|
| Stage 1 (Performing) | 592 | ~$8.5M |
| Stage 2 (Underperforming) | 258 | ~$16.7M |
| Stage 3 (Non-Performing) | 150 | ~$14.4M |

---

## Power BI Dashboard

### Page 1 — Portfolio Overview
- Total EAD: **$187.09M**
- Total ECL: **$39.64M**
- SAMA Flagged Loans: **32**
- ECL by Stage (bar chart)
- ECL by Sector (bar chart)

### Page 2 — Stress Testing

| Scenario | ECL Change |
|----------|------------|
| Base Case | 0% |
| Mild Stress (+20% PD) | +8.69% |
| Moderate Stress (+50% PD) | +18.20% |
| Severe Stress (+100% PD) | +31.74% |

### Page 3 — SAMA Flags
- 32 non-compliant loans
- Columns: Loan ID, Stage, ECL Provision, SAMA Minimum, Shortfall
- Sorted by highest shortfall first

---

## Sector Concentration

| Sector | ECL Rate |
|--------|----------|
| Services | 23.38% |
| Government | 22.71% |
| Retail | 21.05% |
| Manufacturing | 20.36% |
| Real Estate | 18.93% |

---

## Stress Testing Results

| Scenario | Total ECL | ECL Change |
|----------|-----------|------------|
| Base Case | $39.64M | — |
| Mild Stress | $43.08M | +8.69% |
| Moderate Stress | $46.85M | +18.20% |
| Severe Stress | $52.22M | +31.74% |

---

## Regulatory Framework
- **IFRS 9** — Three-stage impairment model
- **SAMA** — Saudi Central Bank minimum provision requirements (1%/5%/20%)
- **CBUAE** — UAE Central Bank provisioning guidelines

---

## Project Structure

```
ifrs9-ecl-calculator/
├── notebooks/
│   └── 01_ecl_calculator.ipynb
├── outputs/
│   ├── ecl_by_stage.png
│   ├── ecl_by_sector.png
│   ├── stress_testing.png
│   ├── ecl_report.xlsx
│   └── ifrs9_dashboard.pdf
├── risk_committee_summary.md
├── requirements.txt
└── README.md
```

---

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, OpenPyXL, Power BI
