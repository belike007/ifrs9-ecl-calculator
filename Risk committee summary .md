\# IFRS 9 ECL Calculator — Risk Committee Summary



\## Objective

Calculate Expected Credit Loss (ECL) provisions on a synthetic 1,000-loan portfolio

under the IFRS 9 three-stage impairment framework, aligned with SAMA regulatory guidelines.



\---



\## Methodology



\- Portfolio: 1,000 synthetic loans across 5 sectors and 4 loan types

\- Stage Assignment: Based on Days Past Due (DPD)

\- ECL Formula: PD × LGD × EAD

\- PD Approach: 12-month PD for Stage 1, Lifetime PD for Stage 2/3

\- Regulatory Overlay: SAMA minimum provision thresholds applied



\---



\## Stage Distribution



| Stage | Loans | Description |

|-------|-------|-------------|

| Stage 1 | 592 | Performing — 12-month ECL |

| Stage 2 | 258 | Underperforming — Lifetime ECL |

| Stage 3 | 150 | Non-Performing — Lifetime ECL (PD = 100%) |



\---



\## ECL Results



| Stage | Total EAD ($) | Total ECL ($) | Avg PD | Avg LGD |

|-------|--------------|--------------|--------|---------|

| Stage 1 | 108,497,700 | 8,487,168 | 15% | 50% |

| Stage 2 | 50,115,880 | 16,725,717 | 70% | 47% |

| Stage 3 | 28,479,360 | 14,427,940 | 100% | 51% |

| \*\*Total\*\* | \*\*187,092,940\*\* | \*\*39,640,825\*\* | — | — |



\---



\## SAMA Regulatory Flags



\- Loans below SAMA minimum provision: \*\*32\*\*

\- Additional provision required: \*\*$60,147.77\*\*

\- Action: Immediate top-up required to maintain regulatory compliance



\---



\## Sector Concentration



| Sector | ECL Rate |

|--------|----------|

| Services | 23.38% |

| Government | 22.71% |

| Retail | 21.05% |

| Manufacturing | 20.36% |

| Real Estate | 18.93% |



Services sector carries highest ECL rate — monitor for concentration risk.



\---



\## Stress Testing Results



| Scenario | Total ECL ($) | ECL Change |

|----------|--------------|------------|

| Base Case | 39,640,825 | — |

| Mild Stress (+20% PD) | 43,084,059 | +8.69% |

| Moderate Stress (+50% PD) | 46,853,915 | +18.20% |

| Severe Stress (+100% PD) | 52,221,499 | +31.74% |



\---



\## Business Recommendation

Under severe stress, ECL increases by 31.74% — the bank must maintain

adequate capital buffers to absorb this shock. Immediate remediation

required for 32 SAMA non-compliant loans. Services sector concentration

should be monitored quarterly.



\---



\## Limitations

\- Synthetic portfolio — real deployment requires internal loan data

\- LGD assumed static — should be collateral-adjusted in production

\- PD not forward-looking — macroeconomic overlays recommended per IFRS 9

