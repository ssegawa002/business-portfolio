# Inventory Replenishment & Supplier Performance Tracker

An Excel workbook exploring a workflow common across procurement, inventory and supply chain
roles: tracking confirmed supplier order quantities against a demand forecast, flagging
discrepancies, running what-if scenarios on delays, and scoring suppliers on sustainability
alongside delivery reliability.

**Live demo:** see the [portfolio showcase page](../../docs/index.html) for an interactive
version of the what-if scenario.

## What's inside (`Inventory_Replenishment_Supplier_Tracker.xlsx`)

| Tab | What it does |
|---|---|
| README | Overview and how to use the file |
| Demand Forecast | Forecasted replenishment demand by SKU and week |
| Supplier Orders | 24 sample purchase orders across 4 suppliers — Status and Delay (days) are calculated automatically from due dates vs. actual delivery dates |
| Stock Coverage Dashboard | Rolls up demand vs. confirmed supply per SKU, flags items AT RISK |
| What-If Scenario | Pick a supplier and a delay (days) to see the effect on stock coverage before it happens |
| Sustainability Scorecard | Weights supplier CO₂ emissions, renewable energy use, ISO 14001 certification and site proximity, blended with on-time delivery into one composite sourcing score |

## Why I built it

I wanted hands-on practice with the kind of demand/supply reconciliation and discrepancy
resolution used in real material planning and procurement roles, going beyond what's covered in
my Data Management coursework (which focuses more on relational database/ER modelling).

## Techniques used
- `SUMIFS` / `COUNTIFS` for cross-sheet rollups
- Nested `IF` logic for automatic status flagging (Late / Short / On Time / Pending)
- Conditional formatting for visual risk flags
- Data validation (dropdown) for the what-if scenario input
- Weighted scoring model (normalized min-max scaling) for the sustainability scorecard

## Note on data
All SKU, supplier and order data is illustrative sample data built to demonstrate the workflow —
not real business data.
