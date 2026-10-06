# Telecoms Customer Churn Analysis

An end-to-end data analysis project investigating the primary drivers of customer churn across **5,960 customer records**. This project bridges data extraction, cleaning, modeling, and executive storytelling to provide actionable, fixable retention strategies.

---

## 📊 Executive Summary & Key Findings

* **The Core Problem:** Month-to-month customers churn at nearly **2.5x the rate** of customers enrolled in one- or two-year contracts, making contract length the single largest lever for lowering risk.
* **Tenure Vulnerability:** Churn peaks sharply during a customer's **first 6 months**, accounting for **51%** of churn behavior.
* **Service Impact:** **Fiber optic** customers exhibit higher churn rates compared to DSL or no-internet users.
* **Pricing Thresholds:** Churn rises steadily with price, with the highest billing tier (**over $95/month**) experiencing nearly double the churn rate of the lowest band.
* **Non-Factors:** Region and payment method showed **no meaningful variance** in churn rate, proving that operational focus should bypass these areas.

---

## 🛠️ Tech Stack & Methodology

1. **Data Cleaning (MySQL):** 
   * Removed duplicates, standardized inconsistent Yes/No formatting, corrected mixed date formats, and resolved blank billing values.
2. **Data Modeling (Power BI & DAX):** 
   * Constructed custom churn-rate measures utilizing `CALCULATE` and `DIVIDE.
   * Grouped customer tenure and pricing points into readable analytical bands.
3. **Verification:** 
   * Cross-checked all metric totals and chart outputs against raw SQL execution queries before final visualization.

---

## 💡 Strategic Recommendations

1. **Incentivize Longer Contracts:** Introduce targeted discounts or perks to help migrate month-to-month subscribers onto annual plans.
2. **Strengthen Early Onboarding:** Implement structured check-ins or dedicated support touchpoints during months 1 through 6 to protect high-risk new signups.
3. **Audit Fiber Optic Value:** Investigate potential reliability or pricing mismatches causing higher churn among fiber optic users.
4. **Reassess High-Tier Pricing:** Review whether plans exceeding $95/month deliver proportionate value to customers.

---

## 📂 Repository Structure

```text
├── data/               # Cleaned dataset (5,960 customer records)
├── sql/                # SQL data cleaning and validation scripts
├── dashboard/          # Power BI report file (.pbix)
└── README.md           # Project documentation
