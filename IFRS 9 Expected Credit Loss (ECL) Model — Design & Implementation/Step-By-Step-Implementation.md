# Project 12: IFRS 9 Expected Credit Loss (ECL) Model — Design & Implementation

---

## 📌 Project Overview

| Field | Details |
|-------|---------|
| **Project Title** | IFRS 9 Expected Credit Loss (ECL) Model — Design & Implementation |
| **Role** | Team Leader / Team Member |
| **Duration** | 2019 – 2024 (Across Multiple Banking Engagements) |
| **Sector** | Commercial Banks & Development Banks |
| **Standard Applied** | IFRS 9 — Financial Instruments (Impairment) |
| **Scope** | ECL Model Design, Staging, PD/LGD/EAD Computation, Forward-Looking Adjustments |

---

## 🎯 Project Objective

IFRS 9 replaced the incurred loss model (IAS 39) with a forward-looking **Expected Credit Loss (ECL) model** — fundamentally changing how banks recognize and measure loan impairment. I designed and implemented Excel-based ECL models for multiple banks during Nepal's first-time IFRS adoption, computing ECL provisions across the entire loan portfolio.

> ⚠️ *Note: All institution-specific ECL parameters, portfolio data, and model outputs remain strictly confidential.*

---

## 🛠️ Step-by-Step: What I Did

---

### ✅ Step 1: Loan Portfolio Segmentation

- Segmented the entire loan portfolio into homogeneous groups for ECL computation:

#### 🔹 Segmentation Criteria:
- **By product type** — term loan, overdraft, housing, vehicle, SME, agriculture, personal, staff loan
- **By collateral type** — real estate, fixed deposit, gold, vehicle, unsecured
- **By sector** — manufacturing, trade, agriculture, services, real estate, consumer
- Created granular portfolio segments — each segment had similar credit risk characteristics

---

### ✅ Step 2: IFRS 9 Staging — 3-Stage Classification

- Classified every loan into IFRS 9 stages based on credit risk deterioration:

| Stage | Criteria | ECL Measurement |
|-------|----------|----------------|
| **Stage 1** | Performing — no significant increase in credit risk since origination | 12-month ECL |
| **Stage 2** | Significant increase in credit risk (SICR) but not credit-impaired | Lifetime ECL |
| **Stage 3** | Credit-impaired — objective evidence of impairment | Lifetime ECL |

#### 🔹 SICR (Significant Increase in Credit Risk) Criteria:

**Quantitative Indicators:**
- Days Past Due (DPD) > 30 days → Stage 2
- Days Past Due (DPD) > 90 days → Stage 3
- Significant decline in borrower's credit score/rating

**Qualitative Indicators:**
- Borrower financial deterioration
- Sector downturn or adverse market conditions
- Loan restructuring or forbearance
- Watch-list classification by credit committee
- Breach of loan covenants

---

### ✅ Step 3: Probability of Default (PD) Estimation

- Estimated PD for each portfolio segment:

#### 🔹 PD Types:
- **12-month PD** (for Stage 1) — probability of default within next 12 months
- **Lifetime PD** (for Stage 2 & 3) — probability of default over remaining loan life

#### 🔹 PD Estimation Methodology:

1. **Historical Default Analysis:**
   - Analyzed historical default data (5+ years)
   - Performed migration analysis / transition matrices
   - Computed historical default rates by segment, product, and risk grade

2. **PD Term Structure:**
   - Built PD curves showing cumulative default probability over time
   - Applied survival analysis techniques for lifetime PD estimation

3. **Point-in-Time (PIT) Adjustments:**
   - Converted long-run average (Through-the-Cycle) PD to current economic conditions
   - Applied macroeconomic overlays to reflect current credit environment

---

### ✅ Step 4: Loss Given Default (LGD) Estimation

- Estimated LGD for each portfolio segment:
- LGD = 1 – Recovery Rate


#### 🔹 LGD Estimation Factors:

**Historical Recovery Analysis:**
- Analyzed historical recovery data — actual recoveries from defaulted loans
- Computed average recovery rates by collateral type and segment

**Collateral Considerations:**
- Collateral type and realizable value
- Time to recovery — discounting future recoveries to present value
- Recovery costs — legal, auction, administrative costs
- Collateral haircuts — market value vs. forced sale value

#### 🔹 LGD by Collateral Type:

| Collateral Type | Typical LGD Range | Rationale |
|----------------|------------------|-----------|
| Fixed Deposit Secured | 0–5% | Near-certain recovery |
| Gold Secured | 10–25% | High liquidity, stable value |
| Real Estate Secured | 25–45% | Market volatility, liquidation time |
| Vehicle Secured | 40–60% | Rapid depreciation, resale uncertainty |
| Unsecured | 60–100% | No collateral backing |

---

### ✅ Step 5: Exposure at Default (EAD) Estimation

- Estimated EAD for each loan:

#### 🔹 EAD by Facility Type:

| Facility Type | EAD Formula |
|--------------|-------------|
| **Fully Drawn Term Loans** | EAD = Outstanding balance |
| **Revolving Facilities (Overdraft, Credit Lines)** | EAD = Drawn amount + (CCF × Undrawn commitment) |
| **Off-Balance Sheet Items (LC, BG)** | EAD = Notional amount × CCF |

#### 🔹 Credit Conversion Factor (CCF):
- Estimated based on historical drawdown behavior before default
- Analyzed pre-default utilization patterns for revolving facilities
- Applied segment-specific CCFs based on product type and borrower behavior

---

### ✅ Step 6: ECL Computation

- Computed ECL using the core formula:
- ECL = PD × LGD × EAD × Discount Factor


#### 🔹 Computation Approach:

