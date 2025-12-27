# Karmic_Seeds_Assignment

Pricing Strategy & Data-Driven Decision Making
Overview

This repository presents a structured, data-driven pricing framework developed to recommend SKU-level prices while balancing profitability, market competitiveness, and inventory risk.

The approach replaces reactive pricing with a repeatable, defensible decision system using cost, competitor, sales, inventory, and advertising signals.

Pricing Logic (High-Level)

The pricing framework follows four sequential layers:

Cost & Margin Protection

Uses total_unit_cost as a pricing floor

Applies SKU-specific target gross margins

Competitive Guardrails

Recommended prices constrained within observed competitor price ranges

Prevents price isolation and aggressive undercutting

Inventory-Driven Adjustments

Inventory pressure measured via weeks_of_cover_t30

Percentile-based thresholds (top/bottom 20%) used for discounts and premiums

Final Validation

Ensures no recommendation falls below total unit cost

Folder Structure 
C:.
│   README.md
│
├───data
│   ├───processed
│   │       ads_sku_aggregated.csv
│   │       master_pricing_table_v1.csv
│   │       sales_sku_aggregated.csv
│   │
│   └───raw
│       │   ads_data_raw.csv
│       │   competitor_data_raw.csv
│       │   inventory_data_raw.csv
│       │   pricing_data_raw.csv
│       │   returns_data_raw.csv
│       │   sales_data_raw.csv
│       │
│       └───.ipynb_checkpoints
│               competitor_data-checkpoint.json
│
├───notebooks
│   │   01_data_loading_cleaning.ipynb
│   │   02_pricing_logic.ipynb
│   │   03_final_recommendations.ipynb
│   │
│   └───.ipynb_checkpoints
│           01_data_loading_cleaning-checkpoint.ipynb
│           02_exploratory_analysis-checkpoint.ipynb
│           02_pricing_logic-checkpoint.ipynb
│           03_final_recommendations-checkpoint.ipynb
│
└───outputs
    ├───charts
    │       chart_competitor_positioning.png
    │       chart_inventory_vs_price_ratio.png
    │       chart_margin_distribution.png
    │
    └───tables
            executive_snapshot_recommended_prices.csv
            recommended_prices_clean.csv
Key Outputs

Executive Snapshot: Prioritized SKUs for pricing intervention

Final Recommended Prices: SKU-level prices ready for implementation

Supporting Charts: Inventory impact, competitor positioning, margin distribution

Business Impact

Protects margins while staying market-aligned

Actively manages overstock and stock-out risk

Produces explainable, operationally usable pricing recommendations

Usage

Run notebooks sequentially from 01 → 03.
Final outputs are available in the outputs/ directory.

Prepared for Pricing Strategy & Data-Driven Decision Making assignment.
