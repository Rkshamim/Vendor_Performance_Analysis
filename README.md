# 📊 Retail Vendor Performance & Inventory Analytics

End-to-end data analytics project evaluating **10,692 vendor records** to resolve inventory holding costs, supplier concentration risk, volume purchase economics, and margin variance.

---

## 🚀 Key Business Impact

| Area | Finding | Impact Metric | Action |
| :--- | :--- | :--- | :--- |
| **Vendor Dependency** | Heavy reliance on top suppliers | **Top 10 contribute 65.69%** of purchases (Diageo leads with 16.3%) | Diversify tier-2 suppliers |
| **Bulk Purchasing** | High volume price elasticity | **72% unit cost reduction** ($39.06 ➔ $10.78 per unit) | Set bulk reorder thresholds |
| **Dead Inventory** | Working capital blocked in slow stock | **$2.71M locked capital** (Diageo: $722K, Jim Beam: $555K) | Run markdown clearance campaigns |
| **Pricing Opportunities** | High margins, low sales volume | **198 brands** with >65% margins underperforming | Test bundle deals & price drops |

---

## 🧪 Statistical Validation (Hypothesis Testing)
* **Goal:** Compare profit margins of Top vs. Low performing vendors.
* **Top Vendors (95% CI):** `30.74% – 31.61%` (Mean: `31.17%`)
* **Low Vendors (95% CI):** `40.48% – 42.62%` (Mean: `41.55%`)
* **Result:** Null Hypothesis rejected ($p < 0.05$). Low-performing vendors run on higher theoretical margins but lack distribution reach.

---

## 🛠️ Tech Stack
* **Analysis:** Python (Pandas, NumPy, SciPy Stats, Matplotlib, Seaborn)
* **Dashboard:** Microsoft Power BI (`.pbix`)
* **Data Processing:** Jupyter Notebooks, Git

---

## 📁 Repository Structure
```text
├── README.md                            # Executive project summary
├── Vendor_Performance_Report.pdf        # Detailed analytical report
├── Vendor_Performance_Dashboard.pbix    # Interactive Power BI dashboard
├── dataset/
│   └── vendor_sales_summary.csv         # Cleaned dataset (10,692 rows x 18 cols)
└── notebooks/
    ├── 01_Data_Cleaning.ipynb           # Missing values & outlier removal
    ├── 02_Exploratory_Data_Analysis.ipynb # Distributions & correlation matrix
    └── 03_Vendor_Performance_Analysis.ipynb # Segmentation & hypothesis testing
