# Project 10: Tax Compliance, TDS Reconciliation & Payroll Management — Banking Sector

---

## 📌 Project Overview

| Field | Details |
|-------|---------|
| **Project Title** | Tax Compliance, TDS Reconciliation & Payroll Management — Banking Sector |
| **Role** | Junior Officer — Finance Department (Second-in-Command / Acting HOD) |
| **Duration** | 2022 – 2025 (Across Two Development Banks) |
| **Sector** | Development Banking — Tax Compliance, Payroll Processing & Regulatory Filing |
| **Regulatory Framework** | Income Tax Act 2058, NRB Directives, Social Security Fund Act, Labor Act 2074 |
| **Scope** | TDS Management, Corporate Tax, Payroll Processing, Tax Return Filing, Tax Reconciliation |

---

## 🎯 Project Objective

Tax compliance in the banking sector is an **extraordinarily complex function** — banks are simultaneously **taxpayers** (paying corporate income tax on profits) and **tax collectors** (deducting and remitting TDS on interest payments, salaries, contractors, and commissions on behalf of the government). A single error in TDS computation, untimely remittance, or incorrect tax return filing can result in **penalties, interest charges, and regulatory scrutiny from the Inland Revenue Department (IRD)**. As the officer responsible for tax compliance and payroll management, I ensured the bank's **complete and accurate compliance** across all tax obligations — from monthly TDS remittance to annual corporate tax return filing.

> ⚠️ *Note: All institution-specific tax computations, salary structures, and internal financial data remain strictly confidential. Only general methodologies, processes, and frameworks are described here.*

---

## 🏦 Institutions

| Institution | Period | Role |
|-------------|--------|------|
| **Lumbini Bikas Bank Ltd** | 2022 – 2024 | Tax Compliance & Payroll — Finance Department |
| **Garima Bikas Bank Ltd** | 2024 – 2025 | Tax Compliance & Payroll — Finance Department |

---

## 🛠️ Step-by-Step: What I Did

---

### ✅ Step 1: Understanding the Tax Compliance Framework for BFIs

- Mapped the **complete tax compliance universe** applicable to the bank:

#### 📋 Tax Compliance Obligations Map

| Tax Type | Obligation | Frequency | Governing Law |
|----------|------------|-----------|--------------|
| **Corporate Income Tax** | Tax on bank's net taxable profit | Annual (with quarterly advance) | Income Tax Act 2058 |
| **TDS — Deposit Interest** | TDS on interest paid to depositors | Per interest payment cycle | Income Tax Act 2058, Sec. 88 |
| **TDS — Employee Salary** | TDS on staff salaries and allowances | Monthly | Income Tax Act 2058, Sec. 87 |
| **TDS — Contractors/Vendors** | TDS on payments to contractors and service providers | Per payment | Income Tax Act 2058, Sec. 87A |
| **TDS — Rent** | TDS on rental payments | Per payment | Income Tax Act 2058 |
| **TDS — Debenture Interest** | TDS on interest payments to debenture holders | Per coupon payment | Income Tax Act 2058 |
| **TDS — Dividend** | TDS on dividend distributions to shareholders | Per dividend payment | Income Tax Act 2058 |
| **TDS — Commission/Fees** | TDS on commission, professional fees, consultancy | Per payment | Income Tax Act 2058 |
| **Social Security Fund (SSF)** | Employer and employee SSF contributions | Monthly | Social Security Fund Act |
| **VAT (on specific services)** | VAT on certain fee-based services (if applicable) | Monthly | VAT Act |

- Prepared a **tax compliance calendar** — a master tracker with:
  - Tax type and description
  - Due date (monthly / quarterly / annual)
  - Responsible person (maker / checker)
  - Filing method (IRD Portal / Manual)
  - Payment method (bank transfer to IRD)
  - Status tracker (Computed / Verified / Filed / Paid)
- This calendar ensured **zero missed tax deadlines** — preventing penalties and interest

---

### ✅ Step 2: TDS on Deposit Interest — Computation & Management

