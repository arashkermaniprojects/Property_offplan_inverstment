# Dubai Real Estate Investment Analyzer

## Overview

This Python-based analytical tool processes transaction data from the **Dubai Land Department** to evaluate the profitability of off-plan property investments compared to resale values. The system helps investors identify promising opportunities in Dubai's dynamic real estate market.

## Features

### Data Processing Pipeline
- **Multi-source data integration**: Combines transaction records with:
  - Property area data
  - Market type classifications
  - Transaction groups
  - Procedure details
- **Off-plan identification**: Flags pre-construction purchases
- **Price delta calculation**: Computes value changes between initial purchase and resale

### Predictive Analytics
- **Random Forest Classifier** (79% accuracy) predicts:
  - Likelihood of profitable investments
  - Key factors influencing returns
- Feature importance analysis reveals what makes projects successful

### Visualization & Reporting
- Interactive distribution charts of price changes
- Top/bottom performer identification:
  - Best case: +4,297% returns
  - Worst case: -99% losses
- Statistical summaries:
  - Average gain: -6.72%
  - Median gain: -12.31%

## Data Sources

| File | Records | Description |
|------|---------|-------------|
| `Transactions.csv` | 1,475,500 | Core transaction data (46 attributes) |
| `Lkp_Areas.csv` | - | Geographic district information |
| `Lkp_Market_Types.csv` | - | Property classification data |
| `Lkp_Transaction_Groups.csv` | - | Transaction category definitions |
| `Lkp_Transaction_Procedures.csv` | - | Legal process details |

