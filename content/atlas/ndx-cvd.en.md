---
title: "NDX CVD — Cash Index Cumulative Volume Delta Aggregation"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "aggregation", "microstructure"]
---

# NDX CVD — Cash Index Volume Delta Aggregation

**In Antigravity cosmology:** Central Star Fuel (NDX).
**In standard terms:** Index-weighted Cumulative Volume Delta (CVD) across the 100 components of the NASDAQ-100 index.

## How NDX CVD is Computed

The NASDAQ-100 index is a basket of securities rather than a single tradable asset. The **NDX CVD** metric in Heniu's telemetry is calculated as follows:

1. **Transaction Feed:** Continuous market data feed across all 100 constituents of the index.
2. **Trade Classification (Tick Rule / BBO):** Trades executed at the Ask price (aggressive market buying) add volume (+); trades executed at the Bid price (aggressive market selling) subtract volume (-).
3. **Index Weighting & Aggregation:** Component volume deltas are aggregated in real time according to their index weights:
   $$ \text{CVD}_{NDX} = \sum_{i=1}^{100} w_i \cdot (\text{Vol}_{\text{Ask}, i} - \text{Vol}_{\text{Bid}, i}) $$
   where $w_i$ represents the company's index weighting. This ensures mega-caps (such as Apple or NVIDIA) influence the aggregate proportionally to their index impact.
4. **Session Reset:** The CVD baseline resets at the cash market open at 9:30 ET (15:30 CET), measuring pure aggressive order flow dynamics for the active spot session.

## Units and Semantic Interpretation

* **Unit:** Values published in telemetry (e.g., `+162.49M` or `-175.43M`) denote **NDX Weighted Flow Units**. Due to index weighting, this is not an unweighted raw sum of disparate share quantities, but a standardized aggregate aggressive order flow vector.
* **CVD is NOT "capital inflow/outflow":** In every transaction, cash and shares are exchanged simultaneously in equal dollar amount. CVD does not measure external net cash flow; it measures **signed aggressive order flow** — quantifying which side (market buyers crossing the spread vs market sellers hitting the bid) is driving transaction immediacy.
* **NDX / CVD Divergences:**
  - Price declines while NDX CVD rises: passive absorption of aggressive sell flow by limit buy orders (accumulation).
  - Price advances with negative NDX CVD: passive supply distribution into aggressive buy orders.

---

*Atlas entry. Zero trading signals — strictly market physics.*