- Managed the **most voluminous TDS obligation** — TDS on interest paid to depositors:

#### 📊 TDS on Deposit Interest — Process

##### Scope of TDS on Interest
- TDS was required on interest paid/credited on:
  - **Fixed Deposits** — interest credited at maturity or periodically
  - **Savings Accounts** — interest credited quarterly or semi-annually
  - **Call Deposits** — interest credited as per terms
  - **Recurring Deposits** — interest component at maturity
  - **Any other interest-bearing deposit products**
- TDS rates as prescribed by **Income Tax Act 2058**:
  - Natural persons (individuals): prescribed rate (typically 5%)
  - Entities / corporates: prescribed rate (typically 15%)
  - Tax-exempt entities: Nil (with IRD exemption certificate)
  - Non-resident depositors: applicable withholding rate

##### TDS Computation Process
- After every interest crediting cycle in CBS:
  - Extracted **interest credited report** from Core Banking System (Pumori / Finacle)
  - Report included: Account number, depositor name, PAN, interest amount, TDS amount, net interest credited
  - Verified **TDS computation accuracy**:
    - TDS rate applied correctly based on depositor type (individual / entity)
    - PAN/non-PAN rate differential applied correctly
    - Tax-exempt depositors correctly excluded from TDS
    - Threshold exemptions applied correctly (if applicable)
  - Identified and corrected any **CBS computation errors** — system sometimes had edge cases requiring manual correction:
    - Joint accounts with different PAN status
    - Minor accounts linked to guardian PAN
    - Institutional accounts with exemption certificates
    - NRN (Non-Resident Nepali) account special tax treatment
  - Reconciled **total TDS computed** against **total interest expense** — the ratio should match expected TDS rate

##### TDS Remittance
- After verification, remitted TDS to IRD:
  - Prepared **TDS remittance challan** (payment voucher to IRD)
  - Transferred TDS amount from bank's account to **IRD's designated revenue account**
  - Filed **monthly TDS return** with IRD disclosing:
    - Total interest paid/credited during the month
    - Total TDS deducted
    - Total TDS remitted
    - Date of remittance
    - Challan reference number
  - Maintained **TDS remittance records** — challans, bank payment receipts, filing acknowledgments
  - Ensured TDS was remitted within **IRD prescribed deadline** (typically by 25th of following month)

---

### ✅ Step 3: TDS on Employee Salary — Payroll Tax Management

- Managed **TDS computation on employee salaries** — one of the most complex TDS categories due to progressive tax slabs and multiple salary components:

#### 📊 Salary TDS Computation Process

##### Step 3.1: Annual Taxable Salary Estimation
- At the beginning of each fiscal year, estimated **annual taxable salary** for each employee:

**Gross Salary Components:**
- Basic salary
- Grade allowance
- Dearness allowance
- Other fixed allowances (communication, fuel, entertainment)
- Festival allowance (Dashain allowance — 1 month basic)
- Leave encashment (estimated taxable portion)
- Performance bonus (estimated)

**Tax-Exempt Components (excluded):**
- Provident Fund (PF) — employer contribution (within prescribed limits)
- Gratuity (within prescribed limits)
- Social Security Fund (SSF) — within limits
- Medical insurance premium (within prescribed limits)
- Remote area allowance (if applicable)
- Retirement benefits within exempt limits

##### Taxable Income = Gross Salary – Exempt Deductions


##### Step 3.2: Tax Slab Application
- Applied **progressive income tax slabs** as prescribed by Finance Act for the relevant fiscal year:

| Taxable Income Slab | Tax Rate |
|---------------------|----------|
| Up to NPR X (First slab) | 1% (Social Security Tax) |
| NPR X to NPR Y | 10% |
| NPR Y to NPR Z | 20% |
| NPR Z to NPR W | 30% |
| Above NPR W | 36% |

- Applied **differential tax treatment** for:
  - Single vs. married employees (different slab thresholds)
  - Female employees (reduced rate for certain slabs in some fiscal years)
  - Disabled employees (special provisions)
  - Non-resident employees (flat rate)

