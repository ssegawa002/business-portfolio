# Supplier Sustainability Scorecard

An Excel workbook exploring a sourcing decision that comes up across procurement and supply chain
roles: suppliers increasingly need to be evaluated on environmental performance alongside price
and delivery reliability. This scores a small supplier panel on both, and blends them into one
composite sourcing score.

**Live demo:** see the [portfolio showcase page](../../docs/index.html).

## What's inside (`Supplier_Sustainability_Scorecard.xlsx`)

| Tab | What it does |
|---|---|
| README | Overview, methodology and how to use the file |
| Supplier Data | Sustainability inputs (CO₂ emissions, renewable energy use, ISO 14001 certification, distance to site) and a delivery performance summary, per supplier |
| Scorecard | Calculates a weighted Sustainability Score and a Composite Sourcing Score per supplier, with a Preferred / Acceptable / Review recommendation |

## Methodology

**Sustainability Score (0–100)** weights:
- Emissions intensity — 35% (lower is better)
- Renewable energy use — 25%
- ISO 14001 certification — 20%
- Proximity to site — 20% (shorter transport distance → lower logistics emissions)

Emissions and distance are normalised with min-max scaling across the supplier panel.

**Composite Sourcing Score** blends the Sustainability Score (60%) with on-time delivery rate
(40%) — a simple, adjustable model of how a buyer might weigh the two when deciding which
suppliers to grow volume with.

## Why I built it

Environmental criteria are increasingly part of supplier evaluation, not a separate checkbox
exercise. I wanted to practise building a scoring model that treats it that way — quantified,
weighted, and sitting next to operational metrics rather than off to the side.

## Techniques used
- Weighted scoring model with min-max normalization
- Cross-sheet formulas referencing a separate data input tab
- Nested `IF` logic for the recommendation band
- Conditional formatting for visual flags

## Note on data
Supplier data in this file is illustrative sample data built to demonstrate the scoring model —
not real business data.

## Related project
See the companion [Inventory Replenishment & Supplier Performance Tracker](../inventory-supplier-tracker/),
which tracks the same kind of supplier panel on delivery performance in more operational detail.
