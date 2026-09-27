# Inventory Replenishment & Supplier Performance Tracker

An Excel decision-support tool built around a procurement workflow: compare forecast demand with confirmed supplier supply, identify delivery exceptions, monitor stock coverage and test supplier-delay scenarios.

## Business question
How can procurement or supply-chain teams identify replenishment risks and supplier delivery issues early enough to support action?

## Workbook tabs
- README — overview and instructions
- Demand Forecast — forecasted replenishment demand by SKU and week
- Supplier Orders — sample purchase orders and calculated delivery status
- Stock Coverage Dashboard — demand vs. confirmed supply and risk flags
- What-If Scenario — supplier-delay sensitivity analysis
- Sustainability Scorecard — supplier sustainability and delivery-performance assessment

## Techniques
- `SUMIFS` / `COUNTIFS` cross-sheet rollups
- `IF` logic for Late / Short / On Time / Pending status
- Conditional formatting for risk flags
- Data validation for what-if inputs
- Weighted scoring for supplier assessment

## Data note
All supplier, SKU and order data is illustrative sample data created for portfolio demonstration.

[Download the workbook](../../docs/downloads/Inventory_Replenishment_Supplier_Tracker.xlsx)