##### Step 3.3: Monthly TDS Deduction
- Computed **monthly TDS amount** = Annual estimated tax ÷ 12 (or remaining months)
- Adjusted monthly TDS for:
  - Actual bonus payments received (when bonus is confirmed)
  - Salary revisions during the year
  - Overtime and additional allowances
  - Investment declarations for tax relief (insurance premium, donations)
  - Any tax paid by employee directly (advance tax)
- Ensured **monthly TDS deduction was smooth** — avoiding large year-end adjustments

##### Step 3.4: Year-End Tax Finalization
- At fiscal year-end:
  - Computed **actual taxable salary** based on full-year actual payments
  - Computed **actual annual tax liability** for each employee
  - Compared **total TDS deducted during the year** against actual liability
  - Adjusted final month's TDS for any **shortfall or excess**:
    - Shortfall: additional TDS deducted in final month
    - Excess: TDS refunded or adjusted

---

### ✅ Step 4: Salary Posting & Payroll Processing

- Managed the **monthly payroll processing** for the bank:

#### 📊 Payroll Processing Workflow

| Step | Activity | Details |
|------|----------|---------|
| **1** | HR Data Collection | Received employee attendance, leave records, new joinings, resignations, transfers from HR |
| **2** | Salary Computation | Computed gross salary for each employee — basic + allowances + OT + adjustments |
| **3** | Deduction Computation | Computed deductions — TDS, PF (employee share), SSF (employee share), loan EMIs, advances, other deductions |
| **4** | Net Salary Computation | Net Salary = Gross Salary – Total Deductions |
| **5** | Salary Register Preparation | Prepared comprehensive salary register with employee-wise breakup |
| **6** | Verification & Approval | Cross-verified salary register with HR records; obtained HOD/CEO approval |
| **7** | Salary Posting in CBS | Posted salary entries in Core Banking System — crediting each employee's bank account |
| **8** | Accounting Entries | Recorded salary expense, TDS liability, PF liability, SSF liability in General Ledger |
| **9** | TDS Remittance | Remitted salary TDS to IRD within prescribed deadline |
| **10** | PF/SSF Remittance | Remitted PF and SSF contributions (both employer and employee portions) |
| **11** | Pay Slip Distribution | Generated and distributed individual pay slips to employees |
| **12** | Reconciliation | Reconciled total salary debits with individual credits + deduction liabilities |

- Handled **special payroll events**:
  - **Dashain Allowance** — festival bonus computation and TDS treatment
  - **Performance Bonus** — annual bonus computation, Board approval, TDS deduction, payment processing
  - **Gratuity Settlement** — computation for departing employees, tax treatment, payment
  - **Leave Encashment** — accumulated leave computation, taxable treatment, payment
  - **Final Settlement** — full and final settlement for resigning/retiring employees including:
    - Remaining salary
    - Leave encashment
    - Gratuity
    - PF withdrawal
    - Loan adjustment
    - TDS finalization

---

### ✅ Step 5: TDS on Contractors, Vendors & Professional Services

- Managed TDS on **all non-salary payments** requiring tax deduction:

#### 📊 Vendor/Contractor TDS Categories

| Payment Type | TDS Rate | Examples |
|--------------|----------|----------|
| **Contractor Payments** | 1.5% (individual) / 1.5% (entity) | Construction, renovation, maintenance contracts |
| **Rent Payments** | 10% (individual) / 10% (entity) | Office rent, branch rent, warehouse rent |
| **Professional Fees** | 15% | Audit fees, legal fees, consultancy, valuation fees |
| **Commission Payments** | 15% | Insurance commission, agent commission |
| **Service Payments** | 1.5% | Security services, cleaning, catering |
| **Vehicle Hire** | 1.5% | Vehicle rental, transport services |

