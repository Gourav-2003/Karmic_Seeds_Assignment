# 📊 Karmic Seeds — Pricing Strategy & Data‑Driven Decision Making

**Author:** Gourav  
📧 [gouravmuchhal476@gmail.com](mailto:gouravmuchhal476@gmail.com)

---

## Overview
A **data‑driven pricing framework** designed to recommend **SKU‑level prices** balancing profitability, market competitiveness, and inventory risk.  
It replaces reactive pricing with a **structured, explainable** system using cost, competition, sales, inventory, and ads data.

---

## Pricing Framework

1. **Cost & Margin Protection:** Prices never drop below total unit cost; target gross margins applied.  
2. **Competitive Guardrails:** Recommended prices stay within competitor ranges.  
3. **Inventory Adjustments:** Inventory pressure (weeks of cover) drives percentile‑based discounts/premiums.  
4. **Final Validation:** Ensures every recommendation passes cost and logic checks.

---

## Folder Structure
Karmic_Seeds_Assignment/
│
├── data/
│ ├── raw/ # Input datasets
│ └── processed/ # Cleaned & merged data
│
├── notebooks/
│ ├── 01_data_loading_cleaning.ipynb
│ ├── 02_pricing_logic.ipynb
│ └── 03_final_recommendations.ipynb
│
└── outputs/
├── charts/
└── tables/

text

---

## Key Outputs
- **Executive Snapshot:** Priority SKUs for pricing action.  
- **Final Recommendations:** SKU‑level optimal prices.  
- **Charts:** Margin distribution, competitor positioning, inventory impact.

---

## Usage
Run notebooks sequentially (`01 → 03`).  
Final outputs available in the `/outputs/` folder.

---

## Tech Stack
**Python**, **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **Jupyter Notebook**

---

## Business Impact
- Maintains margin discipline and competitiveness.  
- Reduces stock‑out and overstock risk.  
- Produces transparent, defensible pricing recommendations.