| Stage | PD Used | ECL Horizon |
|-------|---------|-------------|
| **Stage 1** | 12-month PD | 12-month ECL |
| **Stage 2** | Lifetime PD | Lifetime ECL |
| **Stage 3** | Lifetime PD (100% default probability) | Lifetime ECL |

#### 🔹 Discounting:
- Applied discount factor using the loan's original **Effective Interest Rate (EIR)**
- Discounted future cash shortfalls to present value at reporting date

#### 🔹 Granularity:
- Computed ECL at **individual loan level** for large exposures
- Computed ECL at **portfolio level** for homogeneous small-balance segments

---

### ✅ Step 7: Forward-Looking Macroeconomic Adjustment

> Incorporating forward-looking information into ECL — a key IFRS 9 requirement

#### 🔹 Macroeconomic Variable Selection:
- Identified macroeconomic variables correlated with default rates:
  - GDP growth rate
  - Inflation rate
  - Unemployment indicators
  - Sectoral indicators (real estate prices, commodity prices)
  - Interest rate environment

#### 🔹 Multi-Scenario Approach:

| Scenario | Weight | Assumptions |
|----------|--------|-------------|
| **Base Case** | 50% | Most likely economic outcome based on central forecasts |
| **Optimistic** | 25% | Favorable economic conditions — higher growth, lower defaults |
| **Pessimistic** | 25% | Adverse economic conditions — recession, higher defaults |

#### 🔹 Probability-Weighted ECL:

-Probability-Weighted ECL = Σ (Scenario Weight × Scenario ECL)
= (50% × Base Case ECL) + (25% × Optimistic ECL) + (25% × Pessimistic ECL)


- Adjusted PD under each scenario using macroeconomic overlay models
- Computed scenario-specific ECL and aggregated using probability weights

---

### ✅ Step 8: ECL vs. NRB Regulatory Provision Comparison

- Compared IFRS 9 ECL provisions against NRB regulatory provisions:

#### 🔹 NRB Regulatory Provisioning Framework:

| Loan Classification | NRB Provision Rate |
|-------------------|-------------------|
| Pass | 1% |
| Watch List | 5% |
| Substandard | 25% |
| Doubtful | 50% |
| Loss | 100% |

#### 🔹 Higher-of Treatment:
- Applied **higher of treatment** as directed by NRB:
  - Computed IFRS 9 ECL provision
  - Computed NRB regulatory provision
  - Recognized the **higher amount** in financial statements
- Documented the comparison and variance analysis for auditor and regulatory review

#### 🔹 Reconciliation Schedule:
- IFRS 9 ECL Provision : NPR XX,XXX
- NRB Regulatory Provision : NPR XX,XXX
─────────────────────────────
- Provision Recognized (Higher) : NPR XX,XXX
- Variance (Disclosed in Notes) : NPR XX,XXX


---

### ✅ Step 9: ECL Model Documentation

- Prepared comprehensive ECL model documentation:

#### 📋 Documentation Components:

| Document | Purpose |
|----------|---------|
| **Model Methodology Document** | Explaining PD, LGD, EAD estimation, staging logic, forward-looking approach |
| **Data Sources & Assumptions Register** | Documenting data origins, quality checks, and key assumptions |
| **Sensitivity Analysis Report** | Impact of changing PD/LGD/macroeconomic assumptions on ECL output |
| **Model Limitations & Management Overlays** | Disclosing model constraints and expert judgment adjustments |
| **Governance & Approval Framework** | Model validation, approval process, and periodic review procedures |

- Documentation was:
  - Reviewed by **external auditors** during statutory audit
  - Presented to **Senior Management and Board** for approval
  - Maintained as part of the bank's **model risk management framework**

---

## 📊 Key Outcomes & Impact

| Outcome | Detail |
|---------|--------|
| **ECL Models Built** | Multiple Excel-based ECL models for commercial and development banks |
| **3-Stage Classification** | IFRS 9 staging framework implemented across all loan portfolios |
| **Forward-Looking** | 3-scenario macroeconomic adjustment incorporated into ECL estimates |
| **Regulatory Alignment** | ECL vs. NRB provision comparison with higher-of treatment applied |
| **Audit-Ready Documentation** | Complete ECL model documentation for auditor and regulatory review |
| **Technical Capacity** | Built internal capability for ongoing ECL computation and model maintenance |

---

## 🧰 Tools & Skills Applied

- **IFRS 9 Technical**: IFRS 9 Impairment, ECL Modeling, Probability of Default (PD), Loss Given Default (LGD), Exposure at Default (EAD), Staging (SICR)
- **Advanced Analytics**: Forward-Looking Adjustment, Macroeconomic Scenarios, Transition Matrix Analysis, Sensitivity Analysis
- **Financial Modeling**: Microsoft Excel (Advanced), Financial Modeling, Scenario Analysis, Discounted Cash Flow
- **Documentation & Governance**: Model Documentation, Audit Support, Regulatory Compliance, Board Reporting

---

## 🏷️ Tags

`#IFRS9` `#ECL` `#ExpectedCreditLoss` `#Impairment` `#CreditRisk` `#PD` `#LGD` `#EAD` `#ForwardLooking` `#BankingFinance` `#Nepal` `#ICAN` `#CAManishShrestha` `#CISA`

---

> *— CA Manish Shrestha, CISA®*  
> Chartered Accountant (ICAN) | Certified Information Systems Auditor (ISACA-USA)  
> 🌐 [camanishshrestha.com.np](https://www.camanishshrestha.com.np) | [GitHub](https://github.com/camanishshrestha) | [LinkedIn](https://www.linkedin.com/in/manish-shrestha-cisa-grc)
