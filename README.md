# Optimizing Sanitaryware Retail: Credit, Pricing and Inventory Loss Analysis

**BDM Capstone Project, IIT Madras BS Degree Program (Data Science and Applications)**
Author: Jatin Kumar

> Data-driven analysis of a small retail sanitaryware store to improve cash flow, fix pricing gaps and reduce losses from broken goods.

> **Privacy note:** The store's name is hidden and personal details (email, roll number) are masked as `XXXXXX` in the shared files.
---

## 1. Problem Statement

A local retail store sells sanitaryware (toilets, taps, showers and fittings) to households, contractors and builders. It runs on manual registers, with a mix of cash and credit sales. The owner faced three problems:

| # | Problem | Question |
|---|---------|----------|
| 1 | **Delayed customer payments** | Which customers hold most of the outstanding credit? |
| 2 | **Frequent MRP changes** | How much is the inventory value affected, and which product ranges changed most? |
| 3 | **Losses from broken or missing goods** | Which products cause most of the loss? |

## 2. Data

The records were not digital. They came from physical registers, supplier price lists and conversations with the owner, and were converted into structured sheets.

| Dataset | Size | Content |
|---------|------|---------|
| Credit records | 40 customers | Purchase date, amount, payments, balance |
| MRP records | 217 products | Old MRP, new MRP, product range |
| Broken goods | 61 entries | Quantity, broken quantity, unit price, loss value |

## 3. Tools

- **Excel / Google Sheets:** data entry, cleaning, formulas, pivot tables
- **Power BI:** dashboards and visuals (pie, bar, line, treemap, waterfall, Pareto, bubble, KPI cards)

## 4. Methodology

1. **Data collection:** digitized register entries and price lists.
2. **Pre-processing:** standardized names and dates, resolved split entries, and created calculated fields (total price, loss value, damage rate, % price change).
3. **Descriptive analysis:** pivot tables and summary statistics (sum, max, min) per customer, product range and product.
4. **Diagnostic analysis:** looked for the causes behind debt concentration, pricing gaps and product losses.
5. **Prescriptive analysis:** turned the findings into recommendations for the owner.

## 5. Key Findings

### Credit and payments
- Total outstanding balance is about **₹2.44 lakh**.
- A handful of customers hold about **55%** of it. The remaining **44.21%** is spread across many small accounts.
- The largest single balances are about **₹46K, ₹35K and ₹27K**.
- One customer is both the largest payer (about ₹202K) and the largest debtor.
- Business activity (sales and payments) **peaked in 2019**, dipped in 2020, then fluctuated, with another rise around 2022.

### Pricing (MRP changes)
- Total inventory value rose from **₹7,744K to ₹8,455K**, a change of about **₹711K (9.19%)**.
- The highest percentage increases were in **Kitchen Tap and Small Ideal (about 21%)**.
- The largest absolute increase came from **OH Shower, Element, Edge, Thermostat and Avior**, which together account for over ₹300K of the rise.
- Delays in updating selling prices cause items to be sold at outdated rates, which cuts margins.

### Inventory loss
- **One product (EWC 1 Pc Flora S220) alone causes about ₹20.6K of loss**, more than five times the next item.
- The cumulative loss curve reaches roughly **80% within the first 4 to 5 items**, so losses are highly concentrated.
- Losses are concentrated in fragile premium items (**EWC units and Orissa pans**).
- Products with higher damage rates tend to have higher losses.

## 6. Recommendations

| Area | Action |
|------|--------|
| Credit | Prioritize recovery from the few high-balance customers |
| Credit | Set tiered credit limits for smaller accounts |
| Pricing | Update selling prices as soon as a new MRP is announced |
| Pricing | Manage stock of high-value ranges (e.g. OH Shower) carefully |
| Loss | Improve packaging, storage and handling of EWC units and Orissa pans |
| Loss | Focus wastage reduction on the top-loss product, and consider insurance for costly breakages |
| Monitoring | Track the link between sales value and payments received, to avoid over-extending credit |

## 7. Possible Future Work

- Build a forecasting model for sales and payment timing.
- Build a credit risk score for customers.
- Automate price updates when MRP changes.

## 8. Author

**Jatin Kumar**
IIT Madras BS Degree Program
