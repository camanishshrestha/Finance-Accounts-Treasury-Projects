# Project 12: IFRS 9 Expected Credit Loss (ECL) Model — Design & Implementation

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project Title** | IFRS 9 Expected Credit Loss (ECL) Model — Design & Implementation |
| **Role** | Team Leader / Team Member |
| **Duration** | 2019 – 2024 (Across Multiple Banking Engagements) |
| **Sector** | Commercial Banks & Development Banks |
| **Standard Applied** | IFRS 9 — Financial Instruments (Impairment) |
| **Scope** | ECL Model Design, Staging, PD/LGD/EAD Computation, Forward-Looking Adjustments |

---

## 🎯 Project Objective

IFRS 9 introduced a **forward-looking Expected Credit Loss (ECL) model**, replacing the incurred loss model.

Role:
- Designed **Excel-based ECL models**
- Computed provisions across entire loan portfolios
- Supported **first-time IFRS adoption in Nepal**

> ⚠️ Confidential: Only methodology and framework described.

---

## 🛠️ Key Work (Simplified)

### 1. Loan Portfolio Segmentation
- By product: term loan, OD, housing, SME, etc.
- By collateral: real estate, FD, gold, unsecured
- By sector: manufacturing, trade, agriculture, services
- Created **homogeneous risk groups**

---

### 2. IFRS 9 Staging

| Stage | Criteria | ECL Type |
|---|---|---|
| **Stage 1** | Performing | 12-month ECL |
| **Stage 2** | SICR | Lifetime ECL |
| **Stage 3** | Credit-impaired | Lifetime ECL |

**SICR Triggers:**
- Quantitative: DPD >30 → Stage 2, >90 → Stage 3
- Qualitative: restructuring, sector risk, financial stress

---

### 3. Probability of Default (PD)
- 12-month PD (Stage 1)
- Lifetime PD (Stage 2 & 3)

Method:
- Historical data (5+ years)
- Transition matrices
- PD curves (term structure)
- PIT adjustments (current conditions)

---

### 4. Loss Given Default (LGD)

- Formula: **LGD = 1 – Recovery Rate**
- Based on:
  - Collateral value
  - Recovery time (discounted)
  - Recovery costs

**By type:**
- Secured → Low LGD  
- FD-backed → Near zero  
- Unsecured → High LGD  

---

### 5. Exposure at Default (EAD)

- Term loans → Outstanding balance  
- OD/limits → Drawn + (CCF × Undrawn)  
- Off-balance → Notional × CCF  

---

### 6. ECL Computation
- ECL = PD × LGD × EAD × Discount Factor


- Stage 1 → 12-month PD  
- Stage 2 & 3 → Lifetime PD  
- Discounted using **EIR**  
- Loan-level + portfolio-level computation  

---

### 7. Forward-Looking Adjustment

**Macroeconomic factors:**
- GDP
- Inflation
- Sector indicators

**Scenarios:**

| Scenario | Weight |
|---|---|
| Base | 50% |
| Optimistic | 25% |
| Pessimistic | 25% |

- Final ECL = Probability-weighted outcome

---

### 8. IFRS vs NRB Provision

- Compared with NRB provisioning:
  - Pass 1%, Watch 5%, Sub 25%, Doubtful 50%, Loss 100%
- Applied **higher-of rule**
- Documented variance

---

### 9. Model Documentation

- Methodology (PD, LGD, EAD)
- Assumptions & data sources
- Sensitivity analysis
- Model limitations
- Governance & approval

---

## 📊 Key Outcomes

- ECL models implemented across multiple banks
- Full IFRS 9 staging applied
- Forward-looking macro overlay integrated
- Regulatory alignment with NRB achieved
- Audit-ready documentation delivered

---

## 🧰 Tools & Skills

`IFRS 9`  
`ECL Modeling`  
`PD / LGD / EAD`  
`Staging (SICR)`  
`Macroeconomic Modeling`  
`Transition Matrix`  
`Financial Modeling (Excel)`  

---

## 🏷️ Tags

`#IFRS9` `#ECL` `#CreditRisk` `#PD` `#LGD` `#EAD` `#Banking`

---
