# Credit Portfolio Stress Testing Under Macroeconomic Scenarios

## Overview

This project builds a **portfolio-level credit risk stress testing framework**
using historical loan-level data and macroeconomic scenario analysis.

The work focuses on:
- Constructing a realistic retail credit portfolio
- Estimating baseline defaults and losses
- Stressing portfolio losses under adverse macroeconomic conditions
- Decomposing loss amplification by credit quality
- Extending the framework across geographies (US → India)

The goal is to demonstrate how **macro stress testing frameworks** used by banks
and risk teams can be implemented using public data while remaining interpretable
and decision-relevant.

---

## Notebook Summaries

### 01 — Portfolio Construction (LendingClub)

- Built a large-scale retail credit portfolio using historical LendingClub
  loan-level data (2007–2018)
- Defined defaults, recoveries, exposure, and realized losses
- Analyzed portfolio risk across:
  - Credit grades
  - Loan terms
  - Loan purposes
- Established baseline default and loss rates

**Outcome:**  
A realistic, well-stratified credit portfolio suitable for stress testing.

---

### 02 — US Macroeconomic Stress Framework (FRED)

- Integrated US macroeconomic indicators from FRED:
  - Unemployment rate
  - Fed Funds rate
  - Real GDP
  - CPI
  - Yield curve spread
- Defined baseline, adverse, and severe macroeconomic scenarios
- Converted scenarios into relative macro shock multipliers

**Outcome:**  
A transparent scenario-based macro stress framework aligned with regulatory
stress testing practices.

---

### 03 — Portfolio Loss Amplification Analysis

- Applied macro shock multipliers to baseline portfolio losses
- Modeled loss amplification under adverse and severe scenarios
- Decomposed stressed losses by credit grade
- Analyzed:
  - Incremental losses
  - Loss concentration shifts
  - Portfolio loss distribution under stress

**Outcome:**  
Clear attribution of how macroeconomic stress propagates through different
credit risk segments.

---

### 04 — India Macro Extension (World Bank + RBI)

- Extended the stress-testing framework to India using:
  - World Bank indicators (GDP growth, inflation, unemployment)
  - RBI policy repo rates as a monetary transmission proxy
- Constructed India-specific macro stress scenarios
- Compared stress intensity between US and India scenarios

**Outcome:**  
Demonstrated that portfolio stress-testing frameworks are portable across
geographies, even under constrained data environments.

---

## Key Insights

- Portfolio losses respond non-linearly to macroeconomic stress
- Credit quality strongly determines loss amplification under stress
- Monetary tightening acts as a powerful amplifier of credit losses
- Scenario design is more important than model complexity
- Stress-testing frameworks can be adapted to emerging markets using
  limited but robust macro indicators

---

## Methodological Principles

- Portfolio-level analysis over individual loan prediction
- Scenario-based stress testing instead of point forecasting
- Interpretability and economic reasoning over black-box optimization
- Conservative assumptions aligned with risk management practices

---

## Technologies Used

- Python (pandas, numpy)
- Macroeconomic data (FRED, World Bank, RBI)
- Data visualization (matplotlib, seaborn)

---

## Why This Project Matters

Banks and financial institutions rely on stress testing to assess resilience
under adverse economic conditions. This project demonstrates how such frameworks
can be built using public data while preserving economic intuition, transparency,
and practical relevance.

---

## Repository

GitHub:  
https://github.com/sainihimanshu1999/credit-portfolio-stress-testing