- For every qualifying payment:
  - Verified **vendor PAN** — higher TDS rate for payments without PAN
  - Computed **TDS amount** at prescribed rate
  - Deducted TDS from **gross payment amount** — paying net to vendor
  - Issued **TDS deduction certificate** (withholding certificate) to vendor
  - Recorded TDS liability in General Ledger
  - Remitted TDS to IRD within prescribed deadline
  - Filed monthly TDS return

- Maintained **vendor-wise TDS register** tracking:
  - Vendor name, PAN, payment date, gross amount, TDS amount, TDS rate, challan reference
- Issued **Annual TDS Certificates** to all vendors at fiscal year-end — required for vendors' own tax return filing

---

### ✅ Step 6: TDS Reconciliation

> This was one of the **most meticulous and time-consuming tasks** — ensuring complete reconciliation of all TDS

#### 📊 TDS Reconciliation Framework

| Reconciliation | Process |
|---------------|---------|
| **Interest TDS Reconciliation** | Total interest expense (P&L) × TDS rate ≈ Total interest TDS deducted (GL liability) ≈ Total TDS remitted to IRD |
| **Salary TDS Reconciliation** | Total salary expense (P&L) → Individual tax computations → Total salary TDS deducted (GL) ≈ Total TDS remitted to IRD |
| **Vendor TDS Reconciliation** | Total qualifying vendor payments → Individual TDS computations → Total vendor TDS deducted (GL) ≈ Total TDS remitted to IRD |
| **TDS Liability Account Reconciliation** | Opening TDS liability + TDS deducted during period – TDS remitted during period = Closing TDS liability (should be current month's TDS pending remittance) |
| **IRD Reconciliation** | Bank's TDS remittance records ≈ IRD portal acknowledgments ≈ IRD ledger (taxpayer profile) |

- Performed **monthly TDS reconciliation** ensuring:
  - All TDS deducted was recorded in General Ledger
  - All TDS recorded was remitted to IRD within deadline
  - TDS liability account was clean — no aged/unreconciled items
  - IRD portal reflected correct TDS credits matching bank's remittance records
- Investigated and resolved **reconciliation differences**:
  - Timing differences (deducted in month X, remitted in month X+1)
  - CBS system errors in TDS computation
  - Manual computation errors
  - Payment processing delays
  - IRD portal posting delays
- Prepared **TDS reconciliation report** for management review and external audit support

---

### ✅ Step 7: Corporate Income Tax — Computation & Advance Tax

- Managed the bank's **corporate income tax compliance**:

#### 📊 Advance Tax (Quarterly)
- Computed and paid **quarterly advance corporate income tax** to IRD:
  - As per Income Tax Act — banks are required to pay advance tax in **3 quarterly installments**:
    - 1st installment: 40% of estimated annual tax (by end of Poush)
    - 2nd installment: 70% of estimated annual tax (by end of Chaitra)
    - 3rd installment: 100% of estimated annual tax (by end of Ashad)
  - **Estimated annual tax** based on:
    - Year-to-date actual profit extrapolated to full year
    - Prior year actual tax (as baseline)
    - Known adjustments — non-deductible expenses, exempt income, timing differences
  - Prepared **advance tax computation workpaper** for each installment
  - Ensured timely payment to avoid **interest on underpayment**
  - Reconciled advance tax payments against final tax liability at year-end

#### 📊 Annual Corporate Tax Computation
- At fiscal year-end, prepared comprehensive **corporate income tax computation**:

##### Accounting Profit to Taxable Profit Reconciliation


##### Deferred Tax Computation (IAS 12)
- Computed **Deferred Tax Asset (DTA) and Deferred Tax Liability (DTL)** arising from temporary differences:

| Item | Accounting Treatment | Tax Treatment | Temporary Difference | DTA/DTL |
|------|---------------------|---------------|---------------------|---------|
| ECL Provisions | Recognized per IFRS 9 | Deductible only when written off | Deductible temporary difference | DTA |
| Depreciation | Straight-line (accounting) | Accelerated (tax) | Taxable temporary difference | DTL |
| Employee Benefits | Actuarial provision (IAS 19) | Deductible when paid | Deductible temporary difference | DTA |
| Staff Loan Day-1 Loss | Recognized per IFRS 9 | Not deductible until reversed | Deductible temporary difference | DTA |
| Fair Value Changes | FVOCI/FVTPL gains | Taxable when realized | Taxable temporary difference | DTL |

##### DTA/DTL = Temporary Difference × Tax Rate


- Net DTA/DTL recognized in financial statements per IAS 12 recognition criteria

---

### ✅ Step 8: Tax Return Filing

- Prepared and filed the **annual corporate income tax return** with IRD:

#### 📋 Tax Return Components:
- Audited financial statements
- Tax computation schedule (accounting profit to taxable profit reconciliation)
- Depreciation schedule (tax depreciation vs. accounting depreciation)
- TDS summary — total TDS deducted and remitted during the year (by category)
- Advance tax payment details
- Balance tax payment challan
- Deferred tax computation
- Transfer pricing documentation (if applicable for related party transactions)

- Filed tax return through **IRD portal (e-filing system)**
- Ensured filing within **IRD prescribed deadline** — typically within 3 months of fiscal year-end
- Maintained **tax return acknowledgment** and filing records
- Prepared supporting schedules for potential **tax assessment/scrutiny** by IRD

---

### ✅ Step 9: Social Security Fund (SSF) & Provident Fund (PF) Compliance

- Managed the bank's **SSF and PF compliance obligations**:

#### 📊 SSF Compliance

| Component | Rate | Details |
|-----------|------|---------|
| **Employer Contribution** | 20% of basic salary | Bank's contribution to SSF |
| **Employee Contribution** | 11% of basic salary | Deducted from employee salary |
| **Total Contribution** | 31% | Remitted monthly to SSF |

- Computed **monthly SSF contributions** for each employee
- Deducted employee's share from salary during payroll processing
- Remitted **total SSF contribution** (employer + employee) to SSF within prescribed deadline
- Filed **monthly SSF return** with contribution details
- Maintained **employee-wise SSF contribution register** for reconciliation and audit

#### 📊 Provident Fund (PF) Compliance
- For employees under the PF scheme (pre-SSF transition):
  - Computed monthly PF contributions (employer + employee shares)
  - Remitted to approved PF fund
  - Managed **PF withdrawal/transfer requests** for departing employees
  - Reconciled PF balance with fund statements

---

### ✅ Step 10: Tax Assessment & IRD Coordination

- Coordinated with **Inland Revenue Department (IRD)** during tax assessments and audits:

#### 🔹 Self-Assessment:
- Bank filed self-assessed tax return — IRD may accept or issue amended assessment

#### 🔹 IRD Scrutiny/Audit:
- When IRD selected the bank for detailed scrutiny:
  - Provided all requested documents — financial statements, tax computation, TDS records, PF/SSF records
  - Prepared **responses to IRD queries** with supporting evidence
  - Attended meetings with IRD officers as required
  - Negotiated **disputed items** — providing legal and factual justifications for tax positions taken
  - Received **assessment order** from IRD — accepted or appealed as appropriate

#### 🔹 Tax Dispute Resolution:
- For any disputed assessments:
  - Analyzed IRD assessment order and grounds
  - Consulted with **tax consultants / legal counsel**
  - Filed **administrative review** or **appeal** at Revenue Tribunal (if warranted)
  - Maintained complete records of dispute proceedings

---

### ✅ Step 11: Annual TDS Certificate Issuance

- At fiscal year-end, prepared and issued **Annual TDS Certificates** to all stakeholders:

| Recipient | Certificate Type | Content |
|-----------|-----------------|---------|
| **Employees** | Salary TDS Certificate | Employee name, PAN, total salary, total TDS deducted, tax slab-wise breakup |
| **Depositors** | Interest TDS Certificate | Depositor name, PAN, total interest, TDS amount (available on request or through CBS) |
| **Vendors/Contractors** | Vendor TDS Certificate | Vendor name, PAN, total payments, TDS deducted, TDS remittance details |
| **Debenture Holders** | Interest TDS Certificate | Holder name, PAN, total interest, TDS amount (through RTS) |

- TDS certificates were essential for recipients to **claim TDS credit** in their own tax returns
- Ensured certificates were **accurate, issued timely, and matched IRD remittance records**

---

### ✅ Step 12: Tax Compliance Reporting & Documentation

- Maintained comprehensive **tax compliance documentation** for internal records and audit trail:
  - **Tax compliance register** — master list of all tax obligations, due dates, filing status, and payment records
  - **Monthly TDS returns** — filed copies with IRD acknowledgments
  - **TDS challan records** — all TDS payment receipts organized by month and category
  - **TDS reconciliation workpapers** — monthly reconciliation schedules
  - **Salary tax computation files** — employee-wise annual tax workpapers
  - **Corporate tax computation file** — full workpaper with profit-to-tax reconciliation
  - **Advance tax computation workpapers** — quarterly estimation schedules
  - **Deferred tax workpapers** — temporary difference schedules and DTA/DTL computations
  - **SSF/PF remittance records** — monthly contribution records and fund reconciliation
  - **IRD correspondence file** — all letters, assessment orders, query responses
- All documentation was maintained for the **statutory retention period** (minimum 5 years beyond assessment year)
- Documentation was always **audit-ready** — organized for seamless review by external auditors and IRD

---

## 📊 Key Outcomes & Impact

| Outcome | Detail |
|---------|--------|
| **Zero Penalty Record** | Maintained zero tax penalty/interest record — all filings and payments within prescribed deadlines |
| **TDS Management** | Managed TDS across 5+ categories — deposits, salary, vendors, rent, debentures |
| **TDS Reconciliation** | Monthly reconciliation ensuring complete TDS trail from deduction to remittance to IRD acknowledgment |
| **Payroll Processing** | Complete monthly payroll processing for entire bank — computation to payment to reconciliation |
| **Corporate Tax** | Annual corporate tax computation with accounting-to-tax reconciliation and deferred tax |
| **Advance Tax** | Quarterly advance tax computation and timely payment — minimizing interest on underpayment |
| **SSF/PF Compliance** | Monthly SSF and PF contribution computation, remittance, and reconciliation |
| **Tax Certificates** | Annual TDS certificates issued to all employees, vendors, and depositors |
| **IRD Coordination** | Managed IRD assessments and queries with complete documentation support |

---

## 🧰 Tools & Skills Applied

- **Tax Compliance**: Income Tax Act 2058, TDS Computation & Reconciliation, Corporate Income Tax, Advance Tax, Deferred Tax (IAS 12)
- **Payroll Management**: Payroll Processing, Salary Tax (Progressive Slabs), Social Security Fund (SSF), Provident Fund (PF)
- **Filing & Reporting**: Tax Return Filing (IRD Portal), Vendor TDS Management, Annual TDS Certificates, Tax Assessment Coordination
- **Core Banking Systems**: Pumori CBS, Finacle CBS
- **Analytical Tools**: Microsoft Excel (Advanced), IRD E-Filing Portal

---

## 🏷️ Tags

`#TaxCompliance` `#TDS` `#CorporateIncomeTax` `#PayrollManagement` `#SalaryTax` `#TDSReconciliation` `#AdvanceTax` `#DeferredTax` `#IAS12` `#SSF` `#ProvidentFund` `#IRD` `#IncomeTaxAct` `#BankingTax` `#Nepal` `#DevelopmentBank` `#PayrollProcessing` `#TaxReturn` `#CAManishShrestha` `#CISA`

---

> *— CA Manish Shrestha, CISA®*  
> Chartered Accountant (ICAN) | Certified Information Systems Auditor (ISACA-USA)  
> 🌐 [camanishshrestha.com.np](https://www.camanishshrestha.com.np) | [GitHub](https://github.com/camanishshrestha) | [LinkedIn](https://www.linkedin.com/in/manish-shrestha-cisa-grc)
